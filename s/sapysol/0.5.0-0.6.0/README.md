# Comparing `tmp/sapysol-0.5.0.tar.gz` & `tmp/sapysol-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapysol-0.5.0.tar", max compression
+gzip compressed data, was "sapysol-0.6.0.tar", max compression
```

## Comparing `sapysol-0.5.0.tar` & `sapysol-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1080 2024-04-01 16:52:51.371732 sapysol-0.5.0/LICENSE
--rw-r--r--   0        0        0     4644 2024-04-09 17:19:46.025088 sapysol-0.5.0/README.md
--rw-r--r--   0        0        0      529 2024-04-08 19:05:51.383703 sapysol-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2744 2024-04-10 22:59:19.237955 sapysol-0.5.0/sapysol/__init__.py
--rw-r--r--   0        0        0     9019 2024-04-08 12:48:28.490259 sapysol-0.5.0/sapysol/helpers.py
--rw-r--r--   0        0        0     8082 2024-04-10 22:59:41.907791 sapysol-0.5.0/sapysol/ix.py
--rw-r--r--   0        0        0     5921 2024-04-08 07:30:51.470374 sapysol-0.5.0/sapysol/jupag.py
--rw-r--r--   0        0        0     4775 2024-04-04 22:25:05.883961 sapysol-0.5.0/sapysol/snippets/batcher.py
--rw-r--r--   0        0        0     4668 2024-04-08 07:29:48.650854 sapysol-0.5.0/sapysol/snippets/token_selloff.py
--rw-r--r--   0        0        0     4454 2024-04-05 20:16:05.330344 sapysol-0.5.0/sapysol/snippets/wallets_balance.py
--rw-r--r--   0        0        0     3949 2024-04-08 10:17:13.391023 sapysol-0.5.0/sapysol/sysvar/clock.py
--rw-r--r--   0        0        0     7102 2024-04-06 18:57:26.944570 sapysol-0.5.0/sapysol/token.py
--rw-r--r--   0        0        0      847 2024-04-02 11:13:18.066218 sapysol-0.5.0/sapysol/tokenMetadata2022.py
--rw-r--r--   0        0        0      845 2024-03-21 11:53:44.681342 sapysol-0.5.0/sapysol/tokenMetadataMetaplex.py
--rw-r--r--   0        0        0     7233 2024-04-05 20:08:23.397989 sapysol-0.5.0/sapysol/token_cache.py
--rw-r--r--   0        0        0    13796 2024-04-06 18:47:21.503484 sapysol-0.5.0/sapysol/tx.py
--rw-r--r--   0        0        0     4963 2024-04-08 07:29:31.640984 sapysol-0.5.0/sapysol/wallet.py
--rw-r--r--   0        0        0     5578 1970-01-01 00:00:00.000000 sapysol-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-01 16:52:51.371732 sapysol-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4644 2024-04-11 16:42:00.004566 sapysol-0.6.0/README.md
+-rw-r--r--   0        0        0      529 2024-04-10 23:01:09.337154 sapysol-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2744 2024-04-10 22:59:19.237955 sapysol-0.6.0/sapysol/__init__.py
+-rw-r--r--   0        0        0     9080 2024-04-17 18:39:32.974330 sapysol-0.6.0/sapysol/helpers.py
+-rw-r--r--   0        0        0     8082 2024-04-17 18:37:02.185618 sapysol-0.6.0/sapysol/ix.py
+-rw-r--r--   0        0        0     5953 2024-04-17 18:37:23.622101 sapysol-0.6.0/sapysol/jupag.py
+-rw-r--r--   0        0        0     4812 2024-04-17 18:38:33.228174 sapysol-0.6.0/sapysol/snippets/batcher.py
+-rw-r--r--   0        0        0     5024 2024-04-17 18:38:41.828100 sapysol-0.6.0/sapysol/snippets/token_selloff.py
+-rw-r--r--   0        0        0     4483 2024-04-17 18:39:04.361241 sapysol-0.6.0/sapysol/snippets/wallets_balance.py
+-rw-r--r--   0        0        0     3949 2024-04-08 10:17:13.391023 sapysol-0.6.0/sapysol/sysvar/clock.py
+-rw-r--r--   0        0        0     7076 2024-04-17 18:37:50.088542 sapysol-0.6.0/sapysol/token.py
+-rw-r--r--   0        0        0      847 2024-04-02 11:13:18.066218 sapysol-0.6.0/sapysol/tokenMetadata2022.py
+-rw-r--r--   0        0        0      845 2024-03-21 11:53:44.681342 sapysol-0.6.0/sapysol/tokenMetadataMetaplex.py
+-rw-r--r--   0        0        0     7270 2024-04-17 18:37:42.461940 sapysol-0.6.0/sapysol/token_cache.py
+-rw-r--r--   0        0        0    13831 2024-04-17 18:38:11.941689 sapysol-0.6.0/sapysol/tx.py
+-rw-r--r--   0        0        0     4922 2024-04-17 18:38:20.158285 sapysol-0.6.0/sapysol/wallet.py
+-rw-r--r--   0        0        0     5578 1970-01-01 00:00:00.000000 sapysol-0.6.0/PKG-INFO
```

### Comparing `sapysol-0.5.0/LICENSE` & `sapysol-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sapysol-0.5.0/README.md` & `sapysol-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -82,8 +82,8 @@
 ### Opinions and Views
 The views and opinions expressed herein are those of Anton Platonov and do not necessarily reflect the official policy, position, or views of any other agency, organization, employer, or company. These views are subject to change, revision, and rethinking at any time.
 
 ### Third-Party Content and Intellectual Property
 Some Content may include or link to third-party materials. The User agrees to respect all applicable intellectual property laws, including copyrights and trademarks, when engaging with this Content.
 
 ### Amendments
-Chintan Gurjar reserves the right to update or change this disclaimer at any time without notice. Continued use of the Content following modifications to this disclaimer will constitute acceptance of the revised terms.
+Anton Platonov reserves the right to update or change this disclaimer at any time without notice. Continued use of the Content following modifications to this disclaimer will constitute acceptance of the revised terms.
```

### Comparing `sapysol-0.5.0/pyproject.toml` & `sapysol-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sapysol"
-version = "0.5.0"
+version = "0.6.0"
 description = "SuperArmor's Solana Python wrapper."
 authors = ["Anton Platonov <anton@platonov.io>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `sapysol-0.5.0/sapysol/__init__.py` & `sapysol-0.6.0/sapysol/__init__.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.5.0/sapysol/helpers.py` & `sapysol-0.6.0/sapysol/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,16 @@
 #
 def SetupLogging(fileName: str = "log.log",
                  format:   str = "%(name)s: %(asctime)s | %(levelname)s | %(filename)s:%(lineno)s | %(process)d >>> %(message)s",
                  dateFmt:  str = "%Y-%m-%dT%H:%M:%SZ",
                  logLevel: int = logging.INFO):
     EnsurePathExists(os.path.dirname(fileName))
     logging.basicConfig(filename=fileName, filemode="a", format=format, datefmt=dateFmt, level=logLevel)
-    logging.getLogger().addHandler(logging.StreamHandler())
+    logging.getLogger("sapysol").addHandler(logging.StreamHandler())
+    logging.getLogger("sapysol").setLevel(logLevel)
 
 # ================================================================================
 #
 def NestedAttributeExists(target: object, attributePath: str) -> bool:
     parts = attributePath.split(".")
     while parts:
        next, parts = parts[0], parts[1:]
```

### Comparing `sapysol-0.5.0/sapysol/ix.py` & `sapysol-0.6.0/sapysol/ix.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.5.0/sapysol/jupag.py` & `sapysol-0.6.0/sapysol/jupag.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from  .token_cache    import TokenCacheEntry, TokenCache
 from   solana.rpc.api import Client, Pubkey, Keypair
 from   typing         import List, Any, TypedDict, Union, Literal
 from   dataclasses    import dataclass
 import logging
 import requests
 
+logger = logging.getLogger("sapysol")
+
 # =============================================================================
 # 
 @dataclass
 class SapysolJupagParams:
     # Quote
     swapMode:                Literal["ExactIn", "ExactOut"] = "ExactIn"
     slippageBps:             int  = 50 # 50 = 0.5%
@@ -69,33 +71,33 @@
             "onlyDirectRoutes":    "true" if swapParams.onlyDirectRoutes    else "false", # For some weird reason Python's `bool` can't be parsed here correctly, looks like JupAg parses it as str
             "asLegacyTransaction": "true" if swapParams.asLegacyTransaction else "false", # For some weird reason Python's `bool` can't be parsed here correctly, looks like JupAg parses it as str
         }
         coinQuote = requests.get(url="https://quote-api.jup.ag/v6/quote", params=paramsQuote).json()
 
         if "error" in coinQuote:
             if coinQuote["error"] in ["Could not find any route", "The route plan does not consume all the amount, please lower your amount"]:
-                logging.warning(f"Swap {str(tokenFrom)} to {str(tokenTo)}: NO ROUTES; bailing...")
+                logger.warning(f"Swap {str(tokenFrom)} to {str(tokenTo)}: NO ROUTES; bailing...")
                 return None
             else:
-                logging.warning(f"Swap {str(tokenFrom)} to {str(tokenTo)}: UNKNOWN ERROR; bailing...")
-                logging.warning(coinQuote["error"])
+                logger.warning(f"Swap {str(tokenFrom)} to {str(tokenTo)}: UNKNOWN ERROR; bailing...")
+                logger.warning(coinQuote["error"])
                 return None
 
         outLamports = int(coinQuote["outAmount"])
         outAmount   = outLamports / 10**(TO.decimals)
 
         # Check desired amount, should be at least that
         if desiredOutAmount:
             finalDesiredOutAmountLamports = int(desiredOutAmount) if outAmountInLamports else int(desiredOutAmount * 10**TO.decimals)
             finalDesiredOutAmount         = int(desiredOutAmount) if outAmountInLamports else int(desiredOutAmount * 10**TO.decimals)
             if outLamports < finalDesiredOutAmountLamports:
-                logging.warning(f"{tokenTo} desiredOutAmount: {round(finalDesiredOutAmount, 4):.4f} and outAmount: {round(outAmount, 4):.4f}! bailing...")
+                logger.warning(f"{tokenTo} desiredOutAmount: {round(finalDesiredOutAmount, 4):.4f} and outAmount: {round(outAmount, 4):.4f}! bailing...")
                 return None
 
-        logging.debug(f"Selling {inAmount} of {tokenFrom} for {outAmount} of {tokenTo}...")
+        logger.debug(f"Selling {inAmount} of {tokenFrom} for {outAmount} of {tokenTo}...")
         return coinQuote
 
     # ========================================
     # 
     @staticmethod
     def GetSwapTxBase64(walletAddress: SapysolPubkey,
                         coinQuote:     dict,
@@ -107,14 +109,14 @@
             "wrapAndUnwrapSol":          swapParams.wrapAndUnwrapSol,
             "autoMultiplier":            swapParams.quoteAutoMultiplier,     # will 2x of the auto fees
             "dynamicComputeUnitLimit":   swapParams.dynamicComputeUnitLimit, # allow dynamic compute limit instead of max 1,400,000
             "prioritizationFeeLamports": swapParams.quotePrioFeeLamports     # or custom lamports: 1000
         }
         tx = requests.post(url = "https://quote-api.jup.ag/v6/swap", json=paramsSwap).json()
         if not "swapTransaction" in tx:
-            logging.warning(f"tx: {tx}")
-            logging.warning(f"No swapTransaction in tx! bailing...")
+            logger.warning(f"tx: {tx}")
+            logger.warning(f"No swapTransaction in tx! bailing...")
             return None
         return tx["swapTransaction"]
 
 # =============================================================================
 #
```

### Comparing `sapysol-0.5.0/sapysol/snippets/batcher.py` & `sapysol-0.6.0/sapysol/snippets/batcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from   queue             import Queue, Empty
 from   threading         import Thread
 from   solana.exceptions import SolanaRpcException
 import copy
 import time
 import logging
 
+logger = logging.getLogger("sapysol")
+
 # =============================================================================
 # 
 SAPYSOL_ERROR_ACTION = Literal["ignore", "print", "raise"]
 
 # =============================================================================
 # 
 class SapysolBatcher:
@@ -94,23 +96,23 @@
                         self.CALLBACK(entity, *self.ARGS, **self.KWARGS)
                     return
                 except SolanaRpcException as e:
                     match self.RPC_ERROR_ACTION:
                         case "ignore":
                             pass
                         case "print":
-                            logging.error(f"SapysolBatcher::__ProcessSingle(), RPC error:\n{e}")
+                            logger.error(f"SapysolBatcher::__ProcessSingle(), RPC error:\n{e}")
                         case "raise":
                             raise
                 except Exception as e:
                     match self.ALL_ERROR_ACTION:
                         case "ignore":
                             pass
                         case "print":
-                            logging.error(f"SapysolBatcher::__ProcessSingle(), Error:\n{e}")
+                            logger.error(f"SapysolBatcher::__ProcessSingle(), Error:\n{e}")
                         case "raise":
                             raise
 
         while True:
             try:
                 if self.QUEUE.qsize() <= 0:
                     return
```

### Comparing `sapysol-0.5.0/sapysol/snippets/token_selloff.py` & `sapysol-0.6.0/sapysol/snippets/token_selloff.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,50 +25,55 @@
 from ..helpers           import MakePubkey, SapysolPubkey
 from ..token             import SapysolToken
 from ..jupag             import SapysolJupagParams, SapysolJupag
 from ..tx                import SapysolTxParams, SapysolTxStatus, SapysolTx, SendAndWaitBatchTx
 from  .batcher           import SapysolBatcher
 import logging
 
+logger = logging.getLogger("sapysol")
+
 # =============================================================================
 # 
 class SapysolTokenSelloff:
     def __init__(self,
                  connection:         Client,
                  walletsList:        List[Keypair],
                  tokenToSell:        SapysolPubkey,
                  tokenToBuy:         SapysolPubkey,
+                 balanceThreshold:   int = 0,
                  txParams:           SapysolTxParams          = SapysolTxParams(),
                  swapParams:         SapysolJupagParams       = SapysolJupagParams(),
                  connectionOverride: List[Union[str, Client]] = None,
                  numThreads:         int = 10):
 
         assert(all(isinstance(n, Keypair) for n in walletsList))
         self.CONNECTION:          Client                   = connection
         self.TOKEN_TO_SELL:       SapysolToken             = SapysolToken(connection=connection, tokenMint=MakePubkey(tokenToSell))
         self.TOKEN_TO_BUY:        SapysolToken             = SapysolToken(connection=connection, tokenMint=MakePubkey(tokenToBuy ))
+        self.BALANCE_THRESHOLD:   int                      = balanceThreshold
         self.TX_PARAMS:           SapysolTxParams          = txParams
         self.SWAP_PARAMS:         SapysolJupagParams       = swapParams
         self.CONNECTION_OVERRIDE: List[Union[str, Client]] = connectionOverride
         self.BATCHER:             SapysolBatcher           = SapysolBatcher(callback    = self.SellSingle,
                                                                             entityList  = walletsList,
                                                                             entityKwarg = "wallet",
                                                                             numThreads  = numThreads)
 
     # ========================================
     #
     def SellSingle(self, wallet: Keypair):
         while True:
-            balance:   int = self.TOKEN_TO_SELL.GetWalletBalanceLamports(walletAddress=wallet.pubkey())
-            delimiter: int = 10**self.TOKEN_TO_SELL.TOKEN_INFO.decimals
-            if balance <= 0:
-                logging.info(f"Wallet: {str(wallet.pubkey()):>44}; balance: 0, skipping...")
+            balance:    int = self.TOKEN_TO_SELL.GetWalletBalanceLamports(walletAddress=wallet.pubkey())
+            delimiter:  int = 10**self.TOKEN_TO_SELL.TOKEN_INFO.decimals
+            balanceStr: str = f"{0:>{self.TOKEN_TO_SELL.TOKEN_INFO.decimals+2}}" if balance == 0 else f"{balance / delimiter:.{self.TOKEN_TO_SELL.TOKEN_INFO.decimals}f}"
+            if balance <= self.BALANCE_THRESHOLD:
+                logger.info(f"Wallet: {str(wallet.pubkey()):>44}; balance: {balanceStr}, skipping...")
                 break
             else:
-                logging.info(f"Wallet: {str(wallet.pubkey()):>44}; balance: {balance / delimiter}, trying to sell all...")
+                logger.info(f"Wallet: {str(wallet.pubkey()):>44}; balance: {balanceStr}, trying to sell all...")
 
             quote = SapysolJupag.GetSwapQuote(connection = self.CONNECTION,
                                               tokenFrom  = self.TOKEN_TO_SELL.TOKEN_MINT,
                                               tokenTo    = self.TOKEN_TO_BUY.TOKEN_MINT,
                                               inAmount   = balance,
                                               swapParams = self.SWAP_PARAMS)
             txb64         = SapysolJupag.GetSwapTxBase64(walletAddress=wallet.pubkey(), coinQuote=quote, swapParams=self.SWAP_PARAMS)
```

### Comparing `sapysol-0.5.0/sapysol/snippets/wallets_balance.py` & `sapysol-0.6.0/sapysol/snippets/wallets_balance.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 from ..helpers        import MakePubkey, SapysolPubkey
 from ..token          import SapysolToken
 from  .batcher        import SapysolBatcher
 import time
 import threading
 import logging
 
+logger = logging.getLogger("sapysol")
+
 # =============================================================================
 # 
 class SapysolWalletsBalance:
     def __init__(self,
                  connection:  Client,
                  pubkeysList: List[Pubkey],
                  tokenMint:   SapysolPubkey,
@@ -72,41 +74,41 @@
     #
     def OutputPretty(self, 
                      ignoreEmpty:       bool = False,
                      balanceInLamports: bool = False) -> None:
 
         delimiter = 10**self.TOKEN.TOKEN_INFO.decimals
         # HEADER
-        logging.info((2+44+3+32+2)*"-")
-        logging.info(f"| {'WALLET':<44} | {'BALANCE':<32} |")
-        logging.info((2+44+3+32+2)*"-")
+        logger.info((2+44+3+32+2)*"-")
+        logger.info(f"| {'WALLET':<44} | {'BALANCE':<32} |")
+        logger.info((2+44+3+32+2)*"-")
 
         sum:          int = 0
         walletsFull:  int = 0
         walletsEmpty: int = 0
         for wallet, balance in self.RESULTS.items():
             sum += balance
             if balance > 0:
                 walletsFull  += 1
             else:
                 walletsEmpty += 1
 
             if balanceInLamports:
                 if not ignoreEmpty or balance > 0:
-                    logging.info(f"| {str(wallet):>44} | {balance:<32} |")
+                    logger.info(f"| {str(wallet):>44} | {balance:<32} |")
             else:
                 if not ignoreEmpty or balance > 0:
-                    logging.info(f"| {str(wallet):>44} | {balance/delimiter:<32} |")
+                    logger.info(f"| {str(wallet):>44} | {balance/delimiter:<32} |")
 
         # FOOTER
         delimiter: int = 10**self.TOKEN.TOKEN_INFO.decimals
-        logging.info((2+44+3+32+2)*"-")
+        logger.info((2+44+3+32+2)*"-")
 
-        logging.info(f"Wallets with balance: {walletsFull}" )
-        logging.info(f"Wallets empty:        {walletsEmpty}")
+        logger.info(f"Wallets with balance: {walletsFull}" )
+        logger.info(f"Wallets empty:        {walletsEmpty}")
         if balanceInLamports:
-            logging.info(f"TOKENS TOTAL (lamports): {sum}\n")
+            logger.info(f"TOKENS TOTAL (lamports): {sum}\n")
         else:
-            logging.info(f"TOKENS TOTAL: {sum/delimiter}\n")
+            logger.info(f"TOKENS TOTAL: {sum/delimiter}\n")
 
 # =============================================================================
 #
```

### Comparing `sapysol-0.5.0/sapysol/sysvar/clock.py` & `sapysol-0.6.0/sapysol/sysvar/clock.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.5.0/sapysol/token.py` & `sapysol-0.6.0/sapysol/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,14 @@
 import solders.system_program as sp
 
 from solders.rpc.errors import  InvalidParamsMessage
 from solders.rpc.responses import RpcKeyedAccountJsonParsed
 from solders.account import AccountJSON
 from spl.token._layouts import ACCOUNT_LAYOUT, MINT_LAYOUT, MULTISIG_LAYOUT  # type: ignore
 import spl.token.instructions as spl_token
-import os
-import logging
-
 
 # =============================================================================
 # 
 class SapysolToken:
     # ========================================
     #
     def __init__(self, connection: Client, tokenMint: SapysolPubkey):
```

### Comparing `sapysol-0.5.0/sapysol/tokenMetadata2022.py` & `sapysol-0.6.0/sapysol/tokenMetadata2022.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.5.0/sapysol/tokenMetadataMetaplex.py` & `sapysol-0.6.0/sapysol/tokenMetadataMetaplex.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.5.0/sapysol/token_cache.py` & `sapysol-0.6.0/sapysol/token_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 from   typing                 import List, Any, TypedDict, Union, Optional
 from  .tx                     import *
 from  .helpers                import *
 from  .ix                     import *
 import os
 import logging
 
+logger = logging.getLogger("sapysol")
+
 # =============================================================================
 # 
 SAPYSOL_TOKEN_VERSION: int = 1
 
 # =============================================================================
 # 
 class TokenCacheEntry(NamedTuple):
@@ -65,15 +67,15 @@
     # ========================================
     #
     @staticmethod
     def __LoadFromFile(tokenMint: SapysolPubkey) -> TokenCacheEntry:
         try:
             tokenCachePath: str = TokenCache.__TokenCachePath()
             tokenInfoFile:  str = TokenCache.__TokenFilename(tokenMint=tokenMint)
-            logging.debug(f"Loading token info from file: {tokenInfoFile}")
+            logger.debug(f"Loading token info from file: {tokenInfoFile}")
             if not os.path.isfile(tokenInfoFile):
                 return None
             with open(tokenInfoFile) as f:
                 tokenInfoJson = json.load(f)
                 if "SAPYSOL_TOKEN_VERSION" not in tokenInfoJson:
                     return None
                 if tokenInfoJson["SAPYSOL_TOKEN_VERSION"] < SAPYSOL_TOKEN_VERSION:
@@ -94,15 +96,15 @@
     # ========================================
     #
     @staticmethod
     def __LoadFromBlockchain(connection: Client, tokenMint: SapysolPubkey) -> TokenCacheEntry:
         tokenCachePath: str = TokenCache.__TokenCachePath()
         tokenInfoFile:  str = TokenCache.__TokenFilename(tokenMint=tokenMint)
 
-        logging.debug(f"Loading token info from Solana Node for token: {str(tokenMint)}")
+        logger.debug(f"Loading token info from Solana Node for token: {str(tokenMint)}")
         accountInfo: Account  = connection.get_account_info(pubkey=MakePubkey(tokenMint)).value
         mintInfo:    MintInfo = Token(conn       = connection, 
                                       pubkey     = MakePubkey(tokenMint),
                                       program_id = accountInfo.owner, 
                                       payer      = None).get_mint_info()
         
         with open(tokenInfoFile, "w") as f:
```

### Comparing `sapysol-0.5.0/sapysol/tx.py` & `sapysol-0.6.0/sapysol/tx.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 from   datetime                             import datetime
 from   enum                                 import Enum
 from  .helpers                              import MakeKeypair, SapysolKeypair, NestedAttributeExists
 import base64
 import logging
 import time
 
+logger = logging.getLogger("sapysol")
+
 # ================================================================================
 #
 @dataclass
 class SapysolTxParams:
     maxSecondsPerTx:       int        = 30          # 
     sleepBetweenRetry:     float      = 0.3         # 
     skipConfirmation:      bool       = True        # 
@@ -172,20 +174,20 @@
 
         if self.LAST_VALID_BLOCKHEIGHT is None:
             latestBlockHash = (connection.get_latest_blockhash(commitment=txParams.blockhashCommitment)).value
             self.LAST_VALID_BLOCKHEIGHT: int = latestBlockHash.last_valid_block_height
 
         if txParams.maxSecondsPerTx is not None and (datetime.now() - self.SENT_DT).seconds >= txParams.maxSecondsPerTx:
             self.CONFIRMED_RESULT = SapysolTxStatus.TIMEOUT
-            logging.info(f"{self.CONFIRMED_RESULT.name}: https://solscan.io/tx/{self.TXID}")
+            logger.info(f"{self.CONFIRMED_RESULT.name}: https://solscan.io/tx/{self.TXID}")
             return self
 
         blockheight = (connection.get_block_height()).value
         if blockheight < self.LAST_VALID_BLOCKHEIGHT:
-            logging.debug(f"SapysolTx::Send() blockheight={blockheight}; lastValidBlockHeight={self.LAST_VALID_BLOCKHEIGHT}; {self.LAST_VALID_BLOCKHEIGHT-blockheight}")
+            logger.debug(f"SapysolTx::Send() blockheight={blockheight}; lastValidBlockHeight={self.LAST_VALID_BLOCKHEIGHT}; {self.LAST_VALID_BLOCKHEIGHT-blockheight}")
 
             txOpts: TxOpts = TxOpts(skip_confirmation = txParams.skipConfirmation, 
                                     skip_preflight    = txParams.skipPreFlight, 
                                     max_retries       = txParams.maxRetries)
             self.TXID: Signature = (connection.send_raw_transaction(txn=self.Decode(), opts=txOpts)).value
 
         return self
@@ -241,30 +243,30 @@
 
         if self.TXID is None:
             return SapysolTxStatus.PENDING
 
         if self.CONFIRMED_TX is not None:
             self.CONFIRMED_RESULT = SapysolTxStatus.SUCCESS if self.CONFIRMED_TX.meta.err is None \
                                else SapysolTxStatus.FAIL
-            logging.info(f"{self.CONFIRMED_RESULT.name}: https://solscan.io/tx/{self.TXID}")
+            logger.info(f"{self.CONFIRMED_RESULT.name}: https://solscan.io/tx/{self.TXID}")
             return self.CONFIRMED_RESULT
 
         try:
             trans = connection.get_transaction(tx_sig     = self.TXID,
                                                commitment = self.TX_PARAMS.transactionCommitment,
                                                max_supported_transaction_version=0)
 
             if NestedAttributeExists(target=trans, attributePath="value.transaction"):
                 self.CONFIRMED_TX = trans.value.transaction
                 return self.Confirm() # one more pass because we need to hit `if self.CONFIRMED_TX is not None` case
 
         except KeyboardInterrupt as e:
             raise
         except Exception as e:
-            logging.error(e, exc_info=(type(e), e, e.__traceback__))
+            logger.error(e, exc_info=(type(e), e, e.__traceback__))
 
         return self.CONFIRMED_RESULT
 
     # ========================================
     #
     def Confirm(self) -> SapysolTxStatus:
         return self.__ConfirmInternal(connection=self.CONNECTION)
```

### Comparing `sapysol-0.5.0/sapysol/wallet.py` & `sapysol-0.6.0/sapysol/wallet.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,17 +23,14 @@
 from   solders.system_program import TransferParams, transfer
 from   typing                 import List, Any, TypedDict, Union, Optional
 from   dataclasses            import dataclass, field
 from   datetime               import datetime
 from   enum                   import Enum
 from  .helpers                import MakePubkey, MakeKeypair, SapysolKeypair, LAMPORTS_PER_SOL, ListToChunks, SapysolPubkey
 from  .tx                     import SapysolTxParams, SapysolTxStatus, SapysolTx, SendAndWaitBatchTx
-import base64
-import logging
-import time
 
 # =============================================================================
 #
 class SapysolWalletReadonly:
     # ========================================
     #
     def __init__(self, connection: Client, pubkey: SapysolPubkey):
```

### Comparing `sapysol-0.5.0/PKG-INFO` & `sapysol-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapysol
-Version: 0.5.0
+Version: 0.6.0
 Summary: SuperArmor's Solana Python wrapper.
 License: MIT
 Author: Anton Platonov
 Author-email: anton@platonov.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -108,8 +108,8 @@
 ### Opinions and Views
 The views and opinions expressed herein are those of Anton Platonov and do not necessarily reflect the official policy, position, or views of any other agency, organization, employer, or company. These views are subject to change, revision, and rethinking at any time.
 
 ### Third-Party Content and Intellectual Property
 Some Content may include or link to third-party materials. The User agrees to respect all applicable intellectual property laws, including copyrights and trademarks, when engaging with this Content.
 
 ### Amendments
-Chintan Gurjar reserves the right to update or change this disclaimer at any time without notice. Continued use of the Content following modifications to this disclaimer will constitute acceptance of the revised terms.
+Anton Platonov reserves the right to update or change this disclaimer at any time without notice. Continued use of the Content following modifications to this disclaimer will constitute acceptance of the revised terms.
```

