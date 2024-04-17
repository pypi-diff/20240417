# Comparing `tmp/sybil_engine-6.7.0.tar.gz` & `tmp/sybil_engine-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil_engine-6.7.0.tar", last modified: Sun Apr 14 13:47:03 2024, max compression
+gzip compressed data, was "sybil_engine-6.8.0.tar", last modified: Wed Apr 17 11:47:24 2024, max compression
```

## Comparing `sybil_engine-6.7.0.tar` & `sybil_engine-6.8.0.tar`

### file list

```diff
@@ -1,104 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.519494 sybil_engine-6.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-14 13:47:03.519494 sybil_engine-6.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 13:47:03.519494 sybil_engine-6.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.503494 sybil_engine-6.7.0/sybil_engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.507494 sybil_engine-6.7.0/sybil_engine/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/config/app_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.507494 sybil_engine-6.7.0/sybil_engine/contract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/contract/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/contract/erc20_test_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/contract/erc20contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/contract/send.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/contract/transaction_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/contract/weth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.507494 sybil_engine-6.7.0/sybil_engine/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/data/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/data/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/data/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/data/pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/data/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.507494 sybil_engine-6.7.0/sybil_engine/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/account_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.511494 sybil_engine-6.7.0/sybil_engine/domain/balance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/balance/balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/balance/balance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/balance/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/dex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/generic_swap_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.511494 sybil_engine-6.7.0/sybil_engine/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/module/execution_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/module/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/module/module_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/module/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.515494 sybil_engine-6.7.0/sybil_engine/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/accumulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/app_account_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/arguments_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/binance_prices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/binance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/cex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/configuration_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/decryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/fee_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/file_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/gas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/l0_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/okx_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/scal_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/telegram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/validation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/wallet_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/web3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.519494 sybil_engine-6.7.0/sybil_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-14 13:47:03.000000 sybil_engine-6.7.0/sybil_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-14 13:47:03.000000 sybil_engine-6.7.0/sybil_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:47:03.000000 sybil_engine-6.7.0/sybil_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-14 13:47:03.000000 sybil_engine-6.7.0/sybil_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-14 13:47:03.000000 sybil_engine-6.7.0/sybil_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.515494 sybil_engine-6.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.515494 sybil_engine-6.7.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/data/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/data/test_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.515494 sybil_engine-6.7.0/test/module/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.515494 sybil_engine-6.7.0/test/module/contract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/contract/mock_router.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/mock_fail_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/mock_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/mock_not_enoguth_native_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/repeatable_mock_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.515494 sybil_engine-6.7.0/test/module/swap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/swap/mock_dex.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/swap/mock_test_swap_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/swap/test_dex.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/swap/test_swap_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/test_execution_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/test_module_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.519494 sybil_engine-6.7.0/test/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/utils/test_binance_prices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/utils/test_create_app_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/utils/test_validation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.313271 sybil_engine-6.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-17 11:47:24.313271 sybil_engine-6.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 11:47:24.313271 sybil_engine-6.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.301271 sybil_engine-6.8.0/sybil_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.301271 sybil_engine-6.8.0/sybil_engine/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/config/app_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.301271 sybil_engine-6.8.0/sybil_engine/contract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/contract/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/contract/erc20_test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/contract/erc20contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/contract/send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/contract/transaction_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/contract/weth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.301271 sybil_engine-6.8.0/sybil_engine/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/data/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/data/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/data/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/data/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/data/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.301271 sybil_engine-6.8.0/sybil_engine/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/domain/account_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.305271 sybil_engine-6.8.0/sybil_engine/domain/balance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/domain/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/domain/balance/balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/domain/balance/balance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/domain/balance/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/domain/dex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/domain/generic_swap_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.305271 sybil_engine-6.8.0/sybil_engine/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/module/execution_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/module/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/module/module_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/module/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.309271 sybil_engine-6.8.0/sybil_engine/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/app_account_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/arguments_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/binance_prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/binance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/cex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/configuration_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/decryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/fee_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/gas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/google_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/l0_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/okx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/scal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/validation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/wallet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/sybil_engine/utils/web3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.313271 sybil_engine-6.8.0/sybil_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-17 11:47:24.000000 sybil_engine-6.8.0/sybil_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-17 11:47:24.000000 sybil_engine-6.8.0/sybil_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:47:24.000000 sybil_engine-6.8.0/sybil_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-17 11:47:24.000000 sybil_engine-6.8.0/sybil_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 11:47:24.000000 sybil_engine-6.8.0/sybil_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.309271 sybil_engine-6.8.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.309271 sybil_engine-6.8.0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/data/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/data/test_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.309271 sybil_engine-6.8.0/test/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.309271 sybil_engine-6.8.0/test/module/contract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/module/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/module/contract/mock_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/module/mock_fail_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/module/mock_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/module/mock_not_enoguth_native_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/module/repeatable_mock_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.309271 sybil_engine-6.8.0/test/module/swap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/module/swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/module/swap/mock_dex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/module/swap/mock_test_swap_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/module/swap/test_dex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/module/swap/test_swap_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/module/test_execution_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/module/test_module_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/module/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:24.313271 sybil_engine-6.8.0/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/utils/test_binance_prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/utils/test_create_app_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-17 11:47:16.000000 sybil_engine-6.8.0/test/utils/test_validation_utils.py
```

### Comparing `sybil_engine-6.7.0/PKG-INFO` & `sybil_engine-6.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil_engine
-Version: 6.7.0
+Version: 6.8.0
 Summary: Engine for web3 smart contracts automatization.
 Home-page: https://github.com/Indeoo/sybil-engine/
 Author: Indeoo
 Author-email: indeooars@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: loguru==0.7.2
 Requires-Dist: setuptools==69.0.3
@@ -15,14 +15,17 @@
 Requires-Dist: requests==2.31.0
 Requires-Dist: pyTelegramBotAPI==4.14.1
 Requires-Dist: python-okx==0.2.2
 Requires-Dist: termcolor==2.4.0
 Requires-Dist: bumpversion==0.6.0
 Requires-Dist: binance-connector==3.5.1
 Requires-Dist: base58==2.1.1
+Requires-Dist: google-api-python-client==2.126.0
+Requires-Dist: google-auth-httplib2==0.2.0
+Requires-Dist: google-auth-oauthlib==1.2.0
 
 # Sybil Engine
 
 ## Introduction
 Sybil Engine is a powerful Python library designed for testing web3 contracts. It facilitates seamless interactions with blockchain networks and smart contracts, providing developers with efficient tools to execute, plan, and manage web3 transactions.
 
 ## Key Features
```

### Comparing `sybil_engine-6.7.0/README.md` & `sybil_engine-6.8.0/README.md`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/setup.py` & `sybil_engine-6.8.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = file.readlines()
 
 setup(
     name='sybil_engine',
-    version='6.7.0',
+    version='6.8.0',
     py_modules=['sybil_engine'],
     packages=find_packages(),
     install_requires=requirements,
     data_files=[('', ['requirements.txt'])],
     author='Indeoo',
     author_email='indeooars@gmail.com',
     description='Engine for web3 smart contracts automatization.',
```

### Comparing `sybil_engine-6.7.0/sybil_engine/app.py` & `sybil_engine-6.8.0/sybil_engine/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,27 +19,29 @@
     modules_data = load_module_vars(modules_data_file)['modules_data']
 
     load_logger(send_to_bot, config_map['telegram_enabled'], config_map['telegram_log_level'])
 
     set_telegram_api_chat_id(config_map['telegram_api_chat_id'])
     set_telegram_api_key(config_map['telegram_api_key'])
 
-    args = parse_arguments(config_map['password'], module_map['module'])
-
     if 'shell_mode' not in config_map:
         config_map['shell_mode'] = 'classic'
 
     if 'account_creation_mode' not in config_map:
         config_map['account_creation_mode'] = 'TXT'
 
     if 'cex_address_validation' not in config_map:
         config_map['cex_address_validation'] = True
 
     if 'interactive_confirmation' not in config_map:
         config_map['interactive_confirmation'] = True
+    if 'spreadsheet_id' not in config_map:
+        config_map['spreadsheet_id'] = None
+
+    args = parse_arguments(config_map['password'], config_map['spreadsheet_id'], module_map['module'])
 
     if config_map['shell_mode'] == 'interactive':
         logger.info("Choose module (by id):")
 
         for module_id, module in modules_data.get_module_map().items():
             module_name = get_module_name(module)
             logger.info(f"  {module_id} {module_name}")
```

### Comparing `sybil_engine-6.7.0/sybil_engine/config/app_config.py` & `sybil_engine-6.8.0/sybil_engine/config/app_config.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/contract/contract.py` & `sybil_engine-6.8.0/sybil_engine/contract/contract.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/contract/erc20_test_contract.py` & `sybil_engine-6.8.0/sybil_engine/contract/erc20_test_contract.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/contract/erc20contract.py` & `sybil_engine-6.8.0/sybil_engine/contract/erc20contract.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/contract/send.py` & `sybil_engine-6.8.0/sybil_engine/contract/send.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/contract/transaction_executor.py` & `sybil_engine-6.8.0/sybil_engine/contract/transaction_executor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/contract/weth.py` & `sybil_engine-6.8.0/sybil_engine/contract/weth.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/data/contracts.py` & `sybil_engine-6.8.0/sybil_engine/data/contracts.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/data/networks.py` & `sybil_engine-6.8.0/sybil_engine/data/networks.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/data/pairs.py` & `sybil_engine-6.8.0/sybil_engine/data/pairs.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/data/tokens.py` & `sybil_engine-6.8.0/sybil_engine/data/tokens.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/domain/balance/balance.py` & `sybil_engine-6.8.0/sybil_engine/domain/balance/balance.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/domain/balance/balance_utils.py` & `sybil_engine-6.8.0/sybil_engine/domain/balance/balance_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/domain/balance/tokens.py` & `sybil_engine-6.8.0/sybil_engine/domain/balance/tokens.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/domain/dex.py` & `sybil_engine-6.8.0/sybil_engine/domain/dex.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/domain/generic_swap_facade.py` & `sybil_engine-6.8.0/sybil_engine/domain/generic_swap_facade.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/module/execution_planner.py` & `sybil_engine-6.8.0/sybil_engine/module/execution_planner.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/module/module.py` & `sybil_engine-6.8.0/sybil_engine/module/module.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/module/module_executor.py` & `sybil_engine-6.8.0/sybil_engine/module/module_executor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/module/modules.py` & `sybil_engine-6.8.0/sybil_engine/module/modules.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/accumulator.py` & `sybil_engine-6.8.0/sybil_engine/utils/accumulator.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/app_account_utils.py` & `sybil_engine-6.8.0/sybil_engine/utils/app_account_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from loguru import logger
 from web3 import Web3
 
 from sybil_engine.utils.cex_utils import get_cex_addresses
 from sybil_engine.utils.csv_reader import read_csv_rows
 from sybil_engine.utils.decryptor import decrypt_private_key
 from sybil_engine.utils.file_loader import load_file_rows
+from sybil_engine.utils.google_utils import get_google_spreadsheet
 from sybil_engine.utils.utils import ConfigurationException
 from sybil_engine.utils.wallet_loader import load_addresses
 
 
 def create_app_account(args, encryption, proxy_mode, account_creation_mode, cex_address_validation):
     if account_creation_mode == 'TXT' or account_creation_mode is None:
         accounts = create_app_accounts_from_txt(
@@ -20,17 +21,26 @@
             (proxy_mode, args.proxy_file),
             args.cex_addresses,
             args.starknet_addresses,
             args.password.encode('utf-8'),
             encryption
         )
     elif account_creation_mode == 'CSV':
-        accounts = create_app_accounts_from_csv(args.account_csv, args.password.encode('utf-8'), encryption)
+        rows = read_csv_rows(args.account_csv)
+
+        accounts = create_app_accounts_from_table(rows, args.password.encode('utf-8'), encryption)
+    elif account_creation_mode == 'GOOGLE':
+        if args.spreadsheet_id is None:
+            raise Exception(f"account_creation_mode is GOOGLE, spreadsheet_id is required in config")
+
+        rows = get_google_spreadsheet(args.spreadsheet_id, args.wallets)
+
+        accounts = create_app_accounts_from_table(rows, args.password.encode('utf-8'), encryption)
     else:
-        raise ConfigurationException("account_creation_mode should be CSV or TXT")
+        raise ConfigurationException("account_creation_mode should be TXT, CSV or GOOGLE")
 
     if cex_address_validation:
         validate_cex_addresses(accounts, get_cex_addresses(args.cex_conf))
 
     return accounts
 
 
@@ -44,16 +54,15 @@
         load_addresses(private_keys),
         load_file_rows(proxy_file),
         proxy_mode,
         load_addresses(starknet_addresses)
     )
 
 
-def create_app_accounts_from_csv(account_csv, password, encryption):
-    rows = read_csv_rows(account_csv)
+def create_app_accounts_from_table(rows, password, encryption):
     app_accounts = []
 
     starknet = False
     cex = False
 
     for row in rows:
         if row['ENABLE'] == 'FALSE':
```

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/arguments_parser.py` & `sybil_engine-6.8.0/sybil_engine/utils/arguments_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import os
 import sys
 
 
-def parse_arguments(default_password, default_module):
+def parse_arguments(default_password, spreadsheet_id, default_module):
     parser = argparse.ArgumentParser(description='Process arguments.')
 
     data_folder = 'data'
     wallets_folder = f'{data_folder}/wallets'
 
     parser.add_argument('--profile', type=str, required=False,
                         default=os.environ.get('PROFILE', 'default'),
@@ -34,14 +34,17 @@
                         help='a string to be processed')
     parser.add_argument('--network', type=str, required=False, default=os.environ.get('NETWORK', 'MAIN'),
                         help='a string to be processed')
     parser.add_argument('--module', type=str, required=False, default=os.environ.get('MODULE', default_module),
                         help='a string to be processed')
     parser.add_argument('--cex_conf', type=str, required=False, default=os.environ.get('CEX_CONF', 'okx'),
                         help='a string to be processed')
+    parser.add_argument('--spreadsheet_id', type=str, required=False,
+                        default=os.environ.get('SPREADSHEET_ID', spreadsheet_id),
+                        help='a string to be processed')
 
     args = parser.parse_args()
 
     if '--private_keys' not in sys.argv:
         args.private_keys = os.path.join(args.wallets, 'private_keys.txt')
     if '--cex_addresses' not in sys.argv:
         args.cex_addresses = os.path.join(args.wallets, 'cex_addresses.txt')
```

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/binance_prices.py` & `sybil_engine-6.8.0/sybil_engine/utils/binance_prices.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/binance_utils.py` & `sybil_engine-6.8.0/sybil_engine/utils/binance_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/configuration_loader.py` & `sybil_engine-6.8.0/sybil_engine/utils/configuration_loader.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/decryptor.py` & `sybil_engine-6.8.0/sybil_engine/utils/decryptor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/fee_storage.py` & `sybil_engine-6.8.0/sybil_engine/utils/fee_storage.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/gas_utils.py` & `sybil_engine-6.8.0/sybil_engine/utils/gas_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/logs.py` & `sybil_engine-6.8.0/sybil_engine/utils/logs.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/okx_utils.py` & `sybil_engine-6.8.0/sybil_engine/utils/okx_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/retry.py` & `sybil_engine-6.8.0/sybil_engine/utils/retry.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/scal_utils.py` & `sybil_engine-6.8.0/sybil_engine/utils/scal_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/telegram.py` & `sybil_engine-6.8.0/sybil_engine/utils/telegram.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/utils.py` & `sybil_engine-6.8.0/sybil_engine/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/validation_utils.py` & `sybil_engine-6.8.0/sybil_engine/utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine/utils/web3_utils.py` & `sybil_engine-6.8.0/sybil_engine/utils/web3_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/sybil_engine.egg-info/PKG-INFO` & `sybil_engine-6.8.0/sybil_engine.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil_engine
-Version: 6.7.0
+Version: 6.8.0
 Summary: Engine for web3 smart contracts automatization.
 Home-page: https://github.com/Indeoo/sybil-engine/
 Author: Indeoo
 Author-email: indeooars@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: loguru==0.7.2
 Requires-Dist: setuptools==69.0.3
@@ -15,14 +15,17 @@
 Requires-Dist: requests==2.31.0
 Requires-Dist: pyTelegramBotAPI==4.14.1
 Requires-Dist: python-okx==0.2.2
 Requires-Dist: termcolor==2.4.0
 Requires-Dist: bumpversion==0.6.0
 Requires-Dist: binance-connector==3.5.1
 Requires-Dist: base58==2.1.1
+Requires-Dist: google-api-python-client==2.126.0
+Requires-Dist: google-auth-httplib2==0.2.0
+Requires-Dist: google-auth-oauthlib==1.2.0
 
 # Sybil Engine
 
 ## Introduction
 Sybil Engine is a powerful Python library designed for testing web3 contracts. It facilitates seamless interactions with blockchain networks and smart contracts, providing developers with efficient tools to execute, plan, and manage web3 transactions.
 
 ## Key Features
```

### Comparing `sybil_engine-6.7.0/sybil_engine.egg-info/SOURCES.txt` & `sybil_engine-6.8.0/sybil_engine.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 sybil_engine/utils/cex_utils.py
 sybil_engine/utils/configuration_loader.py
 sybil_engine/utils/csv_reader.py
 sybil_engine/utils/decryptor.py
 sybil_engine/utils/fee_storage.py
 sybil_engine/utils/file_loader.py
 sybil_engine/utils/gas_utils.py
+sybil_engine/utils/google_utils.py
 sybil_engine/utils/l0_utils.py
 sybil_engine/utils/logs.py
 sybil_engine/utils/okx_utils.py
 sybil_engine/utils/retry.py
 sybil_engine/utils/scal_utils.py
 sybil_engine/utils/telegram.py
 sybil_engine/utils/utils.py
```

### Comparing `sybil_engine-6.7.0/test/__init__.py` & `sybil_engine-6.8.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/test/data/test_networks.py` & `sybil_engine-6.8.0/test/data/test_networks.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/test/data/test_pairs.py` & `sybil_engine-6.8.0/test/data/test_pairs.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/test/module/contract/mock_router.py` & `sybil_engine-6.8.0/test/module/contract/mock_router.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/test/module/swap/mock_dex.py` & `sybil_engine-6.8.0/test/module/swap/mock_dex.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/test/module/swap/mock_test_swap_facade.py` & `sybil_engine-6.8.0/test/module/swap/mock_test_swap_facade.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/test/module/swap/test_dex.py` & `sybil_engine-6.8.0/test/module/swap/test_dex.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/test/module/swap/test_swap_facade.py` & `sybil_engine-6.8.0/test/module/swap/test_swap_facade.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/test/module/test_execution_planner.py` & `sybil_engine-6.8.0/test/module/test_execution_planner.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/test/module/test_module_executor.py` & `sybil_engine-6.8.0/test/module/test_module_executor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/test/test_config.py` & `sybil_engine-6.8.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/test/utils/test_binance_prices.py` & `sybil_engine-6.8.0/test/utils/test_binance_prices.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.7.0/test/utils/test_create_app_accounts.py` & `sybil_engine-6.8.0/test/utils/test_create_app_accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 
 from sybil_engine.domain.balance.balance_utils import interval_to_eth_balance
-from sybil_engine.utils.app_account_utils import create_app_account_with_proxies, create_app_accounts_from_csv, \
+from sybil_engine.utils.app_account_utils import create_app_account_with_proxies, create_app_accounts_from_table, \
     validate_cex_addresses, AppAccount
 from test import zksync_test_account
 
 
 class TestCreateAppAccounts(unittest.TestCase):
 
     def test_create_zksync(self):
@@ -31,15 +31,15 @@
             'RANDOM',
             ['0x6317842385f344acf68561f4e65f0f39e4fb4f1ad104b92bd007361aed39d8'],
         )[0]
 
         base_min_native_balance = interval_to_eth_balance({'from': 1, 'to': 1}, base_test_account, None, None)
 
     def test_create_zksync_from_csv(self):
-        accounts = create_app_accounts_from_csv(
+        accounts = create_app_accounts_from_table(
             'test/data/wallets/accounts.csv',
             'password',
             False
         )
 
         self.assertEqual(
             len(accounts),
```

### Comparing `sybil_engine-6.7.0/test/utils/test_validation_utils.py` & `sybil_engine-6.8.0/test/utils/test_validation_utils.py`

 * *Files identical despite different names*

