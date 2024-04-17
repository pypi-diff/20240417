# Comparing `tmp/arion_library-1.1rc64.dev64.tar.gz` & `tmp/arion_library-1.1rc65.dev65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc64.dev64.tar", last modified: Mon Apr 15 16:11:14 2024, max compression
+gzip compressed data, was "arion_library-1.1rc65.dev65.tar", last modified: Wed Apr 17 11:23:08 2024, max compression
```

## Comparing `arion_library-1.1rc64.dev64.tar` & `arion_library-1.1rc65.dev65.tar`

### file list

```diff
@@ -1,55 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.618125 arion_library-1.1rc64.dev64/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 16:11:14.618125 arion_library-1.1rc64.dev64/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.614125 arion_library-1.1rc64.dev64/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 16:11:14.000000 arion_library-1.1rc64.dev64/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-15 16:11:14.000000 arion_library-1.1rc64.dev64/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:11:14.000000 arion_library-1.1rc64.dev64/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-15 16:11:14.000000 arion_library-1.1rc64.dev64/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 16:11:14.000000 arion_library-1.1rc64.dev64/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.614125 arion_library-1.1rc64.dev64/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.614125 arion_library-1.1rc64.dev64/processors/FTP_connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/FTP_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.614125 arion_library-1.1rc64.dev64/processors/FTP_connector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/FTP_connector/lib/FTPconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/FTP_connector/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.614125 arion_library-1.1rc64.dev64/processors/FTP_connector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/FTP_connector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/FTP_connector/tests/test_ftp_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.614125 arion_library-1.1rc64.dev64/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.614125 arion_library-1.1rc64.dev64/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.614125 arion_library-1.1rc64.dev64/processors/SFTP/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/SFTP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/SFTP/tests/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.614125 arion_library-1.1rc64.dev64/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.614125 arion_library-1.1rc64.dev64/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/TableStorage/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.614125 arion_library-1.1rc64.dev64/processors/TableStorage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/TableStorage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/TableStorage/tests/test_table_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.614125 arion_library-1.1rc64.dev64/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.614125 arion_library-1.1rc64.dev64/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3086 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.614125 arion_library-1.1rc64.dev64/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.614125 arion_library-1.1rc64.dev64/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.618125 arion_library-1.1rc64.dev64/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:11:14.618125 arion_library-1.1rc64.dev64/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-15 16:10:41.000000 arion_library-1.1rc64.dev64/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:11:14.618125 arion_library-1.1rc64.dev64/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-15 16:11:13.000000 arion_library-1.1rc64.dev64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.911776 arion_library-1.1rc65.dev65/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-17 11:23:08.911776 arion_library-1.1rc65.dev65/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.907776 arion_library-1.1rc65.dev65/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-17 11:23:08.000000 arion_library-1.1rc65.dev65/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-17 11:23:08.000000 arion_library-1.1rc65.dev65/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:23:08.000000 arion_library-1.1rc65.dev65/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-17 11:23:08.000000 arion_library-1.1rc65.dev65/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 11:23:08.000000 arion_library-1.1rc65.dev65/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.907776 arion_library-1.1rc65.dev65/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.907776 arion_library-1.1rc65.dev65/processors/FTP_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/FTP_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.907776 arion_library-1.1rc65.dev65/processors/FTP_connector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/FTP_connector/lib/FTPconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/FTP_connector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.907776 arion_library-1.1rc65.dev65/processors/FTP_connector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/FTP_connector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/FTP_connector/tests/test_ftp_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.907776 arion_library-1.1rc65.dev65/processors/OracleConnector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/OracleConnector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.907776 arion_library-1.1rc65.dev65/processors/OracleConnector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/OracleConnector/lib/OracleDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/OracleConnector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.907776 arion_library-1.1rc65.dev65/processors/OracleConnector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/OracleConnector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/OracleConnector/tests/test_oracle_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.911776 arion_library-1.1rc65.dev65/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.911776 arion_library-1.1rc65.dev65/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.911776 arion_library-1.1rc65.dev65/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.911776 arion_library-1.1rc65.dev65/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.911776 arion_library-1.1rc65.dev65/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.911776 arion_library-1.1rc65.dev65/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.911776 arion_library-1.1rc65.dev65/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.911776 arion_library-1.1rc65.dev65/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3086 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.911776 arion_library-1.1rc65.dev65/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.911776 arion_library-1.1rc65.dev65/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.911776 arion_library-1.1rc65.dev65/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:23:08.911776 arion_library-1.1rc65.dev65/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-17 11:22:04.000000 arion_library-1.1rc65.dev65/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 11:23:08.911776 arion_library-1.1rc65.dev65/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-17 11:23:01.000000 arion_library-1.1rc65.dev65/setup.py
```

### Comparing `arion_library-1.1rc64.dev64/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc65.dev65/arion_library.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 arion_library.egg-info/top_level.txt
 processors/__init__.py
 processors/FTP_connector/__init__.py
 processors/FTP_connector/lib/FTPconnector.py
 processors/FTP_connector/lib/__init__.py
 processors/FTP_connector/tests/__init__.py
 processors/FTP_connector/tests/test_ftp_connector.py
+processors/OracleConnector/__init__.py
+processors/OracleConnector/lib/OracleDatabase.py
+processors/OracleConnector/lib/__init__.py
+processors/OracleConnector/tests/__init__.py
+processors/OracleConnector/tests/test_oracle_connector.py
 processors/SFTP/__init__.py
 processors/SFTP/lib/__init__.py
 processors/SFTP/lib/sftp.py
 processors/SFTP/tests/__init__.py
 processors/SFTP/tests/test_sftp.py
 processors/TableStorage/__init__.py
 processors/TableStorage/lib/TableStorage.py
```

### Comparing `arion_library-1.1rc64.dev64/processors/FTP_connector/lib/FTPconnector.py` & `arion_library-1.1rc65.dev65/processors/FTP_connector/lib/FTPconnector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc64.dev64/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc65.dev65/processors/SFTP/lib/sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc64.dev64/processors/SFTP/tests/test_sftp.py` & `arion_library-1.1rc65.dev65/processors/SFTP/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc64.dev64/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc65.dev65/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc64.dev64/processors/TableStorage/tests/test_table_storage.py` & `arion_library-1.1rc65.dev65/processors/TableStorage/tests/test_table_storage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc64.dev64/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc65.dev65/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc64.dev64/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc65.dev65/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc64.dev64/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc65.dev65/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc64.dev64/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc65.dev65/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc64.dev64/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc65.dev65/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc64.dev64/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc65.dev65/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc64.dev64/setup.py` & `arion_library-1.1rc65.dev65/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='arion_library',  # Replace with your package name
-    version='1.1rc64.dev64',  # Replace with your package version
+    version='1.1rc65.dev65',  # Replace with your package version
     author='Heni Nechi',  # Replace with your name
     author_email='h.nechi@arion-tech.com',  # Replace with your email
     url='https://github.com/Ariontech/ArionLibrary.git',  # Replace with your repository URL
     packages=find_packages(),  # Automatically find all packages
     python_requires='>=3.8',  # Specify Python version requirements
     install_requires=['pysftp==0.2.9', 'azure-core==1.29.6', 'azure-data-tables==12.5.0', 'azure-storage-blob==12.19.1', 'python-dotenv==1.0.1', 'pytest==8.1.1', 'pandas==2.0.3', 'pytest'],
 )
```

