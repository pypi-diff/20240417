# Comparing `tmp/coapts-0.0.8.tar.gz` & `tmp/coapts-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coapts-0.0.8.tar", last modified: Sat Mar  9 03:02:02 2024, max compression
+gzip compressed data, was "coapts-0.0.9.tar", last modified: Sat Mar  9 03:17:07 2024, max compression
```

## Comparing `coapts-0.0.8.tar` & `coapts-0.0.9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:02:02.456509 coapts-0.0.8/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1086 2024-02-24 23:40:03.000000 coapts-0.0.8/LICENSE
--rw-r--r--   0 erikg     (1000) erikg     (1000)      792 2024-03-09 03:02:02.456509 coapts-0.0.8/PKG-INFO
--rw-rw-r--   0 erikg     (1000) erikg     (1000)        8 2024-02-24 23:40:03.000000 coapts-0.0.8/README.md
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      872 2024-03-09 03:01:27.000000 coapts-0.0.8/pyproject.toml
--rw-rw-r--   0 erikg     (1000) erikg     (1000)       38 2024-03-09 03:02:02.456509 coapts-0.0.8/setup.cfg
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:02:02.448509 coapts-0.0.8/src/
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:02:02.452509 coapts-0.0.8/src/coapts/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1075 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     4510 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/blockwise.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:02:02.452509 coapts-0.0.8/src/coapts/cli/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      515 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/cli/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    17334 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/cli/client.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5538 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/cli/common.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     2158 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/cli/defaults.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    14554 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/cli/fileserver.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     6283 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/cli/proxy.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    29388 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/cli/rd.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    12589 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/credentials.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     7793 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/defaults.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     7233 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/error.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    20509 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/interfaces.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    27693 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/message.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    21127 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/messagemanager.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      670 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/meta.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:02:02.452509 coapts-0.0.8/src/coapts/numbers/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1425 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/numbers/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5275 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/numbers/codes.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5795 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/numbers/constants.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    12199 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/numbers/contentformat.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5534 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/numbers/optionnumbers.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      928 2024-03-09 03:01:15.000000 coapts-0.0.8/src/coapts/numbers/types.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     9296 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/options.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     8207 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/optiontypes.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    80685 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/oscore.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     6275 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/oscore_sitewrapper.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    13282 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/pipe.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    46714 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/protocol.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:02:02.456509 coapts-0.0.8/src/coapts/proxy/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      242 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/proxy/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1615 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/proxy/client.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    15717 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/proxy/server.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    17175 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/resource.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:02:02.456509 coapts-0.0.8/src/coapts/resourcedirectory/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      382 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/resourcedirectory/__init__.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:02:02.456509 coapts-0.0.8/src/coapts/resourcedirectory/client/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      304 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/resourcedirectory/client/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    13702 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/resourcedirectory/client/register.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    11199 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/tokenmanager.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:02:02.456509 coapts-0.0.8/src/coapts/transports/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      828 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/transports/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     2485 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/transports/generic_udp.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    10545 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/transports/oscore.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     8288 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/transports/rfc8323common.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    11182 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/transports/simple6.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     7998 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/transports/simplesocketserver.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    14842 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/transports/tcp.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    14956 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/transports/tinydtls.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    11343 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/transports/tinydtls_server.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1140 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/transports/tls.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    25068 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/transports/udp6.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    17659 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/transports/ws.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:02:02.456509 coapts-0.0.8/src/coapts/util/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5844 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/util/__init__.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:02:02.456509 coapts-0.0.8/src/coapts/util/asyncio/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      486 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/util/asyncio/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     4126 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/util/asyncio/getaddrinfo_addrconfig.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     6703 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/util/asyncio/recvmsg.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1972 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/util/asyncio/timeoutdict.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5687 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/util/cli.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1140 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/util/contenttype.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     2503 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/util/cryptography_additions.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1412 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/util/linkformat.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1200 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/util/linkformat_pygments.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     7029 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/util/prettyprint.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     4636 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/util/pyodide_websockets.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     2126 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/util/socknumbers.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      832 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/util/uri.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:02:02.456509 coapts-0.0.8/src/coapts/util/vendored/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    12359 2024-02-24 23:40:03.000000 coapts-0.0.8/src/coapts/util/vendored/link_header.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:02:02.456509 coapts-0.0.8/src/coapts.egg-info/
--rw-r--r--   0 erikg     (1000) erikg     (1000)      792 2024-03-09 03:02:02.000000 coapts-0.0.8/src/coapts.egg-info/PKG-INFO
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     2088 2024-03-09 03:02:02.000000 coapts-0.0.8/src/coapts.egg-info/SOURCES.txt
--rw-rw-r--   0 erikg     (1000) erikg     (1000)        1 2024-03-09 03:02:02.000000 coapts-0.0.8/src/coapts.egg-info/dependency_links.txt
--rw-rw-r--   0 erikg     (1000) erikg     (1000)        7 2024-03-09 03:02:02.000000 coapts-0.0.8/src/coapts.egg-info/top_level.txt
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:17:07.813980 coapts-0.0.9/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1086 2024-02-24 23:40:03.000000 coapts-0.0.9/LICENSE
+-rw-r--r--   0 erikg     (1000) erikg     (1000)      792 2024-03-09 03:17:07.813980 coapts-0.0.9/PKG-INFO
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)        8 2024-02-24 23:40:03.000000 coapts-0.0.9/README.md
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      872 2024-03-09 03:16:43.000000 coapts-0.0.9/pyproject.toml
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)       38 2024-03-09 03:17:07.813980 coapts-0.0.9/setup.cfg
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:17:07.801980 coapts-0.0.9/src/
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:17:07.805980 coapts-0.0.9/src/coapts/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1075 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     4510 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/blockwise.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:17:07.805980 coapts-0.0.9/src/coapts/cli/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      515 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/cli/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    17334 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/cli/client.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5538 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/cli/common.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     2158 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/cli/defaults.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    14554 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/cli/fileserver.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     6283 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/cli/proxy.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    29388 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/cli/rd.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    12589 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/credentials.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     7793 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/defaults.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     7233 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/error.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    20509 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/interfaces.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    27693 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/message.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    21127 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/messagemanager.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      670 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/meta.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:17:07.809980 coapts-0.0.9/src/coapts/numbers/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1425 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/numbers/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5275 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/numbers/codes.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5795 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/numbers/constants.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    12199 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/numbers/contentformat.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5534 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/numbers/optionnumbers.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      684 2024-03-09 03:16:02.000000 coapts-0.0.9/src/coapts/numbers/types.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     9296 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/options.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     8207 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/optiontypes.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    80685 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/oscore.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     6275 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/oscore_sitewrapper.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    13282 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/pipe.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    46714 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/protocol.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:17:07.809980 coapts-0.0.9/src/coapts/proxy/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      242 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/proxy/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1615 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/proxy/client.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    15717 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/proxy/server.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    17175 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/resource.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:17:07.809980 coapts-0.0.9/src/coapts/resourcedirectory/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      382 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/resourcedirectory/__init__.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:17:07.809980 coapts-0.0.9/src/coapts/resourcedirectory/client/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      304 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/resourcedirectory/client/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    13702 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/resourcedirectory/client/register.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    11199 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/tokenmanager.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:17:07.809980 coapts-0.0.9/src/coapts/transports/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      828 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/transports/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     2485 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/transports/generic_udp.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    10545 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/transports/oscore.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     8288 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/transports/rfc8323common.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    11182 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/transports/simple6.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     7998 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/transports/simplesocketserver.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    14842 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/transports/tcp.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    14956 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/transports/tinydtls.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    11343 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/transports/tinydtls_server.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1140 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/transports/tls.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    25068 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/transports/udp6.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    17659 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/transports/ws.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:17:07.813980 coapts-0.0.9/src/coapts/util/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5844 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/util/__init__.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:17:07.813980 coapts-0.0.9/src/coapts/util/asyncio/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      486 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/util/asyncio/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     4126 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/util/asyncio/getaddrinfo_addrconfig.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     6703 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/util/asyncio/recvmsg.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1972 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/util/asyncio/timeoutdict.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5687 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/util/cli.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1140 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/util/contenttype.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     2503 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/util/cryptography_additions.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1412 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/util/linkformat.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1200 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/util/linkformat_pygments.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     7029 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/util/prettyprint.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     4636 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/util/pyodide_websockets.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     2126 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/util/socknumbers.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      832 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/util/uri.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:17:07.813980 coapts-0.0.9/src/coapts/util/vendored/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    12359 2024-02-24 23:40:03.000000 coapts-0.0.9/src/coapts/util/vendored/link_header.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-03-09 03:17:07.813980 coapts-0.0.9/src/coapts.egg-info/
+-rw-r--r--   0 erikg     (1000) erikg     (1000)      792 2024-03-09 03:17:07.000000 coapts-0.0.9/src/coapts.egg-info/PKG-INFO
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     2088 2024-03-09 03:17:07.000000 coapts-0.0.9/src/coapts.egg-info/SOURCES.txt
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)        1 2024-03-09 03:17:07.000000 coapts-0.0.9/src/coapts.egg-info/dependency_links.txt
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)        7 2024-03-09 03:17:07.000000 coapts-0.0.9/src/coapts.egg-info/top_level.txt
```

### Comparing `coapts-0.0.8/LICENSE` & `coapts-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/PKG-INFO` & `coapts-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coapts
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python aiocoap dialect: CoAP Type Shuffling 
 Author-email: Erik Gonzalez <erikglez_ipn@hotmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ErikGlz/coapts
 Keywords: coap,asyncio,iot
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `coapts-0.0.8/pyproject.toml` & `coapts-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools >= 66.0" ]
 build-backend = "setuptools.build_meta"
  
 [project]
 name = "coapts"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python aiocoap dialect: CoAP Type Shuffling "
 readme = "README.md"
 authors = [
     { name = "Erik Gonzalez", email = "erikglez_ipn@hotmail.com" },
 ]
 license = { text = "MIT" }
 keywords = [ "coap", "asyncio", "iot" ]
```

### Comparing `coapts-0.0.8/src/coapts/__init__.py` & `coapts-0.0.9/src/coapts/__init__.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/blockwise.py` & `coapts-0.0.9/src/coapts/blockwise.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/cli/__init__.py` & `coapts-0.0.9/src/coapts/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/cli/client.py` & `coapts-0.0.9/src/coapts/cli/client.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/cli/common.py` & `coapts-0.0.9/src/coapts/cli/common.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/cli/defaults.py` & `coapts-0.0.9/src/coapts/cli/defaults.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/cli/fileserver.py` & `coapts-0.0.9/src/coapts/cli/fileserver.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/cli/proxy.py` & `coapts-0.0.9/src/coapts/cli/proxy.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/cli/rd.py` & `coapts-0.0.9/src/coapts/cli/rd.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/credentials.py` & `coapts-0.0.9/src/coapts/credentials.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/defaults.py` & `coapts-0.0.9/src/coapts/defaults.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/error.py` & `coapts-0.0.9/src/coapts/error.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/interfaces.py` & `coapts-0.0.9/src/coapts/interfaces.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/message.py` & `coapts-0.0.9/src/coapts/message.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/messagemanager.py` & `coapts-0.0.9/src/coapts/messagemanager.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/meta.py` & `coapts-0.0.9/src/coapts/meta.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/numbers/__init__.py` & `coapts-0.0.9/src/coapts/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/numbers/codes.py` & `coapts-0.0.9/src/coapts/numbers/codes.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/numbers/constants.py` & `coapts-0.0.9/src/coapts/numbers/constants.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/numbers/contentformat.py` & `coapts-0.0.9/src/coapts/numbers/contentformat.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/numbers/optionnumbers.py` & `coapts-0.0.9/src/coapts/numbers/optionnumbers.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/options.py` & `coapts-0.0.9/src/coapts/options.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/optiontypes.py` & `coapts-0.0.9/src/coapts/optiontypes.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/oscore.py` & `coapts-0.0.9/src/coapts/oscore.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/oscore_sitewrapper.py` & `coapts-0.0.9/src/coapts/oscore_sitewrapper.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/pipe.py` & `coapts-0.0.9/src/coapts/pipe.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/protocol.py` & `coapts-0.0.9/src/coapts/protocol.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/proxy/client.py` & `coapts-0.0.9/src/coapts/proxy/client.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/proxy/server.py` & `coapts-0.0.9/src/coapts/proxy/server.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/resource.py` & `coapts-0.0.9/src/coapts/resource.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/resourcedirectory/client/register.py` & `coapts-0.0.9/src/coapts/resourcedirectory/client/register.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/tokenmanager.py` & `coapts-0.0.9/src/coapts/tokenmanager.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/transports/__init__.py` & `coapts-0.0.9/src/coapts/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/transports/generic_udp.py` & `coapts-0.0.9/src/coapts/transports/generic_udp.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/transports/oscore.py` & `coapts-0.0.9/src/coapts/transports/oscore.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/transports/rfc8323common.py` & `coapts-0.0.9/src/coapts/transports/rfc8323common.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/transports/simple6.py` & `coapts-0.0.9/src/coapts/transports/simple6.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/transports/simplesocketserver.py` & `coapts-0.0.9/src/coapts/transports/simplesocketserver.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/transports/tcp.py` & `coapts-0.0.9/src/coapts/transports/tcp.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/transports/tinydtls.py` & `coapts-0.0.9/src/coapts/transports/tinydtls.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/transports/tinydtls_server.py` & `coapts-0.0.9/src/coapts/transports/tinydtls_server.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/transports/tls.py` & `coapts-0.0.9/src/coapts/transports/tls.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/transports/udp6.py` & `coapts-0.0.9/src/coapts/transports/udp6.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/transports/ws.py` & `coapts-0.0.9/src/coapts/transports/ws.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/util/__init__.py` & `coapts-0.0.9/src/coapts/util/__init__.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/util/asyncio/getaddrinfo_addrconfig.py` & `coapts-0.0.9/src/coapts/util/asyncio/getaddrinfo_addrconfig.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/util/asyncio/recvmsg.py` & `coapts-0.0.9/src/coapts/util/asyncio/recvmsg.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/util/asyncio/timeoutdict.py` & `coapts-0.0.9/src/coapts/util/asyncio/timeoutdict.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/util/cli.py` & `coapts-0.0.9/src/coapts/util/cli.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/util/contenttype.py` & `coapts-0.0.9/src/coapts/util/contenttype.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/util/cryptography_additions.py` & `coapts-0.0.9/src/coapts/util/cryptography_additions.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/util/linkformat.py` & `coapts-0.0.9/src/coapts/util/linkformat.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/util/linkformat_pygments.py` & `coapts-0.0.9/src/coapts/util/linkformat_pygments.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/util/prettyprint.py` & `coapts-0.0.9/src/coapts/util/prettyprint.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/util/pyodide_websockets.py` & `coapts-0.0.9/src/coapts/util/pyodide_websockets.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/util/socknumbers.py` & `coapts-0.0.9/src/coapts/util/socknumbers.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/util/uri.py` & `coapts-0.0.9/src/coapts/util/uri.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts/util/vendored/link_header.py` & `coapts-0.0.9/src/coapts/util/vendored/link_header.py`

 * *Files identical despite different names*

### Comparing `coapts-0.0.8/src/coapts.egg-info/PKG-INFO` & `coapts-0.0.9/src/coapts.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coapts
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python aiocoap dialect: CoAP Type Shuffling 
 Author-email: Erik Gonzalez <erikglez_ipn@hotmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ErikGlz/coapts
 Keywords: coap,asyncio,iot
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `coapts-0.0.8/src/coapts.egg-info/SOURCES.txt` & `coapts-0.0.9/src/coapts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

