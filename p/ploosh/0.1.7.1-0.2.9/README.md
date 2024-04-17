# Comparing `tmp/ploosh-0.1.7.1.tar.gz` & `tmp/ploosh-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploosh-0.1.7.1.tar", last modified: Tue Feb  6 15:22:46 2024, max compression
+gzip compressed data, was "ploosh-0.2.9.tar", last modified: Wed Apr 17 21:25:11 2024, max compression
```

## Comparing `ploosh-0.1.7.1.tar` & `ploosh-0.2.9.tar`

### file list

```diff
@@ -1,36 +1,42 @@
-drwxr-xr-x   0 csharplie  (1000) csharplie  (1000)        0 2024-02-06 15:22:46.544078 ploosh-0.1.7.1/
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     2346 2024-02-06 15:22:46.544078 ploosh-0.1.7.1/PKG-INFO
-drwxr-xr-x   0 csharplie  (1000) csharplie  (1000)        0 2024-02-06 15:22:46.533245 ploosh-0.1.7.1/ploosh/
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)      103 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/__init__.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     4293 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/__main__.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     6730 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/case.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     4943 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/configuration.py
-drwxr-xr-x   0 csharplie  (1000) csharplie  (1000)        0 2024-02-06 15:22:46.544078 ploosh-0.1.7.1/ploosh/connectors/
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)      642 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/connectors/__init__.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)      337 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/connectors/connector.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)      890 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/connectors/connector_bigquery.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)      640 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/connectors/connector_csv.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     1398 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/connectors/connector_databricks.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)      468 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/connectors/connector_empty.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     2713 2024-02-02 15:40:54.000000 ploosh-0.1.7.1/ploosh/connectors/connector_mssql.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     2231 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/connectors/connector_mysql.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     2219 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/connectors/connector_postgresql.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     1953 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/connectors/connector_snowflake.py
-drwxr-xr-x   0 csharplie  (1000) csharplie  (1000)        0 2024-02-06 15:22:46.544078 ploosh-0.1.7.1/ploosh/exporters/
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)      637 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/exporters/__init__.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)      475 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/exporters/exporter.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     1846 2024-02-06 09:14:55.000000 ploosh-0.1.7.1/ploosh/exporters/exporter_csv.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     1991 2024-02-06 09:14:59.000000 ploosh-0.1.7.1/ploosh/exporters/exporter_json.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     5135 2024-02-06 14:36:16.000000 ploosh-0.1.7.1/ploosh/exporters/exporter_trx.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     3064 2024-02-06 09:30:24.000000 ploosh-0.1.7.1/ploosh/logs.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     1820 2024-01-27 16:04:03.000000 ploosh-0.1.7.1/ploosh/parameters.py
-drwxr-xr-x   0 csharplie  (1000) csharplie  (1000)        0 2024-02-06 15:22:46.544078 ploosh-0.1.7.1/ploosh.egg-info/
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     2346 2024-02-06 15:22:46.000000 ploosh-0.1.7.1/ploosh.egg-info/PKG-INFO
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)      847 2024-02-06 15:22:46.000000 ploosh-0.1.7.1/ploosh.egg-info/SOURCES.txt
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)        1 2024-02-06 15:22:46.000000 ploosh-0.1.7.1/ploosh.egg-info/dependency_links.txt
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)       48 2024-02-06 15:22:46.000000 ploosh-0.1.7.1/ploosh.egg-info/entry_points.txt
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)      261 2024-02-06 15:22:46.000000 ploosh-0.1.7.1/ploosh.egg-info/requires.txt
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)        7 2024-02-06 15:22:46.000000 ploosh-0.1.7.1/ploosh.egg-info/top_level.txt
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)       54 2024-02-06 15:16:05.000000 ploosh-0.1.7.1/setup-full.py
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)       38 2024-02-06 15:22:46.544078 ploosh-0.1.7.1/setup.cfg
--rw-r--r--   0 csharplie  (1000) csharplie  (1000)     1761 2024-02-06 15:22:24.000000 ploosh-0.1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:25:11.837555 ploosh-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-17 21:25:11.837555 ploosh-0.2.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:25:11.833555 ploosh-0.2.9/ploosh/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:25:11.833555 ploosh-0.2.9/ploosh/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_csv_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_delta_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_empty_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/connectors/connector_sql_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/execute.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:25:11.837555 ploosh-0.2.9/ploosh/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/exporters/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/exporters/exporter_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/exporters/exporter_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/exporters/exporter_trx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 21:24:21.000000 ploosh-0.2.9/ploosh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:25:11.833555 ploosh-0.2.9/ploosh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-17 21:25:11.000000 ploosh-0.2.9/ploosh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-17 21:25:11.000000 ploosh-0.2.9/ploosh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 21:25:11.000000 ploosh-0.2.9/ploosh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 21:25:11.000000 ploosh-0.2.9/ploosh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-17 21:25:11.000000 ploosh-0.2.9/ploosh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 21:25:11.000000 ploosh-0.2.9/ploosh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-17 21:24:21.000000 ploosh-0.2.9/setup-full.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 21:25:11.837555 ploosh-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-17 21:24:21.000000 ploosh-0.2.9/setup.py
```

### Comparing `ploosh-0.1.7.1/PKG-INFO` & `ploosh-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploosh
-Version: 0.1.7.1
+Version: 0.2.9
 Summary: A framework to automatize your tests for data projects
 Home-page: https://github.com/CSharplie/ploosh/
 Download-URL: https://pypi.org/project/ploosh/
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/CSharplie/ploosh/issues
 Project-URL: CI, https://github.com/CSharplie/ploosh/actions
 Project-URL: Documentation, https://github.com/CSharplie/ploosh
```

### Comparing `ploosh-0.1.7.1/ploosh/case.py` & `ploosh-0.2.9/ploosh/case.py`

 * *Files 18% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         self.compare_duration.start = datetime.now()
 
         count_source = len(self.source.df_data)
         count_expected = len(self.expected.df_data)
 
         if count_source != count_expected:
             self.error_type = "count"
-            self.error_message = f"The count in source dataset ({count_source}) is differant than the count the in expected dataset ({count_expected})"
+            self.error_message = f"The count in source dataset ({count_source}) is differant than the count in the expected dataset ({count_expected})"
 
         if self.error_message is None and count_source != 0:
             if self.options is not None and self.options["ignore"] is not None:
                 self.source.df_data = self.source.df_data.drop(columns = self.options["ignore"], axis = 1, errors = "ignore")
                 self.expected.df_data = self.expected.df_data.drop(columns = self.options["ignore"], axis = 1, errors = "ignore")
 
             df_columns_source = pd.DataFrame({ "columns": self.source.df_data.columns }).sort_values(by = ["columns"]).reset_index(drop=True)
@@ -162,14 +162,57 @@
 
         self.compare_duration.end = datetime.now()
 
         if self.error_message is None:
             self.state = "passed"
         else:
             self.state = "failed"
+
+    def compare_dataframes_with_spark(self, spark_session):
+        """Compare source and expected dataframe using Spark"""
+
+        self.compare_duration.start = datetime.now()
+
+        count_source = self.source.df_data.count()
+        count_expected = self.expected.df_data.count()
+
+        if count_source != count_expected:
+            self.error_type = "count"
+            self.error_message = f"The count in source dataset ({count_source}) is different than the count in the expected dataset ({count_expected})"
+
+        if self.error_message is None and count_source != 0:
+            if self.options is not None and self.options["ignore"] is not None:
+                ignore_columns = self.options["ignore"]
+                self.source.df_data = self.source.df_data.drop(*ignore_columns)
+                self.expected.df_data = self.expected.df_data.drop(*ignore_columns)
+
+            source_columns = sorted(self.source.df_data.columns)
+            expected_columns = sorted(self.expected.df_data.columns)
+
+            if source_columns != expected_columns:
+                self.error_message = "The headers are different between source dataset and expected dataset"
+                self.error_type = "headers"
+
+            if self.error_message is None and count_source != 0:
+                #if self.options is not None and self.options["sort"] is not None:
+                #    self.source.df_data = self.source.df_data.orderBy(*self.options["sort"]).drop("index")
+                #    self.expected.df_data = self.expected.df_data.orderBy(*self.options["sort"]).drop("index")
+
+                df_compare = self.source.df_data.exceptAll(self.expected.df_data)
+                if df_compare.count() != 0:
+                    self.error_message = "Some rows are not equal between source dataset and expected dataset"
+                    self.error_type = "data"
+                    self.df_compare_gap = df_compare.toPandas()
+
+        self.compare_duration.end = datetime.now()
+
+        if self.error_message is None:
+            self.state = "passed"
+        else:
+            self.state = "failed"
 
     def compare_dataframes_error(self, message):
         """Setup error message for compare engine"""
 
         self.state = "Error"
         self.error_type = "compare"
         self.error_message = message
```

### Comparing `ploosh-0.1.7.1/ploosh/configuration.py` & `ploosh-0.2.9/ploosh/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,32 +55,35 @@
             raise InvalidParameterException(f"Connection {name} do not exists")
 
         return self.connections[name]
 
     def init_connections(self):
         """Load connections and apply control and variable setup"""
 
-        with open(self.parameters.path_connection, encoding="UTF-8") as file:
-            content = file.read()
-            self.connections = yaml.safe_load(content)
+        if self.parameters.path_connection is None:
+            self.connections = {}
+        else:
+            with open(self.parameters.path_connection, encoding="UTF-8") as file:
+                content = file.read()
+                self.connections = yaml.safe_load(content)
 
         connections = copy.copy(self.connections)
         for connection_name in connections:
             connection = connections[connection_name]
             module_type = self.get_module_type(connection)
 
             connection_definition = self.connectors[module_type].connection_definition
 
             self.connections[module_type] = control_and_setup(connection, connection_definition, self.parameters.variables, None)
 
     def get_cases(self):
-        """Get cases from user confiration and apply control and variable setup"""
+        """Get cases from user configuration and apply control and variable setup"""
 
         cases = {}
-        files_list = list(pathlib.Path(self.parameters.path_cases).rglob("*.yml"))
+        files_list = list(pathlib.Path(self.parameters.path_cases).rglob(self.parameters.path_cases_filter))
 
         for file_path in files_list:
             with open(file_path, encoding="UTF-8") as file:
                 configurations = yaml.load(file, Loader = yaml.loader.SafeLoader)
                 for case_name in configurations.keys():
                     configuration = configurations[case_name]
 
@@ -96,14 +99,16 @@
                     expected_module_type = self.get_module_type(configuration["expected"])
                     expected_connector = self.connectors[expected_module_type]
                     expected_configuration_definition = expected_connector.configuration_definition
 
                     case["expected"] = control_and_setup(case["expected"], expected_configuration_definition, self.parameters.variables, None)
                     expected_definition = ConnectionDescription(expected_connector, self.get_connection(case["expected"]["connection"]))
 
+                    if source_connector.is_spark != expected_connector.is_spark:
+                        raise InvalidParameterException(f"'{case_name}': Source and expected must be both Spark or not Spark connectors")
 
                     cases[case_name] = Case(configuration, source_definition, expected_definition, case["options"], case["disabled"])
 
         return cases
 
     def set_exporter(self, exporters):
         """Set exporter from args"""
```

### Comparing `ploosh-0.1.7.1/ploosh/connectors/connector_bigquery.py` & `ploosh-0.2.9/ploosh/connectors/connector_bigquery.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.1.7.1/ploosh/connectors/connector_csv.py` & `ploosh-0.2.9/ploosh/connectors/connector_csv.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.1.7.1/ploosh/connectors/connector_databricks.py` & `ploosh-0.2.9/ploosh/connectors/connector_databricks.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.1.7.1/ploosh/connectors/connector_mssql.py` & `ploosh-0.2.9/ploosh/connectors/connector_mssql.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.1.7.1/ploosh/connectors/connector_mysql.py` & `ploosh-0.2.9/ploosh/connectors/connector_mysql.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.1.7.1/ploosh/connectors/connector_postgresql.py` & `ploosh-0.2.9/ploosh/connectors/connector_postgresql.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.1.7.1/ploosh/connectors/connector_snowflake.py` & `ploosh-0.2.9/ploosh/connectors/connector_snowflake.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.1.7.1/ploosh/exporters/__init__.py` & `ploosh-0.2.9/ploosh/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.1.7.1/ploosh/exporters/exporter_csv.py` & `ploosh-0.2.9/ploosh/exporters/exporter_csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,12 +46,18 @@
                 case.compare_duration.duration,
                 case.error_type,
                 case.error_message,
             ]
 
             data.append(case_data)
 
+            if case.df_compare_gap is not None:
+                detail_file_path = f"{self.output_path}/json/test_results/{name}.xlsx"
+
+                os.makedirs(os.path.dirname(detail_file_path), exist_ok=True)
+                case.df_compare_gap.to_excel(detail_file_path)
+
         os.makedirs(os.path.dirname(output_file), exist_ok=True)
         with open(output_file, "w", encoding="UTF-8") as f:
             writer = csv.writer(f, lineterminator="\n")
             writer.writerows(data)
             f.close()
```

### Comparing `ploosh-0.1.7.1/ploosh/exporters/exporter_json.py` & `ploosh-0.2.9/ploosh/exporters/exporter_json.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,18 +41,24 @@
             if case.compare_duration.start is not None:
                 case_data["compare"] = {
                     "start": Exporter.date_to_string(case.compare_duration.start),
                     "end": Exporter.date_to_string(case.compare_duration.end),
                     "duration": case.compare_duration.duration,
                 }
 
-            if case.state != "passed":
+            if case.state in ["error", "failed"]:
                 case_data["error"] = {
                     "type": case.error_type,
                     "message": case.error_message
                 }
 
             data.append(case_data)
 
+            if case.df_compare_gap is not None:
+                detail_file_path = f"{self.output_path}/json/test_results/{name}.xlsx"
+
+                os.makedirs(os.path.dirname(detail_file_path), exist_ok=True)
+                case.df_compare_gap.to_excel(detail_file_path)
+
         os.makedirs(os.path.dirname(output_file), exist_ok=True)
         with open(output_file, "w", encoding="UTF-8") as f:
-            f.write(json.dumps(data, indent=2))
+            f.write(json.dumps(data, indent=2))
```

### Comparing `ploosh-0.1.7.1/ploosh/exporters/exporter_trx.py` & `ploosh-0.2.9/ploosh/exporters/exporter_trx.py`

 * *Files identical despite different names*

### Comparing `ploosh-0.1.7.1/ploosh/parameters.py` & `ploosh-0.2.9/ploosh/parameters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """Module for parsing input parameters"""
 
 class Parameters:
     """Parse input parameters"""
     args = {}
     path_connection = None
     path_cases = None
+    path_cases_filter = None
     path_output = None
     export = None
     failure_on_error = None
     variables = {}
 
     def __init__(self, argv:list):
         self.set_args(argv[1:])
         self.set_variables()
-        self.path_connection = self.get_value("connections", "connections.yaml")
+        self.path_connection = self.get_value("connections", None)
         self.path_cases = self.get_value("cases", "./cases")
+        self.path_cases_filter = self.get_value("filter", "*.yml")
         self.path_output = self.get_value("output", "./output")
         self.export = self.get_value("export", "JSON").upper()
         self.failure_on_error = self.get_value("failure", True)
+        self.spark_mode = self.get_value("spark", False)
 
     def set_args(self, args):
         """Set dictionary of args with cleaned name"""
         for i, name in enumerate(args):
             if not name.startswith("-"):
                 continue
```

### Comparing `ploosh-0.1.7.1/ploosh.egg-info/PKG-INFO` & `ploosh-0.2.9/ploosh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploosh
-Version: 0.1.7.1
+Version: 0.2.9
 Summary: A framework to automatize your tests for data projects
 Home-page: https://github.com/CSharplie/ploosh/
 Download-URL: https://pypi.org/project/ploosh/
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/CSharplie/ploosh/issues
 Project-URL: CI, https://github.com/CSharplie/ploosh/actions
 Project-URL: Documentation, https://github.com/CSharplie/ploosh
```

### Comparing `ploosh-0.1.7.1/ploosh.egg-info/SOURCES.txt` & `ploosh-0.2.9/ploosh.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 setup-full.py
 setup.py
 ploosh/__init__.py
 ploosh/__main__.py
 ploosh/case.py
 ploosh/configuration.py
+ploosh/execute.py
 ploosh/logs.py
 ploosh/parameters.py
+ploosh/version.py
 ploosh.egg-info/PKG-INFO
 ploosh.egg-info/SOURCES.txt
 ploosh.egg-info/dependency_links.txt
 ploosh.egg-info/entry_points.txt
 ploosh.egg-info/requires.txt
 ploosh.egg-info/top_level.txt
 ploosh/connectors/__init__.py
 ploosh/connectors/connector.py
 ploosh/connectors/connector_bigquery.py
 ploosh/connectors/connector_csv.py
+ploosh/connectors/connector_csv_spark.py
 ploosh/connectors/connector_databricks.py
+ploosh/connectors/connector_delta_spark.py
 ploosh/connectors/connector_empty.py
+ploosh/connectors/connector_empty_spark.py
 ploosh/connectors/connector_mssql.py
 ploosh/connectors/connector_mysql.py
 ploosh/connectors/connector_postgresql.py
 ploosh/connectors/connector_snowflake.py
+ploosh/connectors/connector_sql_spark.py
 ploosh/exporters/__init__.py
 ploosh/exporters/exporter.py
 ploosh/exporters/exporter_csv.py
 ploosh/exporters/exporter_json.py
 ploosh/exporters/exporter_trx.py
```

### Comparing `ploosh-0.1.7.1/setup.py` & `ploosh-0.2.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 """Setup PyPi module"""
 # pylint: disable=C0103
 
 from setuptools import setup, find_packages
+from ploosh.version import PLOOSH_VERSION
 
-def setup_ploosh(name):
+def setup_ploosh(name, install_requires):
     with open("../readme.md", encoding="UTF-8") as f:
         long_description = "".join(f.readlines())
 
     # replace relative link by absolute github link
     long_description = long_description.replace("(/", "(https://github.com/CSharplie/ploosh/blob/main/")
 
+    install_requires = install_requires + [
+            "colorama==0.4.6",
+            "PyYAML==6.0.1",
+            "Pyjeb==0.2.1",
+            "numpy==1.26.3",
+            "pandas==2.1.4",
+            "openpyxl==3.1.2",
+            "sqlalchemy==1.4.51",
+            "pyspark==3.5.1",
+        ]
+
     setup (
         name = name,
-        version = "0.1.7.1",
+        version = PLOOSH_VERSION,
         description="A framework to automatize your tests for data projects",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/CSharplie/ploosh/",
         project_urls={
             "Bug Tracker": "https://github.com/CSharplie/ploosh/issues",
             "CI": "https://github.com/CSharplie/ploosh/actions",
@@ -28,23 +40,9 @@
         python_requires=">=3.6",
         license= "Apache License 2.0",
         entry_points = {
             "console_scripts": [
                 "ploosh = ploosh.__main__:main"
             ]
         },
-        install_requires=[
-            "colorama==0.4.6",
-            "PyYAML==6.0.1",
-            "Pyjeb==0.2.1",
-            "pandas==2.1.4",
-            "openpyxl==3.1.2",
-            "sqlalchemy==1.4.51",
-            "pyodbc==5.0.1",
-            "pymysql==1.1.0",
-            "pg8000==1.30.3",
-            "snowflake-sqlalchemy==1.5.1",
-            "databricks-sql-connector==2.9.3",
-            "sqlalchemy-bigquery==1.9.0",
-            "google-cloud-bigquery-storage==2.24.0",
-        ],
+        install_requires=install_requires,
     )
```

