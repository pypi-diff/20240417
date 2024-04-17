# Comparing `tmp/fmeval-1.0.0-py3-none-any.whl.zip` & `tmp/fmeval-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 129699 bytes, number of entries: 65
+Zip file size: 131058 bytes, number of entries: 65
 -rw-r--r--  2.0 unx       41 b- defN 80-Jan-01 00:00 fmeval/COMMIT_HASH
 -rw-r--r--  2.0 unx     4864 b- defN 80-Jan-01 00:00 fmeval/constants.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fmeval/data_loaders/__init__.py
 -rw-r--r--  2.0 unx     2685 b- defN 80-Jan-01 00:00 fmeval/data_loaders/data_config.py
--rw-r--r--  2.0 unx     2812 b- defN 80-Jan-01 00:00 fmeval/data_loaders/data_sources.py
+-rw-r--r--  2.0 unx     3400 b- defN 80-Jan-01 00:00 fmeval/data_loaders/data_sources.py
 -rw-r--r--  2.0 unx     1907 b- defN 80-Jan-01 00:00 fmeval/data_loaders/jmespath_util.py
 -rw-r--r--  2.0 unx     4292 b- defN 80-Jan-01 00:00 fmeval/data_loaders/json_data_loader.py
 -rw-r--r--  2.0 unx    12342 b- defN 80-Jan-01 00:00 fmeval/data_loaders/json_parser.py
--rw-r--r--  2.0 unx     8214 b- defN 80-Jan-01 00:00 fmeval/data_loaders/util.py
+-rw-r--r--  2.0 unx     8073 b- defN 80-Jan-01 00:00 fmeval/data_loaders/util.py
 -rw-r--r--  2.0 unx     1424 b- defN 80-Jan-01 00:00 fmeval/eval.py
 -rw-r--r--  2.0 unx     2085 b- defN 80-Jan-01 00:00 fmeval/eval_algo_mapping.py
 -rw-r--r--  2.0 unx    13115 b- defN 80-Jan-01 00:00 fmeval/eval_algorithms/__init__.py
 -rw-r--r--  2.0 unx    17889 b- defN 80-Jan-01 00:00 fmeval/eval_algorithms/classification_accuracy.py
 -rw-r--r--  2.0 unx    11684 b- defN 80-Jan-01 00:00 fmeval/eval_algorithms/classification_accuracy_semantic_robustness.py
 -rw-r--r--  2.0 unx     3358 b- defN 80-Jan-01 00:00 fmeval/eval_algorithms/eval_algorithm.py
 -rw-r--r--  2.0 unx     9356 b- defN 80-Jan-01 00:00 fmeval/eval_algorithms/factual_knowledge.py
@@ -54,14 +54,14 @@
 -rw-r--r--  2.0 unx     1404 b- defN 80-Jan-01 00:00 fmeval/transforms/batched_transform.py
 -rw-r--r--  2.0 unx     7049 b- defN 80-Jan-01 00:00 fmeval/transforms/common.py
 -rw-r--r--  2.0 unx    12300 b- defN 80-Jan-01 00:00 fmeval/transforms/semantic_perturbations.py
 -rw-r--r--  2.0 unx     6241 b- defN 80-Jan-01 00:00 fmeval/transforms/semantic_robustness_metrics.py
 -rw-r--r--  2.0 unx    11718 b- defN 80-Jan-01 00:00 fmeval/transforms/summarization_accuracy_metrics.py
 -rw-r--r--  2.0 unx     4437 b- defN 80-Jan-01 00:00 fmeval/transforms/transform.py
 -rw-r--r--  2.0 unx     4572 b- defN 80-Jan-01 00:00 fmeval/transforms/transform_pipeline.py
--rw-r--r--  2.0 unx     6248 b- defN 80-Jan-01 00:00 fmeval/transforms/util.py
+-rw-r--r--  2.0 unx     4684 b- defN 80-Jan-01 00:00 fmeval/transforms/util.py
 -rw-r--r--  2.0 unx     4526 b- defN 80-Jan-01 00:00 fmeval/util.py
--rw-r--r--  2.0 unx    10142 b- defN 80-Jan-01 00:00 fmeval-1.0.0.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 fmeval-1.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     7471 b- defN 16-Jan-01 00:00 fmeval-1.0.0.dist-info/METADATA
-?rw-r--r--  2.0 unx     6097 b- defN 16-Jan-01 00:00 fmeval-1.0.0.dist-info/RECORD
-65 files, 413190 bytes uncompressed, 119835 bytes compressed:  71.0%
+-rw-r--r--  2.0 unx    10142 b- defN 80-Jan-01 00:00 fmeval-1.0.1.dist-info/LICENSE
+?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 fmeval-1.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    12438 b- defN 16-Jan-01 00:00 fmeval-1.0.1.dist-info/METADATA
+?rw-r--r--  2.0 unx     6098 b- defN 16-Jan-01 00:00 fmeval-1.0.1.dist-info/RECORD
+65 files, 417041 bytes uncompressed, 121194 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -177,20 +177,20 @@
 
 Filename: fmeval/transforms/util.py
 Comment: 
 
 Filename: fmeval/util.py
 Comment: 
 
-Filename: fmeval-1.0.0.dist-info/LICENSE
+Filename: fmeval-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: fmeval-1.0.0.dist-info/WHEEL
+Filename: fmeval-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: fmeval-1.0.0.dist-info/METADATA
+Filename: fmeval-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: fmeval-1.0.0.dist-info/RECORD
+Filename: fmeval-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fmeval/COMMIT_HASH

```diff
@@ -1 +1 @@
-e893f7005c993058c0f35e26709e6e3fa7f5957b
+91e675be24800a262faf8bf6e59f07522b5314ea
```

## fmeval/data_loaders/data_sources.py

```diff
@@ -1,13 +1,14 @@
 import boto3
 import botocore.response
 import botocore.errorfactory
 import urllib.parse
 from typing import IO
 from abc import ABC, abstractmethod
+from fmeval.constants import BUILT_IN_DATASET_PREFIX, BUILT_IN_DATASET_DEFAULT_REGION
 from fmeval.exceptions import EvalAlgorithmClientError
 
 
 class DataSource(ABC):
     """
     Managed data resource
     """
@@ -81,15 +82,15 @@
     """
     DataFile class for s3 files
     """
 
     def __init__(self, file_path: str):
         # We cannot inject the client b/c
         # it is not serializable by Ray.
-        self._client = boto3.client("s3")
+        self._client = get_s3_client(file_path)
         super().__init__(file_path)
 
     def open(self, mode="r") -> botocore.response.StreamingBody:  # type: ignore
         try:
             s3_uri = S3Uri(self.uri)
             return self._client.get_object(Bucket=s3_uri.bucket, Key=s3_uri.key)["Body"]
         except botocore.errorfactory.ClientError as e:
@@ -101,7 +102,22 @@
         """
         Custom serializer method used by Ray when it serializes
         JsonDataLoaderConfig objects during data loading
         (see the load_dataset method in src.fmeval.data_loaders.json_data_loader.py).
         """
         serialized_data = (self.uri,)
         return S3DataFile, serialized_data
+
+
+def get_s3_client(uri: str) -> boto3.client:
+    """
+    Util method to return boto3 s3 client. For built-in datasets, the boto3 client region is default to us-west-2 as
+        the bucket is not accessible in opt-in regions.
+    :param uri: s3 dataset uri
+    :return: boto3 s3 client
+    """
+    s3_client = (
+        boto3.client("s3", region_name=BUILT_IN_DATASET_DEFAULT_REGION)
+        if uri.startswith(BUILT_IN_DATASET_PREFIX)
+        else boto3.client("s3")
+    )
+    return s3_client
```

## fmeval/data_loaders/util.py

```diff
@@ -9,18 +9,16 @@
 from fmeval import util
 from fmeval.constants import (
     MIME_TYPE_JSON,
     MIME_TYPE_JSONLINES,
     PARTITION_MULTIPLIER,
     SEED,
     MAX_ROWS_TO_TAKE,
-    BUILT_IN_DATASET_PREFIX,
-    BUILT_IN_DATASET_DEFAULT_REGION,
 )
-from fmeval.data_loaders.data_sources import DataSource, LocalDataFile, S3DataFile, DataFile, S3Uri
+from fmeval.data_loaders.data_sources import DataSource, LocalDataFile, S3DataFile, DataFile, S3Uri, get_s3_client
 from fmeval.data_loaders.json_data_loader import JsonDataLoaderConfig, JsonDataLoader
 from fmeval.data_loaders.json_parser import JsonParser
 from fmeval.data_loaders.data_config import DataConfig
 from fmeval.util import get_num_actors
 from fmeval.exceptions import EvalAlgorithmClientError, EvalAlgorithmInternalError
 from fmeval.perf_util import timed_block
 
@@ -151,19 +149,15 @@
 
 
 def _get_s3_data_source(dataset_uri) -> S3DataFile:
     """
     :param dataset_uri: s3 dataset uri
     :return: S3DataFile object with dataset uri
     """
-    s3_client = (
-        boto3.client("s3", region_name=BUILT_IN_DATASET_DEFAULT_REGION)
-        if dataset_uri.startswith(BUILT_IN_DATASET_PREFIX)
-        else client
-    )
+    s3_client = get_s3_client(dataset_uri)
     s3_uri = S3Uri(dataset_uri)
     s3_obj = s3_client.get_object(Bucket=s3_uri.bucket, Key=s3_uri.key)
     if "application/x-directory" in s3_obj["ContentType"]:
         # TODO: extend support to directories
         raise EvalAlgorithmClientError("Please provide a s3 file path instead of a directory path.")
     else:
         # There isn't a good way to check if s3_obj corresponds specifically to a file,
@@ -176,16 +170,17 @@
     :param uri: s3 file path
     :return: True if uri is a valid s3 path, False otherwise
     """
     parsed_url = urllib.parse.urlparse(uri)
     if parsed_url.scheme.lower() not in ["s3", "s3n", "s3a"]:
         return False
     try:
+        s3_client = get_s3_client(uri)
         s3_uri = S3Uri(uri)
-        client.get_object(Bucket=s3_uri.bucket, Key=s3_uri.key)
+        s3_client.get_object(Bucket=s3_uri.bucket, Key=s3_uri.key)
         return True
     except botocore.errorfactory.ClientError:
         return False
 
 
 def _is_valid_local_path(path: str) -> bool:
     """
```

## fmeval/transforms/util.py

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Set, Callable, Tuple
+from typing import Any, Callable, Dict, List, Tuple
 from fmeval.util import assert_condition
 
 
 def validate_key_uniqueness(keys: List[str]) -> None:
     """Validate that a list of keys contains unique values.
 
     This function exists to capture the full list of duplicate keys
@@ -34,38 +34,14 @@
             missing_keys.append(key)
     assert_condition(
         len(missing_keys) == 0,
         f"Record {record} is expected to contain the following keys, " f"but they are missing: {missing_keys}.",
     )
 
 
-def validate_added_keys(current_keys: Set[str], original_keys: Set[str], keys_to_add: Set[str]) -> None:
-    """Validate that the set difference between `current_keys` and `original_keys` is `keys_to_add`.
-
-    Note: this function should only be used when by Transforms that mutate their input record.
-    It doesn't make sense to call this function if the Transform constructs a new record to
-    be used as output, since said output record need not contain all the keys in the input record.
-
-    :param current_keys: The keys that are currently present in a record.
-    :param original_keys: The keys that were originally present in a record
-        (prior to performing transform-specific logic, which adds new keys).
-    :param keys_to_add: The keys that a transform should have added to its input record.
-        When this function is called from within a Transform's __call__ method (which should
-        be the primary use case for this function), this parameter should be the transform's
-        `output_keys` attribute.
-    :raises: EvalAlgorithmInternalError if any validation fails.
-    """
-    assert_condition(
-        current_keys - original_keys == keys_to_add,
-        f"The set difference between the current keys: {current_keys} "
-        f"and the original keys: {original_keys} does not match "
-        f"the expected keys to be added: {keys_to_add}.",
-    )
-
-
 def validate_call(call_method: Callable) -> Callable:
     """Decorator for the __call__ method of Transforms used for validating input and output.
 
     This decorator validates that all keys in a Transform's `input_keys` attribute are
     present in the input record that is passed to `__call__` and that the keys that
     are added to the record by the Transform's internal `__call__` logic are limited
     to the keys specified by the Transform's `output_keys` attribute.
@@ -90,20 +66,16 @@
         )
         assert_condition(
             self.output_keys is not None,
             "self.output_keys has not been set. You should set this attribute using "
             "the register_input_output_keys method.",
         )
         validate_existing_keys(record, self.input_keys)
-        original_keys = set(record.keys())
         call_output = call_method(self, record)
-        validate_key_uniqueness(self.output_keys)
-        validate_added_keys(
-            current_keys=set(record.keys()), original_keys=original_keys, keys_to_add=set(self.output_keys)
-        )
+        validate_existing_keys(call_output, self.output_keys)
         return call_output
 
     return wrapper
 
 
 def create_output_key(transform_name: str, *args, **kwargs) -> str:
     """Create an output key to be used by a Transform instance.
```

## Comparing `fmeval-1.0.0.dist-info/LICENSE` & `fmeval-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fmeval-1.0.0.dist-info/RECORD` & `fmeval-1.0.1.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-fmeval/COMMIT_HASH,sha256=EbZazoqsU_AouYTQ6fdtGUQxcpls8KCtPh55xmV7mis,41
+fmeval/COMMIT_HASH,sha256=DzsbgicgvtB-ppdM0fNgEg-Mn4F7HJlOFvAAMiXFDL8,41
 fmeval/constants.py,sha256=gNwBJQGCISMDIUMu5H-Cy9nH0nkIQ6fMwoWHulx4cTI,4864
 fmeval/data_loaders/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fmeval/data_loaders/data_config.py,sha256=jZyFS6DmZ8QEgAMiIdnhHumGpIRj7WT3YPmiUpUu7O0,2685
-fmeval/data_loaders/data_sources.py,sha256=pzhecP3GqDOvleC64P7yIcefQ9H2g9DSl4WePaWBU1s,2812
+fmeval/data_loaders/data_sources.py,sha256=Vm6LSCrE_BG144KQKXYV23xjMyydClxBv3PyW4Ux9Ck,3400
 fmeval/data_loaders/jmespath_util.py,sha256=eYLHQnJY4woIJjm2UH1STnkIvQHfe7gl7sPlVROudOc,1907
 fmeval/data_loaders/json_data_loader.py,sha256=uPzYBJJAaCPuibKnitXCAmef5-yBNHFEqy9i6g0dVTo,4292
 fmeval/data_loaders/json_parser.py,sha256=x-ZHGXu_HToLVLEjAt1uYYdt6c5n3XOaKIGjImPGU1w,12342
-fmeval/data_loaders/util.py,sha256=dzgTQQKpMLWY197ICORMDnBwavj7OnwLmE5iCDOKxS4,8214
+fmeval/data_loaders/util.py,sha256=y_XW6D-ICjGuNqFdAHr_OBMpRjzOR0b15glQqgOgbY0,8073
 fmeval/eval.py,sha256=tfDa4njg7gUqneStKF8QK9fXxmDM41eHRC1k4YFO0EM,1424
 fmeval/eval_algo_mapping.py,sha256=UG9LCEw3LnPwnJyf4WmO4UuAIAA8cwUGVYqWK5IWzDE,2085
 fmeval/eval_algorithms/__init__.py,sha256=SdErgrIAe56QwaqqBhRg825j5O7RhCZrClwnwaY2FAI,13115
 fmeval/eval_algorithms/classification_accuracy.py,sha256=WiLCPTLOsI49jTy6RJvK32d27VoNStIFKI4qHlFhgKQ,17889
 fmeval/eval_algorithms/classification_accuracy_semantic_robustness.py,sha256=oc_6lVYLJqmJ3R2FD9bzipR3opdhKLif25K6QVq9XRg,11684
 fmeval/eval_algorithms/eval_algorithm.py,sha256=oLiJiKLcjIBTgVLge-Ztjg6l0gBqr3Dy_FBL_KrjRZ0,3358
 fmeval/eval_algorithms/factual_knowledge.py,sha256=QPNXIOfDlmkRt5fEjWLi7HGwyuH56wfdWUeQS2R2ylg,9356
@@ -53,13 +53,13 @@
 fmeval/transforms/batched_transform.py,sha256=ZgGGstVZ2p8EDq65rye6QBuLwVFOXu7oTvE-G28zcG0,1404
 fmeval/transforms/common.py,sha256=6njUK3s0eiAsLed-jHHbtEQPxCp7DJVN8nOKb0yJpHY,7049
 fmeval/transforms/semantic_perturbations.py,sha256=etmFWOlOYJWu4sINy268GUI8YV3S7Ispj4z5hM30ClM,12300
 fmeval/transforms/semantic_robustness_metrics.py,sha256=lEv6vHVzDvUOqHTDIeS6RfFaoYXcSkXKqvYwwKzrcOU,6241
 fmeval/transforms/summarization_accuracy_metrics.py,sha256=KUAYevzgSLTjbVwddtogavfT1tPPAcEAVqsxkAag8Ag,11718
 fmeval/transforms/transform.py,sha256=brePXgZJTVRzldiCpD96ayEuVb5tOHXbauYzz6fDyWY,4437
 fmeval/transforms/transform_pipeline.py,sha256=UUZtxSrmqMqEH6su28TDz-8GCmgG0IaQ2E5iOIfcDdE,4572
-fmeval/transforms/util.py,sha256=WKbdVaE8HvDYUthBfZcln2vDCr3kstwKixOEAY5V4t4,6248
+fmeval/transforms/util.py,sha256=9aQPqL7LEYCh5co-0QCrSxsePwRo9j3Co-S5frwtTIE,4684
 fmeval/util.py,sha256=GHQQepz7qX0v3cFyw3ihPNaKDLf3U-G_mmD23XJHEC4,4526
-fmeval-1.0.0.dist-info/LICENSE,sha256=CeipvOyAZxBGUsFoaFqwkx54aPnIKEtm9a5u2uXxEws,10142
-fmeval-1.0.0.dist-info/WHEEL,sha256=bbU3AyvhQ312rVm7zzRQjs6axI1UYWC3nmFA2E6FFSI,88
-fmeval-1.0.0.dist-info/METADATA,sha256=Y5iph90xJpdxh9BGghgRHSE33bY1CtQGBKm89NIW0z4,7471
-fmeval-1.0.0.dist-info/RECORD,,
+fmeval-1.0.1.dist-info/LICENSE,sha256=CeipvOyAZxBGUsFoaFqwkx54aPnIKEtm9a5u2uXxEws,10142
+fmeval-1.0.1.dist-info/WHEEL,sha256=bbU3AyvhQ312rVm7zzRQjs6axI1UYWC3nmFA2E6FFSI,88
+fmeval-1.0.1.dist-info/METADATA,sha256=AI2I5sEXdO2uau0iRFc529tyfsfO9JKKYXEhqnhucq0,12438
+fmeval-1.0.1.dist-info/RECORD,,
```

