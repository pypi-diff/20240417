# Comparing `tmp/integ-db-0.0.9.tar.gz` & `tmp/integ_db-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integ-db-0.0.9.tar", last modified: Fri Apr  5 05:34:00 2024, max compression
+gzip compressed data, was "integ_db-0.1.0.tar", last modified: Wed Apr 17 05:58:44 2024, max compression
```

## Comparing `integ-db-0.0.9.tar` & `integ_db-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 05:34:00.266577 integ-db-0.0.9/
--rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integ-db-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     2143 2024-04-05 05:34:00.263574 integ-db-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      983 2024-04-05 04:09:59.000000 integ-db-0.0.9/README.md
--rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integ-db-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 05:34:00.266577 integ-db-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1435 2024-04-05 05:33:39.000000 integ-db-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 05:34:00.212352 integ-db-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 05:34:00.262571 integ-db-0.0.9/src/integ_db.egg-info/
--rw-rw-rw-   0        0        0     2143 2024-04-05 05:34:00.000000 integ-db-0.0.9/src/integ_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2024-04-05 05:34:00.000000 integ-db-0.0.9/src/integ_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 05:34:00.000000 integ-db-0.0.9/src/integ_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-05 05:34:00.000000 integ-db-0.0.9/src/integ_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 05:34:00.000000 integ-db-0.0.9/src/integ_db.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 05:34:00.244459 integ-db-0.0.9/src/integdb/
--rw-rw-rw-   0        0        0       34 2024-04-05 03:16:38.000000 integ-db-0.0.9/src/integdb/__init__.py
--rw-rw-rw-   0        0        0      599 2024-04-05 04:55:25.000000 integ-db-0.0.9/src/integdb/controller.py
-drwxrwxrwx   0        0        0        0 2024-04-05 05:34:00.259569 integ-db-0.0.9/src/integdb/module/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:13:56.000000 integ-db-0.0.9/src/integdb/module/__init__.py
--rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integ-db-0.0.9/src/integdb/module/interface.py
--rw-rw-rw-   0        0        0     1090 2024-04-05 03:22:42.000000 integ-db-0.0.9/src/integdb/module/mariadb.py
--rw-rw-rw-   0        0        0      618 2024-04-05 03:22:45.000000 integ-db-0.0.9/src/integdb/module/mssql.py
--rw-rw-rw-   0        0        0     1156 2024-04-05 05:30:01.000000 integ-db-0.0.9/src/integdb/module/mysql.py
--rw-rw-rw-   0        0        0     1825 2024-04-05 03:23:06.000000 integ-db-0.0.9/src/integdb/module/sqlalchemy.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:58:44.869547 integ_db-0.1.0/
+-rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integ_db-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2266 2024-04-17 05:58:44.866542 integ_db-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1106 2024-04-17 05:55:37.000000 integ_db-0.1.0/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integ_db-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 05:58:44.870554 integ_db-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1435 2024-04-17 05:49:34.000000 integ_db-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:58:44.790553 integ_db-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 05:58:44.864565 integ_db-0.1.0/src/integ_db.egg-info/
+-rw-rw-rw-   0        0        0     2266 2024-04-17 05:58:44.000000 integ_db-0.1.0/src/integ_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2024-04-17 05:58:44.000000 integ_db-0.1.0/src/integ_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 05:58:44.000000 integ_db-0.1.0/src/integ_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-17 05:58:44.000000 integ_db-0.1.0/src/integ_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 05:58:44.000000 integ_db-0.1.0/src/integ_db.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 05:58:44.845461 integ_db-0.1.0/src/integdb/
+-rw-rw-rw-   0        0        0       34 2024-04-05 03:16:38.000000 integ_db-0.1.0/src/integdb/__init__.py
+-rw-rw-rw-   0        0        0      599 2024-04-05 04:55:25.000000 integ_db-0.1.0/src/integdb/controller.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:58:44.861599 integ_db-0.1.0/src/integdb/module/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:13:56.000000 integ_db-0.1.0/src/integdb/module/__init__.py
+-rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integ_db-0.1.0/src/integdb/module/interface.py
+-rw-rw-rw-   0        0        0     1090 2024-04-05 03:22:42.000000 integ_db-0.1.0/src/integdb/module/mariadb.py
+-rw-rw-rw-   0        0        0      618 2024-04-05 03:22:45.000000 integ_db-0.1.0/src/integdb/module/mssql.py
+-rw-rw-rw-   0        0        0     1156 2024-04-05 05:30:01.000000 integ_db-0.1.0/src/integdb/module/mysql.py
+-rw-rw-rw-   0        0        0     3246 2024-04-17 05:57:53.000000 integ_db-0.1.0/src/integdb/module/sqlalchemy.py
```

### Comparing `integ-db-0.0.9/LICENSE` & `integ_db-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.9/PKG-INFO` & `integ_db-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integ-db
-Version: 0.0.9
+Version: 0.1.0
 Summary: This package Integrated Database library
 Home-page: https://github.com/Byeongin-Jeong/integdb
 Author: byeongin.jeong
 Author-email: jbi0214@gmail.com
 Project-URL: Bug Tracker, https://github.com/Byeongin-Jeong/integdb/issues
 Keywords: mysql,mssql,mariadb,python db,python database,integrate database,sqlalchemy
 Classifier: Programming Language :: Python :: 3
@@ -73,7 +73,12 @@
     rows = controller.MySQL.sql_executer(sql_context)
     print (rows)
 except Exception as e:
     print (e)
 finally:
     controller.MySQL.close()
 ```
+
+---
+## Reference
+1. duplicate SQLalchemy 
+Github : https://gist.github.com/tombohub/0c666583c48c1686c736ae2eb76cb2ea
```

### Comparing `integ-db-0.0.9/README.md` & `integ_db-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -42,8 +42,13 @@
     sql_context = "SELECT * FROM TEST_DB"
     rows = controller.MySQL.sql_executer(sql_context)
     print (rows)
 except Exception as e:
     print (e)
 finally:
     controller.MySQL.close()
-```
+```
+
+---
+## Reference
+1. duplicate SQLalchemy 
+Github : https://gist.github.com/tombohub/0c666583c48c1686c736ae2eb76cb2ea
```

### Comparing `integ-db-0.0.9/setup.py` & `integ_db-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="integ-db",
-    version="0.0.9",
+    version="0.1.0",
     author="byeongin.jeong",
     author_email="jbi0214@gmail.com",
     description="This package Integrated Database library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Byeongin-Jeong/integdb",
     project_urls={
```

### Comparing `integ-db-0.0.9/src/integ_db.egg-info/PKG-INFO` & `integ_db-0.1.0/src/integ_db.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integ-db
-Version: 0.0.9
+Version: 0.1.0
 Summary: This package Integrated Database library
 Home-page: https://github.com/Byeongin-Jeong/integdb
 Author: byeongin.jeong
 Author-email: jbi0214@gmail.com
 Project-URL: Bug Tracker, https://github.com/Byeongin-Jeong/integdb/issues
 Keywords: mysql,mssql,mariadb,python db,python database,integrate database,sqlalchemy
 Classifier: Programming Language :: Python :: 3
@@ -73,7 +73,12 @@
     rows = controller.MySQL.sql_executer(sql_context)
     print (rows)
 except Exception as e:
     print (e)
 finally:
     controller.MySQL.close()
 ```
+
+---
+## Reference
+1. duplicate SQLalchemy 
+Github : https://gist.github.com/tombohub/0c666583c48c1686c736ae2eb76cb2ea
```

### Comparing `integ-db-0.0.9/src/integdb/controller.py` & `integ_db-0.1.0/src/integdb/controller.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.9/src/integdb/module/interface.py` & `integ_db-0.1.0/src/integdb/module/interface.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.9/src/integdb/module/mariadb.py` & `integ_db-0.1.0/src/integdb/module/mariadb.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.9/src/integdb/module/mssql.py` & `integ_db-0.1.0/src/integdb/module/mssql.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.9/src/integdb/module/mysql.py` & `integ_db-0.1.0/src/integdb/module/mysql.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.9/src/integdb/module/sqlalchemy.py` & `integ_db-0.1.0/src/integdb/module/sqlalchemy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,73 @@
+import random
+import string
 import pandas as pd
 from sqlalchemy import create_engine
 from sqlalchemy.exc import IntegrityError
 from .interface import SessionConfig
 
 class SQLAlchemy(SessionConfig):
     def __init__(self, host, user, password, port, schema, connection_pool):
         super().__init__(host, user, password, port, schema, connection_pool)
 
+    def _table_column_names(self, table: str) -> str:
+        query = f"SELECT column_name FROM information_schema.columns WHERE table_name = '{table}'"
+        rows = self._engine.execute(query)
+        dirty_names = [i[0] for i in rows]
+        clean_names = '`' + '`, `'.join(map(str, dirty_names)) + '`'
+        return clean_names
+
     def connect(self, db_url="mysql+pymysql"):
         try:
             self._connection_str = f'{db_url}://{self._user}:{self._password}@{self._host}:{self._port}/{self._schema}'
             self._engine = create_engine(url=self._connection_str)
         except Exception as e:
             raise Exception(f'Error connecting to the SQLAlchemy: {e}')
         
     def close(self):
         if self._engine is not None:
             self._engine.dispose()
             self._engine = None
 
-    def sql_export(self, df: pd.DataFrame, name, schema=None):
+    def sql_export(self, df: pd.DataFrame, table_name, schema=None):
         try:
             if self._engine is None:
                 self._engine = create_engine(url=self._connection_str)
 
             db_schema = self._schema
             if schema is not None:
                 db_schema = schema
-            df.to_sql(name, con=self._engine, if_exists='append', index=False, schema=db_schema)
+            df.to_sql(table_name, con=self._engine, if_exists='append', index=False, schema=db_schema)
         except IntegrityError as e:
             raise IntegrityError(e.statement, e.params, e.orig)
         except Exception as e:
             raise Exception(e)
+        
+    def sql_export_ignore(self, df: pd.DataFrame, table_name, schema=None):
+        temp_table = ''.join(random.choice(string.ascii_letters) for i in range(10))
+        is_tmp_table = False
+        try:
+            if self._engine is None:
+                self._engine = create_engine(url=self._connection_str)
+
+            db_schema = self._schema
+            if schema is not None:
+                db_schema = schema
+
+            df.to_sql(temp_table, con=self._engine, if_exists='append', index=False, schema=db_schema)
+            is_tmp_table = True
+            columns = self._table_column_names(table=temp_table)
+            insert_query = f'INSERT IGNORE INTO {db_schema}.{table_name}({columns}) SELECT {columns} FROM `{temp_table}`'
+            self._engine.execute(insert_query)
+        except Exception as e:
+            raise Exception(e)
+        finally:
+            # drop temp table
+            if is_tmp_table:
+                self._engine.execute(f'DROP TABLE IF EXISTS `{temp_table}`')
 
     def sql_to_pandas(self, sql_context):
         try:
             if self._engine is None:
                 self._engine = create_engine(url=self._connection_str)
 
             df_rows = pd.read_sql(sql_context, con=self._engine)
```

