# Comparing `tmp/q_alchemy_sdk_py-0.2.2.tar.gz` & `tmp/q_alchemy_sdk_py-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q_alchemy_sdk_py-0.2.2.tar", last modified: Tue Apr  9 12:17:39 2024, max compression
+gzip compressed data, was "q_alchemy_sdk_py-0.2.3.tar", last modified: Wed Apr 17 18:12:00 2024, max compression
```

## Comparing `q_alchemy_sdk_py-0.2.2.tar` & `q_alchemy_sdk_py-0.2.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11556 2024-03-19 19:59:43.321774 q_alchemy_sdk_py-0.2.2/LICENSE
--rw-r--r--   0        0        0     3132 2024-04-03 07:57:53.501345 q_alchemy_sdk_py-0.2.2/README.md
--rw-r--r--   0        0        0      647 2024-04-09 12:17:39.414644 q_alchemy_sdk_py-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      599 2024-04-03 07:57:53.523366 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/__init__.py
--rw-r--r--   0        0        0      844 2024-04-03 07:57:53.524576 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/__init__.py
--rw-r--r--   0        0        0      771 2024-04-03 07:57:53.524576 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/base_relations.py
--rw-r--r--   0        0        0     1237 2024-04-03 07:57:53.525758 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/enterapi.py
--rw-r--r--   0        0        0      645 2024-04-03 07:57:53.525758 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/exceptions.py
--rw-r--r--   0        0        0      599 2024-04-03 07:57:53.527033 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/hco/__init__.py
--rw-r--r--   0        0        0     2955 2024-04-03 07:57:53.528336 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/hco/action_hco.py
--rw-r--r--   0        0        0     3906 2024-04-03 07:57:53.529767 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/hco/action_with_parameters_hco.py
--rw-r--r--   0        0        0     2002 2024-04-03 07:57:53.529767 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/hco/download_link_hco.py
--rw-r--r--   0        0        0     4062 2024-04-03 07:57:53.532279 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/hco/hco_base.py
--rw-r--r--   0        0        0     2573 2024-04-03 07:57:53.532514 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/hco/link_hco.py
--rw-r--r--   0        0        0     5287 2024-04-03 07:57:53.533515 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/hco/upload_action_hco.py
--rw-r--r--   0        0        0      793 2024-04-03 07:57:53.533624 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/http_headers.py
--rw-r--r--   0        0        0     1225 2024-04-03 07:57:53.534906 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/media_types.py
--rw-r--r--   0        0        0      599 2024-04-03 07:57:53.535038 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/model/__init__.py
--rw-r--r--   0        0        0      825 2024-04-03 07:57:53.535038 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/model/error.py
--rw-r--r--   0        0        0     6303 2024-04-03 07:57:53.536408 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/model/sirenmodels.py
--rw-r--r--   0        0        0     1715 2024-04-08 12:05:04.324401 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/polling.py
--rw-r--r--   0        0        0     7752 2024-04-03 07:57:53.537731 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/sirenaccess.py
--rw-r--r--   0        0        0      745 2024-04-03 07:57:53.538986 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/__init__.py
--rw-r--r--   0        0        0     2086 2024-04-03 07:57:53.538986 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/enterjma.py
--rw-r--r--   0        0        0     1009 2024-04-03 07:57:53.540069 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/__init__.py
--rw-r--r--   0        0        0     3006 2024-04-03 07:57:53.541445 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/entrypoint_hco.py
--rw-r--r--   0        0        0     1946 2024-04-03 07:57:53.541445 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/info_hco.py
--rw-r--r--   0        0        0     3704 2024-04-03 07:57:53.542689 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/input_dataslot_hco.py
--rw-r--r--   0        0        0     8200 2024-04-03 07:57:53.543794 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/job_hco.py
--rw-r--r--   0        0        0     3678 2024-04-03 07:57:53.544907 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/job_query_result_hco.py
--rw-r--r--   0        0        0     1591 2024-04-03 07:57:53.546237 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/job_used_tags_hco.py
--rw-r--r--   0        0        0     4361 2024-04-03 07:57:53.547490 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/jobsroot_hco.py
--rw-r--r--   0        0        0     2149 2024-04-03 07:57:53.547490 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/output_dataslot_hco.py
--rw-r--r--   0        0        0     3727 2024-04-03 07:57:53.548796 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/processing_step_hco.py
--rw-r--r--   0        0        0     1714 2024-04-03 07:57:53.549892 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/processing_step_used_tags_hco.py
--rw-r--r--   0        0        0     3937 2024-04-03 07:57:53.549892 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/processingstep_query_result_hco.py
--rw-r--r--   0        0        0     4471 2024-04-03 07:57:53.551160 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/processingsteproot_hco.py
--rw-r--r--   0        0        0     1749 2024-04-03 07:57:53.551160 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/user_hco.py
--rw-r--r--   0        0        0     5694 2024-04-03 07:57:53.552257 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/workdata_hco.py
--rw-r--r--   0        0        0     3616 2024-04-03 07:57:53.553479 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/workdata_query_result_hco.py
--rw-r--r--   0        0        0     1646 2024-04-03 07:57:53.553479 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/workdata_used_tags_hco.py
--rw-r--r--   0        0        0     3911 2024-04-03 07:57:53.554644 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/workdataroot_hco.py
--rw-r--r--   0        0        0     1223 2024-04-03 07:57:53.554644 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/known_relations.py
--rw-r--r--   0        0        0      636 2024-04-03 07:57:53.556045 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/model/__init__.py
--rw-r--r--   0        0        0    29090 2024-04-03 07:57:53.556045 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/model/open_api_generated.py
--rw-r--r--   0        0        0     3890 2024-04-03 07:57:53.557167 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/model/sirenentities.py
--rw-r--r--   0        0        0      623 2024-04-03 07:57:53.557167 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/tool/__init__.py
--rw-r--r--   0        0        0    14157 2024-04-03 07:57:53.558405 q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/tool/job.py
--rw-r--r--   0        0        0        0 2024-04-03 07:57:53.558405 q_alchemy_sdk_py-0.2.2/src/q_alchemy/__init__.py
--rw-r--r--   0        0        0     6932 2024-04-08 14:03:19.606017 q_alchemy_sdk_py-0.2.2/src/q_alchemy/qiskit_integration.py
--rw-r--r--   0        0        0      603 2024-03-19 19:59:43.347535 q_alchemy_sdk_py-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0    16512 2024-03-19 19:59:43.350535 q_alchemy_sdk_py-0.2.2/tests/data/test_baa_state.10.1.npy
--rw-r--r--   0        0        0    65664 2024-03-19 19:59:43.351535 q_alchemy_sdk_py-0.2.2/tests/data/test_baa_state.12.1.npy
--rw-r--r--   0        0        0     2176 2024-03-19 19:59:43.352534 q_alchemy_sdk_py-0.2.2/tests/data/test_baa_state.7.1.npy
--rw-r--r--   0        0        0     3342 1970-01-01 00:00:00.000000 q_alchemy_sdk_py-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11556 2024-03-19 19:59:43.321774 q_alchemy_sdk_py-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3132 2024-04-03 07:57:53.501345 q_alchemy_sdk_py-0.2.3/README.md
+-rw-r--r--   0        0        0      647 2024-04-17 18:12:00.597887 q_alchemy_sdk_py-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      599 2024-04-03 07:57:53.523366 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/__init__.py
+-rw-r--r--   0        0        0      844 2024-04-17 17:54:37.354574 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-17 17:54:32.473184 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/base_relations.py
+-rw-r--r--   0        0        0     1237 2024-04-17 17:54:11.519581 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/enterapi.py
+-rw-r--r--   0        0        0      645 2024-04-17 17:54:15.151139 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/exceptions.py
+-rw-r--r--   0        0        0      599 2024-04-17 17:55:17.420851 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/__init__.py
+-rw-r--r--   0        0        0     2955 2024-04-17 17:54:56.794799 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/action_hco.py
+-rw-r--r--   0        0        0     3906 2024-04-17 17:54:59.617204 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/action_with_parameters_hco.py
+-rw-r--r--   0        0        0     2002 2024-04-17 17:55:02.356072 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/download_link_hco.py
+-rw-r--r--   0        0        0     4062 2024-04-17 17:55:05.889416 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/hco_base.py
+-rw-r--r--   0        0        0     2573 2024-04-17 17:55:09.246155 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/link_hco.py
+-rw-r--r--   0        0        0     5287 2024-04-17 17:55:12.020199 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/upload_action_hco.py
+-rw-r--r--   0        0        0      793 2024-04-17 17:54:18.992349 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/http_headers.py
+-rw-r--r--   0        0        0     1225 2024-04-17 17:54:21.836368 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/media_types.py
+-rw-r--r--   0        0        0      599 2024-04-17 17:54:43.443856 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/model/__init__.py
+-rw-r--r--   0        0        0      825 2024-04-17 17:54:47.871461 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/model/error.py
+-rw-r--r--   0        0        0     6303 2024-04-17 17:54:50.396063 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/model/sirenmodels.py
+-rw-r--r--   0        0        0     1715 2024-04-17 17:54:25.520035 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/polling.py
+-rw-r--r--   0        0        0     7752 2024-04-17 17:54:28.807755 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/sirenaccess.py
+-rw-r--r--   0        0        0      745 2024-04-17 17:58:05.367005 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/__init__.py
+-rw-r--r--   0        0        0     2118 2024-04-17 17:58:05.443658 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/enterjma.py
+-rw-r--r--   0        0        0     1009 2024-04-17 17:55:21.823595 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/__init__.py
+-rw-r--r--   0        0        0     3006 2024-04-17 17:55:24.271483 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/entrypoint_hco.py
+-rw-r--r--   0        0        0     1991 2024-04-17 17:58:05.380312 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/info_hco.py
+-rw-r--r--   0        0        0     3704 2024-04-17 17:55:34.427616 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/input_dataslot_hco.py
+-rw-r--r--   0        0        0     8200 2024-04-17 17:55:38.341171 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/job_hco.py
+-rw-r--r--   0        0        0     3678 2024-04-17 17:55:42.295023 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/job_query_result_hco.py
+-rw-r--r--   0        0        0     1591 2024-04-17 17:55:46.843240 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/job_used_tags_hco.py
+-rw-r--r--   0        0        0     4361 2024-04-17 17:55:50.628166 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/jobsroot_hco.py
+-rw-r--r--   0        0        0     2149 2024-04-17 17:55:54.343397 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/output_dataslot_hco.py
+-rw-r--r--   0        0        0     3727 2024-04-17 17:55:57.027348 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processing_step_hco.py
+-rw-r--r--   0        0        0     1714 2024-04-17 17:56:00.072771 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processing_step_used_tags_hco.py
+-rw-r--r--   0        0        0     3937 2024-04-17 17:56:03.543447 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processingstep_query_result_hco.py
+-rw-r--r--   0        0        0     4471 2024-04-17 17:56:06.626480 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processingsteproot_hco.py
+-rw-r--r--   0        0        0     1749 2024-04-17 17:56:09.508138 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/user_hco.py
+-rw-r--r--   0        0        0     5694 2024-04-17 17:56:12.858256 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdata_hco.py
+-rw-r--r--   0        0        0     3616 2024-04-17 17:56:15.879756 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdata_query_result_hco.py
+-rw-r--r--   0        0        0     1734 2024-04-17 17:58:05.405575 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdata_used_tags_query_result_hco.py
+-rw-r--r--   0        0        0     4772 2024-04-17 17:58:05.393524 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdataroot_hco.py
+-rw-r--r--   0        0        0     1223 2024-04-17 17:57:39.063985 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/known_relations.py
+-rw-r--r--   0        0        0      636 2024-04-17 17:56:40.970595 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/model/__init__.py
+-rw-r--r--   0        0        0    29427 2024-04-17 17:53:00.614623 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/model/open_api_generated.py
+-rw-r--r--   0        0        0     3923 2024-04-17 17:58:05.415173 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/model/sirenentities.py
+-rw-r--r--   0        0        0      623 2024-04-17 17:57:03.466217 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/tool/__init__.py
+-rw-r--r--   0        0        0    14478 2024-04-17 17:58:05.423395 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/tool/job.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:57:53.558405 q_alchemy_sdk_py-0.2.3/src/q_alchemy/__init__.py
+-rw-r--r--   0        0        0     7106 2024-04-17 18:09:47.453203 q_alchemy_sdk_py-0.2.3/src/q_alchemy/qiskit_integration.py
+-rw-r--r--   0        0        0      603 2024-03-19 19:59:43.347535 q_alchemy_sdk_py-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0    16512 2024-03-19 19:59:43.350535 q_alchemy_sdk_py-0.2.3/tests/data/test_baa_state.10.1.npy
+-rw-r--r--   0        0        0    65664 2024-03-19 19:59:43.351535 q_alchemy_sdk_py-0.2.3/tests/data/test_baa_state.12.1.npy
+-rw-r--r--   0        0        0     2176 2024-03-19 19:59:43.352534 q_alchemy_sdk_py-0.2.3/tests/data/test_baa_state.7.1.npy
+-rw-r--r--   0        0        0     3342 1970-01-01 00:00:00.000000 q_alchemy_sdk_py-0.2.3/PKG-INFO
```

### Comparing `q_alchemy_sdk_py-0.2.2/LICENSE` & `q_alchemy_sdk_py-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/README.md` & `q_alchemy_sdk_py-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/pyproject.toml` & `q_alchemy_sdk_py-0.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "q-alchemy-sdk-py"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = [
     { name = "Carsten Blank", email = "blank@data-cybernetics.com" },
 ]
 dependencies = [
     "qiskit>=1.0.2",
     "pydantic>=2.6.4",
```

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/__init__.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/__init__.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/base_relations.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/base_relations.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/enterapi.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/enterapi.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/exceptions.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/hco/__init__.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/hco/action_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/action_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/hco/action_with_parameters_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/action_with_parameters_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/hco/download_link_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/download_link_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/hco/hco_base.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/hco_base.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/hco/link_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/link_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/hco/upload_action_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/upload_action_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/http_headers.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/http_headers.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/media_types.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/media_types.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/model/__init__.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/model/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/model/error.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/model/error.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/model/sirenmodels.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/model/sirenmodels.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/polling.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/polling.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/core/sirenaccess.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/sirenaccess.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/__init__.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ruff: noqa: F401
 from .enterjma import enter_jma
 from .tool import Job
 
 # Protocol version the JMA is using
-__jma_version__ = [5, 0, 0]
+__jma_version__ = [5, 1, 1]
```

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/enterjma.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/enterjma.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 import hypermedia_client.job_management
 
 LOG = logging.getLogger(__name__)
 
 THco = TypeVar("THco", bound=Hco)
 
 
-def _version_match(ver1: list[int], ver2: list[int]) -> bool:
-    return all([v1 == v2 for v1, v2 in zip(ver1, ver2)])
+def _version_match_major_minor(ver1: list[int], ver2: list[int]) -> bool:
+    return all([v1 == v2 for v1, v2 in zip(ver1[:2], ver2[:2])])
 
 
 def enter_jma(
     client: httpx.Client,
     entrypoint_hco_type: Type[THco] = EntryPointHco,
     entrypoint_entity_type: Type[Entity] = EntryPointEntity,
     entrypoint: str = "api/EntryPoint",
@@ -40,14 +40,14 @@
     entry_point_hco = enter_api(client, entrypoint_hco_type, entrypoint_entity_type, entrypoint)
 
     info = entry_point_hco.info_link.navigate()
 
     # Check for matching protocol versions
     client_version = hypermedia_client.job_management.__jma_version__
     jma_version = [int(i) for i in str.split(info.api_version, '.')]
-    if not _version_match(jma_version, client_version):
+    if not _version_match_major_minor(jma_version, client_version):
         LOG.warning(
             f"Version mismatch between 'hypermedia_client' (v{'.'.join(map(str ,client_version))}) "
             f"and 'JobManagementAPI' (v{'.'.join(map(str, jma_version))})! "
         )
 
     return entry_point_hco
```

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/__init__.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/entrypoint_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/entrypoint_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/info_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/info_hco.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         return InfoHco.from_entity(self._navigate_internal(InfoEntity), self._client)
 
 
 class InfoHco(Hco[InfoEntity]):
     api_version: str = Property()
     build_version: str = Property()
     current_user: UserHco
+    used_storage_in_bytes: int = Property()
 
     self_link: InfoLink
 
     @classmethod
     def from_entity(cls, entity: InfoEntity, client: httpx.Client) -> Self:
         instance = cls(client, entity)
```

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/input_dataslot_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/input_dataslot_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/job_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/job_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/job_query_result_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/job_query_result_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/job_used_tags_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/job_used_tags_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/jobsroot_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/jobsroot_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/output_dataslot_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/output_dataslot_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/processing_step_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processing_step_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/processing_step_used_tags_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processing_step_used_tags_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/processingstep_query_result_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processingstep_query_result_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/processingsteproot_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processingsteproot_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/user_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/user_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/workdata_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdata_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/workdata_query_result_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdata_query_result_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/workdata_used_tags_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdata_used_tags_query_result_hco.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 from typing import List, Self
 
 import httpx
 
 from hypermedia_client.core.hco.hco_base import Hco, Property
 from hypermedia_client.core.hco.link_hco import LinkHco
 from hypermedia_client.job_management.known_relations import Relations
-from hypermedia_client.job_management.model.sirenentities import WorkDataUsedTagsEntity
+from hypermedia_client.job_management.model.sirenentities import WorkDataUsedTagsQueryResultEntity
 
 
-class WorkDataUsedTagsHco(Hco[WorkDataUsedTagsEntity]):
+class WorkDataUsedTagsQueryResultHto(Hco[WorkDataUsedTagsQueryResultEntity]):
     tags: List[str] | None = Property()
 
     self_link: 'WorkDataUsedTagsLink'
 
     @classmethod
-    def from_entity(cls, entity: WorkDataUsedTagsEntity, client: httpx.Client) -> Self:
+    def from_entity(cls, entity: WorkDataUsedTagsQueryResultEntity, client: httpx.Client) -> Self:
         instance = cls(client, entity)
 
-        Hco.check_classes(instance._entity.class_, ["WorkDataUsedTags"])
+        Hco.check_classes(instance._entity.class_, ["WorkDataUsedTagsQueryResult"])
 
         instance.self_link = WorkDataUsedTagsLink.from_entity(instance._client, instance._entity, Relations.SELF)
 
         return instance
 
 
 class WorkDataUsedTagsLink(LinkHco):
-    def navigate(self) -> WorkDataUsedTagsHco:
-        return WorkDataUsedTagsHco.from_entity(self._navigate_internal(WorkDataUsedTagsEntity), self._client)
+    def navigate(self) -> WorkDataUsedTagsQueryResultHto:
+        return WorkDataUsedTagsQueryResultHto.from_entity(self._navigate_internal(WorkDataUsedTagsQueryResultEntity), self._client)
```

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/hcos/workdataroot_hco.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdataroot_hco.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,64 +14,77 @@
 import httpx
 
 from hypermedia_client.core import MediaTypes, Link
 from hypermedia_client.core.hco.action_with_parameters_hco import ActionWithParametersHco
 from hypermedia_client.core.hco.hco_base import Hco
 from hypermedia_client.core.hco.link_hco import LinkHco
 from hypermedia_client.core.hco.upload_action_hco import UploadAction, UploadParameters
-from hypermedia_client.job_management.hcos.workdata_used_tags_hco import WorkDataUsedTagsLink
+from hypermedia_client.job_management.hcos.workdata_used_tags_query_result_hco import WorkDataUsedTagsLink
 from hypermedia_client.job_management.hcos.workdata_hco import WorkDataLink
 from hypermedia_client.job_management.hcos.workdata_query_result_hco import (
     WorkDataQueryResultHco,
     WorkDataQueryResultLink,
     WorkDataQueryResultPaginationLink
 )
 from hypermedia_client.job_management.known_relations import Relations
-from hypermedia_client.job_management.model import WorkDataQueryParameters
+from hypermedia_client.job_management.model import WorkDataQueryParameters, WorkDataUsedTagsFilterParameter
 from hypermedia_client.job_management.model.sirenentities import WorkDataRootEntity
 
 
 class WorkDataQueryAction(ActionWithParametersHco[WorkDataQueryParameters]):
     def execute(self, parameters: WorkDataQueryParameters) -> WorkDataQueryResultHco:
         url = self._execute_returns_url(parameters)
         link = Link.from_url(url, [str(Relations.CREATED_RESSOURCE)], "Created query", MediaTypes.SIREN)
         # resolve link immediately
         return WorkDataQueryResultLink.from_link(self._client, link).navigate()
 
     def default_parameters(self) -> WorkDataQueryParameters:
         return self._get_default_parameters(WorkDataQueryParameters, WorkDataQueryParameters())
 
 
+class WorkDataUsedTagsQueryAction(ActionWithParametersHco[WorkDataUsedTagsFilterParameter]):
+    def execute(self, parameters: WorkDataUsedTagsFilterParameter) -> WorkDataUsedTagsLink:
+        url = self._execute_returns_url(parameters)
+        link = Link.from_url(url, [str(Relations.CREATED_RESSOURCE)], "Created query", MediaTypes.SIREN)
+        return WorkDataUsedTagsLink.from_link(self._client, link)
+
+    def default_parameters(self) -> WorkDataUsedTagsFilterParameter:
+        return self._get_default_parameters(WorkDataUsedTagsFilterParameter, WorkDataUsedTagsFilterParameter())
+
+
 class WorkDataUploadAction(UploadAction):
     def execute(self, parameters: UploadParameters) -> WorkDataLink:
         url = self._upload(parameters)
         link = Link.from_url(url, [str(Relations.CREATED_RESSOURCE)], "Uploaded workdata", MediaTypes.SIREN)
         return WorkDataLink.from_link(self._client, link)
 
 
 class WorkDataRootLink(LinkHco):
     def navigate(self) -> 'WorkDataRootHco':
         return WorkDataRootHco.from_entity(self._navigate_internal(WorkDataRootEntity), self._client)
 
 
 class WorkDataRootHco(Hco[WorkDataRootEntity]):
     query_action: WorkDataQueryAction | None
+    query_tags_action: WorkDataUsedTagsQueryAction | None
     upload_action: WorkDataUploadAction | None
 
     self_link: WorkDataRootLink
     all_link: WorkDataQueryResultPaginationLink | None
     used_tags_link: WorkDataUsedTagsLink | None
 
     @classmethod
     def from_entity(cls, entity: WorkDataRootEntity, client: httpx.Client) -> Self:
         instance = cls(client, entity)
         Hco.check_classes(instance._entity.class_, ["WorkDataRoot"])
 
         instance.query_action = WorkDataQueryAction.from_entity_optional(
             client, instance._entity, "CreateWorkDataQuery")
+        instance.query_tags_action = WorkDataUsedTagsQueryAction.from_entity_optional(
+            client, instance._entity, "CreateWorkDataTagsQuery")
         instance.upload_action = WorkDataUploadAction.from_entity_optional(
             client, instance._entity, "Upload")
 
         instance.self_link = WorkDataRootLink.from_entity(
             instance._client, instance._entity, Relations.SELF)
 
         instance.all_link = WorkDataQueryResultPaginationLink.from_entity_optional(
```

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/known_relations.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/known_relations.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/model/__init__.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/model/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/model/open_api_generated.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/model/open_api_generated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2024-03-19T09:07:42+00:00
+#   timestamp: 2024-04-02T14:37:39+00:00
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, List
 
 from pydantic import AwareDatetime, BaseModel, ConfigDict, Field, constr
@@ -131,14 +131,15 @@
 class InfoHtoOpenApiProperties(BaseModel):
     model_config = ConfigDict(
         extra='allow',
         populate_by_name=True,
     )
     api_version: str | None = Field(None, alias='ApiVersion')
     build_version: str | None = Field(None, alias='BuildVersion')
+    used_storage_in_bytes: int | None = Field(None, alias='UsedStorageInBytes')
 
 
 class JobQueryResultHtoOpenApiProperties(BaseModel):
     model_config = ConfigDict(
         extra='allow',
         populate_by_name=True,
     )
@@ -429,15 +430,23 @@
         extra='allow',
         populate_by_name=True,
     )
     property_name: WorkDataSortProperties | None = Field(None, alias='PropertyName')
     sort_type: SortTypes | None = Field(None, alias='SortType')
 
 
-class WorkDataUsedTagsHtoOpenApiProperties(BaseModel):
+class WorkDataUsedTagsFilterParameter(BaseModel):
+    model_config = ConfigDict(
+        extra='allow',
+        populate_by_name=True,
+    )
+    required_tags: List[str] | None = Field(None, alias='RequiredTags')
+
+
+class WorkDataUsedTagsQueryResultHtoOpenApiProperties(BaseModel):
     model_config = ConfigDict(
         extra='allow',
         populate_by_name=True,
     )
     tags: List[str] | None = Field(None, alias='Tags')
 
 
@@ -783,22 +792,22 @@
     title: str | None = None
     properties: WorkDataRootHtoOpenApiProperties | None = None
     entities: List | None = None
     actions: List[Action] | None = None
     links: List[Link] | None = None
 
 
-class WorkDataUsedTagsHtoOpenApi(BaseModel):
+class WorkDataUsedTagsQueryResultHtoOpenApi(BaseModel):
     model_config = ConfigDict(
         extra='allow',
         populate_by_name=True,
     )
     class_: List[str] | None = Field(None, alias='class')
     title: str | None = None
-    properties: WorkDataUsedTagsHtoOpenApiProperties | None = None
+    properties: WorkDataUsedTagsQueryResultHtoOpenApiProperties | None = None
     entities: List | None = None
     actions: List[Action] | None = None
     links: List[Link] | None = None
 
 
 class AdminJobQueryParameters(BaseModel):
     model_config = ConfigDict(
```

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/model/sirenentities.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/model/sirenentities.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,18 @@
     JobHtoOpenApiProperties,
     WorkDataHtoOpenApiProperties,
     ProcessingStepHtoOpenApiProperties,
     WorkDataQueryResultHtoOpenApiProperties,
     WorkDataRootHtoOpenApiProperties,
     ProcessingStepRootHtoOpenApiProperties,
     ProcessingStepQueryResultHtoOpenApiProperties,
-    WorkDataUsedTagsHtoOpenApiProperties,
     JobUsedTagsHtoOpenApiProperties,
     ProcessingStepUsedTagsHtoOpenApiProperties,
     UserHtoOpenApiProperties,
+    WorkDataUsedTagsQueryResultHtoOpenApiProperties,
 )
 
 
 # ToDo: make these Generics bound to Entity
 
 
 class EntryPointEntity(Entity):
@@ -74,16 +74,16 @@
     properties: ProcessingStepRootHtoOpenApiProperties | None = None
 
 
 class ProcessingStepQueryResultEntity(Entity):
     properties: ProcessingStepQueryResultHtoOpenApiProperties | None = None
 
 
-class WorkDataUsedTagsEntity(Entity):
-    properties: WorkDataUsedTagsHtoOpenApiProperties | None = None
+class WorkDataUsedTagsQueryResultEntity(Entity):
+    properties: WorkDataUsedTagsQueryResultHtoOpenApiProperties | None = None
 
 
 class ProcessingStepUsedTagsEntity(Entity):
     properties: ProcessingStepUsedTagsHtoOpenApiProperties | None = None
 
 
 class JobUsedTagsEntity(Entity):
```

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/tool/__init__.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/src/hypermedia_client/job_management/tool/job.py` & `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/tool/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # limitations under the License.
 import json as json_
 from typing import Any, Self
 
 import httpx
 from httpx import URL
 
-
 from hypermedia_client.core import Link, MediaTypes
 from hypermedia_client.core.polling import wait_until, PollingException
 from hypermedia_client.job_management.enterjma import enter_jma
 from hypermedia_client.job_management.hcos import WorkDataLink
 from hypermedia_client.job_management.hcos.entrypoint_hco import EntryPointHco
 from hypermedia_client.job_management.hcos.job_hco import (
     JobHco,
@@ -38,15 +37,15 @@
     ProcessingStepFilterParameter,
     SelectProcessingParameters,
     JobStates,
     CreateSubJobParameters,
     JobQueryParameters,
     JobSortPropertiesSortParameter,
     JobFilterParameter,
-    SelectWorkDataForDataSlotParameters,
+    SelectWorkDataForDataSlotParameters, SetJobTagsParameters,
 )
 
 
 class Job:
     """Convenience wrapper for handling JobHcos in the JobManagement-Api.
 
     This wrapper allows the API to be used with a fluent-style builder pattern:
@@ -227,15 +226,14 @@
         """
         # TODO: return Sentinel or Exception on 'NotDoneYet'
         # TODO: handle return value equivalent to asyncio's Future objects
         self.refresh()
         result = self._job.result
         return json_.loads(result) if result else None
 
-
     def wait_for_state(self, state: JobStates, timeout_ms: int = 5000) -> Self:
         """Wait for this job to reach a state.
 
         Args:
             state: The state to wait for. After the job enters this state this function returns.
             timeout_ms: Time span in milliseconds to wait for reaching the state before
                 raising an exception.
@@ -300,20 +298,20 @@
 
         dataslot.clear_workdata_action.execute()
         self.refresh()
 
         return self
 
     def _get_sub_jobs(
-        self,
-        sort_by: JobSortPropertiesSortParameter | None = None,
-        state: JobStates | None = None,
-        name: str | None = None,
-        show_deleted: bool | None = None,
-        processing_step_url: str | None = None,
+            self,
+            sort_by: JobSortPropertiesSortParameter | None = None,
+            state: JobStates | None = None,
+            name: str | None = None,
+            show_deleted: bool | None = None,
+            processing_step_url: str | None = None,
     ) -> JobQueryResultHco:
         filter_param = JobFilterParameter(
             is_sub_job=True,
             parent_job_url=str(self._job.self_link.get_url()),
             state=state,
             name=name,
             show_deleted=show_deleted,
@@ -401,8 +399,19 @@
     def disallow_output_data_deletion(self):
         """Mark all output workdata from this job as "not deletable".
 
         Returns:
             This `Job` object"""
         self._job.disallow_output_data_deletion_action.execute()
         self.refresh()
-        return self
+        return self
+
+    def set_tags(self, tags: list[str]):
+        """Set tags to the job.
+
+        Returns:
+            This `Job` object"""
+        self._job.edit_tags_action.execute(SetJobTagsParameters(
+            tags=tags
+        ))
+        self.refresh()
+        return self
```

### Comparing `q_alchemy_sdk_py-0.2.2/src/q_alchemy/qiskit_integration.py` & `q_alchemy_sdk_py-0.2.3/src/q_alchemy/qiskit_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright 2022-2023 data cybernetics ssc GmbH.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #     http://www.apache.org/licenses/LICENSE-2.0
-
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import datetime
 import logging
 import os
 import hashlib
 from dataclasses import dataclass, field
 from typing import List, Dict, Tuple
 
 import httpx
@@ -29,14 +30,15 @@
 
 logging.getLogger("httpx").setLevel(logging.WARN)
 LOG = logging.getLogger(__name__)
 
 
 @dataclass
 class OptParams:
+    remove_data: bool = field(default=True)
     max_fidelity_loss: float = field(default=0.0)
     job_tags: List[str] = field(default_factory=list)
     api_key: str = field(default_factory=lambda: os.getenv("Q_ALCHEMY_API_KEY"))
     host: str = field(default="jobs.api.q-alchemy.com")
     schema: str = field(default="https")
     added_headers: Dict[str, str] = field(default_factory=dict)
     isometry_scheme: str = field(default="ccd")
@@ -98,15 +100,15 @@
             headers=headers,
             timeout=httpx.Timeout(timeout=self.opt_params.job_completion_timeout_sec + 10.0, connect=10.0)
         )
         super().__init__("q-alchemy", num_qubits, 0, params=params, label=label)
         self.param_hash = hashlib.md5(np.asarray(self.params).tobytes()).hexdigest()
 
     def _define(self):
-        sequence_wd_tags = [self.param_hash, "Q-Alchemy", "Qiskit-Integration"]
+        sequence_wd_tags = [f"Hash={self.param_hash}", "Source=Qiskit-Integration", f"ImageSize={self.opt_params.image_size}"]
         wd_root = enter_jma(self.client).work_data_root_link.navigate()
 
         existing_wd_query = wd_root.query_action.execute(WorkDataQueryParameters(
             filter=WorkDataFilterParameter(tags_by_and=sequence_wd_tags)
         ))
 
         if existing_wd_query.total_entities == 0:
@@ -119,40 +121,40 @@
             wd_link.navigate().edit_tags_action.execute(SetTagsWorkDataParameters(tags=sequence_wd_tags))
         else:
             wd_link = existing_wd_query.workdatas[0].self_link
 
         job_timeout = self.opt_params.job_completion_timeout_sec * 1000
         job = (
             Job(self.client)
-            .create(name='Execute Transformation')
+            .create(name=f'Execute Transformation ({datetime.datetime.now()})')
             .select_processing(processing_step='convert_circuit_layers')
             .configure_parameters(
                 min_fidelity=1.0 - self.opt_params.max_fidelity_loss,
                 basis_gates=self.opt_params.basis_gates,
                 image_shape_x=self.opt_params.image_size[0],
                 image_shape_y=self.opt_params.image_size[1]
             )
             .assign_input_dataslot(0, wd_link)
             .allow_output_data_deletion()
             .start()
             .wait_for_state(JobStates.completed, timeout_ms=job_timeout)
-            .hide()
         )
         self.result_summary: dict = job.get_result()
         inner_job = job._job
         if self.result_summary["status"].startswith("OK"):
             qasm_wd = [s.assigned_workdata for s in inner_job.output_dataslots if s.assigned_workdata.name == "qasm_circuit.qasm"][0]
             if qasm_wd.size_in_bytes > 0:
                 qasm: str = qasm_wd.download_link.download().decode("utf-8")
                 qc = QuantumCircuit.from_qasm_str(qasm)
                 self.definition = qc
             else:
                 raise IOError("Q-Alchemy API call failed for unknown reasons.")
         else:
             raise IOError(f"Q-Alchemy API call failed. Reason: {self.result_summary['status']}.")
         # Clean-up now.
-        if inner_job is not None:
+        if self.opt_params.remove_data and inner_job is not None:
+            job.hide()
             for wd in inner_job.output_dataslots:
                 delete_action = wd.assigned_workdata.delete_action
                 if delete_action is not None:
                     delete_action.execute()
```

### Comparing `q_alchemy_sdk_py-0.2.2/tests/__init__.py` & `q_alchemy_sdk_py-0.2.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/tests/data/test_baa_state.10.1.npy` & `q_alchemy_sdk_py-0.2.3/tests/data/test_baa_state.10.1.npy`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/tests/data/test_baa_state.12.1.npy` & `q_alchemy_sdk_py-0.2.3/tests/data/test_baa_state.12.1.npy`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/tests/data/test_baa_state.7.1.npy` & `q_alchemy_sdk_py-0.2.3/tests/data/test_baa_state.7.1.npy`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.2/PKG-INFO` & `q_alchemy_sdk_py-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q-alchemy-sdk-py
-Version: 0.2.2
+Version: 0.2.3
 Author-Email: Carsten Blank <blank@data-cybernetics.com>
 License: Apache
 Requires-Python: <4,>=3.11
 Requires-Dist: qiskit>=1.0.2
 Requires-Dist: pydantic>=2.6.4
 Requires-Dist: httpx<1.0.0,>=0.25.0
 Description-Content-Type: text/markdown
```

