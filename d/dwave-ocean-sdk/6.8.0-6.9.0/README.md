# Comparing `tmp/dwave-ocean-sdk-6.8.0.tar.gz` & `tmp/dwave-ocean-sdk-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwave-ocean-sdk-6.8.0.tar", last modified: Tue Jan 16 18:48:13 2024, max compression
+gzip compressed data, was "dwave-ocean-sdk-6.9.0.tar", last modified: Fri Mar  1 18:05:46 2024, max compression
```

## Comparing `dwave-ocean-sdk-6.8.0.tar` & `dwave-ocean-sdk-6.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-16 18:48:13.037906 dwave-ocean-sdk-6.8.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-01-16 18:47:38.000000 dwave-ocean-sdk-6.8.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5694 2024-01-16 18:48:13.037906 dwave-ocean-sdk-6.8.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4143 2024-01-16 18:47:38.000000 dwave-ocean-sdk-6.8.0/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-16 18:48:13.037906 dwave-ocean-sdk-6.8.0/dwave_ocean_sdk.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5694 2024-01-16 18:48:13.000000 dwave-ocean-sdk-6.8.0/dwave_ocean_sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2024-01-16 18:48:13.000000 dwave-ocean-sdk-6.8.0/dwave_ocean_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-01-16 18:48:13.000000 dwave-ocean-sdk-6.8.0/dwave_ocean_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      321 2024-01-16 18:48:13.000000 dwave-ocean-sdk-6.8.0/dwave_ocean_sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-01-16 18:48:13.000000 dwave-ocean-sdk-6.8.0/dwave_ocean_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-16 18:48:13.033906 dwave-ocean-sdk-6.8.0/dwaveoceansdk/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      604 2024-01-16 18:47:38.000000 dwave-ocean-sdk-6.8.0/dwaveoceansdk/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      883 2024-01-16 18:47:38.000000 dwave-ocean-sdk-6.8.0/dwaveoceansdk/package_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-01-16 18:47:38.000000 dwave-ocean-sdk-6.8.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1383 2024-01-16 18:48:13.037906 dwave-ocean-sdk-6.8.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2024-01-16 18:47:38.000000 dwave-ocean-sdk-6.8.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-16 18:48:13.037906 dwave-ocean-sdk-6.8.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3134 2024-01-16 18:47:38.000000 dwave-ocean-sdk-6.8.0/tests/test_individually.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-01 18:05:46.468972 dwave-ocean-sdk-6.9.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-03-01 18:05:16.000000 dwave-ocean-sdk-6.9.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5694 2024-03-01 18:05:46.468972 dwave-ocean-sdk-6.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4143 2024-03-01 18:05:16.000000 dwave-ocean-sdk-6.9.0/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-01 18:05:46.468972 dwave-ocean-sdk-6.9.0/dwave_ocean_sdk.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5694 2024-03-01 18:05:46.000000 dwave-ocean-sdk-6.9.0/dwave_ocean_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2024-03-01 18:05:46.000000 dwave-ocean-sdk-6.9.0/dwave_ocean_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-01 18:05:46.000000 dwave-ocean-sdk-6.9.0/dwave_ocean_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      321 2024-03-01 18:05:46.000000 dwave-ocean-sdk-6.9.0/dwave_ocean_sdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-03-01 18:05:46.000000 dwave-ocean-sdk-6.9.0/dwave_ocean_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-01 18:05:46.468972 dwave-ocean-sdk-6.9.0/dwaveoceansdk/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      604 2024-03-01 18:05:16.000000 dwave-ocean-sdk-6.9.0/dwaveoceansdk/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      883 2024-03-01 18:05:16.000000 dwave-ocean-sdk-6.9.0/dwaveoceansdk/package_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-03-01 18:05:16.000000 dwave-ocean-sdk-6.9.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1383 2024-03-01 18:05:46.472972 dwave-ocean-sdk-6.9.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2024-03-01 18:05:16.000000 dwave-ocean-sdk-6.9.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-01 18:05:46.468972 dwave-ocean-sdk-6.9.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3134 2024-03-01 18:05:16.000000 dwave-ocean-sdk-6.9.0/tests/test_individually.py
```

### Comparing `dwave-ocean-sdk-6.8.0/LICENSE` & `dwave-ocean-sdk-6.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dwave-ocean-sdk-6.8.0/PKG-INFO` & `dwave-ocean-sdk-6.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-ocean-sdk
-Version: 6.8.0
+Version: 6.9.0
 Summary: Software development kit for open source D-Wave tools
 Home-page: https://github.com/dwavesystems/dwave-ocean-sdk
 Author: D-Wave Systems Inc.
 Author-email: tools@dwavesys.com
 License: Apache 2.0
 Project-URL: Changes, https://github.com/dwavesystems/dwave-ocean-sdk/releases
 Project-URL: Documentation, https://docs.ocean.dwavesys.com
@@ -17,17 +17,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: dimod==0.12.14
-Requires-Dist: dwave-cloud-client==0.11.2
+Requires-Dist: dwave-cloud-client==0.11.3
 Requires-Dist: dwave-greedy==0.3.0
-Requires-Dist: dwave-hybrid==0.6.10
+Requires-Dist: dwave-hybrid==0.6.11
 Requires-Dist: dwave-inspector==0.4.4
 Requires-Dist: dwave-neal==0.6.0
 Requires-Dist: dwave-networkx==0.8.14
 Requires-Dist: dwave-preprocessing==0.6.5
 Requires-Dist: dwave-samplers==1.2.0
 Requires-Dist: dwave-system==1.23.0
 Requires-Dist: dwave-tabu==0.5.0
```

### Comparing `dwave-ocean-sdk-6.8.0/README.rst` & `dwave-ocean-sdk-6.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `dwave-ocean-sdk-6.8.0/dwave_ocean_sdk.egg-info/PKG-INFO` & `dwave-ocean-sdk-6.9.0/dwave_ocean_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-ocean-sdk
-Version: 6.8.0
+Version: 6.9.0
 Summary: Software development kit for open source D-Wave tools
 Home-page: https://github.com/dwavesystems/dwave-ocean-sdk
 Author: D-Wave Systems Inc.
 Author-email: tools@dwavesys.com
 License: Apache 2.0
 Project-URL: Changes, https://github.com/dwavesystems/dwave-ocean-sdk/releases
 Project-URL: Documentation, https://docs.ocean.dwavesys.com
@@ -17,17 +17,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: dimod==0.12.14
-Requires-Dist: dwave-cloud-client==0.11.2
+Requires-Dist: dwave-cloud-client==0.11.3
 Requires-Dist: dwave-greedy==0.3.0
-Requires-Dist: dwave-hybrid==0.6.10
+Requires-Dist: dwave-hybrid==0.6.11
 Requires-Dist: dwave-inspector==0.4.4
 Requires-Dist: dwave-neal==0.6.0
 Requires-Dist: dwave-networkx==0.8.14
 Requires-Dist: dwave-preprocessing==0.6.5
 Requires-Dist: dwave-samplers==1.2.0
 Requires-Dist: dwave-system==1.23.0
 Requires-Dist: dwave-tabu==0.5.0
```

### Comparing `dwave-ocean-sdk-6.8.0/dwaveoceansdk/__init__.py` & `dwave-ocean-sdk-6.9.0/dwaveoceansdk/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '6.8.0'
+__version__ = '6.9.0'
```

### Comparing `dwave-ocean-sdk-6.8.0/dwaveoceansdk/package_info.py` & `dwave-ocean-sdk-6.9.0/dwaveoceansdk/package_info.py`

 * *Files identical despite different names*

### Comparing `dwave-ocean-sdk-6.8.0/setup.cfg` & `dwave-ocean-sdk-6.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 author = D-Wave Systems Inc.
 author_email = tools@dwavesys.com
 description = Software development kit for open source D-Wave tools
 
 [options]
 install_requires = 
 	dimod==0.12.14
-	dwave-cloud-client==0.11.2
+	dwave-cloud-client==0.11.3
 	dwave-greedy==0.3.0
-	dwave-hybrid==0.6.10
+	dwave-hybrid==0.6.11
 	dwave-inspector==0.4.4
 	dwave-neal==0.6.0
 	dwave-networkx==0.8.14
 	dwave-preprocessing==0.6.5
 	dwave-samplers==1.2.0
 	dwave-system==1.23.0
 	dwave-tabu==0.5.0
```

### Comparing `dwave-ocean-sdk-6.8.0/setup.py` & `dwave-ocean-sdk-6.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `dwave-ocean-sdk-6.8.0/tests/test_individually.py` & `dwave-ocean-sdk-6.9.0/tests/test_individually.py`

 * *Files identical despite different names*

