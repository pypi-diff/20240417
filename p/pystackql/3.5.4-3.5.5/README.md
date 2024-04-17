# Comparing `tmp/pystackql-3.5.4.tar.gz` & `tmp/pystackql-3.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystackql-3.5.4.tar", last modified: Thu Apr 11 04:43:56 2024, max compression
+gzip compressed data, was "pystackql-3.5.5.tar", last modified: Wed Apr 17 03:51:23 2024, max compression
```

## Comparing `pystackql-3.5.4.tar` & `pystackql-3.5.5.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-11 04:43:56.644050 pystackql-3.5.4/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 pystackql-3.5.4/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)     6948 2024-04-11 04:43:56.635576 pystackql-3.5.4/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5176 2024-04-11 04:43:41.000000 pystackql-3.5.4/README.rst
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-11 04:43:56.223930 pystackql-3.5.4/pystackql/
--rwxrwxrwx   0 javen     (1000) javen     (1000)      101 2024-03-15 01:52:38.000000 pystackql-3.5.4/pystackql/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5209 2024-03-15 01:52:38.000000 pystackql-3.5.4/pystackql/_util.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1751 2024-03-15 01:52:38.000000 pystackql-3.5.4/pystackql/base_stackql_magic.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1740 2024-03-15 01:52:38.000000 pystackql-3.5.4/pystackql/magic.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1743 2024-03-15 01:52:38.000000 pystackql-3.5.4/pystackql/magics.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)    25338 2024-04-11 04:38:32.000000 pystackql-3.5.4/pystackql/stackql.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-11 04:43:56.572406 pystackql-3.5.4/pystackql.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     6948 2024-04-11 04:43:55.000000 pystackql-3.5.4/pystackql.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      324 2024-04-11 04:43:55.000000 pystackql-3.5.4/pystackql.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-11 04:43:55.000000 pystackql-3.5.4/pystackql.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       24 2024-04-11 04:43:55.000000 pystackql-3.5.4/pystackql.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       10 2024-04-11 04:43:55.000000 pystackql-3.5.4/pystackql.egg-info/top_level.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-11 04:43:56.647414 pystackql-3.5.4/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1254 2024-04-11 04:43:41.000000 pystackql-3.5.4/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 03:51:23.008951 pystackql-3.5.5/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 pystackql-3.5.5/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     6997 2024-04-17 03:51:22.982606 pystackql-3.5.5/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5176 2024-04-17 03:50:46.000000 pystackql-3.5.5/README.rst
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 03:51:22.455032 pystackql-3.5.5/pystackql/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      101 2024-04-12 21:02:08.000000 pystackql-3.5.5/pystackql/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5209 2024-03-15 01:52:38.000000 pystackql-3.5.5/pystackql/_util.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1751 2024-03-15 01:52:38.000000 pystackql-3.5.5/pystackql/base_stackql_magic.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1740 2024-03-15 01:52:38.000000 pystackql-3.5.5/pystackql/magic.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1743 2024-03-15 01:52:38.000000 pystackql-3.5.5/pystackql/magics.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    26007 2024-04-17 03:50:46.000000 pystackql-3.5.5/pystackql/stackql.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 03:51:22.955498 pystackql-3.5.5/pystackql.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     6997 2024-04-17 03:51:21.000000 pystackql-3.5.5/pystackql.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      345 2024-04-17 03:51:21.000000 pystackql-3.5.5/pystackql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-17 03:51:21.000000 pystackql-3.5.5/pystackql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       24 2024-04-17 03:51:21.000000 pystackql-3.5.5/pystackql.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       10 2024-04-17 03:51:21.000000 pystackql-3.5.5/pystackql.egg-info/top_level.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-17 03:51:23.013531 pystackql-3.5.5/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1254 2024-04-17 03:50:46.000000 pystackql-3.5.5/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 03:51:22.872036 pystackql-3.5.5/tests/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     2348 2024-04-07 22:41:05.000000 pystackql-3.5.5/tests/test_params.py
```

### Comparing `pystackql-3.5.4/LICENSE` & `pystackql-3.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.4/PKG-INFO` & `pystackql-3.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystackql
-Version: 3.5.4
+Version: 3.5.5
 Summary: A Python interface for StackQL
 Home-page: https://github.com/stackql/pystackql
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT License
         
         Copyright (c) 2022 StackQL Studios
@@ -22,26 +22,28 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Platform: UNKNOWN
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: pandas
+Requires-Dist: IPython
 
 .. image:: https://stackql.io/img/stackql-logo-bold.png
     :alt: "stackql logo"
     :target: https://github.com/stackql/stackql
     :align: center
 
 ======================================
@@ -231,10 +233,8 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload dist/pystackql-3.5.4.tar.gz
-
-
+    twine upload dist/pystackql-3.5.5.tar.gz
```

### Comparing `pystackql-3.5.4/README.rst` & `pystackql-3.5.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -190,8 +190,8 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload dist/pystackql-3.5.4.tar.gz
+    twine upload dist/pystackql-3.5.5.tar.gz
```

### Comparing `pystackql-3.5.4/pystackql/_util.py` & `pystackql-3.5.5/pystackql/_util.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.4/pystackql/base_stackql_magic.py` & `pystackql-3.5.5/pystackql/base_stackql_magic.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.4/pystackql/magic.py` & `pystackql-3.5.5/pystackql/magic.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.4/pystackql/magics.py` & `pystackql-3.5.5/pystackql/magics.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.4/pystackql/stackql.py` & `pystackql-3.5.5/pystackql/stackql.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,19 @@
 				"doc": e.__doc__,
 				"params": local_params,
 				"stdout": stdout.decode('utf-8') if 'stdout' in locals() and isinstance(stdout, bytes) else "",
 				"stderr": stderr.decode('utf-8') if 'stderr' in locals() and isinstance(stderr, bytes) else ""
 			}
 			output["exception"] = f"ERROR: {json.dumps(error_details)}"
 
+		# output = {'data': <stdout str>, 'error': <stderr str>, 'exception': <exception as a json string> }
+		# for a statement you would expect 'error' to exist
+		# for a query you would expect 'data' to exist
+		# 'exception' in output indicates an error occurred during the execution (statement or query)
+
 		return output
 
 	def __init__(self, 
 				 server_mode=False, 
 				 server_address='127.0.0.1', 
 				 server_port=5466,
 				 backend_storage_mode='memory',
@@ -478,41 +483,44 @@
 				return pd.DataFrame(result)
 			elif self.output == 'csv':
 				# return the string representation of the result
 				return result[0]['message']
 			else:
 				return result
 		else:
+			# returns either...
+			# {'error': '<error message>'} if something went wrong; or
+			# {'message': '<message>'} if the statement was executed successfully
 			result = self._run_query(query)
 			if "exception" in result:
 				return {"error": result["exception"]}
 
 			# message on stderr
 			message = result["error"]
 
 			if self.output == 'pandas':
 				return pd.DataFrame({'message': [message]}) if message else pd.DataFrame({'message': []})
 			elif self.output == 'csv':
 				return message
 			else:
-				return [{'message': message}]			
+				return {'message': message}			
 	
 	def execute(self, query, suppress_errors=True):
 		"""
 		Executes a StackQL query and returns the output based on the specified output format.
 
 		This method supports execution both in server mode and locally using subprocess. In server mode,
 		the query is sent to a StackQL server, while in local mode, it runs the query using a local binary.
 
 		Args:
 			query (str): The StackQL query string to be executed.
 			suppress_errors (bool, optional): If set to True, the method will return an empty list if an error occurs.
 
 		Returns:
-			dict, pd.DataFrame, or str: The output of the query, which can be a dictionary, a Pandas DataFrame,
+			list(dict), pd.DataFrame, or str: The output of the query, which can be a list of dictionary objects, a Pandas DataFrame,
 			or a raw CSV string, depending on the configured output format.
 
 		Raises:
 			ValueError: If an unsupported output format is specified.
 
 		Examples:
 			>>> stackql = StackQL()
@@ -530,14 +538,18 @@
 				json_str = json.dumps(result)
 				return pd.read_json(StringIO(json_str))
 			elif self.output == 'csv':
 				raise ValueError("CSV output is not supported in server_mode.")
 			else:  # Assume 'dict' output
 				return result
 		else:
+			# returns either...
+			# {'error': <error json str>} if something went wrong; or
+			# [{<data>}] if the statement was executed successfully, messages to stderr are ignored
+
 			output = self._run_query(query)
 			if "exception" in output:
 				return {"error": output["exception"]}
 
 			if "data" in output:
 				# theres data, return it
 				if self.output == 'csv':
```

### Comparing `pystackql-3.5.4/pystackql.egg-info/PKG-INFO` & `pystackql-3.5.5/pystackql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystackql
-Version: 3.5.4
+Version: 3.5.5
 Summary: A Python interface for StackQL
 Home-page: https://github.com/stackql/pystackql
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT License
         
         Copyright (c) 2022 StackQL Studios
@@ -22,26 +22,28 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Platform: UNKNOWN
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: pandas
+Requires-Dist: IPython
 
 .. image:: https://stackql.io/img/stackql-logo-bold.png
     :alt: "stackql logo"
     :target: https://github.com/stackql/stackql
     :align: center
 
 ======================================
@@ -231,10 +233,8 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload dist/pystackql-3.5.4.tar.gz
-
-
+    twine upload dist/pystackql-3.5.5.tar.gz
```

### Comparing `pystackql-3.5.4/setup.py` & `pystackql-3.5.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     readme = f.read()
 
 with open('LICENSE') as f:
     license = f.read()
 
 setup(
     name='pystackql',
-    version='3.5.4',
+    version='3.5.5',
     description='A Python interface for StackQL',
     long_description=readme,
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/pystackql',
     license=license,
     packages=['pystackql'],
```

