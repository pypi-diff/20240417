# Comparing `tmp/mypy-boto3-qbusiness-1.34.42.tar.gz` & `tmp/mypy_boto3_qbusiness-1.34.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-qbusiness-1.34.42.tar", last modified: Wed Feb 14 20:32:19 2024, max compression
+gzip compressed data, was "mypy_boto3_qbusiness-1.34.86.tar", last modified: Wed Apr 17 19:47:44 2024, max compression
```

## Comparing `mypy-boto3-qbusiness-1.34.42.tar` & `mypy_boto3_qbusiness-1.34.86.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 20:32:19.619386 mypy-boto3-qbusiness-1.34.42/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-14 20:32:06.000000 mypy-boto3-qbusiness-1.34.42/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-02-14 20:32:19.619386 mypy-boto3-qbusiness-1.34.42/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-02-14 20:32:06.000000 mypy-boto3-qbusiness-1.34.42/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 20:32:19.615386 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-02-14 20:32:06.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-02-14 20:32:06.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-14 20:32:06.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43761 2024-02-14 20:32:07.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    43758 2024-02-14 20:32:06.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-02-14 20:32:07.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-02-14 20:32:07.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-02-14 20:32:07.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14217 2024-02-14 20:32:07.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 20:32:06.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    57158 2024-02-14 20:32:08.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    57158 2024-02-14 20:32:07.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-14 20:32:06.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 20:32:19.615386 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-02-14 20:32:19.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-02-14 20:32:19.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 20:32:19.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 20:32:19.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-14 20:32:19.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-14 20:32:19.000000 mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 20:32:19.619386 mypy-boto3-qbusiness-1.34.42/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-14 20:32:06.000000 mypy-boto3-qbusiness-1.34.42/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:47:44.461914 mypy_boto3_qbusiness-1.34.86/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-04-17 19:47:44.461914 mypy_boto3_qbusiness-1.34.86/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:47:44.461914 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44581 2024-04-17 19:47:31.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44578 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-04-17 19:47:31.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-04-17 19:47:31.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14275 2024-04-17 19:47:31.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-17 19:47:31.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    58504 2024-04-17 19:47:32.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58504 2024-04-17 19:47:32.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:47:44.461914 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-04-17 19:47:44.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-17 19:47:44.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:47:44.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:47:44.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-17 19:47:44.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 19:47:44.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:47:44.461914 mypy_boto3_qbusiness-1.34.86/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/setup.py
```

### Comparing `mypy-boto3-qbusiness-1.34.42/LICENSE` & `mypy_boto3_qbusiness-1.34.86/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qbusiness-1.34.42/PKG-INFO` & `mypy_boto3_qbusiness-1.34.86/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qbusiness
-Version: 1.34.42
-Summary: Type annotations for boto3.QBusiness 1.34.42 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.86
+Summary: Type annotations for boto3.QBusiness 1.34.86 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-qbusiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qbusiness)](https://pepy.tech/project/mypy-boto3-qbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QBusiness 1.34.42](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
+[boto3.QBusiness 1.34.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-qbusiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-qbusiness-1.34.42/README.md` & `mypy_boto3_qbusiness-1.34.86/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-qbusiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qbusiness)](https://pepy.tech/project/mypy-boto3-qbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QBusiness 1.34.42](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
+[boto3.QBusiness 1.34.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-qbusiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/__init__.py` & `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/__init__.pyi` & `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/__main__.py` & `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.QBusiness 1.34.42\n"
-        "Version:         1.34.42\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.QBusiness 1.34.86\n"
+        "Version:         1.34.86\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.42")
+    print("1.34.86")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/client.py` & `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    ChatModeType,
     DataSourceSyncJobStatusType,
     MembershipTypeType,
     PluginStateType,
     PluginTypeType,
     ResponseScopeType,
     RetrieverTypeType,
     WebExperienceSamplePromptsControlModeType,
@@ -46,21 +47,23 @@
     ActionExecutionTypeDef,
     AttachmentInputTypeDef,
     AttachmentsConfigurationTypeDef,
     AttributeFilterTypeDef,
     BatchDeleteDocumentResponseTypeDef,
     BatchPutDocumentResponseTypeDef,
     BlockedPhrasesConfigurationUpdateTypeDef,
+    ChatModeConfigurationTypeDef,
     ChatSyncOutputTypeDef,
     CreateApplicationResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreatePluginResponseTypeDef,
     CreateRetrieverResponseTypeDef,
     CreateWebExperienceResponseTypeDef,
+    CreatorModeConfigurationTypeDef,
     DataSourceVpcConfigurationTypeDef,
     DeleteDocumentTypeDef,
     DocumentAttributeConfigurationTypeDef,
     DocumentEnrichmentConfigurationTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionConfigurationTypeDef,
@@ -150,15 +153,15 @@
         applicationId: str,
         documents: Sequence[DeleteDocumentTypeDef],
         indexId: str,
         dataSourceSyncId: str = ...,
     ) -> BatchDeleteDocumentResponseTypeDef:
         """
         Asynchronously deletes one or more documents added using the `BatchPutDocument`
-        API from an Amazon Q
+        API from an Amazon Q Business
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.batch_delete_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#batch_delete_document)
         """
 
     def batch_put_document(
@@ -167,15 +170,15 @@
         applicationId: str,
         documents: Sequence[DocumentTypeDef],
         indexId: str,
         dataSourceSyncId: str = ...,
         roleArn: str = ...,
     ) -> BatchPutDocumentResponseTypeDef:
         """
-        Adds one or more documents to an Amazon Q index.
+        Adds one or more documents to an Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.batch_put_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#batch_put_document)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
@@ -185,26 +188,28 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#can_paginate)
         """
 
     def chat_sync(
         self,
         *,
         applicationId: str,
-        userId: str,
         actionExecution: ActionExecutionTypeDef = ...,
         attachments: Sequence[AttachmentInputTypeDef] = ...,
         attributeFilter: "AttributeFilterTypeDef" = ...,
+        chatMode: ChatModeType = ...,
+        chatModeConfiguration: ChatModeConfigurationTypeDef = ...,
         clientToken: str = ...,
         conversationId: str = ...,
         parentMessageId: str = ...,
         userGroups: Sequence[str] = ...,
+        userId: str = ...,
         userMessage: str = ...,
     ) -> ChatSyncOutputTypeDef:
         """
-        Starts or continues a non-streaming Amazon Q conversation.
+        Starts or continues a non-streaming Amazon Q Business conversation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.chat_sync)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#chat_sync)
         """
 
     def close(self) -> None:
         """
@@ -219,18 +224,19 @@
         *,
         displayName: str,
         roleArn: str,
         attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
         clientToken: str = ...,
         description: str = ...,
         encryptionConfiguration: EncryptionConfigurationTypeDef = ...,
+        identityCenterInstanceArn: str = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
-        Creates an Amazon Q application.
+        Creates an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_application)
         """
 
     def create_data_source(
         self,
@@ -244,15 +250,15 @@
         documentEnrichmentConfiguration: DocumentEnrichmentConfigurationTypeDef = ...,
         roleArn: str = ...,
         syncSchedule: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
-        Creates a data source connector for an Amazon Q application.
+        Creates a data source connector for an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_data_source)
         """
 
     def create_index(
         self,
@@ -261,15 +267,15 @@
         displayName: str,
         capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
         clientToken: str = ...,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIndexResponseTypeDef:
         """
-        Creates an Amazon Q index.
+        Creates an Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_index)
         """
 
     def create_plugin(
         self,
@@ -279,15 +285,15 @@
         displayName: str,
         serverUrl: str,
         type: PluginTypeType,
         clientToken: str = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePluginResponseTypeDef:
         """
-        Creates an Amazon Q plugin.
+        Creates an Amazon Q Business plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_plugin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_plugin)
         """
 
     def create_retriever(
         self,
@@ -297,15 +303,15 @@
         displayName: str,
         type: RetrieverTypeType,
         clientToken: str = ...,
         roleArn: str = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRetrieverResponseTypeDef:
         """
-        Adds a retriever to your Amazon Q application.
+        Adds a retriever to your Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_retriever)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_retriever)
         """
 
     def create_user(
         self,
@@ -325,58 +331,59 @@
         """
 
     def create_web_experience(
         self,
         *,
         applicationId: str,
         clientToken: str = ...,
+        roleArn: str = ...,
         samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
         subtitle: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         title: str = ...,
         welcomeMessage: str = ...,
     ) -> CreateWebExperienceResponseTypeDef:
         """
-        Creates an Amazon Q web experience.
+        Creates an Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_web_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_web_experience)
         """
 
     def delete_application(self, *, applicationId: str) -> Dict[str, Any]:
         """
-        Deletes an Amazon Q application.
+        Deletes an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_application)
         """
 
     def delete_chat_controls_configuration(self, *, applicationId: str) -> Dict[str, Any]:
         """
-        Deletes chat controls configured for an existing Amazon Q application.
+        Deletes chat controls configured for an existing Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_chat_controls_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_chat_controls_configuration)
         """
 
     def delete_conversation(
-        self, *, applicationId: str, conversationId: str, userId: str
+        self, *, applicationId: str, conversationId: str, userId: str = ...
     ) -> Dict[str, Any]:
         """
-        Deletes an Amazon Q web experience conversation.
+        Deletes an Amazon Q Business web experience conversation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_conversation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_conversation)
         """
 
     def delete_data_source(
         self, *, applicationId: str, dataSourceId: str, indexId: str
     ) -> Dict[str, Any]:
         """
-        Deletes an Amazon Q data source connector.
+        Deletes an Amazon Q Business data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_data_source)
         """
 
     def delete_group(
         self, *, applicationId: str, groupName: str, indexId: str, dataSourceId: str = ...
@@ -388,31 +395,31 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_group)
         """
 
     def delete_index(self, *, applicationId: str, indexId: str) -> Dict[str, Any]:
         """
-        Deletes an Amazon Q index.
+        Deletes an Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_index)
         """
 
     def delete_plugin(self, *, applicationId: str, pluginId: str) -> Dict[str, Any]:
         """
-        Deletes an Amazon Q plugin.
+        Deletes an Amazon Q Business plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_plugin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_plugin)
         """
 
     def delete_retriever(self, *, applicationId: str, retrieverId: str) -> Dict[str, Any]:
         """
-        Deletes the retriever used by an Amazon Q application.
+        Deletes the retriever used by an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_retriever)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_retriever)
         """
 
     def delete_user(self, *, applicationId: str, userId: str) -> Dict[str, Any]:
         """
@@ -420,15 +427,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_user)
         """
 
     def delete_web_experience(self, *, applicationId: str, webExperienceId: str) -> Dict[str, Any]:
         """
-        Deletes an Amazon Q web experience.
+        Deletes an Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_web_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_web_experience)
         """
 
     def generate_presigned_url(
         self,
@@ -442,36 +449,37 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#generate_presigned_url)
         """
 
     def get_application(self, *, applicationId: str) -> GetApplicationResponseTypeDef:
         """
-        Gets information about an existing Amazon Q application.
+        Gets information about an existing Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_application)
         """
 
     def get_chat_controls_configuration(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> GetChatControlsConfigurationResponseTypeDef:
         """
         Gets information about an chat controls configured for an existing Amazon Q
+        Business
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_chat_controls_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_chat_controls_configuration)
         """
 
     def get_data_source(
         self, *, applicationId: str, dataSourceId: str, indexId: str
     ) -> GetDataSourceResponseTypeDef:
         """
-        Gets information about an existing Amazon Q data source connector.
+        Gets information about an existing Amazon Q Business data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_data_source)
         """
 
     def get_group(
         self, *, applicationId: str, groupName: str, indexId: str, dataSourceId: str = ...
@@ -481,31 +489,32 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_group)
         """
 
     def get_index(self, *, applicationId: str, indexId: str) -> GetIndexResponseTypeDef:
         """
-        Gets information about an existing Amazon Q index.
+        Gets information about an existing Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_index)
         """
 
     def get_plugin(self, *, applicationId: str, pluginId: str) -> GetPluginResponseTypeDef:
         """
-        Gets information about an existing Amazon Q plugin.
+        Gets information about an existing Amazon Q Business plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_plugin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_plugin)
         """
 
     def get_retriever(self, *, applicationId: str, retrieverId: str) -> GetRetrieverResponseTypeDef:
         """
-        Gets information about an existing retriever used by an Amazon Q application.
+        Gets information about an existing retriever used by an Amazon Q Business
+        application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_retriever)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_retriever)
         """
 
     def get_user(self, *, applicationId: str, userId: str) -> GetUserResponseTypeDef:
         """
@@ -517,35 +526,35 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_user)
         """
 
     def get_web_experience(
         self, *, applicationId: str, webExperienceId: str
     ) -> GetWebExperienceResponseTypeDef:
         """
-        Gets information about an existing Amazon Q web experience.
+        Gets information about an existing Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_web_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_web_experience)
         """
 
     def list_applications(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListApplicationsResponseTypeDef:
         """
-        Lists Amazon Q applications.
+        Lists Amazon Q Business applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_applications)
         """
 
     def list_conversations(
-        self, *, applicationId: str, userId: str, maxResults: int = ..., nextToken: str = ...
+        self, *, applicationId: str, maxResults: int = ..., nextToken: str = ..., userId: str = ...
     ) -> ListConversationsResponseTypeDef:
         """
-        Lists one or more Amazon Q conversations.
+        Lists one or more Amazon Q Business conversations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_conversations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_conversations)
         """
 
     def list_data_source_sync_jobs(
         self,
@@ -556,25 +565,26 @@
         endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         startTime: TimestampTypeDef = ...,
         statusFilter: DataSourceSyncJobStatusType = ...,
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
-        Get information about an Amazon Q data source connector synchronization.
+        Get information about an Amazon Q Business data source connector
+        synchronization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_data_source_sync_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_data_source_sync_jobs)
         """
 
     def list_data_sources(
         self, *, applicationId: str, indexId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListDataSourcesResponseTypeDef:
         """
-        Lists the Amazon Q data source connectors that you have created.
+        Lists the Amazon Q Business data source connectors that you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_data_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_data_sources)
         """
 
     def list_documents(
         self,
@@ -609,51 +619,51 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_groups)
         """
 
     def list_indices(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListIndicesResponseTypeDef:
         """
-        Lists the Amazon Q indices you have created.
+        Lists the Amazon Q Business indices you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_indices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_indices)
         """
 
     def list_messages(
         self,
         *,
         applicationId: str,
         conversationId: str,
-        userId: str,
         maxResults: int = ...,
         nextToken: str = ...,
+        userId: str = ...,
     ) -> ListMessagesResponseTypeDef:
         """
-        Gets a list of messages associated with an Amazon Q web experience.
+        Gets a list of messages associated with an Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_messages)
         """
 
     def list_plugins(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListPluginsResponseTypeDef:
         """
-        Lists configured Amazon Q plugins.
+        Lists configured Amazon Q Business plugins.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_plugins)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_plugins)
         """
 
     def list_retrievers(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListRetrieversResponseTypeDef:
         """
-        Lists the retriever used by an Amazon Q application.
+        Lists the retriever used by an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_retrievers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_retrievers)
         """
 
     def list_tags_for_resource(self, *, resourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
@@ -663,32 +673,33 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_tags_for_resource)
         """
 
     def list_web_experiences(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListWebExperiencesResponseTypeDef:
         """
-        Lists one or more Amazon Q Web Experiences.
+        Lists one or more Amazon Q Business Web Experiences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_web_experiences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_web_experiences)
         """
 
     def put_feedback(
         self,
         *,
         applicationId: str,
         conversationId: str,
         messageId: str,
-        userId: str,
         messageCopiedAt: TimestampTypeDef = ...,
         messageUsefulness: MessageUsefulnessFeedbackTypeDef = ...,
+        userId: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Enables your end user to to provide feedback on their Amazon Q generated chat
+        Enables your end user to provide feedback on their Amazon Q Business generated
+        chat
         responses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.put_feedback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#put_feedback)
         """
 
     def put_group(
@@ -718,32 +729,34 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#start_data_source_sync_job)
         """
 
     def stop_data_source_sync_job(
         self, *, applicationId: str, dataSourceId: str, indexId: str
     ) -> Dict[str, Any]:
         """
-        Stops an Amazon Q data source connector synchronization job already in progress.
+        Stops an Amazon Q Business data source connector synchronization job already in
+        progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.stop_data_source_sync_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#stop_data_source_sync_job)
         """
 
     def tag_resource(self, *, resourceARN: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
-        Adds the specified tag to the specified Amazon Q application or data source
+        Adds the specified tag to the specified Amazon Q Business application or data
+        source
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#tag_resource)
         """
 
     def untag_resource(self, *, resourceARN: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes a tag from an Amazon Q application or a data source.
+        Removes a tag from an Amazon Q Business application or a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#untag_resource)
         """
 
     def update_application(
         self,
@@ -751,32 +764,34 @@
         applicationId: str,
         attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
         description: str = ...,
         displayName: str = ...,
         roleArn: str = ...,
     ) -> Dict[str, Any]:
         """
-        Updates an existing Amazon Q application.
+        Updates an existing Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_application)
         """
 
     def update_chat_controls_configuration(
         self,
         *,
         applicationId: str,
         blockedPhrasesConfigurationUpdate: BlockedPhrasesConfigurationUpdateTypeDef = ...,
         clientToken: str = ...,
+        creatorModeConfiguration: CreatorModeConfigurationTypeDef = ...,
         responseScope: ResponseScopeType = ...,
         topicConfigurationsToCreateOrUpdate: Sequence[TopicConfigurationTypeDef] = ...,
         topicConfigurationsToDelete: Sequence[TopicConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
-        Updates an set of chat controls configured for an existing Amazon Q application.
+        Updates an set of chat controls configured for an existing Amazon Q Business
+        application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_chat_controls_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_chat_controls_configuration)
         """
 
     def update_data_source(
         self,
@@ -789,15 +804,15 @@
         displayName: str = ...,
         documentEnrichmentConfiguration: DocumentEnrichmentConfigurationTypeDef = ...,
         roleArn: str = ...,
         syncSchedule: str = ...,
         vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
-        Updates an existing Amazon Q data source connector.
+        Updates an existing Amazon Q Business data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_data_source)
         """
 
     def update_index(
         self,
@@ -806,15 +821,15 @@
         indexId: str,
         capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
         description: str = ...,
         displayName: str = ...,
         documentAttributeConfigurations: Sequence[DocumentAttributeConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
-        Updates an Amazon Q index.
+        Updates an Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_index)
         """
 
     def update_plugin(
         self,
@@ -823,15 +838,15 @@
         pluginId: str,
         authConfiguration: PluginAuthConfigurationTypeDef = ...,
         displayName: str = ...,
         serverUrl: str = ...,
         state: PluginStateType = ...,
     ) -> Dict[str, Any]:
         """
-        Updates an Amazon Q plugin.
+        Updates an Amazon Q Business plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_plugin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_plugin)
         """
 
     def update_retriever(
         self,
@@ -839,15 +854,15 @@
         applicationId: str,
         retrieverId: str,
         configuration: RetrieverConfigurationTypeDef = ...,
         displayName: str = ...,
         roleArn: str = ...,
     ) -> Dict[str, Any]:
         """
-        Updates the retriever used for your Amazon Q application.
+        Updates the retriever used for your Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_retriever)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_retriever)
         """
 
     def update_user(
         self,
@@ -872,15 +887,15 @@
         authenticationConfiguration: WebExperienceAuthConfigurationTypeDef = ...,
         samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
         subtitle: str = ...,
         title: str = ...,
         welcomeMessage: str = ...,
     ) -> Dict[str, Any]:
         """
-        Updates an Amazon Q web experience.
+        Updates an Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_web_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_web_experience)
         """
 
     @overload
     def get_paginator(
```

### Comparing `mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/client.pyi` & `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    ChatModeType,
     DataSourceSyncJobStatusType,
     MembershipTypeType,
     PluginStateType,
     PluginTypeType,
     ResponseScopeType,
     RetrieverTypeType,
     WebExperienceSamplePromptsControlModeType,
@@ -46,21 +47,23 @@
     ActionExecutionTypeDef,
     AttachmentInputTypeDef,
     AttachmentsConfigurationTypeDef,
     AttributeFilterTypeDef,
     BatchDeleteDocumentResponseTypeDef,
     BatchPutDocumentResponseTypeDef,
     BlockedPhrasesConfigurationUpdateTypeDef,
+    ChatModeConfigurationTypeDef,
     ChatSyncOutputTypeDef,
     CreateApplicationResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreatePluginResponseTypeDef,
     CreateRetrieverResponseTypeDef,
     CreateWebExperienceResponseTypeDef,
+    CreatorModeConfigurationTypeDef,
     DataSourceVpcConfigurationTypeDef,
     DeleteDocumentTypeDef,
     DocumentAttributeConfigurationTypeDef,
     DocumentEnrichmentConfigurationTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionConfigurationTypeDef,
@@ -147,15 +150,15 @@
         applicationId: str,
         documents: Sequence[DeleteDocumentTypeDef],
         indexId: str,
         dataSourceSyncId: str = ...,
     ) -> BatchDeleteDocumentResponseTypeDef:
         """
         Asynchronously deletes one or more documents added using the `BatchPutDocument`
-        API from an Amazon Q
+        API from an Amazon Q Business
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.batch_delete_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#batch_delete_document)
         """
 
     def batch_put_document(
@@ -164,15 +167,15 @@
         applicationId: str,
         documents: Sequence[DocumentTypeDef],
         indexId: str,
         dataSourceSyncId: str = ...,
         roleArn: str = ...,
     ) -> BatchPutDocumentResponseTypeDef:
         """
-        Adds one or more documents to an Amazon Q index.
+        Adds one or more documents to an Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.batch_put_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#batch_put_document)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
@@ -182,26 +185,28 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#can_paginate)
         """
 
     def chat_sync(
         self,
         *,
         applicationId: str,
-        userId: str,
         actionExecution: ActionExecutionTypeDef = ...,
         attachments: Sequence[AttachmentInputTypeDef] = ...,
         attributeFilter: "AttributeFilterTypeDef" = ...,
+        chatMode: ChatModeType = ...,
+        chatModeConfiguration: ChatModeConfigurationTypeDef = ...,
         clientToken: str = ...,
         conversationId: str = ...,
         parentMessageId: str = ...,
         userGroups: Sequence[str] = ...,
+        userId: str = ...,
         userMessage: str = ...,
     ) -> ChatSyncOutputTypeDef:
         """
-        Starts or continues a non-streaming Amazon Q conversation.
+        Starts or continues a non-streaming Amazon Q Business conversation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.chat_sync)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#chat_sync)
         """
 
     def close(self) -> None:
         """
@@ -216,18 +221,19 @@
         *,
         displayName: str,
         roleArn: str,
         attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
         clientToken: str = ...,
         description: str = ...,
         encryptionConfiguration: EncryptionConfigurationTypeDef = ...,
+        identityCenterInstanceArn: str = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
-        Creates an Amazon Q application.
+        Creates an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_application)
         """
 
     def create_data_source(
         self,
@@ -241,15 +247,15 @@
         documentEnrichmentConfiguration: DocumentEnrichmentConfigurationTypeDef = ...,
         roleArn: str = ...,
         syncSchedule: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
-        Creates a data source connector for an Amazon Q application.
+        Creates a data source connector for an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_data_source)
         """
 
     def create_index(
         self,
@@ -258,15 +264,15 @@
         displayName: str,
         capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
         clientToken: str = ...,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIndexResponseTypeDef:
         """
-        Creates an Amazon Q index.
+        Creates an Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_index)
         """
 
     def create_plugin(
         self,
@@ -276,15 +282,15 @@
         displayName: str,
         serverUrl: str,
         type: PluginTypeType,
         clientToken: str = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePluginResponseTypeDef:
         """
-        Creates an Amazon Q plugin.
+        Creates an Amazon Q Business plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_plugin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_plugin)
         """
 
     def create_retriever(
         self,
@@ -294,15 +300,15 @@
         displayName: str,
         type: RetrieverTypeType,
         clientToken: str = ...,
         roleArn: str = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRetrieverResponseTypeDef:
         """
-        Adds a retriever to your Amazon Q application.
+        Adds a retriever to your Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_retriever)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_retriever)
         """
 
     def create_user(
         self,
@@ -322,58 +328,59 @@
         """
 
     def create_web_experience(
         self,
         *,
         applicationId: str,
         clientToken: str = ...,
+        roleArn: str = ...,
         samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
         subtitle: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         title: str = ...,
         welcomeMessage: str = ...,
     ) -> CreateWebExperienceResponseTypeDef:
         """
-        Creates an Amazon Q web experience.
+        Creates an Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_web_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_web_experience)
         """
 
     def delete_application(self, *, applicationId: str) -> Dict[str, Any]:
         """
-        Deletes an Amazon Q application.
+        Deletes an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_application)
         """
 
     def delete_chat_controls_configuration(self, *, applicationId: str) -> Dict[str, Any]:
         """
-        Deletes chat controls configured for an existing Amazon Q application.
+        Deletes chat controls configured for an existing Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_chat_controls_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_chat_controls_configuration)
         """
 
     def delete_conversation(
-        self, *, applicationId: str, conversationId: str, userId: str
+        self, *, applicationId: str, conversationId: str, userId: str = ...
     ) -> Dict[str, Any]:
         """
-        Deletes an Amazon Q web experience conversation.
+        Deletes an Amazon Q Business web experience conversation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_conversation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_conversation)
         """
 
     def delete_data_source(
         self, *, applicationId: str, dataSourceId: str, indexId: str
     ) -> Dict[str, Any]:
         """
-        Deletes an Amazon Q data source connector.
+        Deletes an Amazon Q Business data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_data_source)
         """
 
     def delete_group(
         self, *, applicationId: str, groupName: str, indexId: str, dataSourceId: str = ...
@@ -385,31 +392,31 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_group)
         """
 
     def delete_index(self, *, applicationId: str, indexId: str) -> Dict[str, Any]:
         """
-        Deletes an Amazon Q index.
+        Deletes an Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_index)
         """
 
     def delete_plugin(self, *, applicationId: str, pluginId: str) -> Dict[str, Any]:
         """
-        Deletes an Amazon Q plugin.
+        Deletes an Amazon Q Business plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_plugin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_plugin)
         """
 
     def delete_retriever(self, *, applicationId: str, retrieverId: str) -> Dict[str, Any]:
         """
-        Deletes the retriever used by an Amazon Q application.
+        Deletes the retriever used by an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_retriever)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_retriever)
         """
 
     def delete_user(self, *, applicationId: str, userId: str) -> Dict[str, Any]:
         """
@@ -417,15 +424,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_user)
         """
 
     def delete_web_experience(self, *, applicationId: str, webExperienceId: str) -> Dict[str, Any]:
         """
-        Deletes an Amazon Q web experience.
+        Deletes an Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_web_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_web_experience)
         """
 
     def generate_presigned_url(
         self,
@@ -439,36 +446,37 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#generate_presigned_url)
         """
 
     def get_application(self, *, applicationId: str) -> GetApplicationResponseTypeDef:
         """
-        Gets information about an existing Amazon Q application.
+        Gets information about an existing Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_application)
         """
 
     def get_chat_controls_configuration(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> GetChatControlsConfigurationResponseTypeDef:
         """
         Gets information about an chat controls configured for an existing Amazon Q
+        Business
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_chat_controls_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_chat_controls_configuration)
         """
 
     def get_data_source(
         self, *, applicationId: str, dataSourceId: str, indexId: str
     ) -> GetDataSourceResponseTypeDef:
         """
-        Gets information about an existing Amazon Q data source connector.
+        Gets information about an existing Amazon Q Business data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_data_source)
         """
 
     def get_group(
         self, *, applicationId: str, groupName: str, indexId: str, dataSourceId: str = ...
@@ -478,31 +486,32 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_group)
         """
 
     def get_index(self, *, applicationId: str, indexId: str) -> GetIndexResponseTypeDef:
         """
-        Gets information about an existing Amazon Q index.
+        Gets information about an existing Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_index)
         """
 
     def get_plugin(self, *, applicationId: str, pluginId: str) -> GetPluginResponseTypeDef:
         """
-        Gets information about an existing Amazon Q plugin.
+        Gets information about an existing Amazon Q Business plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_plugin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_plugin)
         """
 
     def get_retriever(self, *, applicationId: str, retrieverId: str) -> GetRetrieverResponseTypeDef:
         """
-        Gets information about an existing retriever used by an Amazon Q application.
+        Gets information about an existing retriever used by an Amazon Q Business
+        application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_retriever)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_retriever)
         """
 
     def get_user(self, *, applicationId: str, userId: str) -> GetUserResponseTypeDef:
         """
@@ -514,35 +523,35 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_user)
         """
 
     def get_web_experience(
         self, *, applicationId: str, webExperienceId: str
     ) -> GetWebExperienceResponseTypeDef:
         """
-        Gets information about an existing Amazon Q web experience.
+        Gets information about an existing Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_web_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_web_experience)
         """
 
     def list_applications(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListApplicationsResponseTypeDef:
         """
-        Lists Amazon Q applications.
+        Lists Amazon Q Business applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_applications)
         """
 
     def list_conversations(
-        self, *, applicationId: str, userId: str, maxResults: int = ..., nextToken: str = ...
+        self, *, applicationId: str, maxResults: int = ..., nextToken: str = ..., userId: str = ...
     ) -> ListConversationsResponseTypeDef:
         """
-        Lists one or more Amazon Q conversations.
+        Lists one or more Amazon Q Business conversations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_conversations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_conversations)
         """
 
     def list_data_source_sync_jobs(
         self,
@@ -553,25 +562,26 @@
         endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         startTime: TimestampTypeDef = ...,
         statusFilter: DataSourceSyncJobStatusType = ...,
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
-        Get information about an Amazon Q data source connector synchronization.
+        Get information about an Amazon Q Business data source connector
+        synchronization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_data_source_sync_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_data_source_sync_jobs)
         """
 
     def list_data_sources(
         self, *, applicationId: str, indexId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListDataSourcesResponseTypeDef:
         """
-        Lists the Amazon Q data source connectors that you have created.
+        Lists the Amazon Q Business data source connectors that you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_data_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_data_sources)
         """
 
     def list_documents(
         self,
@@ -606,51 +616,51 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_groups)
         """
 
     def list_indices(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListIndicesResponseTypeDef:
         """
-        Lists the Amazon Q indices you have created.
+        Lists the Amazon Q Business indices you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_indices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_indices)
         """
 
     def list_messages(
         self,
         *,
         applicationId: str,
         conversationId: str,
-        userId: str,
         maxResults: int = ...,
         nextToken: str = ...,
+        userId: str = ...,
     ) -> ListMessagesResponseTypeDef:
         """
-        Gets a list of messages associated with an Amazon Q web experience.
+        Gets a list of messages associated with an Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_messages)
         """
 
     def list_plugins(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListPluginsResponseTypeDef:
         """
-        Lists configured Amazon Q plugins.
+        Lists configured Amazon Q Business plugins.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_plugins)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_plugins)
         """
 
     def list_retrievers(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListRetrieversResponseTypeDef:
         """
-        Lists the retriever used by an Amazon Q application.
+        Lists the retriever used by an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_retrievers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_retrievers)
         """
 
     def list_tags_for_resource(self, *, resourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
@@ -660,32 +670,33 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_tags_for_resource)
         """
 
     def list_web_experiences(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListWebExperiencesResponseTypeDef:
         """
-        Lists one or more Amazon Q Web Experiences.
+        Lists one or more Amazon Q Business Web Experiences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_web_experiences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_web_experiences)
         """
 
     def put_feedback(
         self,
         *,
         applicationId: str,
         conversationId: str,
         messageId: str,
-        userId: str,
         messageCopiedAt: TimestampTypeDef = ...,
         messageUsefulness: MessageUsefulnessFeedbackTypeDef = ...,
+        userId: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Enables your end user to to provide feedback on their Amazon Q generated chat
+        Enables your end user to provide feedback on their Amazon Q Business generated
+        chat
         responses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.put_feedback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#put_feedback)
         """
 
     def put_group(
@@ -715,32 +726,34 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#start_data_source_sync_job)
         """
 
     def stop_data_source_sync_job(
         self, *, applicationId: str, dataSourceId: str, indexId: str
     ) -> Dict[str, Any]:
         """
-        Stops an Amazon Q data source connector synchronization job already in progress.
+        Stops an Amazon Q Business data source connector synchronization job already in
+        progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.stop_data_source_sync_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#stop_data_source_sync_job)
         """
 
     def tag_resource(self, *, resourceARN: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
-        Adds the specified tag to the specified Amazon Q application or data source
+        Adds the specified tag to the specified Amazon Q Business application or data
+        source
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#tag_resource)
         """
 
     def untag_resource(self, *, resourceARN: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes a tag from an Amazon Q application or a data source.
+        Removes a tag from an Amazon Q Business application or a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#untag_resource)
         """
 
     def update_application(
         self,
@@ -748,32 +761,34 @@
         applicationId: str,
         attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
         description: str = ...,
         displayName: str = ...,
         roleArn: str = ...,
     ) -> Dict[str, Any]:
         """
-        Updates an existing Amazon Q application.
+        Updates an existing Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_application)
         """
 
     def update_chat_controls_configuration(
         self,
         *,
         applicationId: str,
         blockedPhrasesConfigurationUpdate: BlockedPhrasesConfigurationUpdateTypeDef = ...,
         clientToken: str = ...,
+        creatorModeConfiguration: CreatorModeConfigurationTypeDef = ...,
         responseScope: ResponseScopeType = ...,
         topicConfigurationsToCreateOrUpdate: Sequence[TopicConfigurationTypeDef] = ...,
         topicConfigurationsToDelete: Sequence[TopicConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
-        Updates an set of chat controls configured for an existing Amazon Q application.
+        Updates an set of chat controls configured for an existing Amazon Q Business
+        application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_chat_controls_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_chat_controls_configuration)
         """
 
     def update_data_source(
         self,
@@ -786,15 +801,15 @@
         displayName: str = ...,
         documentEnrichmentConfiguration: DocumentEnrichmentConfigurationTypeDef = ...,
         roleArn: str = ...,
         syncSchedule: str = ...,
         vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
-        Updates an existing Amazon Q data source connector.
+        Updates an existing Amazon Q Business data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_data_source)
         """
 
     def update_index(
         self,
@@ -803,15 +818,15 @@
         indexId: str,
         capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
         description: str = ...,
         displayName: str = ...,
         documentAttributeConfigurations: Sequence[DocumentAttributeConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
-        Updates an Amazon Q index.
+        Updates an Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_index)
         """
 
     def update_plugin(
         self,
@@ -820,15 +835,15 @@
         pluginId: str,
         authConfiguration: PluginAuthConfigurationTypeDef = ...,
         displayName: str = ...,
         serverUrl: str = ...,
         state: PluginStateType = ...,
     ) -> Dict[str, Any]:
         """
-        Updates an Amazon Q plugin.
+        Updates an Amazon Q Business plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_plugin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_plugin)
         """
 
     def update_retriever(
         self,
@@ -836,15 +851,15 @@
         applicationId: str,
         retrieverId: str,
         configuration: RetrieverConfigurationTypeDef = ...,
         displayName: str = ...,
         roleArn: str = ...,
     ) -> Dict[str, Any]:
         """
-        Updates the retriever used for your Amazon Q application.
+        Updates the retriever used for your Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_retriever)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_retriever)
         """
 
     def update_user(
         self,
@@ -869,15 +884,15 @@
         authenticationConfiguration: WebExperienceAuthConfigurationTypeDef = ...,
         samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
         subtitle: str = ...,
         title: str = ...,
         welcomeMessage: str = ...,
     ) -> Dict[str, Any]:
         """
-        Updates an Amazon Q web experience.
+        Updates an Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_web_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_web_experience)
         """
 
     @overload
     def get_paginator(
```

### Comparing `mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/literals.py` & `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 __all__ = (
     "ActionPayloadFieldTypeType",
     "ApplicationStatusType",
     "AttachmentStatusType",
     "AttachmentsControlModeType",
     "AttributeTypeType",
     "AttributeValueOperatorType",
+    "ChatModeType",
     "ContentTypeType",
+    "CreatorModeControlType",
     "DataSourceStatusType",
     "DataSourceSyncJobStatusType",
     "DocumentAttributeBoostingLevelType",
     "DocumentContentOperatorType",
     "DocumentEnrichmentConditionOperatorType",
     "DocumentStatusType",
     "ErrorCodeType",
@@ -74,28 +76,30 @@
 
 ActionPayloadFieldTypeType = Literal["ARRAY", "BOOLEAN", "NUMBER", "STRING"]
 ApplicationStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
 AttachmentStatusType = Literal["FAILED", "SUCCEEDED"]
 AttachmentsControlModeType = Literal["DISABLED", "ENABLED"]
 AttributeTypeType = Literal["DATE", "NUMBER", "STRING", "STRING_LIST"]
 AttributeValueOperatorType = Literal["DELETE"]
+ChatModeType = Literal["CREATOR_MODE", "PLUGIN_MODE", "RETRIEVAL_MODE"]
 ContentTypeType = Literal[
     "CSV",
     "HTML",
     "JSON",
     "MD",
     "MS_EXCEL",
     "MS_WORD",
     "PDF",
     "PLAIN_TEXT",
     "PPT",
     "RTF",
     "XML",
     "XSLT",
 ]
+CreatorModeControlType = Literal["DISABLED", "ENABLED"]
 DataSourceStatusType = Literal[
     "ACTIVE", "CREATING", "DELETING", "FAILED", "PENDING_CREATION", "UPDATING"
 ]
 DataSourceSyncJobStatusType = Literal[
     "ABORTED", "FAILED", "INCOMPLETE", "STOPPING", "SUCCEEDED", "SYNCING", "SYNCING_INDEXING"
 ]
 DocumentAttributeBoostingLevelType = Literal["HIGH", "LOW", "MEDIUM", "NONE", "VERY_HIGH"]
@@ -191,14 +195,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -209,14 +214,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -234,14 +240,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -254,24 +261,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -332,15 +341,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -520,14 +528,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/literals.pyi` & `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 __all__ = (
     "ActionPayloadFieldTypeType",
     "ApplicationStatusType",
     "AttachmentStatusType",
     "AttachmentsControlModeType",
     "AttributeTypeType",
     "AttributeValueOperatorType",
+    "ChatModeType",
     "ContentTypeType",
+    "CreatorModeControlType",
     "DataSourceStatusType",
     "DataSourceSyncJobStatusType",
     "DocumentAttributeBoostingLevelType",
     "DocumentContentOperatorType",
     "DocumentEnrichmentConditionOperatorType",
     "DocumentStatusType",
     "ErrorCodeType",
@@ -74,28 +76,30 @@
 
 ActionPayloadFieldTypeType = Literal["ARRAY", "BOOLEAN", "NUMBER", "STRING"]
 ApplicationStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
 AttachmentStatusType = Literal["FAILED", "SUCCEEDED"]
 AttachmentsControlModeType = Literal["DISABLED", "ENABLED"]
 AttributeTypeType = Literal["DATE", "NUMBER", "STRING", "STRING_LIST"]
 AttributeValueOperatorType = Literal["DELETE"]
+ChatModeType = Literal["CREATOR_MODE", "PLUGIN_MODE", "RETRIEVAL_MODE"]
 ContentTypeType = Literal[
     "CSV",
     "HTML",
     "JSON",
     "MD",
     "MS_EXCEL",
     "MS_WORD",
     "PDF",
     "PLAIN_TEXT",
     "PPT",
     "RTF",
     "XML",
     "XSLT",
 ]
+CreatorModeControlType = Literal["DISABLED", "ENABLED"]
 DataSourceStatusType = Literal[
     "ACTIVE", "CREATING", "DELETING", "FAILED", "PENDING_CREATION", "UPDATING"
 ]
 DataSourceSyncJobStatusType = Literal[
     "ABORTED", "FAILED", "INCOMPLETE", "STOPPING", "SUCCEEDED", "SYNCING", "SYNCING_INDEXING"
 ]
 DocumentAttributeBoostingLevelType = Literal["HIGH", "LOW", "MEDIUM", "NONE", "VERY_HIGH"]
@@ -191,14 +195,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -209,14 +214,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -234,14 +240,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -254,24 +261,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -332,15 +341,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -520,14 +528,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/paginator.py` & `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,19 @@
 class ListConversationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListConversations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/paginators/#listconversationspaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, userId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        applicationId: str,
+        userId: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListConversationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListConversations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/paginators/#listconversationspaginator)
         """
 
 
@@ -235,15 +239,15 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         conversationId: str,
-        userId: str,
+        userId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListMessagesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListMessages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/paginators/#listmessagespaginator)
         """
```

### Comparing `mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/paginator.pyi` & `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,19 @@
 class ListConversationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListConversations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/paginators/#listconversationspaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, userId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        applicationId: str,
+        userId: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListConversationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListConversations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/paginators/#listconversationspaginator)
         """
 
 class ListDataSourceSyncJobsPaginator(Paginator):
@@ -225,15 +229,15 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         conversationId: str,
-        userId: str,
+        userId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListMessagesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListMessages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/paginators/#listmessagespaginator)
         """
```

### Comparing `mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/type_defs.py` & `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
 from .literals import (
     ActionPayloadFieldTypeType,
     ApplicationStatusType,
     AttachmentsControlModeType,
     AttachmentStatusType,
     AttributeTypeType,
+    ChatModeType,
     ContentTypeType,
+    CreatorModeControlType,
     DataSourceStatusType,
     DataSourceSyncJobStatusType,
     DocumentAttributeBoostingLevelType,
     DocumentEnrichmentConditionOperatorType,
     DocumentStatusType,
     ErrorCodeType,
     GroupStatusType,
@@ -67,30 +69,33 @@
 
 __all__ = (
     "ActionExecutionPayloadFieldPaginatorTypeDef",
     "ActionExecutionPayloadFieldTypeDef",
     "ActionReviewPayloadFieldAllowedValueTypeDef",
     "ApplicationTypeDef",
     "AppliedAttachmentsConfigurationTypeDef",
+    "AppliedCreatorModeConfigurationTypeDef",
     "BlobTypeDef",
     "ErrorDetailTypeDef",
     "AttachmentsConfigurationTypeDef",
     "BasicAuthConfigurationTypeDef",
     "DeleteDocumentTypeDef",
     "ResponseMetadataTypeDef",
     "BlockedPhrasesConfigurationTypeDef",
     "BlockedPhrasesConfigurationUpdateTypeDef",
+    "PluginConfigurationTypeDef",
     "ContentBlockerRuleTypeDef",
     "EligibleDataSourceTypeDef",
     "ConversationTypeDef",
     "EncryptionConfigurationTypeDef",
     "TagTypeDef",
     "DataSourceVpcConfigurationTypeDef",
     "IndexCapacityConfigurationTypeDef",
     "UserAliasTypeDef",
+    "CreatorModeConfigurationTypeDef",
     "DataSourceSyncJobMetricsTypeDef",
     "DataSourceTypeDef",
     "DateAttributeBoostingConfigurationTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteChatControlsConfigurationRequestRequestTypeDef",
     "DeleteConversationRequestRequestTypeDef",
     "DeleteDataSourceRequestRequestTypeDef",
@@ -159,14 +164,15 @@
     "CreateIndexResponseTypeDef",
     "CreatePluginResponseTypeDef",
     "CreateRetrieverResponseTypeDef",
     "CreateWebExperienceResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListApplicationsResponseTypeDef",
     "StartDataSourceSyncJobResponseTypeDef",
+    "ChatModeConfigurationTypeDef",
     "ContentRetrievalRuleTypeDef",
     "ListConversationsResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateWebExperienceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -204,19 +210,19 @@
     "ListRetrieversResponseTypeDef",
     "ListWebExperiencesResponseTypeDef",
     "PluginAuthConfigurationTypeDef",
     "PrincipalTypeDef",
     "WebExperienceAuthConfigurationTypeDef",
     "SourceAttributionTypeDef",
     "ActionReviewTypeDef",
-    "ChatSyncInputRequestTypeDef",
     "ListDocumentsResponseTypeDef",
     "BatchDeleteDocumentResponseTypeDef",
     "BatchPutDocumentResponseTypeDef",
     "GetGroupResponseTypeDef",
+    "ChatSyncInputRequestTypeDef",
     "RuleConfigurationTypeDef",
     "ListDataSourceSyncJobsResponseTypeDef",
     "NativeIndexConfigurationTypeDef",
     "DocumentAttributeConditionTypeDef",
     "DocumentAttributeTargetTypeDef",
     "DocumentAttributeTypeDef",
     "PutFeedbackRequestRequestTypeDef",
@@ -284,14 +290,20 @@
 )
 AppliedAttachmentsConfigurationTypeDef = TypedDict(
     "AppliedAttachmentsConfigurationTypeDef",
     {
         "attachmentsControlMode": NotRequired[AttachmentsControlModeType],
     },
 )
+AppliedCreatorModeConfigurationTypeDef = TypedDict(
+    "AppliedCreatorModeConfigurationTypeDef",
+    {
+        "creatorModeControl": CreatorModeControlType,
+    },
+)
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "errorCode": NotRequired[ErrorCodeType],
         "errorMessage": NotRequired[str],
     },
@@ -315,18 +327,18 @@
         "documentId": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 BlockedPhrasesConfigurationTypeDef = TypedDict(
     "BlockedPhrasesConfigurationTypeDef",
     {
         "blockedPhrases": NotRequired[List[str]],
         "systemMessageOverride": NotRequired[str],
@@ -336,14 +348,20 @@
     "BlockedPhrasesConfigurationUpdateTypeDef",
     {
         "blockedPhrasesToCreateOrUpdate": NotRequired[Sequence[str]],
         "blockedPhrasesToDelete": NotRequired[Sequence[str]],
         "systemMessageOverride": NotRequired[str],
     },
 )
+PluginConfigurationTypeDef = TypedDict(
+    "PluginConfigurationTypeDef",
+    {
+        "pluginId": str,
+    },
+)
 ContentBlockerRuleTypeDef = TypedDict(
     "ContentBlockerRuleTypeDef",
     {
         "systemMessageOverride": NotRequired[str],
     },
 )
 EligibleDataSourceTypeDef = TypedDict(
@@ -391,14 +409,20 @@
     "UserAliasTypeDef",
     {
         "userId": str,
         "dataSourceId": NotRequired[str],
         "indexId": NotRequired[str],
     },
 )
+CreatorModeConfigurationTypeDef = TypedDict(
+    "CreatorModeConfigurationTypeDef",
+    {
+        "creatorModeControl": CreatorModeControlType,
+    },
+)
 DataSourceSyncJobMetricsTypeDef = TypedDict(
     "DataSourceSyncJobMetricsTypeDef",
     {
         "documentsAdded": NotRequired[str],
         "documentsDeleted": NotRequired[str],
         "documentsFailed": NotRequired[str],
         "documentsModified": NotRequired[str],
@@ -436,15 +460,15 @@
     },
 )
 DeleteConversationRequestRequestTypeDef = TypedDict(
     "DeleteConversationRequestRequestTypeDef",
     {
         "applicationId": str,
         "conversationId": str,
-        "userId": str,
+        "userId": NotRequired[str],
     },
 )
 DeleteDataSourceRequestRequestTypeDef = TypedDict(
     "DeleteDataSourceRequestRequestTypeDef",
     {
         "applicationId": str,
         "dataSourceId": str,
@@ -655,17 +679,17 @@
         "nextToken": NotRequired[str],
     },
 )
 ListConversationsRequestRequestTypeDef = TypedDict(
     "ListConversationsRequestRequestTypeDef",
     {
         "applicationId": str,
-        "userId": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "userId": NotRequired[str],
     },
 )
 ListDataSourcesRequestRequestTypeDef = TypedDict(
     "ListDataSourcesRequestRequestTypeDef",
     {
         "applicationId": str,
         "indexId": str,
@@ -692,17 +716,17 @@
     },
 )
 ListMessagesRequestRequestTypeDef = TypedDict(
     "ListMessagesRequestRequestTypeDef",
     {
         "applicationId": str,
         "conversationId": str,
-        "userId": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "userId": NotRequired[str],
     },
 )
 ListPluginsRequestRequestTypeDef = TypedDict(
     "ListPluginsRequestRequestTypeDef",
     {
         "applicationId": str,
         "maxResults": NotRequired[int],
@@ -984,14 +1008,20 @@
 StartDataSourceSyncJobResponseTypeDef = TypedDict(
     "StartDataSourceSyncJobResponseTypeDef",
     {
         "executionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ChatModeConfigurationTypeDef = TypedDict(
+    "ChatModeConfigurationTypeDef",
+    {
+        "pluginConfiguration": NotRequired[PluginConfigurationTypeDef],
+    },
+)
 ContentRetrievalRuleTypeDef = TypedDict(
     "ContentRetrievalRuleTypeDef",
     {
         "eligibleDataSources": NotRequired[List[EligibleDataSourceTypeDef]],
     },
 )
 ListConversationsResponseTypeDef = TypedDict(
@@ -1009,14 +1039,15 @@
         "applicationId": str,
         "attachmentsConfiguration": AppliedAttachmentsConfigurationTypeDef,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "encryptionConfiguration": EncryptionConfigurationTypeDef,
         "error": ErrorDetailTypeDef,
+        "identityCenterApplicationArn": str,
         "roleArn": str,
         "status": ApplicationStatusType,
         "updatedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateApplicationRequestRequestTypeDef = TypedDict(
@@ -1024,22 +1055,24 @@
     {
         "displayName": str,
         "roleArn": str,
         "attachmentsConfiguration": NotRequired[AttachmentsConfigurationTypeDef],
         "clientToken": NotRequired[str],
         "description": NotRequired[str],
         "encryptionConfiguration": NotRequired[EncryptionConfigurationTypeDef],
+        "identityCenterInstanceArn": NotRequired[str],
         "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 CreateWebExperienceRequestRequestTypeDef = TypedDict(
     "CreateWebExperienceRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": NotRequired[str],
+        "roleArn": NotRequired[str],
         "samplePromptsControlMode": NotRequired[WebExperienceSamplePromptsControlModeType],
         "subtitle": NotRequired[str],
         "tags": NotRequired[Sequence[TagTypeDef]],
         "title": NotRequired[str],
         "welcomeMessage": NotRequired[str],
     },
 )
@@ -1206,15 +1239,15 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListConversationsRequestListConversationsPaginateTypeDef = TypedDict(
     "ListConversationsRequestListConversationsPaginateTypeDef",
     {
         "applicationId": str,
-        "userId": str,
+        "userId": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef = TypedDict(
     "ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef",
     {
         "applicationId": str,
@@ -1261,15 +1294,15 @@
     },
 )
 ListMessagesRequestListMessagesPaginateTypeDef = TypedDict(
     "ListMessagesRequestListMessagesPaginateTypeDef",
     {
         "applicationId": str,
         "conversationId": str,
-        "userId": str,
+        "userId": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListPluginsRequestListPluginsPaginateTypeDef = TypedDict(
     "ListPluginsRequestListPluginsPaginateTypeDef",
     {
         "applicationId": str,
@@ -1381,29 +1414,14 @@
     {
         "payload": NotRequired[Dict[str, ActionReviewPayloadFieldTypeDef]],
         "payloadFieldNameSeparator": NotRequired[str],
         "pluginId": NotRequired[str],
         "pluginType": NotRequired[PluginTypeType],
     },
 )
-ChatSyncInputRequestTypeDef = TypedDict(
-    "ChatSyncInputRequestTypeDef",
-    {
-        "applicationId": str,
-        "userId": str,
-        "actionExecution": NotRequired[ActionExecutionTypeDef],
-        "attachments": NotRequired[Sequence[AttachmentInputTypeDef]],
-        "attributeFilter": NotRequired["AttributeFilterTypeDef"],
-        "clientToken": NotRequired[str],
-        "conversationId": NotRequired[str],
-        "parentMessageId": NotRequired[str],
-        "userGroups": NotRequired[Sequence[str]],
-        "userMessage": NotRequired[str],
-    },
-)
 ListDocumentsResponseTypeDef = TypedDict(
     "ListDocumentsResponseTypeDef",
     {
         "documentDetailList": List[DocumentDetailsTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1426,14 +1444,31 @@
     "GetGroupResponseTypeDef",
     {
         "status": GroupStatusDetailTypeDef,
         "statusHistory": List[GroupStatusDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ChatSyncInputRequestTypeDef = TypedDict(
+    "ChatSyncInputRequestTypeDef",
+    {
+        "applicationId": str,
+        "actionExecution": NotRequired[ActionExecutionTypeDef],
+        "attachments": NotRequired[Sequence[AttachmentInputTypeDef]],
+        "attributeFilter": NotRequired["AttributeFilterTypeDef"],
+        "chatMode": NotRequired[ChatModeType],
+        "chatModeConfiguration": NotRequired[ChatModeConfigurationTypeDef],
+        "clientToken": NotRequired[str],
+        "conversationId": NotRequired[str],
+        "parentMessageId": NotRequired[str],
+        "userGroups": NotRequired[Sequence[str]],
+        "userId": NotRequired[str],
+        "userMessage": NotRequired[str],
+    },
+)
 RuleConfigurationTypeDef = TypedDict(
     "RuleConfigurationTypeDef",
     {
         "contentBlockerRule": NotRequired[ContentBlockerRuleTypeDef],
         "contentRetrievalRule": NotRequired[ContentRetrievalRuleTypeDef],
     },
 )
@@ -1479,17 +1514,17 @@
 )
 PutFeedbackRequestRequestTypeDef = TypedDict(
     "PutFeedbackRequestRequestTypeDef",
     {
         "applicationId": str,
         "conversationId": str,
         "messageId": str,
-        "userId": str,
         "messageCopiedAt": NotRequired[TimestampTypeDef],
         "messageUsefulness": NotRequired[MessageUsefulnessFeedbackTypeDef],
+        "userId": NotRequired[str],
     },
 )
 PutGroupRequestRequestTypeDef = TypedDict(
     "PutGroupRequestRequestTypeDef",
     {
         "applicationId": str,
         "groupMembers": GroupMembersTypeDef,
@@ -1567,14 +1602,15 @@
     "GetWebExperienceResponseTypeDef",
     {
         "applicationId": str,
         "authenticationConfiguration": WebExperienceAuthConfigurationTypeDef,
         "createdAt": datetime,
         "defaultEndpoint": str,
         "error": ErrorDetailTypeDef,
+        "roleArn": str,
         "samplePromptsControlMode": WebExperienceSamplePromptsControlModeType,
         "status": WebExperienceStatusType,
         "subtitle": str,
         "title": str,
         "updatedAt": datetime,
         "webExperienceArn": str,
         "webExperienceId": str,
@@ -1759,26 +1795,28 @@
         "preExtractionHookConfiguration": NotRequired[HookConfigurationTypeDef],
     },
 )
 GetChatControlsConfigurationResponseTypeDef = TypedDict(
     "GetChatControlsConfigurationResponseTypeDef",
     {
         "blockedPhrases": BlockedPhrasesConfigurationTypeDef,
+        "creatorModeConfiguration": AppliedCreatorModeConfigurationTypeDef,
         "nextToken": str,
         "responseScope": ResponseScopeType,
         "topicConfigurations": List[TopicConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 UpdateChatControlsConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateChatControlsConfigurationRequestRequestTypeDef",
     {
         "applicationId": str,
         "blockedPhrasesConfigurationUpdate": NotRequired[BlockedPhrasesConfigurationUpdateTypeDef],
         "clientToken": NotRequired[str],
+        "creatorModeConfiguration": NotRequired[CreatorModeConfigurationTypeDef],
         "responseScope": NotRequired[ResponseScopeType],
         "topicConfigurationsToCreateOrUpdate": NotRequired[Sequence[TopicConfigurationTypeDef]],
         "topicConfigurationsToDelete": NotRequired[Sequence[TopicConfigurationTypeDef]],
     },
 )
 CreateDataSourceRequestRequestTypeDef = TypedDict(
     "CreateDataSourceRequestRequestTypeDef",
```

### Comparing `mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness/type_defs.pyi` & `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
 from .literals import (
     ActionPayloadFieldTypeType,
     ApplicationStatusType,
     AttachmentsControlModeType,
     AttachmentStatusType,
     AttributeTypeType,
+    ChatModeType,
     ContentTypeType,
+    CreatorModeControlType,
     DataSourceStatusType,
     DataSourceSyncJobStatusType,
     DocumentAttributeBoostingLevelType,
     DocumentEnrichmentConditionOperatorType,
     DocumentStatusType,
     ErrorCodeType,
     GroupStatusType,
@@ -67,30 +69,33 @@
 
 __all__ = (
     "ActionExecutionPayloadFieldPaginatorTypeDef",
     "ActionExecutionPayloadFieldTypeDef",
     "ActionReviewPayloadFieldAllowedValueTypeDef",
     "ApplicationTypeDef",
     "AppliedAttachmentsConfigurationTypeDef",
+    "AppliedCreatorModeConfigurationTypeDef",
     "BlobTypeDef",
     "ErrorDetailTypeDef",
     "AttachmentsConfigurationTypeDef",
     "BasicAuthConfigurationTypeDef",
     "DeleteDocumentTypeDef",
     "ResponseMetadataTypeDef",
     "BlockedPhrasesConfigurationTypeDef",
     "BlockedPhrasesConfigurationUpdateTypeDef",
+    "PluginConfigurationTypeDef",
     "ContentBlockerRuleTypeDef",
     "EligibleDataSourceTypeDef",
     "ConversationTypeDef",
     "EncryptionConfigurationTypeDef",
     "TagTypeDef",
     "DataSourceVpcConfigurationTypeDef",
     "IndexCapacityConfigurationTypeDef",
     "UserAliasTypeDef",
+    "CreatorModeConfigurationTypeDef",
     "DataSourceSyncJobMetricsTypeDef",
     "DataSourceTypeDef",
     "DateAttributeBoostingConfigurationTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteChatControlsConfigurationRequestRequestTypeDef",
     "DeleteConversationRequestRequestTypeDef",
     "DeleteDataSourceRequestRequestTypeDef",
@@ -159,14 +164,15 @@
     "CreateIndexResponseTypeDef",
     "CreatePluginResponseTypeDef",
     "CreateRetrieverResponseTypeDef",
     "CreateWebExperienceResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListApplicationsResponseTypeDef",
     "StartDataSourceSyncJobResponseTypeDef",
+    "ChatModeConfigurationTypeDef",
     "ContentRetrievalRuleTypeDef",
     "ListConversationsResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateWebExperienceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -204,19 +210,19 @@
     "ListRetrieversResponseTypeDef",
     "ListWebExperiencesResponseTypeDef",
     "PluginAuthConfigurationTypeDef",
     "PrincipalTypeDef",
     "WebExperienceAuthConfigurationTypeDef",
     "SourceAttributionTypeDef",
     "ActionReviewTypeDef",
-    "ChatSyncInputRequestTypeDef",
     "ListDocumentsResponseTypeDef",
     "BatchDeleteDocumentResponseTypeDef",
     "BatchPutDocumentResponseTypeDef",
     "GetGroupResponseTypeDef",
+    "ChatSyncInputRequestTypeDef",
     "RuleConfigurationTypeDef",
     "ListDataSourceSyncJobsResponseTypeDef",
     "NativeIndexConfigurationTypeDef",
     "DocumentAttributeConditionTypeDef",
     "DocumentAttributeTargetTypeDef",
     "DocumentAttributeTypeDef",
     "PutFeedbackRequestRequestTypeDef",
@@ -284,14 +290,20 @@
 )
 AppliedAttachmentsConfigurationTypeDef = TypedDict(
     "AppliedAttachmentsConfigurationTypeDef",
     {
         "attachmentsControlMode": NotRequired[AttachmentsControlModeType],
     },
 )
+AppliedCreatorModeConfigurationTypeDef = TypedDict(
+    "AppliedCreatorModeConfigurationTypeDef",
+    {
+        "creatorModeControl": CreatorModeControlType,
+    },
+)
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "errorCode": NotRequired[ErrorCodeType],
         "errorMessage": NotRequired[str],
     },
@@ -315,18 +327,18 @@
         "documentId": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 BlockedPhrasesConfigurationTypeDef = TypedDict(
     "BlockedPhrasesConfigurationTypeDef",
     {
         "blockedPhrases": NotRequired[List[str]],
         "systemMessageOverride": NotRequired[str],
@@ -336,14 +348,20 @@
     "BlockedPhrasesConfigurationUpdateTypeDef",
     {
         "blockedPhrasesToCreateOrUpdate": NotRequired[Sequence[str]],
         "blockedPhrasesToDelete": NotRequired[Sequence[str]],
         "systemMessageOverride": NotRequired[str],
     },
 )
+PluginConfigurationTypeDef = TypedDict(
+    "PluginConfigurationTypeDef",
+    {
+        "pluginId": str,
+    },
+)
 ContentBlockerRuleTypeDef = TypedDict(
     "ContentBlockerRuleTypeDef",
     {
         "systemMessageOverride": NotRequired[str],
     },
 )
 EligibleDataSourceTypeDef = TypedDict(
@@ -391,14 +409,20 @@
     "UserAliasTypeDef",
     {
         "userId": str,
         "dataSourceId": NotRequired[str],
         "indexId": NotRequired[str],
     },
 )
+CreatorModeConfigurationTypeDef = TypedDict(
+    "CreatorModeConfigurationTypeDef",
+    {
+        "creatorModeControl": CreatorModeControlType,
+    },
+)
 DataSourceSyncJobMetricsTypeDef = TypedDict(
     "DataSourceSyncJobMetricsTypeDef",
     {
         "documentsAdded": NotRequired[str],
         "documentsDeleted": NotRequired[str],
         "documentsFailed": NotRequired[str],
         "documentsModified": NotRequired[str],
@@ -436,15 +460,15 @@
     },
 )
 DeleteConversationRequestRequestTypeDef = TypedDict(
     "DeleteConversationRequestRequestTypeDef",
     {
         "applicationId": str,
         "conversationId": str,
-        "userId": str,
+        "userId": NotRequired[str],
     },
 )
 DeleteDataSourceRequestRequestTypeDef = TypedDict(
     "DeleteDataSourceRequestRequestTypeDef",
     {
         "applicationId": str,
         "dataSourceId": str,
@@ -655,17 +679,17 @@
         "nextToken": NotRequired[str],
     },
 )
 ListConversationsRequestRequestTypeDef = TypedDict(
     "ListConversationsRequestRequestTypeDef",
     {
         "applicationId": str,
-        "userId": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "userId": NotRequired[str],
     },
 )
 ListDataSourcesRequestRequestTypeDef = TypedDict(
     "ListDataSourcesRequestRequestTypeDef",
     {
         "applicationId": str,
         "indexId": str,
@@ -692,17 +716,17 @@
     },
 )
 ListMessagesRequestRequestTypeDef = TypedDict(
     "ListMessagesRequestRequestTypeDef",
     {
         "applicationId": str,
         "conversationId": str,
-        "userId": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "userId": NotRequired[str],
     },
 )
 ListPluginsRequestRequestTypeDef = TypedDict(
     "ListPluginsRequestRequestTypeDef",
     {
         "applicationId": str,
         "maxResults": NotRequired[int],
@@ -984,14 +1008,20 @@
 StartDataSourceSyncJobResponseTypeDef = TypedDict(
     "StartDataSourceSyncJobResponseTypeDef",
     {
         "executionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ChatModeConfigurationTypeDef = TypedDict(
+    "ChatModeConfigurationTypeDef",
+    {
+        "pluginConfiguration": NotRequired[PluginConfigurationTypeDef],
+    },
+)
 ContentRetrievalRuleTypeDef = TypedDict(
     "ContentRetrievalRuleTypeDef",
     {
         "eligibleDataSources": NotRequired[List[EligibleDataSourceTypeDef]],
     },
 )
 ListConversationsResponseTypeDef = TypedDict(
@@ -1009,14 +1039,15 @@
         "applicationId": str,
         "attachmentsConfiguration": AppliedAttachmentsConfigurationTypeDef,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "encryptionConfiguration": EncryptionConfigurationTypeDef,
         "error": ErrorDetailTypeDef,
+        "identityCenterApplicationArn": str,
         "roleArn": str,
         "status": ApplicationStatusType,
         "updatedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateApplicationRequestRequestTypeDef = TypedDict(
@@ -1024,22 +1055,24 @@
     {
         "displayName": str,
         "roleArn": str,
         "attachmentsConfiguration": NotRequired[AttachmentsConfigurationTypeDef],
         "clientToken": NotRequired[str],
         "description": NotRequired[str],
         "encryptionConfiguration": NotRequired[EncryptionConfigurationTypeDef],
+        "identityCenterInstanceArn": NotRequired[str],
         "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 CreateWebExperienceRequestRequestTypeDef = TypedDict(
     "CreateWebExperienceRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": NotRequired[str],
+        "roleArn": NotRequired[str],
         "samplePromptsControlMode": NotRequired[WebExperienceSamplePromptsControlModeType],
         "subtitle": NotRequired[str],
         "tags": NotRequired[Sequence[TagTypeDef]],
         "title": NotRequired[str],
         "welcomeMessage": NotRequired[str],
     },
 )
@@ -1206,15 +1239,15 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListConversationsRequestListConversationsPaginateTypeDef = TypedDict(
     "ListConversationsRequestListConversationsPaginateTypeDef",
     {
         "applicationId": str,
-        "userId": str,
+        "userId": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef = TypedDict(
     "ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef",
     {
         "applicationId": str,
@@ -1261,15 +1294,15 @@
     },
 )
 ListMessagesRequestListMessagesPaginateTypeDef = TypedDict(
     "ListMessagesRequestListMessagesPaginateTypeDef",
     {
         "applicationId": str,
         "conversationId": str,
-        "userId": str,
+        "userId": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListPluginsRequestListPluginsPaginateTypeDef = TypedDict(
     "ListPluginsRequestListPluginsPaginateTypeDef",
     {
         "applicationId": str,
@@ -1381,29 +1414,14 @@
     {
         "payload": NotRequired[Dict[str, ActionReviewPayloadFieldTypeDef]],
         "payloadFieldNameSeparator": NotRequired[str],
         "pluginId": NotRequired[str],
         "pluginType": NotRequired[PluginTypeType],
     },
 )
-ChatSyncInputRequestTypeDef = TypedDict(
-    "ChatSyncInputRequestTypeDef",
-    {
-        "applicationId": str,
-        "userId": str,
-        "actionExecution": NotRequired[ActionExecutionTypeDef],
-        "attachments": NotRequired[Sequence[AttachmentInputTypeDef]],
-        "attributeFilter": NotRequired["AttributeFilterTypeDef"],
-        "clientToken": NotRequired[str],
-        "conversationId": NotRequired[str],
-        "parentMessageId": NotRequired[str],
-        "userGroups": NotRequired[Sequence[str]],
-        "userMessage": NotRequired[str],
-    },
-)
 ListDocumentsResponseTypeDef = TypedDict(
     "ListDocumentsResponseTypeDef",
     {
         "documentDetailList": List[DocumentDetailsTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1426,14 +1444,31 @@
     "GetGroupResponseTypeDef",
     {
         "status": GroupStatusDetailTypeDef,
         "statusHistory": List[GroupStatusDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ChatSyncInputRequestTypeDef = TypedDict(
+    "ChatSyncInputRequestTypeDef",
+    {
+        "applicationId": str,
+        "actionExecution": NotRequired[ActionExecutionTypeDef],
+        "attachments": NotRequired[Sequence[AttachmentInputTypeDef]],
+        "attributeFilter": NotRequired["AttributeFilterTypeDef"],
+        "chatMode": NotRequired[ChatModeType],
+        "chatModeConfiguration": NotRequired[ChatModeConfigurationTypeDef],
+        "clientToken": NotRequired[str],
+        "conversationId": NotRequired[str],
+        "parentMessageId": NotRequired[str],
+        "userGroups": NotRequired[Sequence[str]],
+        "userId": NotRequired[str],
+        "userMessage": NotRequired[str],
+    },
+)
 RuleConfigurationTypeDef = TypedDict(
     "RuleConfigurationTypeDef",
     {
         "contentBlockerRule": NotRequired[ContentBlockerRuleTypeDef],
         "contentRetrievalRule": NotRequired[ContentRetrievalRuleTypeDef],
     },
 )
@@ -1479,17 +1514,17 @@
 )
 PutFeedbackRequestRequestTypeDef = TypedDict(
     "PutFeedbackRequestRequestTypeDef",
     {
         "applicationId": str,
         "conversationId": str,
         "messageId": str,
-        "userId": str,
         "messageCopiedAt": NotRequired[TimestampTypeDef],
         "messageUsefulness": NotRequired[MessageUsefulnessFeedbackTypeDef],
+        "userId": NotRequired[str],
     },
 )
 PutGroupRequestRequestTypeDef = TypedDict(
     "PutGroupRequestRequestTypeDef",
     {
         "applicationId": str,
         "groupMembers": GroupMembersTypeDef,
@@ -1567,14 +1602,15 @@
     "GetWebExperienceResponseTypeDef",
     {
         "applicationId": str,
         "authenticationConfiguration": WebExperienceAuthConfigurationTypeDef,
         "createdAt": datetime,
         "defaultEndpoint": str,
         "error": ErrorDetailTypeDef,
+        "roleArn": str,
         "samplePromptsControlMode": WebExperienceSamplePromptsControlModeType,
         "status": WebExperienceStatusType,
         "subtitle": str,
         "title": str,
         "updatedAt": datetime,
         "webExperienceArn": str,
         "webExperienceId": str,
@@ -1759,26 +1795,28 @@
         "preExtractionHookConfiguration": NotRequired[HookConfigurationTypeDef],
     },
 )
 GetChatControlsConfigurationResponseTypeDef = TypedDict(
     "GetChatControlsConfigurationResponseTypeDef",
     {
         "blockedPhrases": BlockedPhrasesConfigurationTypeDef,
+        "creatorModeConfiguration": AppliedCreatorModeConfigurationTypeDef,
         "nextToken": str,
         "responseScope": ResponseScopeType,
         "topicConfigurations": List[TopicConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 UpdateChatControlsConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateChatControlsConfigurationRequestRequestTypeDef",
     {
         "applicationId": str,
         "blockedPhrasesConfigurationUpdate": NotRequired[BlockedPhrasesConfigurationUpdateTypeDef],
         "clientToken": NotRequired[str],
+        "creatorModeConfiguration": NotRequired[CreatorModeConfigurationTypeDef],
         "responseScope": NotRequired[ResponseScopeType],
         "topicConfigurationsToCreateOrUpdate": NotRequired[Sequence[TopicConfigurationTypeDef]],
         "topicConfigurationsToDelete": NotRequired[Sequence[TopicConfigurationTypeDef]],
     },
 )
 CreateDataSourceRequestRequestTypeDef = TypedDict(
     "CreateDataSourceRequestRequestTypeDef",
```

### Comparing `mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness.egg-info/PKG-INFO` & `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qbusiness
-Version: 1.34.42
-Summary: Type annotations for boto3.QBusiness 1.34.42 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.86
+Summary: Type annotations for boto3.QBusiness 1.34.86 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-qbusiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qbusiness)](https://pepy.tech/project/mypy-boto3-qbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QBusiness 1.34.42](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
+[boto3.QBusiness 1.34.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-qbusiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-qbusiness-1.34.42/mypy_boto3_qbusiness.egg-info/SOURCES.txt` & `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qbusiness-1.34.42/setup.py` & `mypy_boto3_qbusiness-1.34.86/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-qbusiness",
-    version="1.34.42",
+    version="1.34.86",
     packages=["mypy_boto3_qbusiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.QBusiness 1.34.42 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.QBusiness 1.34.86 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

