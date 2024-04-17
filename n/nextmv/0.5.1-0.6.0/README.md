# Comparing `tmp/nextmv-0.5.1.tar.gz` & `tmp/nextmv-0.6.0.tar.gz`

## Comparing `nextmv-0.5.1.tar` & `nextmv-0.6.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv-py.code-workspace
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextmv-0.5.1/requirements.txt
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 nextmv-0.5.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 nextmv-0.5.1/.github/workflows/python-lint.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 nextmv-0.5.1/.github/workflows/python-test.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/__about__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/base_model.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/cloud/__init__.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/cloud/acceptance_test.py
--rw-r--r--   0        0        0    25508 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/cloud/application.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/cloud/batch_experiment.py
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/cloud/client.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/cloud/input_set.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/__init__.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/check/__init__.py
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/check/schema.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/schema/__init__.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/schema/input.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/schema/location.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/schema/output.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/schema/stop.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/schema/vehicle.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/test_base_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/cloud/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/cloud/test_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/nextroute/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/nextroute/schema/__init__.py
--rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/nextroute/schema/input.json
--rw-r--r--   0        0        0    25755 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/nextroute/schema/output.json
--rw-r--r--   0        0        0    28915 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/nextroute/schema/output_with_check.json
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/nextroute/schema/test_input.py
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/nextroute/schema/test_output.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 nextmv-0.5.1/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 nextmv-0.5.1/LICENSE
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nextmv-0.5.1/README.md
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 nextmv-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 nextmv-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv-py.code-workspace
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextmv-0.6.0/requirements.txt
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 nextmv-0.6.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 nextmv-0.6.0/.github/workflows/python-lint.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 nextmv-0.6.0/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/__about__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/base_model.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/cloud/__init__.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/cloud/acceptance_test.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/cloud/account.py
+-rw-r--r--   0        0        0    26087 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/cloud/application.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/cloud/batch_experiment.py
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/cloud/client.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/cloud/input_set.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/cloud/status.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/nextroute/__init__.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/nextroute/check/__init__.py
+-rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/nextroute/check/schema.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/nextroute/schema/__init__.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/nextroute/schema/input.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/nextroute/schema/location.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/nextroute/schema/output.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/nextroute/schema/stop.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 nextmv-0.6.0/nextmv/nextroute/schema/vehicle.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 nextmv-0.6.0/tests/test_base_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.6.0/tests/cloud/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 nextmv-0.6.0/tests/cloud/test_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.6.0/tests/nextroute/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.6.0/tests/nextroute/schema/__init__.py
+-rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 nextmv-0.6.0/tests/nextroute/schema/input.json
+-rw-r--r--   0        0        0    25755 2020-02-02 00:00:00.000000 nextmv-0.6.0/tests/nextroute/schema/output.json
+-rw-r--r--   0        0        0    28915 2020-02-02 00:00:00.000000 nextmv-0.6.0/tests/nextroute/schema/output_with_check.json
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 nextmv-0.6.0/tests/nextroute/schema/test_input.py
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 nextmv-0.6.0/tests/nextroute/schema/test_output.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 nextmv-0.6.0/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 nextmv-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nextmv-0.6.0/README.md
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 nextmv-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 nextmv-0.6.0/PKG-INFO
```

### Comparing `nextmv-0.5.1/.github/workflows/publish.yml` & `nextmv-0.6.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/.github/workflows/python-lint.yml` & `nextmv-0.6.0/.github/workflows/python-lint.yml`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/.github/workflows/python-test.yml` & `nextmv-0.6.0/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/nextmv/cloud/__init__.py` & `nextmv-0.6.0/nextmv/cloud/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 from .acceptance_test import AcceptanceTest as AcceptanceTest
 from .acceptance_test import Comparison as Comparison
 from .acceptance_test import ComparisonInstance as ComparisonInstance
 from .acceptance_test import Metric as Metric
 from .acceptance_test import MetricParams as MetricParams
 from .acceptance_test import MetricType as MetricType
+from .account import Account as Account
+from .account import Queue as Queue
+from .account import QueuedRun as QueuedRun
 from .application import Application as Application
 from .application import Configuration as Configuration
 from .application import DownloadURL as DownloadURL
 from .application import ErrorLog as ErrorLog
 from .application import Metadata as Metadata
 from .application import PollingOptions as PollingOptions
 from .application import RunInformation as RunInformation
@@ -17,7 +20,9 @@
 from .application import UploadURL as UploadURL
 from .batch_experiment import BatchExperiment as BatchExperiment
 from .batch_experiment import BatchExperimentInformation as BatchExperimentInformation
 from .batch_experiment import BatchExperimentMetadata as BatchExperimentMetadata
 from .batch_experiment import BatchExperimentRun as BatchExperimentRun
 from .client import Client as Client
 from .input_set import InputSet as InputSet
+from .status import Status as Status
+from .status import StatusV2 as StatusV2
```

### Comparing `nextmv-0.5.1/nextmv/cloud/acceptance_test.py` & `nextmv-0.6.0/nextmv/cloud/acceptance_test.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/nextmv/cloud/application.py` & `nextmv-0.6.0/nextmv/cloud/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import requests
 
 from nextmv.base_model import BaseModel
 from nextmv.cloud.acceptance_test import AcceptanceTest, Metric
 from nextmv.cloud.batch_experiment import BatchExperiment, BatchExperimentMetadata, BatchExperimentRun
 from nextmv.cloud.client import Client, get_size
 from nextmv.cloud.input_set import InputSet
+from nextmv.cloud.status import Status, StatusV2
 
 _MAX_RUN_SIZE: int = 5 * 1024 * 1024
 """Maximum size of the run input/output. This value is used to determine
 whether to use the large input upload and/or result download endpoints."""
 
 
 class DownloadURL(BaseModel):
@@ -51,15 +52,17 @@
     """Duration of the run in milliseconds."""
     error: str
     """Error message if the run failed."""
     input_size: float
     """Size of the input in bytes."""
     output_size: float
     """Size of the output in bytes."""
-    status: str
+    status: Status
+    """Deprecated: use status_v2."""
+    status_v2: StatusV2
     """Status of the run."""
 
 
 class PollingOptions(BaseModel):
     """Options to use when polling for a run result."""
 
     backoff: float = 1
@@ -184,14 +187,30 @@
         response = self.client.request(
             method="GET",
             endpoint=f"{self.experiments_endpoint}/batch/{batch_id}",
         )
 
         return BatchExperiment.from_dict(response.json())
 
+    def cancel_run(self, run_id: str) -> None:
+        """
+        Cancel a run.
+
+        Args:
+            run_id: ID of the run.
+
+        Raises:
+            requests.HTTPError: If the response status code is not 2xx.
+        """
+
+        _ = self.client.request(
+            method="PATCH",
+            endpoint=f"{self.endpoint}/runs/{run_id}/cancel",
+        )
+
     def input_set(self, input_set_id: str) -> InputSet:
         """
         Get an input set.
 
         Args:
             input_set_id: ID of the input set.
 
@@ -688,15 +707,19 @@
         """
 
         time.sleep(polling_options.initial_delay)
         delay = polling_options.delay
         polling_ok = False
         for _ in range(polling_options.max_tries):
             run_information = self.run_metadata(run_id=run_id)
-            if run_information.metadata.status in ["succeeded", "failed"]:
+            if run_information.metadata.status_v2 in [
+                StatusV2.succeeded,
+                StatusV2.failed,
+                StatusV2.canceled,
+            ]:
                 polling_ok = True
                 break
 
             if delay > polling_options.max_duration:
                 raise TimeoutError(
                     f"run {run_id} did not succeed after {delay} seconds",
                 )
```

### Comparing `nextmv-0.5.1/nextmv/cloud/batch_experiment.py` & `nextmv-0.6.0/nextmv/cloud/batch_experiment.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/nextmv/cloud/client.py` & `nextmv-0.6.0/nextmv/cloud/client.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/nextmv/cloud/input_set.py` & `nextmv-0.6.0/nextmv/cloud/input_set.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/nextmv/nextroute/check/__init__.py` & `nextmv-0.6.0/nextmv/nextroute/check/__init__.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/nextmv/nextroute/check/schema.py` & `nextmv-0.6.0/nextmv/nextroute/check/schema.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/nextmv/nextroute/schema/__init__.py` & `nextmv-0.6.0/nextmv/nextroute/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/nextmv/nextroute/schema/input.py` & `nextmv-0.6.0/nextmv/nextroute/schema/input.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/nextmv/nextroute/schema/output.py` & `nextmv-0.6.0/nextmv/nextroute/schema/output.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/nextmv/nextroute/schema/stop.py` & `nextmv-0.6.0/nextmv/nextroute/schema/stop.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/nextmv/nextroute/schema/vehicle.py` & `nextmv-0.6.0/nextmv/nextroute/schema/vehicle.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/tests/test_base_model.py` & `nextmv-0.6.0/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/tests/cloud/test_client.py` & `nextmv-0.6.0/tests/cloud/test_client.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/tests/nextroute/schema/input.json` & `nextmv-0.6.0/tests/nextroute/schema/input.json`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/tests/nextroute/schema/output.json` & `nextmv-0.6.0/tests/nextroute/schema/output.json`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/tests/nextroute/schema/output_with_check.json` & `nextmv-0.6.0/tests/nextroute/schema/output_with_check.json`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/tests/nextroute/schema/test_input.py` & `nextmv-0.6.0/tests/nextroute/schema/test_input.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/tests/nextroute/schema/test_output.py` & `nextmv-0.6.0/tests/nextroute/schema/test_output.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/.gitignore` & `nextmv-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/LICENSE` & `nextmv-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/README.md` & `nextmv-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/pyproject.toml` & `nextmv-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.1/PKG-INFO` & `nextmv-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nextmv
-Version: 0.5.1
+Version: 0.6.0
 Summary: The Python SDK for Nextmv
 Project-URL: Homepage, https://www.nextmv.io
 Project-URL: Documentation, https://www.nextmv.io/docs
 Project-URL: Repository, https://github.com/nextmv-io/nextmv-py
 Author-email: Nextmv <tech@nextmv.io>
 Maintainer-email: Nextmv <tech@nextmv.io>
 License:                                  Apache License
```

