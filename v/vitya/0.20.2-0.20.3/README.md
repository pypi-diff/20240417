# Comparing `tmp/vitya-0.20.2.tar.gz` & `tmp/vitya-0.20.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vitya-0.20.2.tar", last modified: Tue Apr  2 11:45:33 2024, max compression
+gzip compressed data, was "dist/vitya-0.20.3.tar", last modified: Wed Apr 17 10:50:48 2024, max compression
```

## Comparing `vitya-0.20.2.tar` & `vitya-0.20.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:33.000000 vitya-0.20.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-02 11:45:25.000000 vitya-0.20.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-02 11:45:33.000000 vitya-0.20.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-02 11:45:25.000000 vitya-0.20.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-02 11:45:25.000000 vitya-0.20.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 11:45:33.000000 vitya-0.20.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-02 11:45:25.000000 vitya-0.20.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:33.000000 vitya-0.20.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-02 11:45:25.000000 vitya-0.20.2/tests/test_error_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-02 11:45:25.000000 vitya-0.20.2/tests/test_vitya.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/error_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/errors_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya/payment_order/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    35702 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya/payment_order/payments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/payments/checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19321 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/payments/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/payments/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/payments/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/payment_order/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/pydantic_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/typing_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-02 11:45:25.000000 vitya-0.20.2/vitya/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 11:45:33.000000 vitya-0.20.2/vitya.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:50:48.000000 vitya-0.20.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-17 10:50:44.000000 vitya-0.20.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-17 10:50:48.000000 vitya-0.20.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-17 10:50:44.000000 vitya-0.20.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-17 10:50:44.000000 vitya-0.20.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 10:50:48.000000 vitya-0.20.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-17 10:50:44.000000 vitya-0.20.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:50:48.000000 vitya-0.20.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-17 10:50:44.000000 vitya-0.20.3/tests/test_error_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-17 10:50:44.000000 vitya-0.20.3/tests/test_vitya.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:50:48.000000 vitya-0.20.3/vitya/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/error_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/errors_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:50:48.000000 vitya-0.20.3/vitya/payment_order/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/payment_order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/payment_order/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35702 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/payment_order/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/payment_order/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:50:48.000000 vitya-0.20.3/vitya/payment_order/payments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/payment_order/payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/payment_order/payments/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19343 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/payment_order/payments/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/payment_order/payments/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/payment_order/payments/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/payment_order/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/pydantic_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/typing_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-17 10:50:44.000000 vitya-0.20.3/vitya/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:50:48.000000 vitya-0.20.3/vitya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-17 10:50:48.000000 vitya-0.20.3/vitya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-17 10:50:48.000000 vitya-0.20.3/vitya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:50:48.000000 vitya-0.20.3/vitya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 10:50:48.000000 vitya-0.20.3/vitya.egg-info/top_level.txt
```

### Comparing `vitya-0.20.2/LICENSE` & `vitya-0.20.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/PKG-INFO` & `vitya-0.20.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitya
-Version: 0.20.2
+Version: 0.20.3
 Summary: Validators for different russian banking values
 Home-page: https://github.com/hicebank/vitya
 Author: hicebank.ru
 Author-email: inyutin@hicebank.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vitya-0.20.2/README.md` & `vitya-0.20.3/README.md`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/setup.py` & `vitya-0.20.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='vitya',
-    version='0.20.2',
+    version='0.20.3',
     author='hicebank.ru',
     author_email='inyutin@hicebank.ru',
     description='Validators for different russian banking values',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/hicebank/vitya',
     packages=setuptools.find_packages(),
```

### Comparing `vitya-0.20.2/tests/test_error_description.py` & `vitya-0.20.3/tests/test_error_description.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/tests/test_vitya.py` & `vitya-0.20.3/tests/test_vitya.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/vitya/error_description.py` & `vitya-0.20.3/vitya/error_description.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/vitya/errors.py` & `vitya-0.20.3/vitya/errors.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/vitya/errors_base.py` & `vitya-0.20.3/vitya/errors_base.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/vitya/payment_order/enums.py` & `vitya-0.20.3/vitya/payment_order/enums.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/vitya/payment_order/errors.py` & `vitya-0.20.3/vitya/payment_order/errors.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/vitya/payment_order/fields.py` & `vitya-0.20.3/vitya/payment_order/fields.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/vitya/payment_order/payments/checkers.py` & `vitya-0.20.3/vitya/payment_order/payments/checkers.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/vitya/payment_order/payments/checks.py` & `vitya-0.20.3/vitya/payment_order/payments/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import re
 from datetime import date
 from typing import Optional
 
 from vitya.payment_order.enums import AccountKind, PaymentType
-from vitya.payment_order.errors import (
+from vitya.payment_order.errors import (  # DocumentNumberValidationBOValueError,
     AccountValidationBICValueError,
     BudgetPaymentForThirdPersonError,
     CBCValidationEmptyNotAllowed,
     DocumentDateValidationBOLenError,
     DocumentDateValidationCustomsLenError,
     DocumentDateValidationCustomsReasonValueError,
     DocumentDateValidationFNSOnlyEmptyError,
     DocumentNumberValidationBOEmptyNotAllowed,
     DocumentNumberValidationBOOnlyEmptyError,
     DocumentNumberValidationBOPayerStatus33OnlyEmptyError,
-    DocumentNumberValidationBOValueError,
     DocumentNumberValidationBOValueLenError,
     DocumentNumberValidationCustoms00ValueError,
     DocumentNumberValidationCustomsValueLen7Error,
     DocumentNumberValidationCustomsValueLen15Error,
     DocumentNumberValidationFNSOnlyEmptyError,
     OKTMOValidationEmptyNotAllowed,
     OKTMOValidationFNSEmptyNotAllowed,
@@ -547,15 +546,16 @@
             return None
         if payer_status == '24' and payer_inn is None and uin is None and value is None:
             raise DocumentNumberValidationBOEmptyNotAllowed
         if value is not None:
             if len(value) > 15:
                 raise DocumentNumberValidationBOValueLenError
             if len(value) < 3 or value[2] != ';' or value[:2] not in DOCUMENT_NUMBERS:
-                raise DocumentNumberValidationBOValueError
+                # raise DocumentNumberValidationBOValueError
+                pass
         return value
     elif payment_type == PaymentType.CUSTOMS:
         if reason == '00' and value is not None and value not in ['00', '0']:
             raise DocumentNumberValidationCustoms00ValueError
         if reason in {'ПК', 'УВ', 'ТГ', 'ТБ', 'ТД', 'ПВ'} and value and len(value) > 7:
             raise DocumentNumberValidationCustomsValueLen7Error
         if (
```

### Comparing `vitya-0.20.2/vitya/payment_order/payments/constants.py` & `vitya-0.20.3/vitya/payment_order/payments/constants.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/vitya/payment_order/payments/tools.py` & `vitya-0.20.3/vitya/payment_order/payments/tools.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/vitya/payment_order/validators.py` & `vitya-0.20.3/vitya/payment_order/validators.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/vitya/pydantic_fields.py` & `vitya-0.20.3/vitya/pydantic_fields.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/vitya/validators.py` & `vitya-0.20.3/vitya/validators.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.2/vitya.egg-info/PKG-INFO` & `vitya-0.20.3/vitya.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitya
-Version: 0.20.2
+Version: 0.20.3
 Summary: Validators for different russian banking values
 Home-page: https://github.com/hicebank/vitya
 Author: hicebank.ru
 Author-email: inyutin@hicebank.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vitya-0.20.2/vitya.egg-info/SOURCES.txt` & `vitya-0.20.3/vitya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

