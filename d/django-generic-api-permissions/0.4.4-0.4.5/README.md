# Comparing `tmp/django_generic_api_permissions-0.4.4.tar.gz` & `tmp/django_generic_api_permissions-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_generic_api_permissions-0.4.4.tar", max compression
+gzip compressed data, was "django_generic_api_permissions-0.4.5.tar", max compression
```

## Comparing `django_generic_api_permissions-0.4.4.tar` & `django_generic_api_permissions-0.4.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    12489 2024-03-20 16:09:48.677335 django_generic_api_permissions-0.4.4/CHANGELOG.md
--rw-r--r--   0        0        0     7651 2024-03-20 16:09:48.677335 django_generic_api_permissions-0.4.4/LICENSE
--rw-r--r--   0        0        0    11571 2024-03-20 16:09:48.681335 django_generic_api_permissions-0.4.4/README.md
--rw-r--r--   0        0        0        0 2024-03-20 16:09:48.681335 django_generic_api_permissions-0.4.4/generic_permissions/__init__.py
--rw-r--r--   0        0        0     1389 2024-03-20 16:09:48.681335 django_generic_api_permissions-0.4.4/generic_permissions/apps.py
--rw-r--r--   0        0        0     4005 2024-03-20 16:09:48.681335 django_generic_api_permissions-0.4.4/generic_permissions/config.py
--rw-r--r--   0        0        0      746 2024-03-20 16:09:48.681335 django_generic_api_permissions-0.4.4/generic_permissions/models.py
--rw-r--r--   0        0        0     2381 2024-03-20 16:09:48.681335 django_generic_api_permissions-0.4.4/generic_permissions/permissions.py
--rw-r--r--   0        0        0      492 2024-03-20 16:09:48.681335 django_generic_api_permissions-0.4.4/generic_permissions/serializers.py
--rw-r--r--   0        0        0     1439 2024-03-20 16:09:48.681335 django_generic_api_permissions-0.4.4/generic_permissions/validation.py
--rw-r--r--   0        0        0      973 2024-03-20 16:09:48.681335 django_generic_api_permissions-0.4.4/generic_permissions/views.py
--rw-r--r--   0        0        0     6997 2024-03-20 16:09:48.681335 django_generic_api_permissions-0.4.4/generic_permissions/visibilities.py
--rw-r--r--   0        0        0     3877 2024-03-20 16:10:08.337441 django_generic_api_permissions-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    12734 1970-01-01 00:00:00.000000 django_generic_api_permissions-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    15276 2024-04-17 11:27:38.601732 django_generic_api_permissions-0.4.5/CHANGELOG.md
+-rw-r--r--   0        0        0     7651 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/LICENSE
+-rw-r--r--   0        0        0    11571 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/__init__.py
+-rw-r--r--   0        0        0     1389 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/apps.py
+-rw-r--r--   0        0        0     4005 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/config.py
+-rw-r--r--   0        0        0      746 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/models.py
+-rw-r--r--   0        0        0     2437 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/permissions.py
+-rw-r--r--   0        0        0      492 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/serializers.py
+-rw-r--r--   0        0        0     1439 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/validation.py
+-rw-r--r--   0        0        0      973 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/views.py
+-rw-r--r--   0        0        0     6997 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/visibilities.py
+-rw-r--r--   0        0        0     4069 2024-04-17 11:27:38.645732 django_generic_api_permissions-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0    12734 1970-01-01 00:00:00.000000 django_generic_api_permissions-0.4.5/PKG-INFO
```

### Comparing `django_generic_api_permissions-0.4.4/CHANGELOG.md` & `django_generic_api_permissions-0.4.5/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,83 @@
 # CHANGELOG
 
 
 
+## v0.4.5 (2024-04-17)
+
+### Chore
+
+* chore: fix maintenance docs (#39) ([`9947377`](https://github.com/adfinis/django-generic-api-permissions/commit/99473779dca83ea5c4affe02f3625683e1b9e1c5))
+
+* chore: add CONTRIBUTING.md, allow running pytest directly in dev (#50)
+
+Co-authored-by: Fabio Ambauen &lt;1833932+open-dynaMIX@users.noreply.github.com&gt; ([`4fd4a34`](https://github.com/adfinis/django-generic-api-permissions/commit/4fd4a34b2e7982048f1a4db695a598d214667dcb))
+
+* chore(deps): bump django from 4.2.9 to 4.2.11
+
+Bumps [django](https://github.com/django/django) from 4.2.9 to 4.2.11.
+- [Commits](https://github.com/django/django/compare/4.2.9...4.2.11)
+
+---
+updated-dependencies:
+- dependency-name: django
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`a6b445d`](https://github.com/adfinis/django-generic-api-permissions/commit/a6b445da1d2baaa304d997320ca77c87ed2f0957))
+
+* chore(deps-dev): bump ruff from 0.2.2 to 0.3.5
+
+Bumps [ruff](https://github.com/astral-sh/ruff) from 0.2.2 to 0.3.5.
+- [Release notes](https://github.com/astral-sh/ruff/releases)
+- [Changelog](https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md)
+- [Commits](https://github.com/astral-sh/ruff/compare/v0.2.2...v0.3.5)
+
+---
+updated-dependencies:
+- dependency-name: ruff
+  dependency-type: direct:development
+  update-type: version-update:semver-minor
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`42d7930`](https://github.com/adfinis/django-generic-api-permissions/commit/42d7930176a5bec01f93159fa8395783a39c8c22))
+
+### Fix
+
+* fix: don&#39;t check permissions for GET requests (#51)
+
+Permissions should only deal with POST/PATCH/DELETE - GET requests
+should be entirely governed by the visibility layer. ([`774f259`](https://github.com/adfinis/django-generic-api-permissions/commit/774f2594a56d824f1b5f9bba3d44de15b115f55c))
+
+
+## v0.4.4 (2024-03-20)
+
+### Chore
+
+* chore(release): 0.4.4
+
+Automatically generated by python-semantic-release ([`d765283`](https://github.com/adfinis/django-generic-api-permissions/commit/d765283ccc338171f5cebf8837e6000cffb8cc93))
+
+### Fix
+
+* fix: add fallback for queryset of read_only related fields (#38)
+
+Read only fields don&#39;t have a queryset (see
+https://github.com/encode/django-rest-framework/blame/77ef27f18fc7c11e1d2e5fd4aaa8acc51cda6792/rest_framework/utils/field_mapping.py#L288), so we need to provide a fallback. ([`9f6ed09`](https://github.com/adfinis/django-generic-api-permissions/commit/9f6ed09b26ee238bdccee401dce8ae4fba5332ff))
+
+
 ## v0.4.3 (2024-03-15)
 
 ### Chore
 
+* chore(release): 0.4.3
+
+Automatically generated by python-semantic-release ([`f9a4687`](https://github.com/adfinis/django-generic-api-permissions/commit/f9a4687256ab602631453ad7b6aaa782ac20b12e))
+
 * chore(deps-dev): bump ruff from 0.1.11 to 0.2.2 (#30)
 
 Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.11 to 0.2.2.
 - [Release notes](https://github.com/astral-sh/ruff/releases)
 - [Changelog](https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md)
 - [Commits](https://github.com/astral-sh/ruff/compare/v0.1.11...v0.2.2)
```

### Comparing `django_generic_api_permissions-0.4.4/LICENSE` & `django_generic_api_permissions-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.4/README.md` & `django_generic_api_permissions-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.4/generic_permissions/apps.py` & `django_generic_api_permissions-0.4.5/generic_permissions/apps.py`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.4/generic_permissions/config.py` & `django_generic_api_permissions-0.4.5/generic_permissions/config.py`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.4/generic_permissions/models.py` & `django_generic_api_permissions-0.4.5/generic_permissions/models.py`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.4/generic_permissions/permissions.py` & `django_generic_api_permissions-0.4.5/generic_permissions/permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,17 @@
         """Check if access to given object is granted.
 
         Raise PermissionDenied if configured permissions do not allow
         accesss to the object.
 
         Called by get_object().
         """
+        if request.method == "GET":
+            return
+
         for handler in ObjectPermissionsConfig.get_handlers(
             self.get_serializer().Meta.model
         ):
             if not handler(request, instance):
                 raise PermissionDenied()
```

### Comparing `django_generic_api_permissions-0.4.4/generic_permissions/validation.py` & `django_generic_api_permissions-0.4.5/generic_permissions/validation.py`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.4/generic_permissions/views.py` & `django_generic_api_permissions-0.4.5/generic_permissions/views.py`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.4/generic_permissions/visibilities.py` & `django_generic_api_permissions-0.4.5/generic_permissions/visibilities.py`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.4/pyproject.toml` & `django_generic_api_permissions-0.4.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-generic-api-permissions"
-version = "0.4.4"
+version = "0.4.5"
 description="Generic API permissions and visibilities for Django"
 authors = ["Adfinis <indo@adfinis.com>"]
 readme = "README.md"
 repository = "https://github.com/adfinis/django-generic-api-permissions"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -31,23 +31,33 @@
 [tool.poetry.dependencies]
 python = ">=3.8.1"
 django = ">=3.2"
 djangorestframework = "^3.14"
 
 [tool.poetry.dev-dependencies]
 black = "^23.12.1"
-ruff = "^0.2.2"
+ruff = "^0.3.5"
 
 [tool.poetry.group.djangorestframework-jsonapi]
 optional = true
 
 [tool.poetry.group.djangorestframework-jsonapi.dependencies]
 djangorestframework-jsonapi= "^6.1"
 
 
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
+pytest-mock = "^3.14.0"
+pytest-django = "^4.8.0"
+pytest-randomly = "^3.15.0"
+pdbpp = "^0.10.3"
+ipdb = "^0.13.13"
+
 [tool.ruff.lint]
 select = ["E", "W", "F", "B", "I", "C4", "C90"]
 
 ignore = [
     # whitespace before ':'
     "E203",
     # too many leading ### in a block comment
```

### Comparing `django_generic_api_permissions-0.4.4/PKG-INFO` & `django_generic_api_permissions-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-generic-api-permissions
-Version: 0.4.4
+Version: 0.4.5
 Summary: Generic API permissions and visibilities for Django
 Home-page: https://github.com/adfinis/django-generic-api-permissions
 Author: Adfinis
 Author-email: indo@adfinis.com
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

