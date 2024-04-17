# Comparing `tmp/aws_comprehend-0.1.1.tar.gz` & `tmp/aws_comprehend-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_comprehend-0.1.1.tar", last modified: Thu Feb 23 20:50:12 2023, max compression
+gzip compressed data, was "aws_comprehend-0.1.2.tar", last modified: Wed Apr 17 03:50:59 2024, max compression
```

## Comparing `aws_comprehend-0.1.1.tar` & `aws_comprehend-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,43 @@
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-23 20:50:12.048848 aws_comprehend-0.1.1/
--rw-r--r--   0 sanhehu    (505) staff       (20)      509 2023-02-23 03:16:18.000000 aws_comprehend-0.1.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     1124 2023-02-23 03:16:18.000000 aws_comprehend-0.1.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      322 2023-02-23 03:16:18.000000 aws_comprehend-0.1.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (505) staff       (20)     3697 2023-02-23 20:50:12.048703 aws_comprehend-0.1.1/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     2578 2023-02-23 20:47:34.000000 aws_comprehend-0.1.1/README.rst
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-23 20:50:12.045700 aws_comprehend-0.1.1/aws_comprehend/
--rw-r--r--   0 sanhehu    (505) staff       (20)      410 2023-02-23 20:44:58.000000 aws_comprehend-0.1.1/aws_comprehend/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)       93 2023-02-23 20:46:35.000000 aws_comprehend-0.1.1/aws_comprehend/_version.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-23 20:50:12.047069 aws_comprehend-0.1.1/aws_comprehend/better_boto/
--rw-r--r--   0 sanhehu    (505) staff       (20)      495 2023-02-23 20:46:21.000000 aws_comprehend-0.1.1/aws_comprehend/better_boto/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    13733 2023-02-23 20:46:12.000000 aws_comprehend-0.1.1/aws_comprehend/better_boto/document_classifier.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    10891 2023-02-23 20:43:58.000000 aws_comprehend-0.1.1/aws_comprehend/better_boto/endpoint.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      336 2023-02-23 18:10:21.000000 aws_comprehend-0.1.1/aws_comprehend/compat.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1660 2023-02-23 16:26:56.000000 aws_comprehend-0.1.1/aws_comprehend/comprehend_csv.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-23 20:50:12.047229 aws_comprehend-0.1.1/aws_comprehend/docs/
--rw-r--r--   0 sanhehu    (505) staff       (20)       43 2023-02-23 03:16:18.000000 aws_comprehend-0.1.1/aws_comprehend/docs/__init__.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-23 20:50:12.048333 aws_comprehend-0.1.1/aws_comprehend/tests/
--rw-r--r--   0 sanhehu    (505) staff       (20)       84 2023-02-23 16:31:59.000000 aws_comprehend-0.1.1/aws_comprehend/tests/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      140 2023-02-23 16:31:36.000000 aws_comprehend-0.1.1/aws_comprehend/tests/boto_ses.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1215 2022-12-07 01:32:56.000000 aws_comprehend-0.1.1/aws_comprehend/tests/helper.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      370 2022-12-07 01:32:30.000000 aws_comprehend-0.1.1/aws_comprehend/tests/paths.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1334 2023-02-23 19:02:59.000000 aws_comprehend-0.1.1/aws_comprehend/waiter.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-23 20:50:12.046623 aws_comprehend-0.1.1/aws_comprehend.egg-info/
--rw-r--r--   0 sanhehu    (505) staff       (20)     3697 2023-02-23 20:50:12.000000 aws_comprehend-0.1.1/aws_comprehend.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)      769 2023-02-23 20:50:12.000000 aws_comprehend-0.1.1/aws_comprehend.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-02-23 20:50:12.000000 aws_comprehend-0.1.1/aws_comprehend.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      342 2023-02-23 20:50:12.000000 aws_comprehend-0.1.1/aws_comprehend.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       15 2023-02-23 20:50:12.000000 aws_comprehend-0.1.1/aws_comprehend.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)     1415 2023-02-23 20:49:09.000000 aws_comprehend-0.1.1/release-history.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      284 2023-02-23 16:32:49.000000 aws_comprehend-0.1.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      621 2023-02-23 03:16:18.000000 aws_comprehend-0.1.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      200 2023-02-23 16:32:58.000000 aws_comprehend-0.1.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      149 2023-02-23 20:11:21.000000 aws_comprehend-0.1.1/requirements.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-02-23 20:50:12.048899 aws_comprehend-0.1.1/setup.cfg
--rw-r--r--   0 sanhehu    (505) staff       (20)     7709 2023-02-23 03:16:18.000000 aws_comprehend-0.1.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-17 03:50:59.638457 aws_comprehend-0.1.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2024-04-16 16:52:18.000000 aws_comprehend-0.1.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2024-04-16 16:52:18.000000 aws_comprehend-0.1.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      354 2024-04-17 03:49:24.000000 aws_comprehend-0.1.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4652 2024-04-17 03:50:59.638255 aws_comprehend-0.1.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2619 2024-04-17 03:50:37.000000 aws_comprehend-0.1.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-17 03:50:59.634256 aws_comprehend-0.1.2/aws_comprehend/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      275 2024-04-16 18:21:11.000000 aws_comprehend-0.1.2/aws_comprehend/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2024-04-17 03:34:26.000000 aws_comprehend-0.1.2/aws_comprehend/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      207 2024-04-16 19:36:17.000000 aws_comprehend-0.1.2/aws_comprehend/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-17 03:50:59.635733 aws_comprehend-0.1.2/aws_comprehend/better_boto/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2024-04-16 18:21:37.000000 aws_comprehend-0.1.2/aws_comprehend/better_boto/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      730 2024-04-16 19:15:59.000000 aws_comprehend-0.1.2/aws_comprehend/better_boto/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    15488 2024-04-16 21:20:07.000000 aws_comprehend-0.1.2/aws_comprehend/better_boto/document_classifier.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12655 2024-04-16 21:19:46.000000 aws_comprehend-0.1.2/aws_comprehend/better_boto/endpoint.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      336 2024-04-16 16:52:18.000000 aws_comprehend-0.1.2/aws_comprehend/compat.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1660 2024-04-16 16:52:18.000000 aws_comprehend-0.1.2/aws_comprehend/comprehend_csv.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-17 03:50:59.635916 aws_comprehend-0.1.2/aws_comprehend/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2024-04-16 16:52:18.000000 aws_comprehend-0.1.2/aws_comprehend/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       64 2024-04-16 18:23:05.000000 aws_comprehend-0.1.2/aws_comprehend/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2024-04-16 18:15:03.000000 aws_comprehend-0.1.2/aws_comprehend/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-17 03:50:59.636396 aws_comprehend-0.1.2/aws_comprehend/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2024-04-16 18:15:03.000000 aws_comprehend-0.1.2/aws_comprehend/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4064 2024-04-16 18:20:05.000000 aws_comprehend-0.1.2/aws_comprehend/vendor/pytest_cov_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2354 2024-04-16 18:19:34.000000 aws_comprehend-0.1.2/aws_comprehend/vendor/waiter.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-17 03:50:59.637210 aws_comprehend-0.1.2/aws_comprehend.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4652 2024-04-17 03:50:59.000000 aws_comprehend-0.1.2/aws_comprehend.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      939 2024-04-17 03:50:59.000000 aws_comprehend-0.1.2/aws_comprehend.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2024-04-17 03:50:59.000000 aws_comprehend-0.1.2/aws_comprehend.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      395 2024-04-17 03:50:59.000000 aws_comprehend-0.1.2/aws_comprehend.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       15 2024-04-17 03:50:59.000000 aws_comprehend-0.1.2/aws_comprehend.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1674 2024-04-17 03:32:31.000000 aws_comprehend-0.1.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2024-04-16 18:15:03.000000 aws_comprehend-0.1.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2024-04-16 18:17:04.000000 aws_comprehend-0.1.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      871 2024-04-16 18:16:55.000000 aws_comprehend-0.1.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2024-04-16 18:15:03.000000 aws_comprehend-0.1.2/requirements-furo-sphinx-search.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      214 2024-04-16 18:17:44.000000 aws_comprehend-0.1.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      149 2024-04-16 16:52:18.000000 aws_comprehend-0.1.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2024-04-17 03:50:59.638518 aws_comprehend-0.1.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7709 2024-04-16 16:52:18.000000 aws_comprehend-0.1.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-17 03:50:59.636887 aws_comprehend-0.1.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      923 2024-04-16 19:48:02.000000 aws_comprehend-0.1.2/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      539 2024-04-16 18:20:37.000000 aws_comprehend-0.1.2/tests/test_comprehend_csv.py
```

### Comparing `aws_comprehend-0.1.1/LICENSE.txt` & `aws_comprehend-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_comprehend-0.1.1/README.rst` & `aws_comprehend-0.1.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     :target: https://pypi.python.org/pypi/aws_comprehend
 
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/aws_comprehend-project
 
 ------
 
-
 .. .. image:: https://img.shields.io/badge/Link-Document-blue.svg
     :target: https://aws_comprehend.readthedocs.io/index.html
 
 .. .. image:: https://img.shields.io/badge/Link-API-blue.svg
     :target: https://aws_comprehend.readthedocs.io/py-modindex.html
 
 .. .. image:: https://img.shields.io/badge/Link-Source_Code-blue.svg
@@ -49,14 +48,16 @@
     :target: https://pypi.org/pypi/aws_comprehend#files
 
 
 Welcome to ``aws_comprehend`` Documentation
 ==============================================================================
 ``aws_comprehend`` improves the vanilla Amazon Comprehend boto3 API.
 
+See `Usage Example <./debug/debug.py>`_.
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``aws_comprehend`` is released on PyPI, so all you need is:
```

### Comparing `aws_comprehend-0.1.1/aws_comprehend/better_boto/document_classifier.py` & `aws_comprehend-0.1.2/aws_comprehend/better_boto/document_classifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 
 import typing as T
 import enum
 import dataclasses
 from datetime import datetime
 
 from iterproxy import IterProxy
-from func_args import NOTHING, resolve_kwargs
 from light_emoji import common
 from boto_session_manager import BotoSesManager
 
-from ..waiter import WaiterError, Waiter
+from ..vendor.waiter import Waiter
+
+from ..exc import WaiterError
+
 
 # ------------------------------------------------------------------------------
 # Data Model
 # ------------------------------------------------------------------------------
 class DocumentClassifierStatusEnum(str, enum.Enum):
     SUBMITTED = "SUBMITTED"
     TRAINING = "TRAINING"
@@ -43,14 +45,16 @@
     zh = "zh"
     zh_TW = "zh-TW"
 
 
 @dataclasses.dataclass
 class DocumentClassifierVersion:
     """
+    Represent a custom document classifier version.
+
     :param arn: example, arn:aws:comprehend:us-east-1:669508176277:document-classifier/tax-document-classifier/version/v000001
     :param language_code: example: en
     """
 
     arn: str = dataclasses.field(default=None)
     language_code: T.Optional[str] = dataclasses.field(default=None)
     version_name: T.Optional[str] = dataclasses.field(default=None)
@@ -91,39 +95,38 @@
         :param document_classifier_properties: the dict at the field "DocumentClassifierProperties"
 
         Ref:
 
         - describe_document_classifier: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_document_classifier
         - list_document_classifiers: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classifiers
         """
+        # fmt: off
         return cls(
             arn=document_classifier_properties.get("DocumentClassifierArn"),
             language_code=document_classifier_properties.get("LanguageCode"),
             version_name=document_classifier_properties.get("VersionName"),
             status=document_classifier_properties.get("Status"),
             status_message=document_classifier_properties.get("Message"),
             submit_time=document_classifier_properties.get("SubmitTime"),
             end_time=document_classifier_properties.get("EndTime"),
             training_start_time=document_classifier_properties.get("TrainingStartTime"),
             training_end_time=document_classifier_properties.get("TrainingEndTime"),
             input_data_config=document_classifier_properties.get("InputDataConfig"),
             output_data_config=document_classifier_properties.get("OutputDataConfig"),
-            classifier_metadata=document_classifier_properties.get(
-                "ClassifierMetadata"
-            ),
-            data_access_role_arn=document_classifier_properties.get(
-                "DataAccessRoleArn"
-            ),
+            classifier_metadata=document_classifier_properties.get("ClassifierMetadata"),
+            data_access_role_arn=document_classifier_properties.get("DataAccessRoleArn"),
             volume_kms_key_id=document_classifier_properties.get("VolumeKmsKeyId"),
             vpc_config=document_classifier_properties.get("VpcConfig"),
             mode=document_classifier_properties.get("Mode"),
             model_kms_key_id=document_classifier_properties.get("ModelKmsKeyId"),
             source_model_arn=document_classifier_properties.get("SourceModelArn"),
         )
 
+    # fmt: on
+
     @classmethod
     def build_arn(
         cls,
         aws_account_id: str,
         aws_region: str,
         classifier_name: str,
         version_name: str,
@@ -136,22 +139,25 @@
     @classmethod
     def get_latest(
         cls,
         bsm: BotoSesManager,
         classifier_name: str,
     ) -> T.Optional["DocumentClassifierVersion"]:
         """
-        :param bsm:
+        Get the latest version of the document classifier. If not found, return None.
+
+        :param bsm: ``boto_session_manager.BotoSesManager`` object.
         :param classifier_name:
         :return:
 
         Ref:
 
         - list_document_classifier_summaries: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classifier_summaries
         """
+        # this API always returns the latest version first.
         response = bsm.comprehend_client.list_document_classifier_summaries(
             MaxResults=100
         )
         for document_classifier_summary in response["DocumentClassifierSummariesList"]:
             if document_classifier_summary["DocumentClassifierName"] == classifier_name:
                 version_name = document_classifier_summary["LatestVersionName"]
                 arn = (
@@ -180,23 +186,23 @@
 ) -> T.Iterable[DocumentClassifierVersion]:
     """
     Use paginator to list all document classifier.
 
     If you use "name" in the filter, then it always returns in descending
      order based on version creation time.
 
-    :param bsm:
-    :param name:
-    :param status:
-    :param submit_time_before:
-    :param submit_time_after:
+    :param bsm: ``boto_session_manager.BotoSesManager`` object.
+    :param name: filter by document classifier name.
+    :param status: filter by status.
+    :param submit_time_before: filter by submit time before this datetime (utc time).
+    :param submit_time_after: filter by submit time after this datetime (utc time).
     :param max_items:
     :param page_size:
 
-    :return:
+    :return: an iterable of :class:`DocumentClassifierVersion` object.
 
     Ref:
 
     - list_document_classifiers: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classifiers
     """
     # You can only set one filter at a time.
     if (
@@ -245,14 +251,17 @@
     name: T.Optional[str] = None,
     status: T.Optional[str] = None,
     submit_time_before: T.Optional[datetime] = None,
     submit_time_after: T.Optional[datetime] = None,
     max_items: int = 1000,
     page_size: int = 100,
 ) -> DocumentClassifierVersionIterProxy:
+    """
+    See :func:`_list_document_classifiers` for more details.
+    """
     return DocumentClassifierVersionIterProxy(
         _list_document_classifiers(
             bsm=bsm,
             name=name,
             status=status,
             submit_time_before=submit_time_before,
             submit_time_after=submit_time_after,
@@ -263,15 +272,17 @@
 
 
 def describe_document_classifier(
     bsm: BotoSesManager,
     arn: str,
 ) -> T.Optional[DocumentClassifierVersion]:
     """
-    :return: DocumentClassifierVersion object or None if not found.
+    Get custom document classifier version details.
+
+    :return: :class:`DocumentClassifierVersion` object or None if not found.
 
     Ref:
 
     - describe_document_classifier: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_document_classifier
     """
     try:
         response = bsm.comprehend_client.describe_document_classifier(
@@ -288,14 +299,19 @@
 
 
 def delete_document_classifier(
     bsm: BotoSesManager,
     arn: str,
 ) -> bool:
     """
+    Delete a custom document classifier.
+
+    :param bsm: ``boto_session_manager.BotoSesManager`` object.
+    :param arn: document classifier arn.
+
     :return: a boolean value indicate that the deletion happened or not.
 
     Ref:
 
     - delete_document_classifier: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_document_classifier
     """
     classifier_version = describe_document_classifier(bsm=bsm, arn=arn)
@@ -312,14 +328,27 @@
     arn: str,
     succeeded_status: T.List[str],
     failed_status: T.List[str] = None,
     delays: int = 5,
     timeout: int = 3600,
     verbose: bool = True,
 ):
+    """
+    Wait for the document classifier to reach the desired status.
+
+    :param bsm: ``boto_session_manager.BotoSesManager`` object.
+    :param arn: document classifier arn.
+    :param succeeded_status: list of status that indicate the waiter should stop
+        as succeeded.
+    :param failed_status: list of status that indicate the waiter should stop
+        and raise exception.
+    :param delays:
+    :param timeout:
+    :param verbose:
+    """
     if failed_status is None:
         failed_status = []
     for _ in Waiter(delays=delays, timeout=timeout, verbose=verbose):
         classifier_version = describe_document_classifier(bsm=bsm, arn=arn)
         if classifier_version is None:
             if verbose:
                 print(f"classifier version doesn't exists.")
@@ -336,14 +365,24 @@
 def wait_create_document_classifier_to_succeed(
     bsm: BotoSesManager,
     arn: str,
     delays: int = 5,
     timeout: int = 3600,
     verbose: bool = True,
 ):
+    """
+    Wait for the "create document classifier" api call to reach succeeded status.
+
+    :param bsm: ``boto_session_manager.BotoSesManager`` object.
+    :param arn: document classifier arn.
+    :param delays:
+    :param timeout:
+    :param verbose:
+    :return:
+    """
     if verbose:  # pragma: no cover
         print(
             f"{common.play_or_pause} wait for "
             f"create document classifier {arn} to finish ..."
         )
     flag = wait_document_classifier(
         bsm=bsm,
@@ -360,24 +399,34 @@
         delays=delays,
         timeout=timeout,
         verbose=verbose,
     )
     if flag is False:
         raise WaiterError(f"{arn} not found!")
     if verbose:  # pragma: no cover
-        print(f"{common.succeeded} document classifier is trained.")
+        print(f"\n{common.succeeded} document classifier is trained.")
 
 
 def wait_delete_document_classifier_to_finish(
     bsm: BotoSesManager,
     arn: str,
     delays: int = 5,
     timeout: int = 3600,
     verbose: bool = True,
 ):
+    """
+    Wait for the "delete document classifier" api call to finish.
+
+    :param bsm: ``boto_session_manager.BotoSesManager`` object.
+    :param arn: document classifier arn.
+    :param delays:
+    :param timeout:
+    :param verbose:
+    :return:
+    """
     if verbose:  # pragma: no cover
         print(
             f"{common.play_or_pause} wait for "
             f"delete document classifier {arn} to finish ..."
         )
     flag = wait_document_classifier(
         bsm=bsm,
@@ -391,8 +440,8 @@
         delays=delays,
         timeout=timeout,
         verbose=verbose,
     )
     if flag is not False:
         raise WaiterError("Deletion failed!")
     if verbose:  # pragma: no cover
-        print(f"{common.succeeded} document classifier is deleted.")
+        print(f"\n{common.succeeded} document classifier is deleted.")
```

### Comparing `aws_comprehend-0.1.1/aws_comprehend/better_boto/endpoint.py` & `aws_comprehend-0.1.2/aws_comprehend/better_boto/endpoint.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from datetime import datetime
 
 from iterproxy import IterProxy
 from func_args import NOTHING, resolve_kwargs
 from light_emoji import common
 from boto_session_manager import BotoSesManager
 
-from ..waiter import WaiterError, Waiter
+from ..vendor.waiter import Waiter
+from ..exc import WaiterError
 
 
 # ------------------------------------------------------------------------------
 # Data Model
 # ------------------------------------------------------------------------------
 class EndpointStatusEnum(str, enum.Enum):
     CREATING = "CREATING"
@@ -114,22 +115,23 @@
     creation_time_after: T.Optional[datetime] = None,
     max_items: int = 1000,
     page_size: int = 100,
 ) -> T.Iterable[Endpoint]:
     """
     Use paginator to list all endpoint.
 
-    :param bsm:
-    :param model_arn:
-    :param status:
-    :param creation_time_before:
-    :param creation_time_after:
+    :param bsm: ``boto_session_manager.BotoSesManager`` object.
+    :param model_arn: filter by model arn.
+    :param status: filter by status.
+    :param creation_time_before: filter by creation time before this datetime (utc time).
+    :param creation_time_after: filter by creation time after this datetime (utc time).
     :param max_items:
     :param page_size:
-    :return:
+
+    :return: an iterator of :class:`Endpoint`
     """
     # You can only set one filter at a time.
     if (
         sum(
             [
                 model_arn is not None,
                 status is not None,
@@ -174,14 +176,17 @@
     model_arn: T.Optional[str] = None,
     status: T.Optional[str] = None,
     creation_time_before: T.Optional[datetime] = None,
     creation_time_after: T.Optional[datetime] = None,
     max_items: int = 1000,
     page_size: int = 100,
 ) -> EndpointIterProxy:
+    """
+    See :func:`_list_endpoints` for more details.
+    """
     return EndpointIterProxy(
         _list_endpoints(
             bsm=bsm,
             model_arn=model_arn,
             status=status,
             creation_time_before=creation_time_before,
             creation_time_after=creation_time_after,
@@ -192,18 +197,19 @@
 
 
 def describe_endpoint(
     bsm: BotoSesManager,
     name_or_arn: str,
 ) -> T.Optional[Endpoint]:
     """
+    Get model endpoint details.
 
-    :param bsm:
-    :param name_or_arn:
-    :return:
+    :param bsm: ``boto_session_manager.BotoSesManager`` object.
+    :param name_or_arn: endpoint name or arn.
+    :return: :class:`Endpoint` or None
 
     Ref:
 
     - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_endpoint
     """
     arn = _ensure_endpoint_arn(bsm=bsm, name_or_arn=name_or_arn)
     try:
@@ -220,16 +226,21 @@
     bsm: BotoSesManager,
     name_or_arn: str,
     desired_model_arn: str = NOTHING,
     desired_inference_units: int = NOTHING,
     desired_data_access_role_arn: str = NOTHING,
 ):
     """
+    Update the model endpoint.
 
-    :return:
+    :param bsm: ``boto_session_manager.BotoSesManager`` object.
+    :param name_or_arn: endpoint name or arn.
+    :param desired_model_arn:
+    :param desired_inference_units:
+    :param desired_data_access_role_arn:
 
     Ref:
 
     - update_endpoint: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.update_endpoint
     """
     arn = _ensure_endpoint_arn(bsm=bsm, name_or_arn=name_or_arn)
     return bsm.comprehend_client.update_endpoint(
@@ -243,14 +254,19 @@
 
 
 def delete_endpoint(
     bsm: BotoSesManager,
     name_or_arn: str,
 ) -> bool:
     """
+    Delete the model endpoint.
+
+    :param bsm: ``boto_session_manager.BotoSesManager`` object.
+    :param name_or_arn:
+
     :return: a boolean value indicate that the deletion happened or not.
 
     Ref:
 
     - delete_endpoint: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_endpoint
     """
     arn = _ensure_endpoint_arn(bsm=bsm, name_or_arn=name_or_arn)
@@ -266,14 +282,28 @@
     name_or_arn: str,
     succeeded_status: T.List[str],
     failed_status: T.List[str] = None,
     delays: int = 5,
     timeout: int = 3600,
     verbose: bool = True,
 ):
+    """
+    Wait for the endpoint to reach the desired status.
+
+    :param bsm: ``boto_session_manager.BotoSesManager`` object.
+    :param name_or_arn: endpoint name or arn.
+    :param succeeded_status: list of status that indicate the waiter should stop
+        as succeeded.
+    :param failed_status: list of status that indicate the waiter should stop
+        and raise exception.
+    :param delays:
+    :param timeout:
+    :param verbose:
+    :return:
+    """
     arn = _ensure_endpoint_arn(bsm=bsm, name_or_arn=name_or_arn)
     if failed_status is None:
         failed_status = []
     for _ in Waiter(delays=delays, timeout=timeout, verbose=verbose):
         endpoint = describe_endpoint(bsm=bsm, name_or_arn=arn)
         if endpoint is None:
             if verbose:
@@ -291,16 +321,26 @@
 def wait_create_or_update_endpoint_to_succeed(
     bsm: BotoSesManager,
     name_or_arn: str,
     delays: int = 5,
     timeout: int = 3600,
     verbose: bool = True,
 ):
+    """
+    Wait for the endpoint to be in service.
+
+    :param bsm: ``boto_session_manager.BotoSesManager`` object.
+    :param name_or_arn: endpoint name or arn.
+    :param delays:
+    :param timeout:
+    :param verbose:
+    :return:
+    """
     arn = _ensure_endpoint_arn(bsm=bsm, name_or_arn=name_or_arn)
-    if verbose: # pragma: no cover
+    if verbose:  # pragma: no cover
         print(
             f"{common.play_or_pause} wait for "
             f"create / update Comprehend endpoint {arn} to finish ..."
         )
     flag = wait_endpoint(
         bsm=bsm,
         name_or_arn=arn,
@@ -313,26 +353,37 @@
         ],
         delays=delays,
         timeout=timeout,
         verbose=verbose,
     )
     if flag is False:
         raise WaiterError(f"{arn} not found!")
-    if verbose: # pragma: no cover
-        print(f"{common.succeeded} Comprehend endpoint is in service.")
+    if verbose:  # pragma: no cover
+        print(f"\n{common.succeeded} Comprehend endpoint is in service.")
+
 
 def wait_delete_endpoint_to_finish(
     bsm: BotoSesManager,
     name_or_arn: str,
     delays: int = 5,
     timeout: int = 3600,
     verbose: bool = True,
 ):
+    """
+    Wait for the endpoint to be deleted.
+
+    :param bsm: ``boto_session_manager.BotoSesManager`` object.
+    :param name_or_arn: endpoint name or arn.
+    :param delays:
+    :param timeout:
+    :param verbose:
+    :return:
+    """
     arn = _ensure_endpoint_arn(bsm=bsm, name_or_arn=name_or_arn)
-    if verbose: # pragma: no cover
+    if verbose:  # pragma: no cover
         print(
             f"{common.play_or_pause} wait for "
             f"delete Comprehend endpoint {arn} to finish ..."
         )
     flag = wait_endpoint(
         bsm=bsm,
         name_or_arn=arn,
@@ -345,9 +396,9 @@
         ],
         delays=delays,
         timeout=timeout,
         verbose=verbose,
     )
     if flag is not False:
         raise WaiterError("Deletion failed!")
-    if verbose: # pragma: no cover
-        print(f"{common.succeeded} Comprehend endpoint is deleted.")
+    if verbose:  # pragma: no cover
+        print(f"\n{common.succeeded} Comprehend endpoint is deleted.")
```

### Comparing `aws_comprehend-0.1.1/aws_comprehend/comprehend_csv.py` & `aws_comprehend-0.1.2/aws_comprehend/comprehend_csv.py`

 * *Files identical despite different names*

### Comparing `aws_comprehend-0.1.1/aws_comprehend.egg-info/SOURCES.txt` & `aws_comprehend-0.1.2/aws_comprehend.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 AUTHORS.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 release-history.rst
+requirements-automation.txt
 requirements-dev.txt
 requirements-doc.txt
+requirements-furo-sphinx-search.txt
 requirements-test.txt
 requirements.txt
 setup.py
 aws_comprehend/__init__.py
 aws_comprehend/_version.py
+aws_comprehend/api.py
 aws_comprehend/compat.py
 aws_comprehend/comprehend_csv.py
-aws_comprehend/waiter.py
+aws_comprehend/exc.py
+aws_comprehend/paths.py
 aws_comprehend.egg-info/PKG-INFO
 aws_comprehend.egg-info/SOURCES.txt
 aws_comprehend.egg-info/dependency_links.txt
 aws_comprehend.egg-info/requires.txt
 aws_comprehend.egg-info/top_level.txt
 aws_comprehend/better_boto/__init__.py
+aws_comprehend/better_boto/api.py
 aws_comprehend/better_boto/document_classifier.py
 aws_comprehend/better_boto/endpoint.py
 aws_comprehend/docs/__init__.py
-aws_comprehend/tests/__init__.py
-aws_comprehend/tests/boto_ses.py
-aws_comprehend/tests/helper.py
-aws_comprehend/tests/paths.py
+aws_comprehend/vendor/__init__.py
+aws_comprehend/vendor/pytest_cov_helper.py
+aws_comprehend/vendor/waiter.py
+tests/test_api.py
+tests/test_comprehend_csv.py
```

### Comparing `aws_comprehend-0.1.1/release-history.rst` & `aws_comprehend-0.1.2/release-history.rst`

 * *Files 20% similar despite different names*

```diff
@@ -4,21 +4,31 @@
 ==============================================================================
 
 
 Backlog (TODO)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
+- Add support to entity recognizer.
+
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.1.2 (2024-04-16)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Minor Improvements**
+
+- Move public api to ``aws_comprehend.api`` module.
+- Improve integration test using sample data.
+
+
 0.1.1 (2023-02-23)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - First release
 - Add the following public API:
     - ``aws_comprehend.to_csv``
```

### Comparing `aws_comprehend-0.1.1/setup.py` & `aws_comprehend-0.1.2/setup.py`

 * *Files identical despite different names*

