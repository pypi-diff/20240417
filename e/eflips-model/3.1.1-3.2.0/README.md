# Comparing `tmp/eflips_model-3.1.1.tar.gz` & `tmp/eflips_model-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips_model-3.1.1.tar", max compression
+gzip compressed data, was "eflips_model-3.2.0.tar", max compression
```

## Comparing `eflips_model-3.1.1.tar` & `eflips_model-3.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34260 2024-01-25 14:04:47.012623 eflips_model-3.1.1/LICENSE.md
--rw-r--r--   0        0        0     6274 2024-02-13 18:22:20.940626 eflips_model-3.1.1/README.md
--rw-r--r--   0        0        0     2522 2024-02-13 18:22:20.941222 eflips_model-3.1.1/eflips/model/__init__.py
--rw-r--r--   0        0        0     3556 2024-02-13 18:22:20.941461 eflips_model-3.1.1/eflips/model/alembic.ini
--rw-r--r--   0        0        0    11793 2024-03-27 12:26:56.120307 eflips_model-3.1.1/eflips/model/depot.py
--rw-r--r--   0        0        0    34913 2024-03-25 15:41:52.646414 eflips_model-3.1.1/eflips/model/general.py
--rw-r--r--   0        0        0     2772 2024-03-15 12:08:31.037325 eflips_model-3.1.1/eflips/model/migrations/env.py
--rw-r--r--   0        0        0      635 2024-02-13 18:22:20.942988 eflips_model-3.1.1/eflips/model/migrations/script.py.mako
--rw-r--r--   0        0        0      969 2024-03-25 15:41:52.646712 eflips_model-3.1.1/eflips/model/migrations/versions/0548463664b4_3_1_0.py
--rw-r--r--   0        0        0      938 2024-02-13 18:22:20.943365 eflips_model-3.1.1/eflips/model/migrations/versions/126892076499_v2_0_0.py
--rw-r--r--   0        0        0     1187 2024-03-18 18:50:34.912225 eflips_model-3.1.1/eflips/model/migrations/versions/6ac022147397_3_0_0.py
--rw-r--r--   0        0        0     1316 2024-02-14 17:51:30.276962 eflips_model-3.1.1/eflips/model/migrations/versions/7483339ae654_v2_2_0.py
--rw-r--r--   0        0        0      665 2024-02-13 18:22:20.943781 eflips_model-3.1.1/eflips/model/migrations/versions/9e29124f8ce6_v1_1_6.py
--rw-r--r--   0        0        0     1497 2024-02-13 18:22:20.944022 eflips_model-3.1.1/eflips/model/migrations/versions/a06c97c98d2c_v2_1_0.py
--rw-r--r--   0        0        0     1048 2024-03-18 18:50:34.912522 eflips_model-3.1.1/eflips/model/migrations/versions/a9f1c33488b6_3_0_0.py
--rw-r--r--   0        0        0      798 2024-02-27 15:24:32.595397 eflips_model-3.1.1/eflips/model/migrations/versions/baef3598b52c_v2_3_0.py
--rw-r--r--   0        0        0    15938 2024-03-18 18:50:34.913013 eflips_model-3.1.1/eflips/model/network.py
--rw-r--r--   0        0        0        0 2024-01-25 14:06:07.781569 eflips_model-3.1.1/eflips/model/py.typed
--rw-r--r--   0        0        0    14194 2024-03-18 18:50:34.913435 eflips_model-3.1.1/eflips/model/schedule.py
--rw-r--r--   0        0        0      920 2024-03-27 12:27:15.060022 eflips_model-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     7245 1970-01-01 00:00:00.000000 eflips_model-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34260 2024-01-25 14:04:47.012623 eflips_model-3.2.0/LICENSE.md
+-rw-r--r--   0        0        0     6274 2024-02-13 18:22:20.940626 eflips_model-3.2.0/README.md
+-rw-r--r--   0        0        0     2522 2024-02-13 18:22:20.941222 eflips_model-3.2.0/eflips/model/__init__.py
+-rw-r--r--   0        0        0     3556 2024-02-13 18:22:20.941461 eflips_model-3.2.0/eflips/model/alembic.ini
+-rw-r--r--   0        0        0    11793 2024-04-17 07:02:23.238136 eflips_model-3.2.0/eflips/model/depot.py
+-rw-r--r--   0        0        0    34829 2024-04-17 07:02:23.259349 eflips_model-3.2.0/eflips/model/general.py
+-rw-r--r--   0        0        0     2772 2024-03-15 12:08:31.037325 eflips_model-3.2.0/eflips/model/migrations/env.py
+-rw-r--r--   0        0        0      635 2024-02-13 18:22:20.942988 eflips_model-3.2.0/eflips/model/migrations/script.py.mako
+-rw-r--r--   0        0        0      969 2024-03-25 15:41:52.646712 eflips_model-3.2.0/eflips/model/migrations/versions/0548463664b4_3_1_0.py
+-rw-r--r--   0        0        0      938 2024-02-13 18:22:20.943365 eflips_model-3.2.0/eflips/model/migrations/versions/126892076499_v2_0_0.py
+-rw-r--r--   0        0        0     1187 2024-03-18 18:50:34.912225 eflips_model-3.2.0/eflips/model/migrations/versions/6ac022147397_3_0_0.py
+-rw-r--r--   0        0        0     1316 2024-02-14 17:51:30.276962 eflips_model-3.2.0/eflips/model/migrations/versions/7483339ae654_v2_2_0.py
+-rw-r--r--   0        0        0      665 2024-02-13 18:22:20.943781 eflips_model-3.2.0/eflips/model/migrations/versions/9e29124f8ce6_v1_1_6.py
+-rw-r--r--   0        0        0     1497 2024-02-13 18:22:20.944022 eflips_model-3.2.0/eflips/model/migrations/versions/a06c97c98d2c_v2_1_0.py
+-rw-r--r--   0        0        0     1048 2024-03-18 18:50:34.912522 eflips_model-3.2.0/eflips/model/migrations/versions/a9f1c33488b6_3_0_0.py
+-rw-r--r--   0        0        0      798 2024-02-27 15:24:32.595397 eflips_model-3.2.0/eflips/model/migrations/versions/baef3598b52c_v2_3_0.py
+-rw-r--r--   0        0        0    15938 2024-03-18 18:50:34.913013 eflips_model-3.2.0/eflips/model/network.py
+-rw-r--r--   0        0        0        0 2024-01-25 14:06:07.781569 eflips_model-3.2.0/eflips/model/py.typed
+-rw-r--r--   0        0        0    14194 2024-03-18 18:50:34.913435 eflips_model-3.2.0/eflips/model/schedule.py
+-rw-r--r--   0        0        0      920 2024-04-17 07:02:50.829619 eflips_model-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7245 1970-01-01 00:00:00.000000 eflips_model-3.2.0/PKG-INFO
```

### Comparing `eflips_model-3.1.1/LICENSE.md` & `eflips_model-3.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/README.md` & `eflips_model-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/eflips/model/__init__.py` & `eflips_model-3.2.0/eflips/model/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/eflips/model/alembic.ini` & `eflips_model-3.2.0/eflips/model/alembic.ini`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/eflips/model/depot.py` & `eflips_model-3.2.0/eflips/model/depot.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/eflips/model/general.py` & `eflips_model-3.2.0/eflips/model/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -825,16 +825,14 @@
         ExcludeConstraint(  # type: ignore
             (Column("scenario_id"), "="),
             (Column("vehicle_id"), "="),
             (func.tstzrange(Column("time_start"), Column("time_end"), "()"), "&&"),
             name="scenario_id_time_range_excl",
             using="gist",
         ),
-        CheckConstraint("soc_start >= 0"),
-        CheckConstraint("soc_end >= 0"),
         CheckConstraint("soc_start <= 1"),
         CheckConstraint("soc_end <= 1"),
         # Also make sure the event type is valid for the nullable fields
         CheckConstraint(
             "(station_id IS NOT NULL AND subloc_no IS NOT NULL AND event_type IN ('CHARGING_OPPORTUNITY')) OR "
             "(area_id IS NOT NULL AND subloc_no IS NOT NULL AND event_type IN ('CHARGING_DEPOT', 'SERVICE', "
             "'STANDBY_DEPARTURE', 'STANDBY', 'PRECONDITIONING')) OR"
```

### Comparing `eflips_model-3.1.1/eflips/model/migrations/env.py` & `eflips_model-3.2.0/eflips/model/migrations/env.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/eflips/model/migrations/script.py.mako` & `eflips_model-3.2.0/eflips/model/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/eflips/model/migrations/versions/0548463664b4_3_1_0.py` & `eflips_model-3.2.0/eflips/model/migrations/versions/0548463664b4_3_1_0.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/eflips/model/migrations/versions/126892076499_v2_0_0.py` & `eflips_model-3.2.0/eflips/model/migrations/versions/126892076499_v2_0_0.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/eflips/model/migrations/versions/6ac022147397_3_0_0.py` & `eflips_model-3.2.0/eflips/model/migrations/versions/6ac022147397_3_0_0.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/eflips/model/migrations/versions/7483339ae654_v2_2_0.py` & `eflips_model-3.2.0/eflips/model/migrations/versions/7483339ae654_v2_2_0.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/eflips/model/migrations/versions/9e29124f8ce6_v1_1_6.py` & `eflips_model-3.2.0/eflips/model/migrations/versions/9e29124f8ce6_v1_1_6.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/eflips/model/migrations/versions/a06c97c98d2c_v2_1_0.py` & `eflips_model-3.2.0/eflips/model/migrations/versions/a06c97c98d2c_v2_1_0.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/eflips/model/migrations/versions/a9f1c33488b6_3_0_0.py` & `eflips_model-3.2.0/eflips/model/migrations/versions/a9f1c33488b6_3_0_0.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/eflips/model/migrations/versions/baef3598b52c_v2_3_0.py` & `eflips_model-3.2.0/eflips/model/migrations/versions/baef3598b52c_v2_3_0.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/eflips/model/network.py` & `eflips_model-3.2.0/eflips/model/network.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/eflips/model/schedule.py` & `eflips_model-3.2.0/eflips/model/schedule.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.1.1/pyproject.toml` & `eflips_model-3.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eflips-model"
-version = "3.1.1"
+version = "3.2.0"
 description = "A common data model for the eflips family of electric vehicle simulation & optimization tools."
 authors = [
 	"Ludger Heide <ludger.heide@tu-berlin.de>",
 	"Shuyao Guo <shuyao.guo@tu-berlin.de>"
 ]
 readme = "README.md"
 license = "AGPL-3.0-or-later"
```

### Comparing `eflips_model-3.1.1/PKG-INFO` & `eflips_model-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eflips-model
-Version: 3.1.1
+Version: 3.2.0
 Summary: A common data model for the eflips family of electric vehicle simulation & optimization tools.
 Home-page: https://github.com/mpm-tu-berlin/eflips-model
 License: AGPL-3.0-or-later
 Author: Ludger Heide
 Author-email: ludger.heide@tu-berlin.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

