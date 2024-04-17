# Comparing `tmp/payla_utils-0.3.1.tar.gz` & `tmp/payla_utils-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payla_utils-0.3.1.tar", max compression
+gzip compressed data, was "payla_utils-0.3.2.tar", max compression
```

## Comparing `payla_utils-0.3.1.tar` & `payla_utils-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     6035 2024-01-16 16:54:22.317528 payla_utils-0.3.1/README-public-pypi.md
--rw-r--r--   0        0        0      151 2024-01-16 16:54:22.317528 payla_utils-0.3.1/payla_utils/__init__.py
--rw-r--r--   0        0        0     4131 2024-01-16 16:54:22.317528 payla_utils-0.3.1/payla_utils/access/README.md
--rw-r--r--   0        0        0       81 2024-01-16 16:54:22.317528 payla_utils-0.3.1/payla_utils/access/__init__.py
--rw-r--r--   0        0        0      786 2024-01-16 16:54:22.317528 payla_utils-0.3.1/payla_utils/access/decorators.py
--rw-r--r--   0        0        0     5298 2024-01-16 16:54:22.317528 payla_utils-0.3.1/payla_utils/access/permission.py
--rw-r--r--   0        0        0      148 2024-01-16 16:54:22.317528 payla_utils-0.3.1/payla_utils/apps.py
--rw-r--r--   0        0        0      201 2024-01-16 16:54:22.317528 payla_utils-0.3.1/payla_utils/logging/__init__.py
--rw-r--r--   0        0        0     3412 2024-01-16 16:54:22.317528 payla_utils-0.3.1/payla_utils/logging/default_configuration.py
--rw-r--r--   0        0        0      862 2024-01-16 16:54:22.317528 payla_utils-0.3.1/payla_utils/logging/logformatter.py
--rw-r--r--   0        0        0     4538 2024-01-16 16:54:22.317528 payla_utils-0.3.1/payla_utils/logging/logger.py
--rw-r--r--   0        0        0     2016 2024-01-16 16:54:22.318528 payla_utils-0.3.1/payla_utils/logging/middlewares.py
--rw-r--r--   0        0        0      581 2024-01-16 16:54:22.318528 payla_utils-0.3.1/payla_utils/logging/sentry_logger.py
--rw-r--r--   0        0        0        0 2024-01-16 16:54:22.348528 payla_utils-0.3.1/payla_utils/management/__init__.py
--rw-r--r--   0        0        0        0 2024-01-16 16:54:22.348528 payla_utils-0.3.1/payla_utils/management/commands/__init__.py
--rw-r--r--   0        0        0      989 2024-01-16 16:54:22.318528 payla_utils-0.3.1/payla_utils/management/commands/i18n.py
--rw-r--r--   0        0        0     3269 2024-01-16 16:54:22.318528 payla_utils-0.3.1/payla_utils/management/commands/init_environment.py
--rw-r--r--   0        0        0      105 2024-01-16 16:54:22.318528 payla_utils-0.3.1/payla_utils/models/__init__.py
--rw-r--r--   0        0        0     7064 2024-01-16 16:54:22.318528 payla_utils-0.3.1/payla_utils/models/base.py
--rw-r--r--   0        0        0        0 2024-01-16 16:54:22.348528 payla_utils-0.3.1/payla_utils/scripts/__init__.py
--rw-r--r--   0        0        0      286 2024-01-16 16:54:22.318528 payla_utils-0.3.1/payla_utils/scripts/custom_test_script.py
--rw-r--r--   0        0        0    10576 2024-01-16 16:54:22.318528 payla_utils-0.3.1/payla_utils/settings.py
--rw-r--r--   0        0        0     3534 2024-01-16 16:54:22.319528 payla_utils-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7135 1970-01-01 00:00:00.000000 payla_utils-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     6035 2024-04-17 10:10:06.766662 payla_utils-0.3.2/README-public-pypi.md
+-rw-r--r--   0        0        0      151 2024-04-17 10:10:06.766662 payla_utils-0.3.2/payla_utils/__init__.py
+-rw-r--r--   0        0        0     4131 2024-04-17 10:10:06.766662 payla_utils-0.3.2/payla_utils/access/README.md
+-rw-r--r--   0        0        0       81 2024-04-17 10:10:06.766662 payla_utils-0.3.2/payla_utils/access/__init__.py
+-rw-r--r--   0        0        0      786 2024-04-17 10:10:06.766662 payla_utils-0.3.2/payla_utils/access/decorators.py
+-rw-r--r--   0        0        0     5298 2024-04-17 10:10:06.766662 payla_utils-0.3.2/payla_utils/access/permission.py
+-rw-r--r--   0        0        0      148 2024-04-17 10:10:06.766662 payla_utils-0.3.2/payla_utils/apps.py
+-rw-r--r--   0        0        0      201 2024-04-17 10:10:06.766662 payla_utils-0.3.2/payla_utils/logging/__init__.py
+-rw-r--r--   0        0        0     3412 2024-04-17 10:10:06.767663 payla_utils-0.3.2/payla_utils/logging/default_configuration.py
+-rw-r--r--   0        0        0      862 2024-04-17 10:10:06.767663 payla_utils-0.3.2/payla_utils/logging/logformatter.py
+-rw-r--r--   0        0        0     4538 2024-04-17 10:10:06.767663 payla_utils-0.3.2/payla_utils/logging/logger.py
+-rw-r--r--   0        0        0     2025 2024-04-17 10:10:06.767663 payla_utils-0.3.2/payla_utils/logging/middlewares.py
+-rw-r--r--   0        0        0      581 2024-04-17 10:10:06.767663 payla_utils-0.3.2/payla_utils/logging/sentry_logger.py
+-rw-r--r--   0        0        0        0 2024-04-17 10:10:06.795662 payla_utils-0.3.2/payla_utils/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 10:10:06.795662 payla_utils-0.3.2/payla_utils/management/commands/__init__.py
+-rw-r--r--   0        0        0      989 2024-04-17 10:10:06.767663 payla_utils-0.3.2/payla_utils/management/commands/i18n.py
+-rw-r--r--   0        0        0     3269 2024-04-17 10:10:06.767663 payla_utils-0.3.2/payla_utils/management/commands/init_environment.py
+-rw-r--r--   0        0        0      105 2024-04-17 10:10:06.767663 payla_utils-0.3.2/payla_utils/models/__init__.py
+-rw-r--r--   0        0        0     7193 2024-04-17 10:10:06.767663 payla_utils-0.3.2/payla_utils/models/base.py
+-rw-r--r--   0        0        0        0 2024-04-17 10:10:06.795662 payla_utils-0.3.2/payla_utils/scripts/__init__.py
+-rw-r--r--   0        0        0      286 2024-04-17 10:10:06.767663 payla_utils-0.3.2/payla_utils/scripts/custom_test_script.py
+-rw-r--r--   0        0        0    10577 2024-04-17 10:10:06.767663 payla_utils-0.3.2/payla_utils/settings.py
+-rw-r--r--   0        0        0     2777 2024-04-17 10:10:06.768663 payla_utils-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     7135 1970-01-01 00:00:00.000000 payla_utils-0.3.2/PKG-INFO
```

### Comparing `payla_utils-0.3.1/README-public-pypi.md` & `payla_utils-0.3.2/README-public-pypi.md`

 * *Files identical despite different names*

### Comparing `payla_utils-0.3.1/payla_utils/access/README.md` & `payla_utils-0.3.2/payla_utils/access/README.md`

 * *Files identical despite different names*

### Comparing `payla_utils-0.3.1/payla_utils/access/decorators.py` & `payla_utils-0.3.2/payla_utils/access/decorators.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.3.1/payla_utils/access/permission.py` & `payla_utils-0.3.2/payla_utils/access/permission.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.3.1/payla_utils/logging/default_configuration.py` & `payla_utils-0.3.2/payla_utils/logging/default_configuration.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.3.1/payla_utils/logging/logformatter.py` & `payla_utils-0.3.2/payla_utils/logging/logformatter.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.3.1/payla_utils/logging/logger.py` & `payla_utils-0.3.2/payla_utils/logging/logger.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.3.1/payla_utils/logging/middlewares.py` & `payla_utils-0.3.2/payla_utils/logging/middlewares.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import uuid
-from typing import Callable
+from collections.abc import Callable
 
 import structlog
 from django.http import HttpRequest, HttpResponse
 
 from payla_utils.settings import payla_utils_settings
 
 logger = structlog.get_logger(__name__)
```

### Comparing `payla_utils-0.3.1/payla_utils/logging/sentry_logger.py` & `payla_utils-0.3.2/payla_utils/logging/sentry_logger.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.3.1/payla_utils/management/commands/i18n.py` & `payla_utils-0.3.2/payla_utils/management/commands/i18n.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.3.1/payla_utils/management/commands/init_environment.py` & `payla_utils-0.3.2/payla_utils/management/commands/init_environment.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.3.1/payla_utils/models/base.py` & `payla_utils-0.3.2/payla_utils/models/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,18 @@
     created_at = models.DateTimeField(verbose_name=_('Created At'), auto_now_add=True)
     modified_at = models.DateTimeField(verbose_name=_('Last modified'), auto_now=True)
 
     objects = PaylaQuerySet.as_manager()
 
     class Meta:
         abstract = True
+        indexes = [
+            models.Index(fields=['created_at']),
+            models.Index(fields=['modified_at']),
+        ]
 
     def save(self, *args, **kwargs):
         """
         Overriding the save method in order to make sure that
         modified field is updated even if it is not given as
         a parameter to the update field argument.
         """
```

### Comparing `payla_utils-0.3.1/payla_utils/settings.py` & `payla_utils-0.3.2/payla_utils/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         },
     }
 }
 This module provides the `payla_utils_setting` object, that is used to access
 Payla Utils settings, checking for user settings first, then falling
 back to the defaults.
 """
+
 from __future__ import annotations
 
 from django.conf import settings
 
 # Import from `django.core.signals` instead of the official location
 # `django.test.signals` to avoid importing the test module unnecessarily.
 from django.core.signals import setting_changed
```

### Comparing `payla_utils-0.3.1/PKG-INFO` & `payla_utils-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payla-utils
-Version: 0.3.1
+Version: 0.3.2
 Summary: payla_utils python package
 License: MIT
 Keywords: payla_utils
 Author: Payla Services
 Author-email: tools@payla.de
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 2 - Pre-Alpha
```

