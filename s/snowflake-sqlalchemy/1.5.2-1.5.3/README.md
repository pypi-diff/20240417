# Comparing `tmp/snowflake_sqlalchemy-1.5.2.tar.gz` & `tmp/snowflake_sqlalchemy-1.5.3.tar.gz`

## Comparing `snowflake_sqlalchemy-1.5.2.tar` & `snowflake_sqlalchemy-1.5.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/.gitmodules
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/DESCRIPTION.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/MANIFEST.in
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/license_header.txt
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/setup.cfg
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tox.ini
--rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/build.sh
--rwxr-xr-x   0        0        0      962 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/build_docker.sh
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/set_base_image.sh
--rwxr-xr-x   0        0        0     1011 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/test.sh
--rwxr-xr-x   0        0        0     1637 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/test_docker.sh
--rwxr-xr-x   0        0        0     1100 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/test_linux.sh
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/docker/sqlalchemy_build/Dockerfile
--rwxr-xr-x   0        0        0      277 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/docker/sqlalchemy_build/scripts/entrypoint.sh
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/_constants.py
--rw-r--r--   0        0        0    38942 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/base.py
--rw-r--r--   0        0        0    21461 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/custom_commands.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/custom_types.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/provision.py
--rw-r--r--   0        0        0     9488 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/requirements.py
--rw-r--r--   0        0        0    32313 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/snowdialect.py
--rw-r--r--   0        0        0    13128 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/util.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/version.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tested_requirements/requirements_310.reqs
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tested_requirements/requirements_37.reqs
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tested_requirements/requirements_38.reqs
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tested_requirements/requirements_39.reqs
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/README.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/__init__.py
--rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/conftest.py
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_compiler.py
--rw-r--r--   0        0        0    15087 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_copy.py
--rw-r--r--   0        0        0    68382 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_core.py
--rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_create.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_custom_types.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_geography.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_geometry.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_multivalues_insert.py
--rw-r--r--   0        0        0    12236 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_orm.py
--rw-r--r--   0        0        0    13966 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_pandas.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_qmark.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_quote.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_semi_structured_datatypes.py
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_sequence.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_timestamp.py
--rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_unit_core.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_unit_cte.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_unit_types.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_unit_url.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/util.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/data/users.txt
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/sqlalchemy_test_suite/README.md
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/sqlalchemy_test_suite/__init__.py
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/sqlalchemy_test_suite/conftest.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/sqlalchemy_test_suite/test_suite.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/.gitignore
--rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/LICENSE.txt
--rw-r--r--   0        0        0    18170 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/README.md
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/pyproject.toml
--rw-r--r--   0        0        0    20688 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/.gitmodules
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/DESCRIPTION.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/MANIFEST.in
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/license_header.txt
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/setup.cfg
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tox.ini
+-rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/ci/build.sh
+-rwxr-xr-x   0        0        0      962 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/ci/build_docker.sh
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/ci/set_base_image.sh
+-rwxr-xr-x   0        0        0     1011 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/ci/test.sh
+-rwxr-xr-x   0        0        0     1637 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/ci/test_docker.sh
+-rwxr-xr-x   0        0        0     1100 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/ci/test_linux.sh
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/ci/docker/sqlalchemy_build/Dockerfile
+-rwxr-xr-x   0        0        0      277 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/ci/docker/sqlalchemy_build/scripts/entrypoint.sh
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/_constants.py
+-rw-r--r--   0        0        0    38942 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/base.py
+-rw-r--r--   0        0        0    21461 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/custom_commands.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/custom_types.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/provision.py
+-rw-r--r--   0        0        0     9488 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0    32313 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/snowdialect.py
+-rw-r--r--   0        0        0    13128 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/util.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/version.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tested_requirements/requirements_310.reqs
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tested_requirements/requirements_37.reqs
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tested_requirements/requirements_38.reqs
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tested_requirements/requirements_39.reqs
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/README.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/__init__.py
+-rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/conftest.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_compiler.py
+-rw-r--r--   0        0        0    15087 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_copy.py
+-rw-r--r--   0        0        0    68382 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_core.py
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_create.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_custom_types.py
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_geography.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_geometry.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_multivalues_insert.py
+-rw-r--r--   0        0        0    12236 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_orm.py
+-rw-r--r--   0        0        0    13966 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_pandas.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_qmark.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_quote.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_semi_structured_datatypes.py
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_sequence.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_timestamp.py
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_unit_core.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_unit_cte.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_unit_types.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/test_unit_url.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/util.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/data/users.txt
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/sqlalchemy_test_suite/README.md
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/sqlalchemy_test_suite/__init__.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/sqlalchemy_test_suite/conftest.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/tests/sqlalchemy_test_suite/test_suite.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/.gitignore
+-rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/LICENSE.txt
+-rw-r--r--   0        0        0    18170 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/README.md
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0    20709 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.3/PKG-INFO
```

### Comparing `snowflake_sqlalchemy-1.5.2/.pre-commit-config.yaml` & `snowflake_sqlalchemy-1.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/DESCRIPTION.md` & `snowflake_sqlalchemy-1.5.3/DESCRIPTION.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 <https://docs.snowflake.net/>
 
 Source code is also available at:
 <https://github.com/snowflakedb/snowflake-sqlalchemy>
 
 # Release Notes
 
+- v1.5.3(Unrelased)
+
+  - Limit SQLAlchemy to < 2.0.0 before releasing version compatible with 2.0
+
 - v1.5.2(April 11, 2024)
 
   - Bump min SQLAlchemy to 1.4.19 for outer lateral join
   - Add support for sequence ordering in tests
 
 - v1.5.1(November 03, 2023)
```

### Comparing `snowflake_sqlalchemy-1.5.2/tox.ini` & `snowflake_sqlalchemy-1.5.3/tox.ini`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/ci/build.sh` & `snowflake_sqlalchemy-1.5.3/ci/build.sh`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/ci/build_docker.sh` & `snowflake_sqlalchemy-1.5.3/ci/build_docker.sh`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/ci/set_base_image.sh` & `snowflake_sqlalchemy-1.5.3/ci/set_base_image.sh`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/ci/test.sh` & `snowflake_sqlalchemy-1.5.3/ci/test.sh`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/ci/test_docker.sh` & `snowflake_sqlalchemy-1.5.3/ci/test_docker.sh`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/ci/test_linux.sh` & `snowflake_sqlalchemy-1.5.3/ci/test_linux.sh`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/ci/docker/sqlalchemy_build/Dockerfile` & `snowflake_sqlalchemy-1.5.3/ci/docker/sqlalchemy_build/Dockerfile`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/__init__.py` & `snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/base.py` & `snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/custom_commands.py` & `snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/custom_commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/custom_types.py` & `snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/custom_types.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/requirements.py` & `snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/snowdialect.py` & `snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/snowdialect.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/util.py` & `snowflake_sqlalchemy-1.5.3/src/snowflake/sqlalchemy/util.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/README.rst` & `snowflake_sqlalchemy-1.5.3/tests/README.rst`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/conftest.py` & `snowflake_sqlalchemy-1.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_compiler.py` & `snowflake_sqlalchemy-1.5.3/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_copy.py` & `snowflake_sqlalchemy-1.5.3/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_core.py` & `snowflake_sqlalchemy-1.5.3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_create.py` & `snowflake_sqlalchemy-1.5.3/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_custom_types.py` & `snowflake_sqlalchemy-1.5.3/tests/test_custom_types.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_geography.py` & `snowflake_sqlalchemy-1.5.3/tests/test_geography.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_geometry.py` & `snowflake_sqlalchemy-1.5.3/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_multivalues_insert.py` & `snowflake_sqlalchemy-1.5.3/tests/test_multivalues_insert.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_orm.py` & `snowflake_sqlalchemy-1.5.3/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_pandas.py` & `snowflake_sqlalchemy-1.5.3/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_qmark.py` & `snowflake_sqlalchemy-1.5.3/tests/test_qmark.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_quote.py` & `snowflake_sqlalchemy-1.5.3/tests/test_quote.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_semi_structured_datatypes.py` & `snowflake_sqlalchemy-1.5.3/tests/test_semi_structured_datatypes.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_sequence.py` & `snowflake_sqlalchemy-1.5.3/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_timestamp.py` & `snowflake_sqlalchemy-1.5.3/tests/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_unit_core.py` & `snowflake_sqlalchemy-1.5.3/tests/test_unit_core.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_unit_cte.py` & `snowflake_sqlalchemy-1.5.3/tests/test_unit_cte.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_unit_types.py` & `snowflake_sqlalchemy-1.5.3/tests/test_unit_types.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/test_unit_url.py` & `snowflake_sqlalchemy-1.5.3/tests/test_unit_url.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/util.py` & `snowflake_sqlalchemy-1.5.3/tests/util.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/sqlalchemy_test_suite/README.md` & `snowflake_sqlalchemy-1.5.3/tests/sqlalchemy_test_suite/README.md`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/sqlalchemy_test_suite/conftest.py` & `snowflake_sqlalchemy-1.5.3/tests/sqlalchemy_test_suite/conftest.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/tests/sqlalchemy_test_suite/test_suite.py` & `snowflake_sqlalchemy-1.5.3/tests/sqlalchemy_test_suite/test_suite.py`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/.gitignore` & `snowflake_sqlalchemy-1.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/LICENSE.txt` & `snowflake_sqlalchemy-1.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/README.md` & `snowflake_sqlalchemy-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `snowflake_sqlalchemy-1.5.2/pyproject.toml` & `snowflake_sqlalchemy-1.5.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   "Topic :: Database",
   "Topic :: Scientific/Engineering :: Information Analysis",
   "Topic :: Software Development",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Libraries :: Application Frameworks",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-dependencies = ["snowflake-connector-python", "SQLAlchemy"]
+dependencies = ["snowflake-connector-python<4.0.0", "SQLAlchemy>=1.4.19,<2.0.0"]
 
 [tool.hatch.version]
 path = "src/snowflake/sqlalchemy/version.py"
 
 [project.optional-dependencies]
 development = [
   "pre-commit",
@@ -69,22 +69,17 @@
 [tool.hatch.build.targets.sdist]
 exclude = ["/.github"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/snowflake"]
 
 [tool.hatch.envs.default]
-extra-dependencies = ["SQLAlchemy<2.0.0,>=1.4.19"]
 features = ["development", "pandas"]
 python = "3.8"
 
-[tool.hatch.envs.sa20]
-extra-dependencies = ["SQLAlchemy>=2.0.0"]
-python = "3.8"
-
 [tool.hatch.envs.default.env-vars]
 COVERAGE_FILE = "coverage.xml"
 SQLACHEMY_WARN_20 = "1"
 
 [tool.hatch.envs.default.scripts]
 check = "pre-commit run --all-files"
 test-dialect = "pytest -ra -vvv --tb=short --cov snowflake.sqlalchemy --cov-append --junitxml ./junit.xml --ignore=tests/sqlalchemy_test_suite"
```

### Comparing `snowflake_sqlalchemy-1.5.2/PKG-INFO` & `snowflake_sqlalchemy-1.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snowflake-sqlalchemy
-Version: 1.5.2
+Version: 1.5.3
 Summary: Snowflake SQLAlchemy Dialect
 Project-URL: Changelog, https://github.com/snowflakedb/snowflake-sqlalchemy/blob/main/DESCRIPTION.md
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/sqlalchemy.html
 Project-URL: Homepage, https://www.snowflake.com/
 Project-URL: Issues, https://github.com/snowflakedb/snowflake-sqlalchemy/issues
 Project-URL: Source, https://github.com/snowflakedb/snowflake-sqlalchemy
 Author-email: "Snowflake Inc." <triage-snowpark-python-api-dl@snowflake.com>
@@ -31,16 +31,16 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Requires-Dist: snowflake-connector-python
-Requires-Dist: sqlalchemy
+Requires-Dist: snowflake-connector-python<4.0.0
+Requires-Dist: sqlalchemy<2.0.0,>=1.4.19
 Provides-Extra: development
 Requires-Dist: mock; extra == 'development'
 Requires-Dist: numpy; extra == 'development'
 Requires-Dist: pre-commit; extra == 'development'
 Requires-Dist: pytest; extra == 'development'
 Requires-Dist: pytest-cov; extra == 'development'
 Requires-Dist: pytest-rerunfailures; extra == 'development'
```

