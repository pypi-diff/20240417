# Comparing `tmp/oteltest-0.7.1.tar.gz` & `tmp/oteltest-0.8.0.tar.gz`

## Comparing `oteltest-0.7.1.tar` & `oteltest-0.8.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rwxr-xr-x   0        0        0     1484 2020-02-02 00:00:00.000000 oteltest-0.7.1/example_scripts/simple_loop.py
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 oteltest-0.7.1/src/oteltest/__init__.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 oteltest-0.7.1/src/oteltest/main.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 oteltest-0.7.1/src/oteltest/private.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.7.1/src/oteltest/version.py
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 oteltest-0.7.1/src/oteltest/sink/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 oteltest-0.7.1/src/oteltest/sink/private.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 oteltest-0.7.1/tests/test_oteltest.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.7.1/.gitignore
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 oteltest-0.7.1/README.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 oteltest-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 oteltest-0.8.0/example_scripts/client_server.0.json
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 oteltest-0.8.0/example_scripts/client_server.1.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 oteltest-0.8.0/example_scripts/client_server.py
+-rw-r--r--   0        0        0     7637 2020-02-02 00:00:00.000000 oteltest-0.8.0/example_scripts/simple_loop.0.json
+-rw-r--r--   0        0        0     7637 2020-02-02 00:00:00.000000 oteltest-0.8.0/example_scripts/simple_loop.1.json
+-rwxr-xr-x   0        0        0     1438 2020-02-02 00:00:00.000000 oteltest-0.8.0/example_scripts/simple_loop.py
+-rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 oteltest-0.8.0/src/oteltest/__init__.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 oteltest-0.8.0/src/oteltest/main.py
+-rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 oteltest-0.8.0/src/oteltest/private.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.8.0/src/oteltest/version.py
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 oteltest-0.8.0/src/oteltest/sink/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 oteltest-0.8.0/src/oteltest/sink/private.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 oteltest-0.8.0/tests/test_oteltest.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.8.0/.gitignore
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 oteltest-0.8.0/README.md
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 oteltest-0.8.0/PKG-INFO
```

### Comparing `oteltest-0.7.1/example_scripts/simple_loop.py` & `oteltest-0.8.0/example_scripts/simple_loop.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,18 +31,15 @@
 class MyOtelTest(OtelTest):
     def requirements(self):
         return "opentelemetry-distro", "opentelemetry-exporter-otlp-proto-grpc"
 
     def environment_variables(self):
         return {"OTEL_SERVICE_NAME": SERVICE_NAME}
 
-    def wrapper_script(self):
+    def wrapper(self):
         return "opentelemetry-instrument"
 
-    def on_script_start(self):
+    def on_start(self):
         return None
 
-    def on_script_end(self, stdout, stderr, returncode) -> None:
-        pass
-
-    def on_shutdown(self, telemetry: Telemetry):
+    def on_stop(self, telemetry: Telemetry, stdout: str, stderr: str, returncode: int) -> None:
         assert telemetry.num_spans() == NUM_ADDS
```

### Comparing `oteltest-0.7.1/src/oteltest/main.py` & `oteltest-0.8.0/src/oteltest/main.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.7.1/src/oteltest/private.py` & `oteltest-0.8.0/src/oteltest/private.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,23 +61,23 @@
     oteltest_dep = wheel_file or "oteltest"
     run_subprocess([pip_path, "install", oteltest_dep])
 
     for req in oteltest_instance.requirements():
         print(f"- Will install requirement: '{req}'")
         run_subprocess([pip_path, "install", req])
 
-    run_python_script(script, script_dir, oteltest_instance, v)
+    stdout, stderr, returncode = run_python_script(script, script_dir, oteltest_instance, v)
 
     v.rm()
 
     filename = get_next_json_file(script_dir, module_name)
     print(f"- Will save telemetry to {filename}")
     save_telemetry_json(script_dir, filename, handler.telemetry_to_json())
 
-    oteltest_instance.on_shutdown(handler.telemetry)
+    oteltest_instance.on_stop(handler.telemetry, stdout, stderr, returncode)
     print(f"- {script} PASSED")
 
 
 def get_next_json_file(path_to_dir: str, module_name: str):
     p = Path(path_to_dir)
     max_index = -1
     for file in p.glob(f"{module_name}.*.json"):
@@ -91,45 +91,43 @@
 
 def save_telemetry_json(script_dir: str, file_name: str, json_str: str):
     path = Path(script_dir) / file_name
     with open(str(path), "w") as file:
         file.write(json_str)
 
 
-def run_python_script(script, script_dir, oteltest_instance: OtelTest, v):
+def run_python_script(script, script_dir, oteltest_instance: OtelTest, v) -> typing.Tuple[str, str, int]:
     python_script_cmd = [
         v.path_to_executable("python"),
         str(Path(script_dir) / script),
     ]
 
-    wrapper_script = oteltest_instance.wrapper_script()
+    wrapper_script = oteltest_instance.wrapper()
     if wrapper_script is not None:
         python_script_cmd.insert(0, v.path_to_executable(wrapper_script))
 
     sprocess = subprocess.Popen(
         python_script_cmd,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         text=True,
         env=oteltest_instance.environment_variables(),
     )
 
-    timeout = oteltest_instance.on_script_start()
+    timeout = oteltest_instance.on_start()
     if timeout is None:
         print(
-            f"- Will wait indefinitely for {script} to finish (on_script_start() returned None)"
+            f"- Will wait indefinitely for {script} to finish (on_start() returned None)"
         )
     else:
         print(
             f"- Will wait for up to {timeout} seconds for {script} to finish"
         )
 
-    stdout, stderr, returncode = wait_for_subprocess(sprocess, script, timeout)
-    print_result(stdout, stderr, returncode)
-    oteltest_instance.on_script_end(stdout, stderr, returncode)
+    return wait_for_subprocess(sprocess, script, timeout)
 
 
 def wait_for_subprocess(
     process: subprocess.Popen, script, timeout
 ) -> typing.Tuple[str, str, int]:
     try:
         stdout, stderr = process.communicate(timeout=timeout)
```

### Comparing `oteltest-0.7.1/src/oteltest/version.py` & `oteltest-0.8.0/src/oteltest/version.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.7.1"
+__version__ = "0.8.0"
```

### Comparing `oteltest-0.7.1/src/oteltest/sink/__init__.py` & `oteltest-0.8.0/src/oteltest/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.7.1/src/oteltest/sink/private.py` & `oteltest-0.8.0/src/oteltest/sink/private.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.7.1/tests/__init__.py` & `oteltest-0.8.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.7.1/tests/test_oteltest.py` & `oteltest-0.8.0/tests/test_oteltest.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.7.1/.gitignore` & `oteltest-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oteltest-0.7.1/LICENSE.txt` & `oteltest-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oteltest-0.7.1/README.md` & `oteltest-0.8.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,30 +14,20 @@
 
 ```console
 pip install oteltest
 ```
 
 ## Overview
 
-The `oteltest` package contains utilities for testing OpenTelemetry Python. The motivation for oteltest is to provide
-an easy way to test OpenTelemetry Python, which involves a Python environment with specific packages
+The `oteltest` package contains utilities for testing OpenTelemetry Python.
 
 ### oteltest
 
 The `oteltest` command runs black box tests against Python scripts that send telemetry.
 
-
-#### Motivation
-
-The motivation for oteltest is to make it as easy as possible to run code that emits telemetry, with all of the
-information required to run a test co-located with the code being tested. With that in place, you should be able to
-point something at it that sets up the environment, runs the script, records the telemetry that the script sends, and
-sends that telemetry back to the script so that the validate can be co-located with the test configuration, and the test
-code.
-
 #### Execution
 
 Run `oteltest` as a shell command and provide a directory as an argument:
 
 ```shell
 oteltest my_script_dir
 ```
@@ -46,57 +36,60 @@
 
 #### Operation
 
 Running `oteltest` against a directory containing `my_script.py`
 
 1) Starts an [otelsink](#otelsink) instance
 2) Creates a new Python virtual environment with `requirements()`
-3) Using that new environment, starts running `my_script.py` in a subprocess
+3) In that environment, starts running `my_script.py` in a subprocess
 4) Meanwhile, calls `OtelTest#on_script_start()` waiting until completion
 5) Depending on the return value from `on_script_start()`, waits for `my_script.py` to complete or interrupts
 6) Stops the OTLP listener
 7) Calls `validate(telemetry)` with otelsink's received telemetry
-8) Writes the telemetry to a `.json` file next to the script (script name but `.json`)
+8) Writes the telemetry to a `.json` file next to the script (script name but with ".{number}.json" instead of ".py")
 
 #### Script Eligibility
 
 For a Python script to be runnable by `oteltest`, it must both be executable and define an implementation of the
-[OtelTest]() abstract base class. The script below has an implementation called `MyTest`:
+[OtelTest]() abstract base class. The script below has an implementation called `MyOtelTest`:
 
 ```python
 import time
 
 from opentelemetry import trace
 from oteltest import OtelTest, Telemetry
 
-SERVICE_NAME = "integration-test"
+SERVICE_NAME = "my-otel-test"
 NUM_ADDS = 12
 
 if __name__ == "__main__":
     tracer = trace.get_tracer("my-tracer")
     for i in range(NUM_ADDS):
         with tracer.start_as_current_span("my-span"):
-            print(f"simple_loop.py: {i + 1}/{NUM_ADDS}")
+            print(f"simple_loop.py: {i+1}/{NUM_ADDS}")
             time.sleep(0.5)
 
 
-class MyTest(OtelTest):
+class MyOtelTest(OtelTest):
     def requirements(self):
         return "opentelemetry-distro", "opentelemetry-exporter-otlp-proto-grpc"
 
     def environment_variables(self):
         return {"OTEL_SERVICE_NAME": SERVICE_NAME}
 
     def wrapper_script(self):
         return "opentelemetry-instrument"
 
     def on_script_start(self):
         return None
 
-    def validate(self, telemetry: Telemetry):
+    def on_script_end(self, stdout, stderr, returncode) -> None:
+        pass
+
+    def on_shutdown(self, telemetry: Telemetry):
         assert telemetry.num_spans() == NUM_ADDS
 ```
 
 ### otelsink
 
 `otelsink` is a gRPC server that listens for OTel metrics, traces, and logs.
```

### Comparing `oteltest-0.7.1/pyproject.toml` & `oteltest-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oteltest-0.7.1/PKG-INFO` & `oteltest-0.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: oteltest
-Version: 0.7.1
+Version: 0.8.0
 Summary: OpenTelemetry Tester
 Project-URL: Documentation, https://github.com/open-telemetry/opentelemetry-python#readme
 Project-URL: Issues, https://github.com/open-telemetry/opentelemetry-python/issues
 Project-URL: Source, https://github.com/open-telemetry/opentelemetry-python/
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
@@ -41,30 +41,20 @@
 
 ```console
 pip install oteltest
 ```
 
 ## Overview
 
-The `oteltest` package contains utilities for testing OpenTelemetry Python. The motivation for oteltest is to provide
-an easy way to test OpenTelemetry Python, which involves a Python environment with specific packages
+The `oteltest` package contains utilities for testing OpenTelemetry Python.
 
 ### oteltest
 
 The `oteltest` command runs black box tests against Python scripts that send telemetry.
 
-
-#### Motivation
-
-The motivation for oteltest is to make it as easy as possible to run code that emits telemetry, with all of the
-information required to run a test co-located with the code being tested. With that in place, you should be able to
-point something at it that sets up the environment, runs the script, records the telemetry that the script sends, and
-sends that telemetry back to the script so that the validate can be co-located with the test configuration, and the test
-code.
-
 #### Execution
 
 Run `oteltest` as a shell command and provide a directory as an argument:
 
 ```shell
 oteltest my_script_dir
 ```
@@ -73,57 +63,60 @@
 
 #### Operation
 
 Running `oteltest` against a directory containing `my_script.py`
 
 1) Starts an [otelsink](#otelsink) instance
 2) Creates a new Python virtual environment with `requirements()`
-3) Using that new environment, starts running `my_script.py` in a subprocess
+3) In that environment, starts running `my_script.py` in a subprocess
 4) Meanwhile, calls `OtelTest#on_script_start()` waiting until completion
 5) Depending on the return value from `on_script_start()`, waits for `my_script.py` to complete or interrupts
 6) Stops the OTLP listener
 7) Calls `validate(telemetry)` with otelsink's received telemetry
-8) Writes the telemetry to a `.json` file next to the script (script name but `.json`)
+8) Writes the telemetry to a `.json` file next to the script (script name but with ".{number}.json" instead of ".py")
 
 #### Script Eligibility
 
 For a Python script to be runnable by `oteltest`, it must both be executable and define an implementation of the
-[OtelTest]() abstract base class. The script below has an implementation called `MyTest`:
+[OtelTest]() abstract base class. The script below has an implementation called `MyOtelTest`:
 
 ```python
 import time
 
 from opentelemetry import trace
 from oteltest import OtelTest, Telemetry
 
-SERVICE_NAME = "integration-test"
+SERVICE_NAME = "my-otel-test"
 NUM_ADDS = 12
 
 if __name__ == "__main__":
     tracer = trace.get_tracer("my-tracer")
     for i in range(NUM_ADDS):
         with tracer.start_as_current_span("my-span"):
-            print(f"simple_loop.py: {i + 1}/{NUM_ADDS}")
+            print(f"simple_loop.py: {i+1}/{NUM_ADDS}")
             time.sleep(0.5)
 
 
-class MyTest(OtelTest):
+class MyOtelTest(OtelTest):
     def requirements(self):
         return "opentelemetry-distro", "opentelemetry-exporter-otlp-proto-grpc"
 
     def environment_variables(self):
         return {"OTEL_SERVICE_NAME": SERVICE_NAME}
 
     def wrapper_script(self):
         return "opentelemetry-instrument"
 
     def on_script_start(self):
         return None
 
-    def validate(self, telemetry: Telemetry):
+    def on_script_end(self, stdout, stderr, returncode) -> None:
+        pass
+
+    def on_shutdown(self, telemetry: Telemetry):
         assert telemetry.num_spans() == NUM_ADDS
 ```
 
 ### otelsink
 
 `otelsink` is a gRPC server that listens for OTel metrics, traces, and logs.
```

