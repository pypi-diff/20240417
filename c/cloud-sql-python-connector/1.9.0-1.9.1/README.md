# Comparing `tmp/cloud-sql-python-connector-1.9.0.tar.gz` & `tmp/cloud-sql-python-connector-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-sql-python-connector-1.9.0.tar", last modified: Tue Apr 16 15:44:45 2024, max compression
+gzip compressed data, was "cloud-sql-python-connector-1.9.1.tar", last modified: Wed Apr 17 15:49:02 2024, max compression
```

## Comparing `cloud-sql-python-connector-1.9.0.tar` & `cloud-sql-python-connector-1.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:44:45.683349 cloud-sql-python-connector-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/LICENSE
--rw-r--r--   0 root         (0)     1003    23771 2024-04-16 15:44:45.683349 cloud-sql-python-connector-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003    22623 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/README.md
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:44:45.679346 cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/
--rw-r--r--   0 root         (0)     1003    23771 2024-04-16 15:44:45.000000 cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      876 2024-04-16 15:44:45.000000 cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-16 15:44:45.000000 cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-16 15:44:45.000000 cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      156 2024-04-16 15:44:45.000000 cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-04-16 15:44:45.000000 cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:44:45.679346 cloud-sql-python-connector-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:44:45.679346 cloud-sql-python-connector-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:44:45.679346 cloud-sql-python-connector-1.9.0/google/cloud/sql/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:44:45.683349 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/
--rw-rw-r--   0 root         (0)     1003      883 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/__init__.py
--rw-rw-r--   0 root         (0)     1003     1838 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/asyncpg.py
--rw-rw-r--   0 root         (0)     1003     8494 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/client.py
--rwxrwxr-x   0 root         (0)     1003    19188 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/connector.py
--rw-rw-r--   0 root         (0)     1003     1524 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/exceptions.py
--rw-rw-r--   0 root         (0)     1003    14920 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/instance.py
--rw-rw-r--   0 root         (0)     1003     1814 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/pg8000.py
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/py.typed
--rw-rw-r--   0 root         (0)     1003     2105 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/pymysql.py
--rw-rw-r--   0 root         (0)     1003     2452 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/pytds.py
--rw-rw-r--   0 root         (0)     1003     2993 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/rate_limiter.py
--rw-rw-r--   0 root         (0)     1003     3680 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/refresh_utils.py
--rwxrwxr-x   0 root         (0)     1003     3448 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/utils.py
--rw-rw-r--   0 root         (0)     1003      597 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/version.py
--rw-rw-r--   0 root         (0)     1003       67 2024-04-16 15:44:45.683349 cloud-sql-python-connector-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2897 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 15:49:02.040125 cloud-sql-python-connector-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/LICENSE
+-rw-r--r--   0 root         (0)     1003    23771 2024-04-17 15:49:02.040125 cloud-sql-python-connector-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003    22623 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/README.md
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 15:49:02.036124 cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/
+-rw-r--r--   0 root         (0)     1003    23771 2024-04-17 15:49:01.000000 cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      876 2024-04-17 15:49:02.000000 cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-17 15:49:01.000000 cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-17 15:49:01.000000 cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      164 2024-04-17 15:49:01.000000 cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-17 15:49:01.000000 cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 15:49:02.032124 cloud-sql-python-connector-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 15:49:02.032124 cloud-sql-python-connector-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 15:49:02.032124 cloud-sql-python-connector-1.9.1/google/cloud/sql/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 15:49:02.040125 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/
+-rw-rw-r--   0 root         (0)     1003      883 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1838 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/asyncpg.py
+-rw-rw-r--   0 root         (0)     1003     8494 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/client.py
+-rwxrwxr-x   0 root         (0)     1003    19188 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/connector.py
+-rw-rw-r--   0 root         (0)     1003     1524 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/exceptions.py
+-rw-rw-r--   0 root         (0)     1003    14920 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/instance.py
+-rw-rw-r--   0 root         (0)     1003     1814 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/pg8000.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/py.typed
+-rw-rw-r--   0 root         (0)     1003     2105 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/pymysql.py
+-rw-rw-r--   0 root         (0)     1003     2452 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/pytds.py
+-rw-rw-r--   0 root         (0)     1003     2993 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/rate_limiter.py
+-rw-rw-r--   0 root         (0)     1003     3680 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/refresh_utils.py
+-rwxrwxr-x   0 root         (0)     1003     3448 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/utils.py
+-rw-rw-r--   0 root         (0)     1003      597 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/version.py
+-rw-rw-r--   0 root         (0)     1003       67 2024-04-17 15:49:02.040125 cloud-sql-python-connector-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2905 2024-04-17 15:46:33.000000 cloud-sql-python-connector-1.9.1/setup.py
```

### Comparing `cloud-sql-python-connector-1.9.0/LICENSE` & `cloud-sql-python-connector-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.0/PKG-INFO` & `cloud-sql-python-connector-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-sql-python-connector
-Version: 1.9.0
+Version: 1.9.1
 Summary: The Cloud SQL Python Connector is a library that can be used alongside a database driver to allow users with sufficient permissions to connect to a Cloud SQL database without having to manually allowlist IPs or manage SSL certificates.
 Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-sql-python-connector Version: 1.9.0 Summary:
+Metadata-Version: 2.1 Name: cloud-sql-python-connector Version: 1.9.1 Summary:
 The Cloud SQL Python Connector is a library that can be used alongside a
 database driver to allow users with sufficient permissions to connect to a
 Cloud SQL database without having to manually allowlist IPs or manage SSL
 certificates. Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-
 python-connector Author: Google LLC Author-email: googleapis-
 packages@google.com License: Apache 2.0 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
```

### Comparing `cloud-sql-python-connector-1.9.0/README.md` & `cloud-sql-python-connector-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/PKG-INFO` & `cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-sql-python-connector
-Version: 1.9.0
+Version: 1.9.1
 Summary: The Cloud SQL Python Connector is a library that can be used alongside a database driver to allow users with sufficient permissions to connect to a Cloud SQL database without having to manually allowlist IPs or manage SSL certificates.
 Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-sql-python-connector Version: 1.9.0 Summary:
+Metadata-Version: 2.1 Name: cloud-sql-python-connector Version: 1.9.1 Summary:
 The Cloud SQL Python Connector is a library that can be used alongside a
 database driver to allow users with sufficient permissions to connect to a
 Cloud SQL database without having to manually allowlist IPs or manage SSL
 certificates. Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-
 python-connector Author: Google LLC Author-email: googleapis-
 packages@google.com License: Apache 2.0 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
```

### Comparing `cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/SOURCES.txt` & `cloud-sql-python-connector-1.9.1/cloud_sql_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/__init__.py` & `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/asyncpg.py` & `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/asyncpg.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/client.py` & `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/client.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/connector.py` & `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/connector.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/exceptions.py` & `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/instance.py` & `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/instance.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/pg8000.py` & `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/pg8000.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/pymysql.py` & `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/pymysql.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/pytds.py` & `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/pytds.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/rate_limiter.py` & `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/refresh_utils.py` & `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/refresh_utils.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/utils.py` & `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/version.py` & `cloud-sql-python-connector-1.9.1/google/cloud/sql/connector/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
```

### Comparing `cloud-sql-python-connector-1.9.0/setup.py` & `cloud-sql-python-connector-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     " to manually allowlist IPs or manage SSL certificates."
 )
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     "aiohttp",
     "cryptography>=42.0.0",
     "Requests",
-    "google-auth",
+    "google-auth>=2.28.0",
 ]
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.md")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

