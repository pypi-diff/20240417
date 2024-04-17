# Comparing `tmp/sat_utils-1.4.2.tar.gz` & `tmp/sat_utils-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sat_utils-1.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sat_utils-1.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sat_utils-1.4.2.tar` & `sat_utils-1.4.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       49 2024-03-19 14:15:25.221026 sat_utils-1.4.2/.coveragerc
--rw-r--r--   0        0        0      220 2024-03-19 14:15:25.221026 sat_utils-1.4.2/.editorconfig
--rw-r--r--   0        0        0      494 2024-03-19 14:15:25.221026 sat_utils-1.4.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     8456 2024-03-19 14:15:25.221026 sat_utils-1.4.2/.github/workflows/test_publish_and_release.yml
--rw-r--r--   0        0        0     3186 2024-03-19 14:15:25.221026 sat_utils-1.4.2/.gitignore
--rw-r--r--   0        0        0      875 2024-03-19 14:15:25.221026 sat_utils-1.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1102 2024-03-19 14:15:25.221026 sat_utils-1.4.2/LICENSE
--rw-r--r--   0        0        0      506 2024-03-19 14:15:25.221026 sat_utils-1.4.2/Makefile
--rw-r--r--   0        0        0     2355 2024-03-19 14:15:25.221026 sat_utils-1.4.2/README.md
--rw-r--r--   0        0        0       24 2024-03-19 14:15:25.221026 sat_utils-1.4.2/bandit.yml
--rw-r--r--   0        0        0      907 2024-03-19 14:15:25.221026 sat_utils-1.4.2/docs/db.md
--rw-r--r--   0        0        0    14648 2024-03-19 14:15:25.221026 sat_utils-1.4.2/notebooks/test_gravity_forms.ipynb
--rw-r--r--   0        0        0     2552 2024-03-19 14:15:25.221026 sat_utils-1.4.2/pyproject.toml
--rw-r--r--   0        0        0      214 2024-03-19 14:15:25.221026 sat_utils-1.4.2/pytest.ini
--rw-r--r--   0        0        0      827 2024-03-19 14:15:25.221026 sat_utils-1.4.2/requirements/base/base.txt
--rw-r--r--   0        0        0     9433 2024-03-19 14:15:25.221026 sat_utils-1.4.2/requirements/dev/dev.txt
--rw-r--r--   0        0        0       56 2024-03-19 14:15:25.221026 sat_utils-1.4.2/sat/__init__.py
--rw-r--r--   0        0        0     1152 2024-03-19 14:15:25.221026 sat_utils-1.4.2/sat/db.py
--rw-r--r--   0        0        0     7361 2024-03-19 14:15:25.221026 sat_utils-1.4.2/sat/gravity_forms.py
--rw-r--r--   0        0        0     1435 2024-03-19 14:15:25.221026 sat_utils-1.4.2/sat/logs.py
--rw-r--r--   0        0        0     1597 2024-03-19 14:15:25.221026 sat_utils-1.4.2/sat/slack.py
--rw-r--r--   0        0        0        0 2024-03-19 14:15:25.221026 sat_utils-1.4.2/tests/__init__.py
--rw-r--r--   0        0        0     1300 2024-03-19 14:15:25.221026 sat_utils-1.4.2/tests/test_db.py
--rw-r--r--   0        0        0     5664 2024-03-19 14:15:25.221026 sat_utils-1.4.2/tests/test_gravity_forms.py
--rw-r--r--   0        0        0     1101 2024-03-19 14:15:25.221026 sat_utils-1.4.2/tests/test_logger.py
--rw-r--r--   0        0        0      538 2024-03-19 14:15:25.221026 sat_utils-1.4.2/tests/test_slack.py
--rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 sat_utils-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0       49 2024-04-17 13:25:03.756410 sat_utils-1.4.3/.coveragerc
+-rw-r--r--   0        0        0      220 2024-04-17 13:25:03.756410 sat_utils-1.4.3/.editorconfig
+-rw-r--r--   0        0        0      494 2024-04-17 13:25:03.756410 sat_utils-1.4.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     8456 2024-04-17 13:25:03.756410 sat_utils-1.4.3/.github/workflows/test_publish_and_release.yml
+-rw-r--r--   0        0        0     3186 2024-04-17 13:25:03.760409 sat_utils-1.4.3/.gitignore
+-rw-r--r--   0        0        0      875 2024-04-17 13:25:03.760409 sat_utils-1.4.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1102 2024-04-17 13:25:03.760409 sat_utils-1.4.3/LICENSE
+-rw-r--r--   0        0        0      506 2024-04-17 13:25:03.760409 sat_utils-1.4.3/Makefile
+-rw-r--r--   0        0        0     2355 2024-04-17 13:25:03.760409 sat_utils-1.4.3/README.md
+-rw-r--r--   0        0        0       24 2024-04-17 13:25:03.760409 sat_utils-1.4.3/bandit.yml
+-rw-r--r--   0        0        0      907 2024-04-17 13:25:03.760409 sat_utils-1.4.3/docs/db.md
+-rw-r--r--   0        0        0    14648 2024-04-17 13:25:03.760409 sat_utils-1.4.3/notebooks/test_gravity_forms.ipynb
+-rw-r--r--   0        0        0     2552 2024-04-17 13:25:03.760409 sat_utils-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0      214 2024-04-17 13:25:03.760409 sat_utils-1.4.3/pytest.ini
+-rw-r--r--   0        0        0      827 2024-04-17 13:25:03.760409 sat_utils-1.4.3/requirements/base/base.txt
+-rw-r--r--   0        0        0     9433 2024-04-17 13:25:03.760409 sat_utils-1.4.3/requirements/dev/dev.txt
+-rw-r--r--   0        0        0       56 2024-04-17 13:25:03.760409 sat_utils-1.4.3/sat/__init__.py
+-rw-r--r--   0        0        0     1152 2024-04-17 13:25:03.760409 sat_utils-1.4.3/sat/db.py
+-rw-r--r--   0        0        0     7557 2024-04-17 13:25:03.760409 sat_utils-1.4.3/sat/gravity_forms.py
+-rw-r--r--   0        0        0     1435 2024-04-17 13:25:03.760409 sat_utils-1.4.3/sat/logs.py
+-rw-r--r--   0        0        0     1597 2024-04-17 13:25:03.760409 sat_utils-1.4.3/sat/slack.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:25:03.760409 sat_utils-1.4.3/tests/__init__.py
+-rw-r--r--   0        0        0     1300 2024-04-17 13:25:03.760409 sat_utils-1.4.3/tests/test_db.py
+-rw-r--r--   0        0        0     5664 2024-04-17 13:25:03.760409 sat_utils-1.4.3/tests/test_gravity_forms.py
+-rw-r--r--   0        0        0     1101 2024-04-17 13:25:03.760409 sat_utils-1.4.3/tests/test_logger.py
+-rw-r--r--   0        0        0      538 2024-04-17 13:25:03.760409 sat_utils-1.4.3/tests/test_slack.py
+-rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 sat_utils-1.4.3/PKG-INFO
```

### Comparing `sat_utils-1.4.2/.github/workflows/test_publish_and_release.yml` & `sat_utils-1.4.3/.github/workflows/test_publish_and_release.yml`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/.gitignore` & `sat_utils-1.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/.pre-commit-config.yaml` & `sat_utils-1.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/LICENSE` & `sat_utils-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/README.md` & `sat_utils-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/docs/db.md` & `sat_utils-1.4.3/docs/db.md`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/notebooks/test_gravity_forms.ipynb` & `sat_utils-1.4.3/notebooks/test_gravity_forms.ipynb`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/pyproject.toml` & `sat_utils-1.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sat-utils"
-version = "1.4.2"
+version = "1.4.3"
 authors = [
     { name="Ryan Semmler", email="rsemmle@ncsu.edu" },
     { name="Shawn Taylor", email="staylor8@ncsu.edu" },
     { name="Jeremy Gibson", email="jmgibso3@ncsu.edu"},
     { name="John Champion", email="jtchampi@ncsu.edu"}
 ]
 description = "Contains a collection of shared utility functions"
```

### Comparing `sat_utils-1.4.2/requirements/base/base.txt` & `sat_utils-1.4.3/requirements/base/base.txt`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/requirements/dev/dev.txt` & `sat_utils-1.4.3/requirements/dev/dev.txt`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/sat/db.py` & `sat_utils-1.4.3/sat/db.py`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/sat/gravity_forms.py` & `sat_utils-1.4.3/sat/gravity_forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -236,13 +236,20 @@
         Parameters:
         - form_id: The ID of the entry.
         """
         response = self.get(f"/entries/{entry_id}")
         entry = Entry(**response)
         return entry
 
-    def search_entry(self, field_filters: str, form_id: int):
-        response = self.get(f"/forms/{form_id}/entries", params={"search": field_filters})
+    def search_entry(self, field_filters: str, form_id: int, page: int = 1, page_size: int = 20):
+        response = self.get(
+            f"/forms/{form_id}/entries",
+            params={
+                "search": field_filters,
+                "paging[current_page]": page,
+                "paging[page_size]": page_size,
+            },
+        )
         entries = []
         for entry in response.get("entries"):
             entries.append(Entry(**entry))
         return entries
```

### Comparing `sat_utils-1.4.2/sat/logs.py` & `sat_utils-1.4.3/sat/logs.py`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/sat/slack.py` & `sat_utils-1.4.3/sat/slack.py`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/tests/test_db.py` & `sat_utils-1.4.3/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/tests/test_gravity_forms.py` & `sat_utils-1.4.3/tests/test_gravity_forms.py`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/tests/test_logger.py` & `sat_utils-1.4.3/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/tests/test_slack.py` & `sat_utils-1.4.3/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `sat_utils-1.4.2/PKG-INFO` & `sat_utils-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sat-utils
-Version: 1.4.2
+Version: 1.4.3
 Summary: Contains a collection of shared utility functions
 Author-email: Ryan Semmler <rsemmle@ncsu.edu>, Shawn Taylor <staylor8@ncsu.edu>, Jeremy Gibson <jmgibso3@ncsu.edu>, John Champion <jtchampi@ncsu.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: slack-sdk==3.27.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: cx_Oracle==8.3.0
```

