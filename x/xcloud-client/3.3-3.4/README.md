# Comparing `tmp/xcloud_client-3.3.tar.gz` & `tmp/xcloud_client-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcloud_client-3.3.tar", last modified: Tue Apr 16 09:48:42 2024, max compression
+gzip compressed data, was "xcloud_client-3.4.tar", last modified: Wed Apr 17 14:01:50 2024, max compression
```

## Comparing `xcloud_client-3.3.tar` & `xcloud_client-3.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 09:48:42.553707 xcloud_client-3.3/
--rw-rw-rw-   0        0        0       19 2024-04-14 06:52:25.000000 xcloud_client-3.3/MANIFEST.in
--rw-rw-rw-   0        0        0      126 2024-04-16 09:48:42.552707 xcloud_client-3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 09:48:42.520586 xcloud_client-3.3/resources/
--rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloud_client-3.3/resources/XCloudJDBC-2.10.6.7.jar
--rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloud_client-3.3/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
--rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloud_client-3.3/resources/libthrift-0.9.2.jar
--rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloud_client-3.3/resources/log4j-1.2.17.jar
--rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloud_client-3.3/resources/lz4-1.3.0.jar
--rw-rw-rw-   0        0        0  1555682 2023-08-17 03:30:59.000000 xcloud_client-3.3/resources/ojdbc14-10.2.0.4.0.jar
--rw-rw-rw-   0        0        0    23445 2019-09-11 10:52:32.000000 xcloud_client-3.3/resources/slf4j-api-1.5.8.jar
--rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloud_client-3.3/resources/slf4j-api-1.7.5.jar
--rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloud_client-3.3/resources/slf4j-log4j12-1.7.5.jar
--rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloud_client-3.3/resources/slf4j-simple-1.7.5.jar
--rw-rw-rw-   0        0        0       42 2024-04-16 09:48:42.554723 xcloud_client-3.3/setup.cfg
--rw-rw-rw-   0        0        0      309 2024-04-16 09:47:07.000000 xcloud_client-3.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 09:48:42.527526 xcloud_client-3.3/xcloud_client/
--rw-rw-rw-   0        0        0       23 2024-04-16 09:46:56.000000 xcloud_client-3.3/xcloud_client/__init__.py
--rw-rw-rw-   0        0        0     2656 2024-04-15 04:56:18.000000 xcloud_client-3.3/xcloud_client/xCloud_client.py
-drwxrwxrwx   0        0        0        0 2024-04-16 09:48:42.546735 xcloud_client-3.3/xcloud_client.egg-info/
--rw-rw-rw-   0        0        0      126 2024-04-16 09:48:41.000000 xcloud_client-3.3/xcloud_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      587 2024-04-16 09:48:42.000000 xcloud_client-3.3/xcloud_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 09:48:41.000000 xcloud_client-3.3/xcloud_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-16 09:48:41.000000 xcloud_client-3.3/xcloud_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-16 09:48:41.000000 xcloud_client-3.3/xcloud_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 14:01:50.654725 xcloud_client-3.4/
+-rw-rw-rw-   0        0        0       19 2024-04-14 06:52:25.000000 xcloud_client-3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      126 2024-04-17 14:01:50.653733 xcloud_client-3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 14:01:50.628328 xcloud_client-3.4/resources/
+-rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloud_client-3.4/resources/XCloudJDBC-2.10.6.7.jar
+-rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloud_client-3.4/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
+-rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloud_client-3.4/resources/libthrift-0.9.2.jar
+-rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloud_client-3.4/resources/log4j-1.2.17.jar
+-rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloud_client-3.4/resources/lz4-1.3.0.jar
+-rw-rw-rw-   0        0        0  1555682 2023-08-17 03:30:59.000000 xcloud_client-3.4/resources/ojdbc14-10.2.0.4.0.jar
+-rw-rw-rw-   0        0        0    23445 2019-09-11 10:52:32.000000 xcloud_client-3.4/resources/slf4j-api-1.5.8.jar
+-rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloud_client-3.4/resources/slf4j-api-1.7.5.jar
+-rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloud_client-3.4/resources/slf4j-log4j12-1.7.5.jar
+-rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloud_client-3.4/resources/slf4j-simple-1.7.5.jar
+-rw-rw-rw-   0        0        0       42 2024-04-17 14:01:50.654725 xcloud_client-3.4/setup.cfg
+-rw-rw-rw-   0        0        0      309 2024-04-17 14:01:09.000000 xcloud_client-3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:01:50.633289 xcloud_client-3.4/xcloud_client/
+-rw-rw-rw-   0        0        0       23 2024-04-16 09:46:56.000000 xcloud_client-3.4/xcloud_client/__init__.py
+-rw-rw-rw-   0        0        0     2875 2024-04-17 13:44:30.000000 xcloud_client-3.4/xcloud_client/xCloud_client.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:01:50.649730 xcloud_client-3.4/xcloud_client.egg-info/
+-rw-rw-rw-   0        0        0      126 2024-04-17 14:01:49.000000 xcloud_client-3.4/xcloud_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2024-04-17 14:01:50.000000 xcloud_client-3.4/xcloud_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 14:01:49.000000 xcloud_client-3.4/xcloud_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-17 14:01:50.000000 xcloud_client-3.4/xcloud_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-17 14:01:50.000000 xcloud_client-3.4/xcloud_client.egg-info/top_level.txt
```

### Comparing `xcloud_client-3.3/resources/XCloudJDBC-2.10.6.7.jar` & `xcloud_client-3.4/resources/XCloudJDBC-2.10.6.7.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.3/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar` & `xcloud_client-3.4/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.3/resources/libthrift-0.9.2.jar` & `xcloud_client-3.4/resources/libthrift-0.9.2.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.3/resources/log4j-1.2.17.jar` & `xcloud_client-3.4/resources/log4j-1.2.17.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.3/resources/lz4-1.3.0.jar` & `xcloud_client-3.4/resources/lz4-1.3.0.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.3/resources/ojdbc14-10.2.0.4.0.jar` & `xcloud_client-3.4/resources/ojdbc14-10.2.0.4.0.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.3/resources/slf4j-api-1.5.8.jar` & `xcloud_client-3.4/resources/slf4j-api-1.5.8.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.3/resources/slf4j-api-1.7.5.jar` & `xcloud_client-3.4/resources/slf4j-api-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.3/resources/slf4j-log4j12-1.7.5.jar` & `xcloud_client-3.4/resources/slf4j-log4j12-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.3/resources/slf4j-simple-1.7.5.jar` & `xcloud_client-3.4/resources/slf4j-simple-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloud_client-3.3/xcloud_client/xCloud_client.py` & `xcloud_client-3.4/xcloud_client/xCloud_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import jaydebeapi
 from pathlib import Path
 
-current_path = Path.cwd()
-jar_files =[]
-for item in current_path.iterdir():
-    if item.suffix =='.jar':
-        jar_files.append(item.name)
-print(jar_files)
+#current_path = Path.cwd()
+#jar_files =[]
+#for item in current_path.iterdir():
+    #if item.suffix =='.jar':
+        #jar_files.append(item.name)
+#print(jar_files)
 class xCloud_client:
     def __init__(self, host, port, username, password):
         self.host = host
         self.port = port
         self.username = username
         self.password = password
         self.conn = None
@@ -33,34 +33,42 @@
                 '/home/airflow/.local/lib/python3.8/site-packages/xcloud_client/slf4j-simple-1.7.5.jar',
                 '/home/airflow/.local/lib/python3.8/site-packages/xcloud_client/log4j-1.2.17.jar',
                 '/home/airflow/.local/lib/python3.8/site-packages/xcloud_client/libthrift-0.9.2.jar',
                 '/home/airflow/.local/lib/python3.8/site-packages/xcloud_client/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar',
                 '/home/airflow/.local/lib/python3.8/site-packages/xcloud_client/lz4-1.3.0.jar'
            ]
               
-            
-            print(jarFile)
             conn = jaydebeapi.connect(jclassname=driver, url=url, driver_args=[self.username, self.password], jars=jarFile)
             return conn
         except jaydebeapi.DatabaseError as e:
-            print('the connection was not consistent ,because of {e}')
+            print('目前数据库无法连接：原因为{e}')
             raise
 
     def execute_query(self, query):
         """
         执行查询并返回结果
         """
-        self.conn = self.connect()
         try:
             with self.conn.cursor() as cursor:
                 cursor.execute(query)
                 result = cursor.fetchall()
+                result_header = [(i[0] for i in cursor.description)]
+                final_result = result_header + result
         except jaydebeapi.Error as e:
             print(f"Error executing query: {e}")
             raise
         finally:
             if self.conn:
                 self.conn.close()
+        return final_result
+
+    def close(self):
+        if self.conn:
+            self.conn.close()
+
+    def cursor(self):
+        if self.conn:
+            return self.conn.cursor()
             
-        return result
+
```

### Comparing `xcloud_client-3.3/xcloud_client.egg-info/SOURCES.txt` & `xcloud_client-3.4/xcloud_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

