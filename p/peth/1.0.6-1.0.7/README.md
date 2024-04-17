# Comparing `tmp/peth-1.0.6.tar.gz` & `tmp/peth-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peth-1.0.6.tar", last modified: Mon Apr 15 09:17:32 2024, max compression
+gzip compressed data, was "peth-1.0.7.tar", last modified: Wed Apr 17 06:59:54 2024, max compression
```

## Comparing `peth-1.0.6.tar` & `peth-1.0.7.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.309538 peth-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-15 09:17:28.000000 peth-1.0.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-15 09:17:28.000000 peth-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 09:17:28.000000 peth-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-15 09:17:32.305538 peth-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-15 09:17:28.000000 peth-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.285538 peth-1.0.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.289538 peth-1.0.6/docs/cn/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/api.md
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/buymeacoffee.md
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_abi.md
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_bytecode.md
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_conf.md
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_dapp.md
--rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_eth.md
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_source.md
--rw-r--r--   0 runner    (1001) docker     (127)    16207 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_tx.md
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_url.md
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_utils.md
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/install.md
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.293538 peth-1.0.6/docs/en/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/api.md
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/buymeacoffee.md
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_abi.md
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_bytecode.md
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_conf.md
--rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_dapp.md
--rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_eth.md
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_source.md
--rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_tx.md
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_url.md
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_utils.md
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/install.md
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.293538 peth-1.0.6/docs/img/
--rw-r--r--   0 runner    (1001) docker     (127)   300459 2024-04-15 09:17:28.000000 peth-1.0.6/docs/img/diffasm.png
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-15 09:17:28.000000 peth-1.0.6/docs/img/peth_eth.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.293538 peth-1.0.6/peth/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 09:17:28.000000 peth-1.0.6/peth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-15 09:17:28.000000 peth-1.0.6/peth/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    70392 2024-04-15 09:17:28.000000 peth-1.0.6/peth/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.297538 peth-1.0.6/peth/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18793 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/peth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.297538 peth-1.0.6/peth/core/tracer/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/tracer/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/tracer/txtrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/tracer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.297538 peth-1.0.6/peth/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.297538 peth-1.0.6/peth/data/bytecode/
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/bytecode/ExecTxWrapper.json
--rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/bytecode/GetBalanceWrapper.json
--rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/bytecode/MockSender.json
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/bytecode/MockSender.sol
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/chains.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/contracts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.301538 peth-1.0.6/peth/data/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/arb.json
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/avax.json
--rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/base.json
--rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/bsc.json
--rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/eth.json
--rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/ftm.json
--rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/matic.json
--rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/op.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.301538 peth-1.0.6/peth/eth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.301538 peth-1.0.6/peth/eth/abi/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/abi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/abi/abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/abi/abifunc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/abi/abitype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/abi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/bytecode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.301538 peth-1.0.6/peth/eth/evm/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/forkchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/receipt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21801 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/vm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10257 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/sigs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/web3ex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.301538 peth-1.0.6/peth/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/peth/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.305538 peth-1.0.6/peth/tools/txexpl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/peth/tools/txexpl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-15 09:17:28.000000 peth-1.0.6/peth/tools/txexpl/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-04-15 09:17:28.000000 peth-1.0.6/peth/tools/txexpl/txexpl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.305538 peth-1.0.6/peth/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8006 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/logos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/slither.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/solc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.305538 peth-1.0.6/peth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-15 09:17:32.000000 peth-1.0.6/peth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-15 09:17:32.000000 peth-1.0.6/peth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:17:32.000000 peth-1.0.6/peth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 09:17:32.000000 peth-1.0.6/peth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 09:17:32.000000 peth-1.0.6/peth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 09:17:32.000000 peth-1.0.6/peth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 09:17:28.000000 peth-1.0.6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.285538 peth-1.0.6/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.305538 peth-1.0.6/scripts/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/scripts/tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-15 09:17:28.000000 peth-1.0.6/scripts/tokens/update_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:17:32.309538 peth-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-15 09:17:28.000000 peth-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.305538 peth-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_bytecode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.305538 peth-1.0.6/tests/test_evm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_evm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    31412 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_evm/evm_test_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_evm/test_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_evm/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_evm/test_vm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_peth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_sigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.325826 peth-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-17 06:59:48.000000 peth-1.0.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-17 06:59:48.000000 peth-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 06:59:48.000000 peth-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-17 06:59:54.325826 peth-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-17 06:59:48.000000 peth-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.297826 peth-1.0.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.305826 peth-1.0.7/docs/cn/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/buymeacoffee.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/cmd_abi.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/cmd_bytecode.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/cmd_conf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/cmd_dapp.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/cmd_eth.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/cmd_source.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16207 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/cmd_tx.md
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/cmd_url.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/cmd_utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-17 06:59:48.000000 peth-1.0.7/docs/cn/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.309826 peth-1.0.7/docs/en/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/buymeacoffee.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/cmd_abi.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/cmd_bytecode.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/cmd_conf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/cmd_dapp.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/cmd_eth.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/cmd_source.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/cmd_tx.md
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/cmd_url.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/cmd_utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-17 06:59:48.000000 peth-1.0.7/docs/en/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.309826 peth-1.0.7/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   300459 2024-04-17 06:59:48.000000 peth-1.0.7/docs/img/diffasm.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-17 06:59:48.000000 peth-1.0.7/docs/img/peth_eth.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.309826 peth-1.0.7/peth/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 06:59:48.000000 peth-1.0.7/peth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-17 06:59:48.000000 peth-1.0.7/peth/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70392 2024-04-17 06:59:48.000000 peth-1.0.7/peth/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.313826 peth-1.0.7/peth/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:48.000000 peth-1.0.7/peth/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18793 2024-04-17 06:59:48.000000 peth-1.0.7/peth/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-17 06:59:48.000000 peth-1.0.7/peth/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-17 06:59:48.000000 peth-1.0.7/peth/core/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-17 06:59:48.000000 peth-1.0.7/peth/core/peth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.313826 peth-1.0.7/peth/core/tracer/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-17 06:59:48.000000 peth-1.0.7/peth/core/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-17 06:59:48.000000 peth-1.0.7/peth/core/tracer/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-17 06:59:48.000000 peth-1.0.7/peth/core/tracer/txtrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-17 06:59:48.000000 peth-1.0.7/peth/core/tracer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.313826 peth-1.0.7/peth/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.313826 peth-1.0.7/peth/data/bytecode/
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/bytecode/ExecTxWrapper.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/bytecode/GetBalanceWrapper.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/bytecode/MockSender.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/bytecode/MockSender.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/chains.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/contracts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.317826 peth-1.0.7/peth/data/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/tokens/arb.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/tokens/avax.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/tokens/base.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/tokens/bsc.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/tokens/eth.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/tokens/ftm.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/tokens/matic.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/tokens/op.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:48.000000 peth-1.0.7/peth/data/tokens.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.317826 peth-1.0.7/peth/eth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.317826 peth-1.0.7/peth/eth/abi/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/abi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/abi/abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/abi/abifunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/abi/abitype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/abi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/bytecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.321826 peth-1.0.7/peth/eth/evm/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/evm/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/evm/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/evm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/evm/forkchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/evm/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/evm/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/evm/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/evm/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/evm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21801 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/evm/vm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10257 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/sigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-04-17 06:59:48.000000 peth-1.0.7/peth/eth/web3ex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.321826 peth-1.0.7/peth/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:48.000000 peth-1.0.7/peth/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.321826 peth-1.0.7/peth/tools/txexpl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:48.000000 peth-1.0.7/peth/tools/txexpl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-17 06:59:48.000000 peth-1.0.7/peth/tools/txexpl/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-04-17 06:59:48.000000 peth-1.0.7/peth/tools/txexpl/txexpl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.321826 peth-1.0.7/peth/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:48.000000 peth-1.0.7/peth/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-17 06:59:48.000000 peth-1.0.7/peth/util/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-04-17 06:59:48.000000 peth-1.0.7/peth/util/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8006 2024-04-17 06:59:48.000000 peth-1.0.7/peth/util/logos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-17 06:59:48.000000 peth-1.0.7/peth/util/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-17 06:59:48.000000 peth-1.0.7/peth/util/slither.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-17 06:59:48.000000 peth-1.0.7/peth/util/solc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-17 06:59:48.000000 peth-1.0.7/peth/util/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.325826 peth-1.0.7/peth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-17 06:59:54.000000 peth-1.0.7/peth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-17 06:59:54.000000 peth-1.0.7/peth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:59:54.000000 peth-1.0.7/peth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-17 06:59:54.000000 peth-1.0.7/peth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-17 06:59:54.000000 peth-1.0.7/peth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-17 06:59:54.000000 peth-1.0.7/peth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-17 06:59:48.000000 peth-1.0.7/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.301826 peth-1.0.7/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.321826 peth-1.0.7/scripts/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:48.000000 peth-1.0.7/scripts/tokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-17 06:59:48.000000 peth-1.0.7/scripts/tokens/update_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:59:54.325826 peth-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-17 06:59:48.000000 peth-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.321826 peth-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-17 06:59:48.000000 peth-1.0.7/tests/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-17 06:59:48.000000 peth-1.0.7/tests/test_bytecode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:54.325826 peth-1.0.7/tests/test_evm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:48.000000 peth-1.0.7/tests/test_evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:48.000000 peth-1.0.7/tests/test_evm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31412 2024-04-17 06:59:48.000000 peth-1.0.7/tests/test_evm/evm_test_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-04-17 06:59:48.000000 peth-1.0.7/tests/test_evm/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-17 06:59:48.000000 peth-1.0.7/tests/test_evm/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-17 06:59:48.000000 peth-1.0.7/tests/test_evm/test_vm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-17 06:59:48.000000 peth-1.0.7/tests/test_peth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-17 06:59:48.000000 peth-1.0.7/tests/test_sigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-17 06:59:48.000000 peth-1.0.7/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-17 06:59:48.000000 peth-1.0.7/tests/test_tokens.py
```

### Comparing `peth-1.0.6/CHANGELOG.md` & `peth-1.0.7/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,19 @@
 
 ### Added
 
 ### Changed
 
 ### Removed
 
+## [1.0.7] - 2024-03-31
 
+### Changed 
+
+- Bug fix. Revert web3.py to 5.31.1 in requirements.txt. 
 
 ## [1.0.6] - 2024-03-31
 
 ### Added 
 
 - Add `tokens`, `addresses`, `portfolio` command.
```

### Comparing `peth-1.0.6/LICENSE` & `peth-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/PKG-INFO` & `peth-1.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: peth
-Version: 1.0.6
+Version: 1.0.7
 Summary: An all-in-one Ethereum SDK and command-line tool written in Python.
 Home-page: https://github.com/lmy375/peth
 Author: Moon
 License: AGPL-3.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: web3==6.15.1
+Requires-Dist: web3==5.31.1
 Requires-Dist: py_solc_x==1.1.1
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests==2.28.1
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: fastapi==0.110.0
 
 # Peth
@@ -57,19 +57,29 @@
 [中文](https://peth.readthedocs.io/zh-cn/)
 
 # Installation
 
 From pypi
 ```
 ➜ pip install peth
+➜ peth
 ```
 
 From github
 ```
 ➜ pip install git+https://github.com/lmy375/peth
+➜ peth
+```
+
+From source
+```
+➜ git clone https://github.com/lmy375/peth
+➜ cd peth
+➜ pip -r requirements.txt
+➜ python main.py
 ```
 
 # Quick Usage
 
 Command-line mode:
 ```
 ➜ peth -h
```

### Comparing `peth-1.0.6/README.md` & `peth-1.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -40,19 +40,29 @@
 [中文](https://peth.readthedocs.io/zh-cn/)
 
 # Installation
 
 From pypi
 ```
 ➜ pip install peth
+➜ peth
 ```
 
 From github
 ```
 ➜ pip install git+https://github.com/lmy375/peth
+➜ peth
+```
+
+From source
+```
+➜ git clone https://github.com/lmy375/peth
+➜ cd peth
+➜ pip -r requirements.txt
+➜ python main.py
 ```
 
 # Quick Usage
 
 Command-line mode:
 ```
 ➜ peth -h
```

### Comparing `peth-1.0.6/docs/cn/api.md` & `peth-1.0.7/docs/cn/api.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/cn/cmd_abi.md` & `peth-1.0.7/docs/cn/cmd_abi.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/cn/cmd_bytecode.md` & `peth-1.0.7/docs/cn/cmd_bytecode.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/cn/cmd_conf.md` & `peth-1.0.7/docs/cn/cmd_conf.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/cn/cmd_dapp.md` & `peth-1.0.7/docs/cn/cmd_dapp.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/cn/cmd_eth.md` & `peth-1.0.7/docs/cn/cmd_eth.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/cn/cmd_source.md` & `peth-1.0.7/docs/cn/cmd_source.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/cn/cmd_tx.md` & `peth-1.0.7/docs/cn/cmd_tx.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/cn/cmd_url.md` & `peth-1.0.7/docs/cn/cmd_url.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/cn/cmd_utils.md` & `peth-1.0.7/docs/cn/cmd_utils.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/cn/conf.py` & `peth-1.0.7/docs/cn/conf.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/cn/contributing.md` & `peth-1.0.7/docs/cn/contributing.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/cn/index.rst` & `peth-1.0.7/docs/cn/index.rst`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/cn/install.md` & `peth-1.0.7/docs/cn/install.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/cn/usage.md` & `peth-1.0.7/docs/cn/usage.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/en/api.md` & `peth-1.0.7/docs/en/api.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/en/cmd_abi.md` & `peth-1.0.7/docs/en/cmd_abi.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/en/cmd_bytecode.md` & `peth-1.0.7/docs/en/cmd_bytecode.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/en/cmd_conf.md` & `peth-1.0.7/docs/en/cmd_conf.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/en/cmd_dapp.md` & `peth-1.0.7/docs/en/cmd_dapp.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/en/cmd_eth.md` & `peth-1.0.7/docs/en/cmd_eth.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/en/cmd_source.md` & `peth-1.0.7/docs/en/cmd_source.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/en/cmd_tx.md` & `peth-1.0.7/docs/en/cmd_tx.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/en/cmd_url.md` & `peth-1.0.7/docs/en/cmd_url.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/en/cmd_utils.md` & `peth-1.0.7/docs/en/cmd_utils.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/en/conf.py` & `peth-1.0.7/docs/en/conf.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/en/contributing.md` & `peth-1.0.7/docs/en/contributing.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/en/index.rst` & `peth-1.0.7/docs/en/index.rst`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/en/install.md` & `peth-1.0.7/docs/en/install.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/en/usage.md` & `peth-1.0.7/docs/en/usage.md`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/img/diffasm.png` & `peth-1.0.7/docs/img/diffasm.png`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/docs/img/peth_eth.png` & `peth-1.0.7/docs/img/peth_eth.png`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/cli.py` & `peth-1.0.7/peth/cli.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/console.py` & `peth-1.0.7/peth/console.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/core/analysis.py` & `peth-1.0.7/peth/core/analysis.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/core/config.py` & `peth-1.0.7/peth/core/config.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/core/peth.py` & `peth-1.0.7/peth/core/peth.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/core/tracer/tracer.py` & `peth-1.0.7/peth/core/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/core/tracer/txtrace.py` & `peth-1.0.7/peth/core/tracer/txtrace.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/core/tracer/utils.py` & `peth-1.0.7/peth/core/tracer/utils.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/data/bytecode/ExecTxWrapper.json` & `peth-1.0.7/peth/data/bytecode/ExecTxWrapper.json`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/data/bytecode/GetBalanceWrapper.json` & `peth-1.0.7/peth/data/bytecode/GetBalanceWrapper.json`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/data/bytecode/MockSender.json` & `peth-1.0.7/peth/data/bytecode/MockSender.json`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/data/bytecode/MockSender.sol` & `peth-1.0.7/peth/data/bytecode/MockSender.sol`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/data/chains.yaml` & `peth-1.0.7/peth/data/chains.yaml`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/data/contracts.yaml` & `peth-1.0.7/peth/data/contracts.yaml`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/data/tokens/arb.json` & `peth-1.0.7/peth/data/tokens/arb.json`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/data/tokens/avax.json` & `peth-1.0.7/peth/data/tokens/avax.json`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/data/tokens/base.json` & `peth-1.0.7/peth/data/tokens/base.json`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/data/tokens/bsc.json` & `peth-1.0.7/peth/data/tokens/bsc.json`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/data/tokens/eth.json` & `peth-1.0.7/peth/data/tokens/eth.json`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/data/tokens/ftm.json` & `peth-1.0.7/peth/data/tokens/ftm.json`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/data/tokens/matic.json` & `peth-1.0.7/peth/data/tokens/matic.json`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/data/tokens/op.json` & `peth-1.0.7/peth/data/tokens/op.json`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/abi/abi.py` & `peth-1.0.7/peth/eth/abi/abi.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/abi/abifunc.py` & `peth-1.0.7/peth/eth/abi/abifunc.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/abi/abitype.py` & `peth-1.0.7/peth/eth/abi/abitype.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/abi/utils.py` & `peth-1.0.7/peth/eth/abi/utils.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/bytecode.py` & `peth-1.0.7/peth/eth/bytecode.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/contract.py` & `peth-1.0.7/peth/eth/contract.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/evm/chain.py` & `peth-1.0.7/peth/eth/evm/chain.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/evm/contract.py` & `peth-1.0.7/peth/eth/evm/contract.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/evm/forkchain.py` & `peth-1.0.7/peth/eth/evm/forkchain.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/evm/inspector.py` & `peth-1.0.7/peth/eth/evm/inspector.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/evm/receipt.py` & `peth-1.0.7/peth/eth/evm/receipt.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/evm/trace.py` & `peth-1.0.7/peth/eth/evm/trace.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/evm/transaction.py` & `peth-1.0.7/peth/eth/evm/transaction.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/evm/utils.py` & `peth-1.0.7/peth/eth/evm/utils.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/evm/vm.py` & `peth-1.0.7/peth/eth/evm/vm.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/opcodes.py` & `peth-1.0.7/peth/eth/opcodes.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/scan.py` & `peth-1.0.7/peth/eth/scan.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/sigs.py` & `peth-1.0.7/peth/eth/sigs.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/utils.py` & `peth-1.0.7/peth/eth/utils.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/eth/web3ex.py` & `peth-1.0.7/peth/eth/web3ex.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/tools/txexpl/txexpl.py` & `peth-1.0.7/peth/tools/txexpl/txexpl.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/util/diff.py` & `peth-1.0.7/peth/util/diff.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/util/graph.py` & `peth-1.0.7/peth/util/graph.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/util/logos.py` & `peth-1.0.7/peth/util/logos.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/util/markdown.py` & `peth-1.0.7/peth/util/markdown.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/util/slither.py` & `peth-1.0.7/peth/util/slither.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/util/solc.py` & `peth-1.0.7/peth/util/solc.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth/util/source.py` & `peth-1.0.7/peth/util/source.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/peth.egg-info/PKG-INFO` & `peth-1.0.7/peth.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: peth
-Version: 1.0.6
+Version: 1.0.7
 Summary: An all-in-one Ethereum SDK and command-line tool written in Python.
 Home-page: https://github.com/lmy375/peth
 Author: Moon
 License: AGPL-3.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: web3==6.15.1
+Requires-Dist: web3==5.31.1
 Requires-Dist: py_solc_x==1.1.1
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests==2.28.1
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: fastapi==0.110.0
 
 # Peth
@@ -57,19 +57,29 @@
 [中文](https://peth.readthedocs.io/zh-cn/)
 
 # Installation
 
 From pypi
 ```
 ➜ pip install peth
+➜ peth
 ```
 
 From github
 ```
 ➜ pip install git+https://github.com/lmy375/peth
+➜ peth
+```
+
+From source
+```
+➜ git clone https://github.com/lmy375/peth
+➜ cd peth
+➜ pip -r requirements.txt
+➜ python main.py
 ```
 
 # Quick Usage
 
 Command-line mode:
 ```
 ➜ peth -h
```

### Comparing `peth-1.0.6/peth.egg-info/SOURCES.txt` & `peth-1.0.7/peth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/scripts/tokens/update_tokens.py` & `peth-1.0.7/scripts/tokens/update_tokens.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/setup.py` & `peth-1.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 requires = list(filter(lambda x: not x.startswith("#"), requires))
 
 setup(
     name="peth",
     description="An all-in-one Ethereum SDK and command-line tool written in Python.",
     url="https://github.com/lmy375/peth",
     author="Moon",
-    version="1.0.6",
+    version="1.0.7",
     packages=find_packages(exclude=["tests", "scripts"]),
     python_requires=">=3.8",
     install_requires=requires,
     license="AGPL-3.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
```

### Comparing `peth-1.0.6/tests/test_abi.py` & `peth-1.0.7/tests/test_abi.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/tests/test_evm/evm_test_codes.py` & `peth-1.0.7/tests/test_evm/evm_test_codes.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/tests/test_evm/test_chain.py` & `peth-1.0.7/tests/test_evm/test_chain.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/tests/test_evm/test_misc.py` & `peth-1.0.7/tests/test_evm/test_misc.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/tests/test_evm/test_vm.py` & `peth-1.0.7/tests/test_evm/test_vm.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/tests/test_peth.py` & `peth-1.0.7/tests/test_peth.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/tests/test_sigs.py` & `peth-1.0.7/tests/test_sigs.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.6/tests/test_source.py` & `peth-1.0.7/tests/test_source.py`

 * *Files identical despite different names*

