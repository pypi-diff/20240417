# Comparing `tmp/sesql-2024.4.0.tar.gz` & `tmp/sesql-2024.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sesql-2024.4.0.tar", last modified: Tue Apr  2 00:44:56 2024, max compression
+gzip compressed data, was "sesql-2024.4.1rc1.tar", last modified: Wed Apr 17 00:37:13 2024, max compression
```

## Comparing `sesql-2024.4.0.tar` & `sesql-2024.4.1rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-02 00:44:56.075851 sesql-2024.4.0/
--rw-r--r--   0 rjd        (501) staff       (20)     1078 2023-12-26 02:50:39.000000 sesql-2024.4.0/License.md
--rw-r--r--   0 rjd        (501) staff       (20)     5894 2024-04-02 00:44:56.075651 sesql-2024.4.0/PKG-INFO
--rw-r--r--   0 rjd        (501) staff       (20)     4234 2024-04-02 00:43:29.000000 sesql-2024.4.0/ReadMe.md
--rw-r--r--   0 rjd        (501) staff       (20)      808 2024-03-31 00:07:50.000000 sesql-2024.4.0/pyproject.toml
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-02 00:44:56.069751 sesql-2024.4.0/seCore/
--rw-r--r--   0 rjd        (501) staff       (20)      839 2024-03-30 23:03:58.000000 sesql-2024.4.0/seCore/CustomLogging.py
--rw-r--r--   0 rjd        (501) staff       (20)        0 2024-03-17 19:54:29.000000 sesql-2024.4.0/seCore/__init__.py
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-02 00:44:56.070060 sesql-2024.4.0/seSql/
--rw-r--r--   0 rjd        (501) staff       (20)      280 2024-04-01 23:44:41.000000 sesql-2024.4.0/seSql/__init__.py
--rw-r--r--   0 rjd        (501) staff       (20)      295 2024-04-02 00:44:53.000000 sesql-2024.4.0/seSql/_version.py
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-02 00:44:56.070832 sesql-2024.4.0/seSql/dbc/
--rw-r--r--   0 rjd        (501) staff       (20)     2383 2024-03-03 23:41:30.000000 sesql-2024.4.0/seSql/dbc/Exceptions.py
--rw-r--r--   0 rjd        (501) staff       (20)     7393 2024-04-01 01:51:00.000000 sesql-2024.4.0/seSql/dbc/JDBC.py
--rw-r--r--   0 rjd        (501) staff       (20)     6868 2024-04-01 01:54:33.000000 sesql-2024.4.0/seSql/dbc/ODBC.py
--rw-r--r--   0 rjd        (501) staff       (20)     5936 2024-02-29 01:59:07.000000 sesql-2024.4.0/seSql/dbc/ODBCError.py
--rw-r--r--   0 rjd        (501) staff       (20)      726 2024-04-01 01:40:37.000000 sesql-2024.4.0/seSql/dbc/Utilities.py
--rw-r--r--   0 rjd        (501) staff       (20)        0 2024-03-17 19:54:29.000000 sesql-2024.4.0/seSql/dbc/__init__.py
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-02 00:44:56.070927 sesql-2024.4.0/seSql/dbc/jars/
--rw-r--r--   0 rjd        (501) staff       (20)  1438398 2024-03-01 01:47:02.000000 sesql-2024.4.0/seSql/dbc/jars/mssql-jdbc-12.4.2.jre8.jar
--rw-r--r--   0 rjd        (501) staff       (20)     4183 2024-04-02 00:13:12.000000 sesql-2024.4.0/seSql/sql.py
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-02 00:44:56.075430 sesql-2024.4.0/sesql.egg-info/
--rw-r--r--   0 rjd        (501) staff       (20)     5894 2024-04-02 00:44:56.000000 sesql-2024.4.0/sesql.egg-info/PKG-INFO
--rw-r--r--   0 rjd        (501) staff       (20)      556 2024-04-02 00:44:56.000000 sesql-2024.4.0/sesql.egg-info/SOURCES.txt
--rw-r--r--   0 rjd        (501) staff       (20)        1 2024-04-02 00:44:56.000000 sesql-2024.4.0/sesql.egg-info/dependency_links.txt
--rw-r--r--   0 rjd        (501) staff       (20)       56 2024-04-02 00:44:56.000000 sesql-2024.4.0/sesql.egg-info/requires.txt
--rw-r--r--   0 rjd        (501) staff       (20)       13 2024-04-02 00:44:56.000000 sesql-2024.4.0/sesql.egg-info/top_level.txt
--rw-r--r--   0 rjd        (501) staff       (20)       38 2024-04-02 00:44:56.075900 sesql-2024.4.0/setup.cfg
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-02 00:44:56.075126 sesql-2024.4.0/tests/
--rw-r--r--   0 rjd        (501) staff       (20)     1790 2024-03-31 01:39:23.000000 sesql-2024.4.0/tests/test_Exceptions.py
--rw-r--r--   0 rjd        (501) staff       (20)      222 2024-03-31 23:51:30.000000 sesql-2024.4.0/tests/test_customlogging.py
--rw-r--r--   0 rjd        (501) staff       (20)      987 2024-04-01 01:44:20.000000 sesql-2024.4.0/tests/test_jdbc.py
--rw-r--r--   0 rjd        (501) staff       (20)      690 2024-04-01 01:35:26.000000 sesql-2024.4.0/tests/test_odbc.py
--rw-r--r--   0 rjd        (501) staff       (20)      238 2024-04-01 01:39:41.000000 sesql-2024.4.0/tests/test_utilities.py
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-17 00:37:13.694845 sesql-2024.4.1rc1/
+-rw-r--r--   0 rjd        (501) staff       (20)     1078 2023-12-26 02:50:39.000000 sesql-2024.4.1rc1/License.md
+-rw-r--r--   0 rjd        (501) staff       (20)     6507 2024-04-17 00:37:13.694640 sesql-2024.4.1rc1/PKG-INFO
+-rw-r--r--   0 rjd        (501) staff       (20)     4844 2024-04-17 00:36:16.000000 sesql-2024.4.1rc1/ReadMe.md
+-rw-r--r--   0 rjd        (501) staff       (20)      808 2024-03-31 00:07:50.000000 sesql-2024.4.1rc1/pyproject.toml
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-17 00:37:13.687099 sesql-2024.4.1rc1/seCore/
+-rw-r--r--   0 rjd        (501) staff       (20)      839 2024-03-30 23:03:58.000000 sesql-2024.4.1rc1/seCore/CustomLogging.py
+-rw-r--r--   0 rjd        (501) staff       (20)        0 2024-03-17 19:54:29.000000 sesql-2024.4.1rc1/seCore/__init__.py
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-17 00:37:13.687412 sesql-2024.4.1rc1/seSql/
+-rw-r--r--   0 rjd        (501) staff       (20)      280 2024-04-01 23:44:41.000000 sesql-2024.4.1rc1/seSql/__init__.py
+-rw-r--r--   0 rjd        (501) staff       (20)      316 2024-04-17 00:37:11.000000 sesql-2024.4.1rc1/seSql/_version.py
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-17 00:37:13.689452 sesql-2024.4.1rc1/seSql/dbc/
+-rw-r--r--   0 rjd        (501) staff       (20)     2383 2024-03-03 23:41:30.000000 sesql-2024.4.1rc1/seSql/dbc/Exceptions.py
+-rw-r--r--   0 rjd        (501) staff       (20)     7673 2024-04-16 01:10:44.000000 sesql-2024.4.1rc1/seSql/dbc/JDBC.py
+-rw-r--r--   0 rjd        (501) staff       (20)     7329 2024-04-16 19:43:40.000000 sesql-2024.4.1rc1/seSql/dbc/ODBC.py
+-rw-r--r--   0 rjd        (501) staff       (20)     5936 2024-02-29 01:59:07.000000 sesql-2024.4.1rc1/seSql/dbc/ODBCError.py
+-rw-r--r--   0 rjd        (501) staff       (20)      726 2024-04-01 01:40:37.000000 sesql-2024.4.1rc1/seSql/dbc/Utilities.py
+-rw-r--r--   0 rjd        (501) staff       (20)        0 2024-03-17 19:54:29.000000 sesql-2024.4.1rc1/seSql/dbc/__init__.py
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-17 00:37:13.689566 sesql-2024.4.1rc1/seSql/dbc/jars/
+-rw-r--r--   0 rjd        (501) staff       (20)  1438398 2024-03-01 01:47:02.000000 sesql-2024.4.1rc1/seSql/dbc/jars/mssql-jdbc-12.4.2.jre8.jar
+-rw-r--r--   0 rjd        (501) staff       (20)     4303 2024-04-16 02:19:23.000000 sesql-2024.4.1rc1/seSql/sql.py
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-17 00:37:13.694375 sesql-2024.4.1rc1/sesql.egg-info/
+-rw-r--r--   0 rjd        (501) staff       (20)     6507 2024-04-17 00:37:13.000000 sesql-2024.4.1rc1/sesql.egg-info/PKG-INFO
+-rw-r--r--   0 rjd        (501) staff       (20)      556 2024-04-17 00:37:13.000000 sesql-2024.4.1rc1/sesql.egg-info/SOURCES.txt
+-rw-r--r--   0 rjd        (501) staff       (20)        1 2024-04-17 00:37:13.000000 sesql-2024.4.1rc1/sesql.egg-info/dependency_links.txt
+-rw-r--r--   0 rjd        (501) staff       (20)       56 2024-04-17 00:37:13.000000 sesql-2024.4.1rc1/sesql.egg-info/requires.txt
+-rw-r--r--   0 rjd        (501) staff       (20)       13 2024-04-17 00:37:13.000000 sesql-2024.4.1rc1/sesql.egg-info/top_level.txt
+-rw-r--r--   0 rjd        (501) staff       (20)       38 2024-04-17 00:37:13.694882 sesql-2024.4.1rc1/setup.cfg
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-17 00:37:13.694177 sesql-2024.4.1rc1/tests/
+-rw-r--r--   0 rjd        (501) staff       (20)     1790 2024-03-31 01:39:23.000000 sesql-2024.4.1rc1/tests/test_Exceptions.py
+-rw-r--r--   0 rjd        (501) staff       (20)      222 2024-03-31 23:51:30.000000 sesql-2024.4.1rc1/tests/test_customlogging.py
+-rw-r--r--   0 rjd        (501) staff       (20)      987 2024-04-01 01:44:20.000000 sesql-2024.4.1rc1/tests/test_jdbc.py
+-rw-r--r--   0 rjd        (501) staff       (20)      690 2024-04-01 01:35:26.000000 sesql-2024.4.1rc1/tests/test_odbc.py
+-rw-r--r--   0 rjd        (501) staff       (20)      238 2024-04-01 01:39:41.000000 sesql-2024.4.1rc1/tests/test_utilities.py
```

### Comparing `sesql-2024.4.0/License.md` & `sesql-2024.4.1rc1/License.md`

 * *Files identical despite different names*

### Comparing `sesql-2024.4.0/PKG-INFO` & `sesql-2024.4.1rc1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sesql
-Version: 2024.4.0
+Version: 2024.4.1rc1
 Summary: CLI to enhance versioning for Python projects
 Author-email: Cybernetic Innovations <github@cyberneticinnovations.com>
 License: MIT License
         
         Copyright (c) 2024 Cybernetic Innovations
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,75 +39,76 @@
 
 ## Install
 ```shell
 pip install seSql
 ```
 
 ## Usage
-### connect, query
-- **_using JDBC_**
+
+### **_using JDBC/ODBC_**
 ```python
 from seSql import sql, logger
 
 if __name__ == '__main__':
     oSql = sql()
     oSql.connect(
         server="SQL.site4now.net",
         port=1433,
         user="db_user",
         password="{pw}",
         trust="no",
-        driverOverride="jdbc"
+        driverOverride="odbc",      # options: odbc/jdbc
+        mars="no"                   # option to use MARS but only works with ODBC, ignored with JDBC
+        
     )
     if oSql.isConnected:
+        # request sql version without try/except
+        oSql.query("select @@version as version")
+        
+        # request sql version with try/except: typo that will generate an exception
         try:
-            oSql.query("select @@version as version;")
             oSql.query("select @@versions as version;")
         except Exception as e:
             logger.error(f'Exception: {e}')
-```
 
-- **_using JDBC_ - output**
-```shell
-2024-04-01 00:00:00 | seSql | INFO     | {"driver-info": {"using": "jdbc", "odbc": {"loaded": true, "driver": "ODBC Driver 18 for SQL Server"}, "jdbc": {"loaded": true, "driver": "mssql-12.4.2"}}}
-2024-04-01 00:00:00 | seSql | INFO     | {"jdbc-connect": {"connection_ms": 889.3, "connected": true, "connStr": {"driver": "mssql-12.4.2", "server": "jdbc:sqlserver://SQL.site4now.net", "port": 1433, "database": "", "user": "db_user", "password": "**********mee68", "encrypt": true, "trustServerCertificate": true}}}
-2024-04-01 00:00:00 | seSql | INFO     | {"jdbc-query": {"connection_ms": 104.95, "query": "select @@version as version;"}}
-2024-04-01 00:00:00 | seSql | ERROR    | {"jdbc-query": {"connection_ms": 59.0, "query": "select @@versions as version;", "error": "com.microsoft.sqlserver.jdbc.SQLServerException: Must declare the scalar variable \"@@versions\"."}}
-2024-04-01 00:00:00 | seSql | ERROR    | Exception: com.microsoft.sqlserver.jdbc.SQLServerException: Must declare the scalar variable "@@versions".
-```
+        # select
+        try:
+            oSql.query("select * from dbo.winequality_red;")
+        except Exception as e:
+            logger.error(f'Exception: {e}')
 
-### connect, query
-- **_using ODBC_**
-```python
-from seSql import sql, logger
+        # insert
+        try:
+            oSql.query("insert into dbo.seSql_Settings ([key], value) values ('Env', 'test');")
+        except Exception as e:
+            logger.error(f'Exception: {e}')
 
-if __name__ == '__main__':
-    oSql = sql()
-    oSql.connect(
-        server="SQL.site4now.net",
-        port=1433,
-        user="db_user",
-        password="{pw}",
-        trust="no",
-        driverOverride="odbc"
-    )
-    if oSql.isConnected:
+        # delete
         try:
-            oSql.query("select @@version as version;")
-            oSql.query("select @@versions as version;")
+            oSql.query("delete from dbo.seSql_Settings where value like '%dev';")
+        except Exception as e:
+            logger.error(f'Exception: {e}')
+
+        # update
+        try:
+            oSql.query("update dbo.seSql_Settings set value = 'false' where [key] like '%Updated';")
         except Exception as e:
             logger.error(f'Exception: {e}')
 ```
-- **_using ODBC_ - output**
+### **_output_**
 ```shell
-2024-04-01 00:00:00 | seSql | INFO     | {"driver-info": {"using": "odbc", "odbc": {"loaded": true, "driver": "ODBC Driver 18 for SQL Server"}, "jdbc": {"loaded": true, "driver": "mssql-12.4.2"}}}
-2024-04-01 00:00:00 | seSql | INFO     | {"odbc-connect": {"connection_ms": 781.27, "connected": true, "connStr": {"driver": "ODBC Driver 18 for SQL Server", "server": "SQL.site4now.net", "port": 1433, "database": "", "user": "db_user", "password": "**********mee68", "trust": "no"}}}
-2024-04-01 00:00:00 | seSql | INFO     | {"odbc-query": {"connection_ms": 56.09, "query": "select @@version as version;"}}
-2024-04-01 00:00:00 | seSql | ERROR    | {"odbc-query": {"connection_ms": 56.53, "query": "select @@versions as version;", "error": "('42000', '[42000] [Microsoft][ODBC Driver 18 for SQL Server][SQL Server]Must declare the scalar variable \"@@versions\". (137) (SQLExecDirectW)')"}}
-2024-04-01 00:00:00 | seSql | ERROR    | Exception: ('42000', '[42000] [Microsoft][ODBC Driver 18 for SQL Server][SQL Server]Must declare the scalar variable "@@versions". (137) (SQLExecDirectW)')
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"driver-info": {"using": "odbc", "odbc": {"loaded": true, "driver": "ODBC Driver 18 for SQL Server"}, "jdbc": {"loaded": true, "driver": "mssql-12.4.2"}}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-connect": {"connection_ms": 711.46, "connected": true, "connStr": {"driver": "ODBC Driver 18 for SQL Server", "server": "SQL5101.site4now.net", "port": 1433, "database": "", "user": "db_user", "password": "**********mee68", "trust": "no", "mars": "no"}}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-query": {"connection_ms": 56.32, "rc": "-1:1", "query": "select @@version as version"}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | ERROR    | {"odbc-query": {"connection_ms": 56.74, "query": "select @@versions as version;", "error": "('42000', '[42000] [Microsoft][ODBC Driver 18 for SQL Server][SQL Server]Must declare the scalar variable \"@@versions\". (137) (SQLExecDirectW)')"}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | ERROR    | Exception: ('42000', '[42000] [Microsoft][ODBC Driver 18 for SQL Server][SQL Server]Must declare the scalar variable "@@versions". (137) (SQLExecDirectW)')
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-query": {"connection_ms": 250.5, "rc": "-1:1599", "query": "select * from dbo.winequality_red;"}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-query": {"connection_ms": 57.83, "rc": "1:1", "query": "insert into dbo.seSql_Settings ([key], value) values ('Env', 'test');"}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-query": {"connection_ms": 56.38, "rc": "0:0", "query": "delete from dbo.seSql_Settings where value like '%dev';"}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-query": {"connection_ms": 56.96, "rc": "1:1", "query": "update dbo.seSql_Settings set value = 'false' where [key] like '%Updated';"}}
 ```
 
 ### hostName, hostIP, mask, seSqlVersion
 ```python
 import json
 from seSql import mask, seSqlVersion, hostName, hostIP, logger
 
@@ -119,17 +120,17 @@
             'mask_all_but_last_12345': mask('all_but_last_12345'),
             'version': seSqlVersion
         }
     }, indent=4))
 ```
 - output
 ```shell
-2024-04-01 00:00:00 | seSql | INFO     | {
+2024-04-15 00:00:00 | seSql | INFO     | {
     "seSql-info": {
         "host": "MacBook-Pro",
         "hostIP": "127.0.0.1",
         "mask_all_but_last_12345": "*************12345",
-        "version": "2024.4.0 build[59]"
+        "version": "2024.4.1 build[68]"
     }
 }
 
 ```
```

### Comparing `sesql-2024.4.0/ReadMe.md` & `sesql-2024.4.1rc1/ReadMe.md`

 * *Files 21% similar despite different names*

```diff
@@ -5,75 +5,76 @@
 
 ## Install
 ```shell
 pip install seSql
 ```
 
 ## Usage
-### connect, query
-- **_using JDBC_**
+
+### **_using JDBC/ODBC_**
 ```python
 from seSql import sql, logger
 
 if __name__ == '__main__':
     oSql = sql()
     oSql.connect(
         server="SQL.site4now.net",
         port=1433,
         user="db_user",
         password="{pw}",
         trust="no",
-        driverOverride="jdbc"
+        driverOverride="odbc",      # options: odbc/jdbc
+        mars="no"                   # option to use MARS but only works with ODBC, ignored with JDBC
+        
     )
     if oSql.isConnected:
+        # request sql version without try/except
+        oSql.query("select @@version as version")
+        
+        # request sql version with try/except: typo that will generate an exception
         try:
-            oSql.query("select @@version as version;")
             oSql.query("select @@versions as version;")
         except Exception as e:
             logger.error(f'Exception: {e}')
-```
 
-- **_using JDBC_ - output**
-```shell
-2024-04-01 00:00:00 | seSql | INFO     | {"driver-info": {"using": "jdbc", "odbc": {"loaded": true, "driver": "ODBC Driver 18 for SQL Server"}, "jdbc": {"loaded": true, "driver": "mssql-12.4.2"}}}
-2024-04-01 00:00:00 | seSql | INFO     | {"jdbc-connect": {"connection_ms": 889.3, "connected": true, "connStr": {"driver": "mssql-12.4.2", "server": "jdbc:sqlserver://SQL.site4now.net", "port": 1433, "database": "", "user": "db_user", "password": "**********mee68", "encrypt": true, "trustServerCertificate": true}}}
-2024-04-01 00:00:00 | seSql | INFO     | {"jdbc-query": {"connection_ms": 104.95, "query": "select @@version as version;"}}
-2024-04-01 00:00:00 | seSql | ERROR    | {"jdbc-query": {"connection_ms": 59.0, "query": "select @@versions as version;", "error": "com.microsoft.sqlserver.jdbc.SQLServerException: Must declare the scalar variable \"@@versions\"."}}
-2024-04-01 00:00:00 | seSql | ERROR    | Exception: com.microsoft.sqlserver.jdbc.SQLServerException: Must declare the scalar variable "@@versions".
-```
+        # select
+        try:
+            oSql.query("select * from dbo.winequality_red;")
+        except Exception as e:
+            logger.error(f'Exception: {e}')
 
-### connect, query
-- **_using ODBC_**
-```python
-from seSql import sql, logger
+        # insert
+        try:
+            oSql.query("insert into dbo.seSql_Settings ([key], value) values ('Env', 'test');")
+        except Exception as e:
+            logger.error(f'Exception: {e}')
 
-if __name__ == '__main__':
-    oSql = sql()
-    oSql.connect(
-        server="SQL.site4now.net",
-        port=1433,
-        user="db_user",
-        password="{pw}",
-        trust="no",
-        driverOverride="odbc"
-    )
-    if oSql.isConnected:
+        # delete
         try:
-            oSql.query("select @@version as version;")
-            oSql.query("select @@versions as version;")
+            oSql.query("delete from dbo.seSql_Settings where value like '%dev';")
+        except Exception as e:
+            logger.error(f'Exception: {e}')
+
+        # update
+        try:
+            oSql.query("update dbo.seSql_Settings set value = 'false' where [key] like '%Updated';")
         except Exception as e:
             logger.error(f'Exception: {e}')
 ```
-- **_using ODBC_ - output**
+### **_output_**
 ```shell
-2024-04-01 00:00:00 | seSql | INFO     | {"driver-info": {"using": "odbc", "odbc": {"loaded": true, "driver": "ODBC Driver 18 for SQL Server"}, "jdbc": {"loaded": true, "driver": "mssql-12.4.2"}}}
-2024-04-01 00:00:00 | seSql | INFO     | {"odbc-connect": {"connection_ms": 781.27, "connected": true, "connStr": {"driver": "ODBC Driver 18 for SQL Server", "server": "SQL.site4now.net", "port": 1433, "database": "", "user": "db_user", "password": "**********mee68", "trust": "no"}}}
-2024-04-01 00:00:00 | seSql | INFO     | {"odbc-query": {"connection_ms": 56.09, "query": "select @@version as version;"}}
-2024-04-01 00:00:00 | seSql | ERROR    | {"odbc-query": {"connection_ms": 56.53, "query": "select @@versions as version;", "error": "('42000', '[42000] [Microsoft][ODBC Driver 18 for SQL Server][SQL Server]Must declare the scalar variable \"@@versions\". (137) (SQLExecDirectW)')"}}
-2024-04-01 00:00:00 | seSql | ERROR    | Exception: ('42000', '[42000] [Microsoft][ODBC Driver 18 for SQL Server][SQL Server]Must declare the scalar variable "@@versions". (137) (SQLExecDirectW)')
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"driver-info": {"using": "odbc", "odbc": {"loaded": true, "driver": "ODBC Driver 18 for SQL Server"}, "jdbc": {"loaded": true, "driver": "mssql-12.4.2"}}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-connect": {"connection_ms": 711.46, "connected": true, "connStr": {"driver": "ODBC Driver 18 for SQL Server", "server": "SQL5101.site4now.net", "port": 1433, "database": "", "user": "db_user", "password": "**********mee68", "trust": "no", "mars": "no"}}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-query": {"connection_ms": 56.32, "rc": "-1:1", "query": "select @@version as version"}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | ERROR    | {"odbc-query": {"connection_ms": 56.74, "query": "select @@versions as version;", "error": "('42000', '[42000] [Microsoft][ODBC Driver 18 for SQL Server][SQL Server]Must declare the scalar variable \"@@versions\". (137) (SQLExecDirectW)')"}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | ERROR    | Exception: ('42000', '[42000] [Microsoft][ODBC Driver 18 for SQL Server][SQL Server]Must declare the scalar variable "@@versions". (137) (SQLExecDirectW)')
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-query": {"connection_ms": 250.5, "rc": "-1:1599", "query": "select * from dbo.winequality_red;"}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-query": {"connection_ms": 57.83, "rc": "1:1", "query": "insert into dbo.seSql_Settings ([key], value) values ('Env', 'test');"}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-query": {"connection_ms": 56.38, "rc": "0:0", "query": "delete from dbo.seSql_Settings where value like '%dev';"}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-query": {"connection_ms": 56.96, "rc": "1:1", "query": "update dbo.seSql_Settings set value = 'false' where [key] like '%Updated';"}}
 ```
 
 ### hostName, hostIP, mask, seSqlVersion
 ```python
 import json
 from seSql import mask, seSqlVersion, hostName, hostIP, logger
 
@@ -85,17 +86,17 @@
             'mask_all_but_last_12345': mask('all_but_last_12345'),
             'version': seSqlVersion
         }
     }, indent=4))
 ```
 - output
 ```shell
-2024-04-01 00:00:00 | seSql | INFO     | {
+2024-04-15 00:00:00 | seSql | INFO     | {
     "seSql-info": {
         "host": "MacBook-Pro",
         "hostIP": "127.0.0.1",
         "mask_all_but_last_12345": "*************12345",
-        "version": "2024.4.0 build[59]"
+        "version": "2024.4.1 build[68]"
     }
 }
 
 ```
```

### Comparing `sesql-2024.4.0/pyproject.toml` & `sesql-2024.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sesql-2024.4.0/seCore/CustomLogging.py` & `sesql-2024.4.1rc1/seCore/CustomLogging.py`

 * *Files identical despite different names*

### Comparing `sesql-2024.4.0/seSql/dbc/Exceptions.py` & `sesql-2024.4.1rc1/seSql/dbc/Exceptions.py`

 * *Files identical despite different names*

### Comparing `sesql-2024.4.0/seSql/dbc/JDBC.py` & `sesql-2024.4.1rc1/seSql/dbc/JDBC.py`

 * *Files 5% similar despite different names*

```diff
@@ -157,23 +157,28 @@
 
     def query(self, query: str):
         if self.isConnected:
             start_time = time.time()
             try:
                 with self.__cnxn.cursor() as curs:
                     curs.execute(query)
-                    r = [dict((curs.description[i][0], value)
-                              for i, value in enumerate(row)) for row in curs.fetchall()]
-
-                logger.info(json.dumps({
-                    f'jdbc-{inspect.currentframe().f_code.co_name}': {
-                        'connection_ms': float(f'{(time.time() - start_time) * 1000:.2f}'),
-                        'query': f'{query}'
-                    }}))
+                    if curs.rowcount == -1:
+                        r = [dict((curs.description[i][0], value)
+                                  for i, value in enumerate(row)) for row in curs.fetchall()]
+                        rCount = len(r)
+                    else:
+                        r = None
+                        rCount = curs.rowcount
 
+                    logger.info(json.dumps({
+                        f'jdbc-{inspect.currentframe().f_code.co_name}': {
+                            'connection_ms': float(f'{(time.time() - start_time) * 1000:.2f}'),
+                            'rc': f'{curs.rowcount}:{rCount}',
+                            'query': f'{query}'
+                        }}))
                 return r
             except Exception as e:
                 logger.error(json.dumps({
                     f'jdbc-{inspect.currentframe().f_code.co_name}': {
                         'connection_ms': float(f'{(time.time() - start_time) * 1000:.2f}'),
                         'query': f'{query}',
                         'error': f'{e}'
```

### Comparing `sesql-2024.4.0/seSql/dbc/ODBC.py` & `sesql-2024.4.1rc1/seSql/dbc/ODBC.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,26 +51,27 @@
 
     except Exception:  # pragma: no cover
         return "Error finding ODBC driver"
 
 
 class odbcEngine:
 
-    def __init__(self, server: str, port: int, user: str, password: str, trust: str, db: str = ""):
+    def __init__(self, server: str, port: int, user: str, password: str, trust: str, mars: str, db: str = "") -> None:
         """
         Initialize the odbcEngine object
         """
         self.__connStr = {
             "driver": odbcDriver(),
             "server": server,
             "port": port,
             "database": db,
             "user": user,
             "password": password,
-            "trust": trust
+            "trust": trust,
+            "mars": mars
         }
         self.isConnected = False
         self.__cnxn = None
 
     def connect(self):
         """
         Connect to database using pyodbc and ODBC Driver 17 or 18 for SQL Server
@@ -80,30 +81,32 @@
         match self.__connStr["trust"]:
             case "yes":
                 connStr = f'DRIVER={{{self.__connStr["driver"]}}}; ' \
                           f'Server={self.__connStr["server"]},{self.__connStr["port"]}; ' \
                           f'DATABASE={self.__connStr["database"]}; ' \
                           f'UID={self.__connStr["user"]}; ' \
                           f'PWD={self.__connStr["password"]}; ' \
-                          f'Trusted_Connection={self.__connStr["trust"]};'
+                          f'Trusted_Connection={self.__connStr["trust"]};'\
+                          f'MARS_Connection={self.__connStr["mars"]};'
             case _:
                 connStr = f'DRIVER={{{self.__connStr["driver"]}}}; ' \
                           f'Server={self.__connStr["server"]},{self.__connStr["port"]}; ' \
                           f'DATABASE={self.__connStr["database"]}; ' \
                           f'UID={self.__connStr["user"]}; ' \
-                          f'PWD={self.__connStr["password"]};'
+                          f'PWD={self.__connStr["password"]};' \
+                          f'MARS_Connection={self.__connStr["mars"]};'
 
         oJson = {
             f'odbc-{inspect.currentframe().f_code.co_name}': {
                 'connection_ms': float(f'{0 * 1000:.2f}'),
                 'connected': self.isConnected,
                 'connStr': self.__connStr
             }}
         try:
-            with pyodbc.connect(connStr, timeout=1) as cnxn:
+            with pyodbc.connect(connStr, timeout=1, autocommit=False) as cnxn:
                 self.__cnxn = cnxn
                 self.isConnected = True
                 oJson[f'odbc-{inspect.currentframe().f_code.co_name}']['connected'] = self.isConnected
 
         except pyodbc.Error as ex:  # pragma: no cover
             oJson = {
                 f'odbc-{inspect.currentframe().f_code.co_name}': {
@@ -142,23 +145,28 @@
 
     def query(self, query: str):
         if self.isConnected:
             start_time = time.time()
             try:
                 with self.__cnxn.cursor() as cur:
                     cur.execute(query)
-                    r = [dict((cur.description[i][0], value)
-                              for i, value in enumerate(row)) for row in cur.fetchall()]
-
+                    if cur.rowcount == -1:
+                        r = [dict((cur.description[i][0], value)
+                                  for i, value in enumerate(row)) for row in cur.fetchall()]
+                        rCount = len(r)
+                    else:
+                        r = None
+                        rCount = cur.rowcount
                     logger.info(json.dumps({
                         f'odbc-{inspect.currentframe().f_code.co_name}': {
                             'connection_ms': float(f'{(time.time() - start_time) * 1000:.2f}'),
+                            'rc': f'{cur.rowcount}:{rCount}',
                             'query': f'{query}'
                         }}))
-                    return r
+                return r
             except pyodbc.Error as e:  # pragma: no cover
                 logger.error(json.dumps({
                     f'odbc-{inspect.currentframe().f_code.co_name}': {
                         'connection_ms': float(f'{(time.time() - start_time) * 1000:.2f}'),
                         'query': f'{query}',
                         'error': f'{e}'
                     }}))
```

### Comparing `sesql-2024.4.0/seSql/dbc/ODBCError.py` & `sesql-2024.4.1rc1/seSql/dbc/ODBCError.py`

 * *Files identical despite different names*

### Comparing `sesql-2024.4.0/seSql/dbc/Utilities.py` & `sesql-2024.4.1rc1/seSql/dbc/Utilities.py`

 * *Files identical despite different names*

### Comparing `sesql-2024.4.0/seSql/dbc/jars/mssql-jdbc-12.4.2.jre8.jar` & `sesql-2024.4.1rc1/seSql/dbc/jars/mssql-jdbc-12.4.2.jre8.jar`

 * *Files identical despite different names*

### Comparing `sesql-2024.4.0/seSql/sql.py` & `sesql-2024.4.1rc1/seSql/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
                 server: Optional[str] = None,
                 port: Optional[int] = None,
                 user: Optional[str] = None,
                 password: Optional[str] = None,
                 trust: Optional[str] = None,
                 db: Optional[str] = "",
                 trustServerCertificate: Optional[bool] = True,
+                mars: Optional[str] = 'no',
                 driverOverride: Optional[str] = None
                 ):
 
         self.__odbcLoaded = odbcLoaded()
         self.__odbcDriver = odbcDriver()
         self.__jdbcLoaded = jdbcLoaded()
         self.__jdbcDriver = jdbcDriver()
@@ -38,14 +39,15 @@
             "server": server,
             "port": port,
             "user": user,
             "password": password,
             "trust": trust,
             "db": db,
             "trustServerCertificate": trustServerCertificate,
+            "mars": mars,
             "driverOverride": driverOverride
         }
 
         if self.__driverOverride == "odbc" and self.__odbcLoaded:
             self.__driverOverride = "odbc"
         elif self.__driverOverride == "jdbc" and self.__jdbcLoaded:
             self.__driverOverride = "jdbc"
@@ -56,15 +58,16 @@
             case "odbc":
                 self.__cnxn = odbcEngine(
                     server=self.__connStr['server'],
                     port=self.__connStr['port'],
                     db=self.__connStr['db'],
                     user=self.__connStr['user'],
                     password=self.__connStr['password'],
-                    trust=self.__connStr['trust']
+                    trust=self.__connStr['trust'],
+                    mars=self.__connStr['mars'],
                 )
                 self._logging()
 
                 try:
                     self.__cnxn.connect()
                     self.__isConnected = self.__cnxn.isConnected
                 except Exception as e:  # pragma: no cover
```

### Comparing `sesql-2024.4.0/sesql.egg-info/PKG-INFO` & `sesql-2024.4.1rc1/sesql.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sesql
-Version: 2024.4.0
+Version: 2024.4.1rc1
 Summary: CLI to enhance versioning for Python projects
 Author-email: Cybernetic Innovations <github@cyberneticinnovations.com>
 License: MIT License
         
         Copyright (c) 2024 Cybernetic Innovations
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,75 +39,76 @@
 
 ## Install
 ```shell
 pip install seSql
 ```
 
 ## Usage
-### connect, query
-- **_using JDBC_**
+
+### **_using JDBC/ODBC_**
 ```python
 from seSql import sql, logger
 
 if __name__ == '__main__':
     oSql = sql()
     oSql.connect(
         server="SQL.site4now.net",
         port=1433,
         user="db_user",
         password="{pw}",
         trust="no",
-        driverOverride="jdbc"
+        driverOverride="odbc",      # options: odbc/jdbc
+        mars="no"                   # option to use MARS but only works with ODBC, ignored with JDBC
+        
     )
     if oSql.isConnected:
+        # request sql version without try/except
+        oSql.query("select @@version as version")
+        
+        # request sql version with try/except: typo that will generate an exception
         try:
-            oSql.query("select @@version as version;")
             oSql.query("select @@versions as version;")
         except Exception as e:
             logger.error(f'Exception: {e}')
-```
 
-- **_using JDBC_ - output**
-```shell
-2024-04-01 00:00:00 | seSql | INFO     | {"driver-info": {"using": "jdbc", "odbc": {"loaded": true, "driver": "ODBC Driver 18 for SQL Server"}, "jdbc": {"loaded": true, "driver": "mssql-12.4.2"}}}
-2024-04-01 00:00:00 | seSql | INFO     | {"jdbc-connect": {"connection_ms": 889.3, "connected": true, "connStr": {"driver": "mssql-12.4.2", "server": "jdbc:sqlserver://SQL.site4now.net", "port": 1433, "database": "", "user": "db_user", "password": "**********mee68", "encrypt": true, "trustServerCertificate": true}}}
-2024-04-01 00:00:00 | seSql | INFO     | {"jdbc-query": {"connection_ms": 104.95, "query": "select @@version as version;"}}
-2024-04-01 00:00:00 | seSql | ERROR    | {"jdbc-query": {"connection_ms": 59.0, "query": "select @@versions as version;", "error": "com.microsoft.sqlserver.jdbc.SQLServerException: Must declare the scalar variable \"@@versions\"."}}
-2024-04-01 00:00:00 | seSql | ERROR    | Exception: com.microsoft.sqlserver.jdbc.SQLServerException: Must declare the scalar variable "@@versions".
-```
+        # select
+        try:
+            oSql.query("select * from dbo.winequality_red;")
+        except Exception as e:
+            logger.error(f'Exception: {e}')
 
-### connect, query
-- **_using ODBC_**
-```python
-from seSql import sql, logger
+        # insert
+        try:
+            oSql.query("insert into dbo.seSql_Settings ([key], value) values ('Env', 'test');")
+        except Exception as e:
+            logger.error(f'Exception: {e}')
 
-if __name__ == '__main__':
-    oSql = sql()
-    oSql.connect(
-        server="SQL.site4now.net",
-        port=1433,
-        user="db_user",
-        password="{pw}",
-        trust="no",
-        driverOverride="odbc"
-    )
-    if oSql.isConnected:
+        # delete
         try:
-            oSql.query("select @@version as version;")
-            oSql.query("select @@versions as version;")
+            oSql.query("delete from dbo.seSql_Settings where value like '%dev';")
+        except Exception as e:
+            logger.error(f'Exception: {e}')
+
+        # update
+        try:
+            oSql.query("update dbo.seSql_Settings set value = 'false' where [key] like '%Updated';")
         except Exception as e:
             logger.error(f'Exception: {e}')
 ```
-- **_using ODBC_ - output**
+### **_output_**
 ```shell
-2024-04-01 00:00:00 | seSql | INFO     | {"driver-info": {"using": "odbc", "odbc": {"loaded": true, "driver": "ODBC Driver 18 for SQL Server"}, "jdbc": {"loaded": true, "driver": "mssql-12.4.2"}}}
-2024-04-01 00:00:00 | seSql | INFO     | {"odbc-connect": {"connection_ms": 781.27, "connected": true, "connStr": {"driver": "ODBC Driver 18 for SQL Server", "server": "SQL.site4now.net", "port": 1433, "database": "", "user": "db_user", "password": "**********mee68", "trust": "no"}}}
-2024-04-01 00:00:00 | seSql | INFO     | {"odbc-query": {"connection_ms": 56.09, "query": "select @@version as version;"}}
-2024-04-01 00:00:00 | seSql | ERROR    | {"odbc-query": {"connection_ms": 56.53, "query": "select @@versions as version;", "error": "('42000', '[42000] [Microsoft][ODBC Driver 18 for SQL Server][SQL Server]Must declare the scalar variable \"@@versions\". (137) (SQLExecDirectW)')"}}
-2024-04-01 00:00:00 | seSql | ERROR    | Exception: ('42000', '[42000] [Microsoft][ODBC Driver 18 for SQL Server][SQL Server]Must declare the scalar variable "@@versions". (137) (SQLExecDirectW)')
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"driver-info": {"using": "odbc", "odbc": {"loaded": true, "driver": "ODBC Driver 18 for SQL Server"}, "jdbc": {"loaded": true, "driver": "mssql-12.4.2"}}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-connect": {"connection_ms": 711.46, "connected": true, "connStr": {"driver": "ODBC Driver 18 for SQL Server", "server": "SQL5101.site4now.net", "port": 1433, "database": "", "user": "db_user", "password": "**********mee68", "trust": "no", "mars": "no"}}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-query": {"connection_ms": 56.32, "rc": "-1:1", "query": "select @@version as version"}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | ERROR    | {"odbc-query": {"connection_ms": 56.74, "query": "select @@versions as version;", "error": "('42000', '[42000] [Microsoft][ODBC Driver 18 for SQL Server][SQL Server]Must declare the scalar variable \"@@versions\". (137) (SQLExecDirectW)')"}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | ERROR    | Exception: ('42000', '[42000] [Microsoft][ODBC Driver 18 for SQL Server][SQL Server]Must declare the scalar variable "@@versions". (137) (SQLExecDirectW)')
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-query": {"connection_ms": 250.5, "rc": "-1:1599", "query": "select * from dbo.winequality_red;"}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-query": {"connection_ms": 57.83, "rc": "1:1", "query": "insert into dbo.seSql_Settings ([key], value) values ('Env', 'test');"}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-query": {"connection_ms": 56.38, "rc": "0:0", "query": "delete from dbo.seSql_Settings where value like '%dev';"}}
+2024-04-15 00:00:00 | seSql | d46bbd63-01e4-41b8-8fab-e8e657d2bdd8 | ------------ | INFO     | {"odbc-query": {"connection_ms": 56.96, "rc": "1:1", "query": "update dbo.seSql_Settings set value = 'false' where [key] like '%Updated';"}}
 ```
 
 ### hostName, hostIP, mask, seSqlVersion
 ```python
 import json
 from seSql import mask, seSqlVersion, hostName, hostIP, logger
 
@@ -119,17 +120,17 @@
             'mask_all_but_last_12345': mask('all_but_last_12345'),
             'version': seSqlVersion
         }
     }, indent=4))
 ```
 - output
 ```shell
-2024-04-01 00:00:00 | seSql | INFO     | {
+2024-04-15 00:00:00 | seSql | INFO     | {
     "seSql-info": {
         "host": "MacBook-Pro",
         "hostIP": "127.0.0.1",
         "mask_all_but_last_12345": "*************12345",
-        "version": "2024.4.0 build[59]"
+        "version": "2024.4.1 build[68]"
     }
 }
 
 ```
```

### Comparing `sesql-2024.4.0/sesql.egg-info/SOURCES.txt` & `sesql-2024.4.1rc1/sesql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sesql-2024.4.0/tests/test_Exceptions.py` & `sesql-2024.4.1rc1/tests/test_Exceptions.py`

 * *Files identical despite different names*

### Comparing `sesql-2024.4.0/tests/test_jdbc.py` & `sesql-2024.4.1rc1/tests/test_jdbc.py`

 * *Files identical despite different names*

### Comparing `sesql-2024.4.0/tests/test_odbc.py` & `sesql-2024.4.1rc1/tests/test_odbc.py`

 * *Files identical despite different names*

