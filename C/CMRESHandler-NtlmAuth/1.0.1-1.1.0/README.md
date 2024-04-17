# Comparing `tmp/CMRESHandler-NtlmAuth-1.0.1.tar.gz` & `tmp/CMRESHandler-NtlmAuth-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CMRESHandler-NtlmAuth-1.0.1.tar", last modified: Fri Jun  2 10:34:10 2023, max compression
+gzip compressed data, was "CMRESHandler-NtlmAuth-1.1.0.tar", last modified: Wed Apr 17 18:28:47 2024, max compression
```

## Comparing `CMRESHandler-NtlmAuth-1.0.1.tar` & `CMRESHandler-NtlmAuth-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 10:34:10.032390 CMRESHandler-NtlmAuth-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-02 10:34:10.018531 CMRESHandler-NtlmAuth-1.0.1/CMRESHandler_NtlmAuth.egg-info/
--rw-rw-rw-   0        0        0    10733 2023-06-02 10:34:09.000000 CMRESHandler-NtlmAuth-1.0.1/CMRESHandler_NtlmAuth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-06-02 10:34:09.000000 CMRESHandler-NtlmAuth-1.0.1/CMRESHandler_NtlmAuth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 10:34:09.000000 CMRESHandler-NtlmAuth-1.0.1/CMRESHandler_NtlmAuth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-02 10:34:09.000000 CMRESHandler-NtlmAuth-1.0.1/CMRESHandler_NtlmAuth.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-02 10:34:09.000000 CMRESHandler-NtlmAuth-1.0.1/CMRESHandler_NtlmAuth.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      574 2023-05-18 12:19:18.000000 CMRESHandler-NtlmAuth-1.0.1/LICENSE.md
--rw-rw-rw-   0        0        0    10733 2023-06-02 10:34:10.033381 CMRESHandler-NtlmAuth-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9421 2023-06-02 10:27:33.000000 CMRESHandler-NtlmAuth-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 10:34:10.023522 CMRESHandler-NtlmAuth-1.0.1/cmreslogging/
--rw-rw-rw-   0        0        0        0 2023-05-18 12:19:18.000000 CMRESHandler-NtlmAuth-1.0.1/cmreslogging/__init__.py
--rw-rw-rw-   0        0        0    16250 2023-06-02 10:31:30.000000 CMRESHandler-NtlmAuth-1.0.1/cmreslogging/handlers.py
--rw-rw-rw-   0        0        0      730 2023-05-18 12:19:18.000000 CMRESHandler-NtlmAuth-1.0.1/cmreslogging/serializers.py
--rw-rw-rw-   0        0        0       59 2023-06-02 10:34:10.034770 CMRESHandler-NtlmAuth-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     4322 2023-06-02 10:31:30.000000 CMRESHandler-NtlmAuth-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:34:10.030381 CMRESHandler-NtlmAuth-1.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-05-18 12:19:18.000000 CMRESHandler-NtlmAuth-1.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     9712 2023-06-02 10:31:30.000000 CMRESHandler-NtlmAuth-1.0.1/tests/test_cmreshandler.py
--rw-rw-rw-   0        0        0     3621 2023-05-18 12:19:18.000000 CMRESHandler-NtlmAuth-1.0.1/tests/test_cmresserializer.py
+drwxrwxrwx   0        0        0        0 2024-04-17 18:28:47.586549 CMRESHandler-NtlmAuth-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:28:47.586549 CMRESHandler-NtlmAuth-1.1.0/CMRESHandler_NtlmAuth.egg-info/
+-rw-rw-rw-   0        0        0    10841 2024-04-17 18:28:47.000000 CMRESHandler-NtlmAuth-1.1.0/CMRESHandler_NtlmAuth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2024-04-17 18:28:47.000000 CMRESHandler-NtlmAuth-1.1.0/CMRESHandler_NtlmAuth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 18:28:47.000000 CMRESHandler-NtlmAuth-1.1.0/CMRESHandler_NtlmAuth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-04-17 18:28:47.000000 CMRESHandler-NtlmAuth-1.1.0/CMRESHandler_NtlmAuth.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-17 18:28:47.000000 CMRESHandler-NtlmAuth-1.1.0/CMRESHandler_NtlmAuth.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      574 2024-04-17 12:38:45.000000 CMRESHandler-NtlmAuth-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0    10841 2024-04-17 18:28:47.586549 CMRESHandler-NtlmAuth-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9311 2024-04-17 14:21:27.000000 CMRESHandler-NtlmAuth-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 18:28:47.586549 CMRESHandler-NtlmAuth-1.1.0/cmreslogging/
+-rw-rw-rw-   0        0        0        0 2024-04-17 12:38:45.000000 CMRESHandler-NtlmAuth-1.1.0/cmreslogging/__init__.py
+-rw-rw-rw-   0        0        0    15724 2024-04-17 14:11:10.000000 CMRESHandler-NtlmAuth-1.1.0/cmreslogging/handlers.py
+-rw-rw-rw-   0        0        0      730 2024-04-17 12:38:45.000000 CMRESHandler-NtlmAuth-1.1.0/cmreslogging/serializers.py
+-rw-rw-rw-   0        0        0       59 2024-04-17 18:28:47.586549 CMRESHandler-NtlmAuth-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     4322 2024-04-17 18:28:30.000000 CMRESHandler-NtlmAuth-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 18:28:47.586549 CMRESHandler-NtlmAuth-1.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-17 12:38:45.000000 CMRESHandler-NtlmAuth-1.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     9712 2024-04-17 14:10:06.000000 CMRESHandler-NtlmAuth-1.1.0/tests/test_cmreshandler.py
+-rw-rw-rw-   0        0        0     3621 2024-04-17 12:38:45.000000 CMRESHandler-NtlmAuth-1.1.0/tests/test_cmresserializer.py
```

### Comparing `CMRESHandler-NtlmAuth-1.0.1/CMRESHandler_NtlmAuth.egg-info/PKG-INFO` & `CMRESHandler-NtlmAuth-1.1.0/CMRESHandler_NtlmAuth.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CMRESHandler-NtlmAuth
-Version: 1.0.1
+Version: 1.1.0
 Summary: Elasticsearch Log handler for the logging library
 Home-page: https://github.com/thoscilo/python-elasticsearch-logger/tree/release
 Author: Carlos Manzanedo Rueda
 Author-email: c.manaha@gmail.com
 License: Apache2
 Keywords: logging elasticsearch handler log django instrumentation
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,17 +17,23 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: elasticsearch
+Requires-Dist: requests
 Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
+Requires-Dist: six; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE.md
+Requires-Dist: coverage; extra == "test"
 
 ># Origin project location.
 > Please note that this repo is a fork from: https://github.com/cmanaha/python-elasticsearch-logger
 >
 > Base code is extended by:
 > - adding the HttpNtlmAuth as new authentication
 > - add support for elasticsearch 8.x version
@@ -150,15 +156,14 @@
  - flush_frequency_in_sec: A float representing how often and when the buffer will be flushed
  - es_index_name: A string with the prefix of the elasticsearch index that will be created. Note a date with
    YYYY.MM.dd, ``python_logger`` used by default
  - index_name_frequency: The frequency to use as part of the index naming. Currently supports
    CMRESHandler.IndexNameFrequency.DAILY, CMRESHandler.IndexNameFrequency.WEEKLY,
    CMRESHandler.IndexNameFrequency.MONTHLY, CMRESHandler.IndexNameFrequency.YEARLY by default the daily rotation
    is used
- - es_doc_type: A string with the name of the document type that will be used ``python_log`` used by default
  - es_additional_fields: A dictionary with all the additional fields that you would like to add to the logs
 
 # Django Integration
 
 It is also very easy to integrate the handler to `Django <https://www.djangoproject.com/>`_ And what is even
 better, at DEBUG level django logs information such as how long it takes for DB connections to return so
 they can be plotted on Kibana, or the SQL statements that Django executed.
```

### Comparing `CMRESHandler-NtlmAuth-1.0.1/LICENSE.md` & `CMRESHandler-NtlmAuth-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CMRESHandler-NtlmAuth-1.0.1/PKG-INFO` & `CMRESHandler-NtlmAuth-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CMRESHandler-NtlmAuth
-Version: 1.0.1
+Version: 1.1.0
 Summary: Elasticsearch Log handler for the logging library
 Home-page: https://github.com/thoscilo/python-elasticsearch-logger/tree/release
 Author: Carlos Manzanedo Rueda
 Author-email: c.manaha@gmail.com
 License: Apache2
 Keywords: logging elasticsearch handler log django instrumentation
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,17 +17,23 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: elasticsearch
+Requires-Dist: requests
 Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
+Requires-Dist: six; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE.md
+Requires-Dist: coverage; extra == "test"
 
 ># Origin project location.
 > Please note that this repo is a fork from: https://github.com/cmanaha/python-elasticsearch-logger
 >
 > Base code is extended by:
 > - adding the HttpNtlmAuth as new authentication
 > - add support for elasticsearch 8.x version
@@ -150,15 +156,14 @@
  - flush_frequency_in_sec: A float representing how often and when the buffer will be flushed
  - es_index_name: A string with the prefix of the elasticsearch index that will be created. Note a date with
    YYYY.MM.dd, ``python_logger`` used by default
  - index_name_frequency: The frequency to use as part of the index naming. Currently supports
    CMRESHandler.IndexNameFrequency.DAILY, CMRESHandler.IndexNameFrequency.WEEKLY,
    CMRESHandler.IndexNameFrequency.MONTHLY, CMRESHandler.IndexNameFrequency.YEARLY by default the daily rotation
    is used
- - es_doc_type: A string with the name of the document type that will be used ``python_log`` used by default
  - es_additional_fields: A dictionary with all the additional fields that you would like to add to the logs
 
 # Django Integration
 
 It is also very easy to integrate the handler to `Django <https://www.djangoproject.com/>`_ And what is even
 better, at DEBUG level django logs information such as how long it takes for DB connections to return so
 they can be plotted on Kibana, or the SQL statements that Django executed.
```

### Comparing `CMRESHandler-NtlmAuth-1.0.1/README.md` & `CMRESHandler-NtlmAuth-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,14 @@
  - flush_frequency_in_sec: A float representing how often and when the buffer will be flushed
  - es_index_name: A string with the prefix of the elasticsearch index that will be created. Note a date with
    YYYY.MM.dd, ``python_logger`` used by default
  - index_name_frequency: The frequency to use as part of the index naming. Currently supports
    CMRESHandler.IndexNameFrequency.DAILY, CMRESHandler.IndexNameFrequency.WEEKLY,
    CMRESHandler.IndexNameFrequency.MONTHLY, CMRESHandler.IndexNameFrequency.YEARLY by default the daily rotation
    is used
- - es_doc_type: A string with the name of the document type that will be used ``python_log`` used by default
  - es_additional_fields: A dictionary with all the additional fields that you would like to add to the logs
 
 # Django Integration
 
 It is also very easy to integrate the handler to `Django <https://www.djangoproject.com/>`_ And what is even
 better, at DEBUG level django logs information such as how long it takes for DB connections to return so
 they can be plotted on Kibana, or the SQL statements that Django executed.
```

### Comparing `CMRESHandler-NtlmAuth-1.0.1/cmreslogging/handlers.py` & `CMRESHandler-NtlmAuth-1.1.0/cmreslogging/handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,14 @@
     __DEFAULT_VERIFY_SSL = True
     __DEFAULT_AUTH_TYPE = AuthType.NO_AUTH
     __DEFAULT_INDEX_FREQUENCY = IndexNameFrequency.DAILY
     __DEFAULT_BUFFER_SIZE = 1000
     __DEFAULT_FLUSH_FREQ_INSEC = 1
     __DEFAULT_ADDITIONAL_FIELDS = {}
     __DEFAULT_ES_INDEX_NAME = 'python_logger'
-    __DEFAULT_ES_DOC_TYPE = 'python_log'
     __DEFAULT_RAISE_ON_EXCEPTION = False
     __DEFAULT_TIMESTAMP_FIELD_NAME = "timestamp"
 
     __LOGGING_FILTER_FIELDS = ['msecs',
                                'relativeCreated',
                                'levelno',
                                'created']
@@ -147,15 +146,14 @@
                  aws_region=__DEFAULT_AWS_REGION,
                  auth_type=__DEFAULT_AUTH_TYPE,
                  verify_ssl=__DEFAULT_VERIFY_SSL,
                  buffer_size=__DEFAULT_BUFFER_SIZE,
                  flush_frequency_in_sec=__DEFAULT_FLUSH_FREQ_INSEC,
                  es_index_name=__DEFAULT_ES_INDEX_NAME,
                  index_name_frequency=__DEFAULT_INDEX_FREQUENCY,
-                 es_doc_type=__DEFAULT_ES_DOC_TYPE,
                  es_additional_fields=__DEFAULT_ADDITIONAL_FIELDS,
                  raise_on_indexing_exceptions=__DEFAULT_RAISE_ON_EXCEPTION,
                  default_timestamp_field_name=__DEFAULT_TIMESTAMP_FIELD_NAME):
         """ Handler constructor
 
         :param hosts: The list of hosts that elasticsearch clients will connect. The list can be provided
                     in the format ```[{'host':'host1','port':9200, 'scheme': 'http'},
@@ -179,16 +177,14 @@
                     if the buffer_size has not been reached yet
         :param es_index_name: A string with the prefix of the elasticsearch index that will be created. Note a
                     date with YYYY.MM.dd, ```python_logger``` used by default
         :param index_name_frequency: Defines what the date used in the postfix of the name would be. available values
                     are selected from the IndexNameFrequency class (IndexNameFrequency.DAILY,
                     IndexNameFrequency.WEEKLY, IndexNameFrequency.MONTHLY, IndexNameFrequency.YEARLY). By default
                     it uses daily indices.
-        :param es_doc_type: A string with the name of the document type that will be used ```python_log``` used
-                    by default
         :param es_additional_fields: A dictionary with all the additional fields that you would like to add
                     to the logs, such the application, environment, etc.
         :param raise_on_indexing_exceptions: A boolean, True only for debugging purposes to raise exceptions
                     caused when
         :return: A ready to be used CMRESHandler.
         """
         logging.Handler.__init__(self)
@@ -200,15 +196,14 @@
         self.aws_region = aws_region
         self.auth_type = auth_type
         self.verify_certs = verify_ssl
         self.buffer_size = buffer_size
         self.flush_frequency_in_sec = flush_frequency_in_sec
         self.es_index_name = es_index_name
         self.index_name_frequency = index_name_frequency
-        self.es_doc_type = es_doc_type
         self.es_additional_fields = es_additional_fields.copy()
         self.es_additional_fields.update({'host': socket.gethostname(),
                                           'host_ip': socket.gethostbyname(socket.gethostname())})
         self.raise_on_indexing_exceptions = raise_on_indexing_exceptions
         self.default_timestamp_field_name = default_timestamp_field_name
 
         self._client = None
@@ -308,26 +303,20 @@
         self._timer = None
 
         if self._buffer:
             try:
                 with self._buffer_lock:
                     logs_buffer = self._buffer
                     self._buffer = []
-                actions = (
-                    {
-                        '_index': self._index_name_func.__func__(self.es_index_name),
-                        '_type': self.es_doc_type,
-                        '_source': log_record
-                    }
-                    for log_record in logs_buffer
-                )
+
                 eshelpers.bulk(
                     client=self.__get_es_client(),
-                    actions=actions,
-                    stats_only=True
+                    actions=logs_buffer,
+                    stats_only=True,
+                    index=self._index_name_func.__func__(self.es_index_name)
                 )
             except Exception as exception:
                 if self.raise_on_indexing_exceptions:
                     raise exception
 
     def close(self):
         """ Flushes the buffer and release any outstanding resource
```

### Comparing `CMRESHandler-NtlmAuth-1.0.1/cmreslogging/serializers.py` & `CMRESHandler-NtlmAuth-1.1.0/cmreslogging/serializers.py`

 * *Files identical despite different names*

### Comparing `CMRESHandler-NtlmAuth-1.0.1/setup.py` & `CMRESHandler-NtlmAuth-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 setup(
     name='CMRESHandler-NtlmAuth',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.1',
+    version='1.1.0',
 
     description='Elasticsearch Log handler for the logging library',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
 
     # The project's main homepage.
```

### Comparing `CMRESHandler-NtlmAuth-1.0.1/tests/test_cmreshandler.py` & `CMRESHandler-NtlmAuth-1.1.0/tests/test_cmreshandler.py`

 * *Files identical despite different names*

### Comparing `CMRESHandler-NtlmAuth-1.0.1/tests/test_cmresserializer.py` & `CMRESHandler-NtlmAuth-1.1.0/tests/test_cmresserializer.py`

 * *Files identical despite different names*

