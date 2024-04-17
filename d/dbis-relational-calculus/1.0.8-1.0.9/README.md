# Comparing `tmp/dbis-relational-calculus-1.0.8.tar.gz` & `tmp/dbis-relational-calculus-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-relational-calculus-1.0.8.tar", last modified: Tue Jun 13 16:56:59 2023, max compression
+gzip compressed data, was "dbis-relational-calculus-1.0.9.tar", last modified: Fri Dec 22 12:50:43 2023, max compression
```

## Comparing `dbis-relational-calculus-1.0.8.tar` & `dbis-relational-calculus-1.0.9.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 16:56:59.807143 dbis-relational-calculus-1.0.8/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/LICENSE
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-06-13 16:56:59.807143 dbis-relational-calculus-1.0.8/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11343 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/README.md
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 16:56:59.805143 dbis-relational-calculus-1.0.8/dbis_relational_calculus.egg-info/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-06-13 16:56:59.000000 dbis-relational-calculus-1.0.8/dbis_relational_calculus.egg-info/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2739 2023-06-13 16:56:59.000000 dbis-relational-calculus-1.0.8/dbis_relational_calculus.egg-info/SOURCES.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-06-13 16:56:59.000000 dbis-relational-calculus-1.0.8/dbis_relational_calculus.egg-info/dependency_links.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       32 2023-06-13 16:56:59.000000 dbis-relational-calculus-1.0.8/dbis_relational_calculus.egg-info/requires.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       20 2023-06-13 16:56:59.000000 dbis-relational-calculus-1.0.8/dbis_relational_calculus.egg-info/top_level.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      709 2023-06-13 16:56:33.000000 dbis-relational-calculus-1.0.8/pyproject.toml
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 16:56:59.805143 dbis-relational-calculus-1.0.8/relational_calculus/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/relational_calculus/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 16:56:59.805143 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6956 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/DomainCalculus.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      953 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/Result.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      546 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/Variable.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1358 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 16:56:59.805143 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8504 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/Formula.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4546 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/Tuple.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 16:56:59.806143 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/atoms/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2840 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/atoms/Equals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2692 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2679 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2680 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2667 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/atoms/LessThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/atoms/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 16:56:59.806143 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/connectives/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7748 2023-06-13 16:56:33.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/connectives/And.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3397 2023-06-13 16:36:39.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/connectives/Not.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7725 2023-06-13 16:56:33.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/connectives/Or.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/connectives/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 16:56:59.806143 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/quantifiers/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4719 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4583 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/quantifiers/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 16:56:59.806143 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1182 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/Result.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4105 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/TupleCalculus.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1281 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 16:56:59.806143 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11218 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/Formula.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2289 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/Variable.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 16:56:59.806143 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/atoms/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4080 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/atoms/Equals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3940 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3929 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3931 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3917 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/atoms/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 16:56:59.806143 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/connectives/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12660 2023-06-13 16:56:33.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/connectives/And.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4600 2023-06-13 16:56:33.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/connectives/Not.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12619 2023-06-13 16:56:33.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/connectives/Or.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/connectives/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 16:56:59.807143 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/quantifiers/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8794 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8543 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/quantifiers/__init__.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-06-13 16:56:59.807143 dbis-relational-calculus-1.0.8/setup.cfg
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 16:56:59.807143 dbis-relational-calculus-1.0.8/tests/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4425 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/tests/test_domain_calculus_sql.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      580 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/tests/test_domain_calculus_validity.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3100 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/tests/test_tuple_calculus_attribute_access.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4388 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/tests/test_tuple_calculus_sql.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      733 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.8/tests/test_tuple_calculus_validity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 12:50:43.145186 dbis-relational-calculus-1.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-02-06 12:04:28.000000 dbis-relational-calculus-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11899 2023-12-22 12:50:43.145186 dbis-relational-calculus-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11343 2023-02-06 12:04:28.000000 dbis-relational-calculus-1.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      709 2023-12-22 12:34:17.000000 dbis-relational-calculus-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-12-22 12:50:43.145186 dbis-relational-calculus-1.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 12:50:43.133185 dbis-relational-calculus-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 12:50:43.145186 dbis-relational-calculus-1.0.9/src/dbis_relational_calculus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11899 2023-12-22 12:50:43.000000 dbis-relational-calculus-1.0.9/src/dbis_relational_calculus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-12-22 12:50:43.000000 dbis-relational-calculus-1.0.9/src/dbis_relational_calculus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-22 12:50:43.000000 dbis-relational-calculus-1.0.9/src/dbis_relational_calculus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-12-22 12:50:43.000000 dbis-relational-calculus-1.0.9/src/dbis_relational_calculus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-12-22 12:50:43.000000 dbis-relational-calculus-1.0.9/src/dbis_relational_calculus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 12:50:43.137186 dbis-relational-calculus-1.0.9/src/relational_calculus/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 12:50:43.137186 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/
+-rw-rw-rw-   0 root         (0) root         (0)     6956 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/DomainCalculus.py
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/Result.py
+-rw-rw-rw-   0 root         (0) root         (0)      546 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/Variable.py
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 12:50:43.137186 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/
+-rw-rw-rw-   0 root         (0) root         (0)     8504 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/Formula.py
+-rw-rw-rw-   0 root         (0) root         (0)     4546 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/Tuple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 12:50:43.137186 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/atoms/
+-rw-rw-rw-   0 root         (0) root         (0)     2840 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/atoms/Equals.py
+-rw-rw-rw-   0 root         (0) root         (0)     2692 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py
+-rw-rw-rw-   0 root         (0) root         (0)     2679 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py
+-rw-rw-rw-   0 root         (0) root         (0)     2680 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/atoms/LessThan.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/atoms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 12:50:43.141186 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/connectives/
+-rw-rw-rw-   0 root         (0) root         (0)     7748 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/connectives/And.py
+-rw-rw-rw-   0 root         (0) root         (0)     3397 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/connectives/Not.py
+-rw-rw-rw-   0 root         (0) root         (0)     7725 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/connectives/Or.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/connectives/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 12:50:43.141186 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/quantifiers/
+-rw-rw-rw-   0 root         (0) root         (0)     4719 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py
+-rw-rw-rw-   0 root         (0) root         (0)     4583 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/quantifiers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 12:50:43.141186 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/Result.py
+-rw-rw-rw-   0 root         (0) root         (0)     4105 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/TupleCalculus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1281 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 12:50:43.141186 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/
+-rw-rw-rw-   0 root         (0) root         (0)    11218 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/Formula.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/Variable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 12:50:43.141186 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/atoms/
+-rw-rw-rw-   0 root         (0) root         (0)     4080 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/atoms/Equals.py
+-rw-rw-rw-   0 root         (0) root         (0)     3940 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py
+-rw-rw-rw-   0 root         (0) root         (0)     3929 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py
+-rw-rw-rw-   0 root         (0) root         (0)     3931 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py
+-rw-rw-rw-   0 root         (0) root         (0)     3917 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/atoms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 12:50:43.141186 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/connectives/
+-rw-rw-rw-   0 root         (0) root         (0)    12660 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/connectives/And.py
+-rw-rw-rw-   0 root         (0) root         (0)     4600 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/connectives/Not.py
+-rw-rw-rw-   0 root         (0) root         (0)    12619 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/connectives/Or.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/connectives/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 12:50:43.145186 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/quantifiers/
+-rw-rw-rw-   0 root         (0) root         (0)     8794 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py
+-rw-rw-rw-   0 root         (0) root         (0)     8543 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-22 12:23:15.000000 dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/quantifiers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-22 12:50:43.145186 dbis-relational-calculus-1.0.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4425 2023-02-06 12:04:28.000000 dbis-relational-calculus-1.0.9/tests/test_domain_calculus_sql.py
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-02-06 12:04:28.000000 dbis-relational-calculus-1.0.9/tests/test_domain_calculus_validity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3100 2023-02-06 12:04:28.000000 dbis-relational-calculus-1.0.9/tests/test_tuple_calculus_attribute_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4388 2023-02-06 12:04:28.000000 dbis-relational-calculus-1.0.9/tests/test_tuple_calculus_sql.py
+-rw-rw-rw-   0 root         (0) root         (0)      733 2023-02-06 12:04:28.000000 dbis-relational-calculus-1.0.9/tests/test_tuple_calculus_validity.py
```

### Comparing `dbis-relational-calculus-1.0.8/LICENSE` & `dbis-relational-calculus-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/PKG-INFO` & `dbis-relational-calculus-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: dbis-relational-calculus
-Version: 1.0.8
+Version: 1.0.9
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis-relational-calculus
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: docstring_inheritance
+Requires-Dist: typeguard
 
 # DBIS Relational Calculus
 
 [![pypi](https://img.shields.io/pypi/pyversions/dbis-relational-calculus)](https://pypi.org/project/dbis-relational-calculus/)
 [![PyPI Status](https://img.shields.io/pypi/v/dbis-relational-calculus)](https://pypi.org/project/dbis-relational-calculus/)
 
 This set of classes is used to define objects of the relational model (as a result of a conversion from an ER-diagram)
```

### Comparing `dbis-relational-calculus-1.0.8/README.md` & `dbis-relational-calculus-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/dbis_relational_calculus.egg-info/PKG-INFO` & `dbis-relational-calculus-1.0.9/src/dbis_relational_calculus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: dbis-relational-calculus
-Version: 1.0.8
+Version: 1.0.9
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis-relational-calculus
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: docstring_inheritance
+Requires-Dist: typeguard
 
 # DBIS Relational Calculus
 
 [![pypi](https://img.shields.io/pypi/pyversions/dbis-relational-calculus)](https://pypi.org/project/dbis-relational-calculus/)
 [![PyPI Status](https://img.shields.io/pypi/v/dbis-relational-calculus)](https://pypi.org/project/dbis-relational-calculus/)
 
 This set of classes is used to define objects of the relational model (as a result of a conversion from an ER-diagram)
```

### Comparing `dbis-relational-calculus-1.0.8/dbis_relational_calculus.egg-info/SOURCES.txt` & `dbis-relational-calculus-1.0.9/src/dbis_relational_calculus.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 LICENSE
 README.md
 pyproject.toml
-dbis_relational_calculus.egg-info/PKG-INFO
-dbis_relational_calculus.egg-info/SOURCES.txt
-dbis_relational_calculus.egg-info/dependency_links.txt
-dbis_relational_calculus.egg-info/requires.txt
-dbis_relational_calculus.egg-info/top_level.txt
-relational_calculus/__init__.py
-relational_calculus/domain_calculus/DomainCalculus.py
-relational_calculus/domain_calculus/Result.py
-relational_calculus/domain_calculus/Variable.py
-relational_calculus/domain_calculus/__init__.py
-relational_calculus/domain_calculus/formulas/Formula.py
-relational_calculus/domain_calculus/formulas/Tuple.py
-relational_calculus/domain_calculus/formulas/atoms/Equals.py
-relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py
-relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py
-relational_calculus/domain_calculus/formulas/atoms/LessEquals.py
-relational_calculus/domain_calculus/formulas/atoms/LessThan.py
-relational_calculus/domain_calculus/formulas/atoms/__init__.py
-relational_calculus/domain_calculus/formulas/connectives/And.py
-relational_calculus/domain_calculus/formulas/connectives/Not.py
-relational_calculus/domain_calculus/formulas/connectives/Or.py
-relational_calculus/domain_calculus/formulas/connectives/__init__.py
-relational_calculus/domain_calculus/formulas/quantifiers/Exists.py
-relational_calculus/domain_calculus/formulas/quantifiers/Forall.py
-relational_calculus/domain_calculus/formulas/quantifiers/__init__.py
-relational_calculus/tuple_calculus/Result.py
-relational_calculus/tuple_calculus/TupleCalculus.py
-relational_calculus/tuple_calculus/__init__.py
-relational_calculus/tuple_calculus/formulas/Formula.py
-relational_calculus/tuple_calculus/formulas/Variable.py
-relational_calculus/tuple_calculus/formulas/atoms/Equals.py
-relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py
-relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py
-relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py
-relational_calculus/tuple_calculus/formulas/atoms/LessThan.py
-relational_calculus/tuple_calculus/formulas/atoms/__init__.py
-relational_calculus/tuple_calculus/formulas/connectives/And.py
-relational_calculus/tuple_calculus/formulas/connectives/Not.py
-relational_calculus/tuple_calculus/formulas/connectives/Or.py
-relational_calculus/tuple_calculus/formulas/connectives/__init__.py
-relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py
-relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py
-relational_calculus/tuple_calculus/formulas/quantifiers/__init__.py
+src/dbis_relational_calculus.egg-info/PKG-INFO
+src/dbis_relational_calculus.egg-info/SOURCES.txt
+src/dbis_relational_calculus.egg-info/dependency_links.txt
+src/dbis_relational_calculus.egg-info/requires.txt
+src/dbis_relational_calculus.egg-info/top_level.txt
+src/relational_calculus/__init__.py
+src/relational_calculus/domain_calculus/DomainCalculus.py
+src/relational_calculus/domain_calculus/Result.py
+src/relational_calculus/domain_calculus/Variable.py
+src/relational_calculus/domain_calculus/__init__.py
+src/relational_calculus/domain_calculus/formulas/Formula.py
+src/relational_calculus/domain_calculus/formulas/Tuple.py
+src/relational_calculus/domain_calculus/formulas/atoms/Equals.py
+src/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py
+src/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py
+src/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py
+src/relational_calculus/domain_calculus/formulas/atoms/LessThan.py
+src/relational_calculus/domain_calculus/formulas/atoms/__init__.py
+src/relational_calculus/domain_calculus/formulas/connectives/And.py
+src/relational_calculus/domain_calculus/formulas/connectives/Not.py
+src/relational_calculus/domain_calculus/formulas/connectives/Or.py
+src/relational_calculus/domain_calculus/formulas/connectives/__init__.py
+src/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py
+src/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py
+src/relational_calculus/domain_calculus/formulas/quantifiers/__init__.py
+src/relational_calculus/tuple_calculus/Result.py
+src/relational_calculus/tuple_calculus/TupleCalculus.py
+src/relational_calculus/tuple_calculus/__init__.py
+src/relational_calculus/tuple_calculus/formulas/Formula.py
+src/relational_calculus/tuple_calculus/formulas/Variable.py
+src/relational_calculus/tuple_calculus/formulas/atoms/Equals.py
+src/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py
+src/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py
+src/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py
+src/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py
+src/relational_calculus/tuple_calculus/formulas/atoms/__init__.py
+src/relational_calculus/tuple_calculus/formulas/connectives/And.py
+src/relational_calculus/tuple_calculus/formulas/connectives/Not.py
+src/relational_calculus/tuple_calculus/formulas/connectives/Or.py
+src/relational_calculus/tuple_calculus/formulas/connectives/__init__.py
+src/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py
+src/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py
+src/relational_calculus/tuple_calculus/formulas/quantifiers/__init__.py
 tests/test_domain_calculus_sql.py
 tests/test_domain_calculus_validity.py
 tests/test_tuple_calculus_attribute_access.py
 tests/test_tuple_calculus_sql.py
 tests/test_tuple_calculus_validity.py
```

### Comparing `dbis-relational-calculus-1.0.8/pyproject.toml` & `dbis-relational-calculus-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbis-relational-calculus"
-version = "1.0.8"
+version = "1.0.9"
 description = "RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 authors = [
 	{ name = "Til Mohr", email = "til.mohr@rwth-aachen.de" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/DomainCalculus.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/DomainCalculus.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/Result.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/Result.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/Variable.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/Variable.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/__init__.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/__init__.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/Formula.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/Formula.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/Tuple.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/Tuple.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/atoms/Equals.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/atoms/Equals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/atoms/LessThan.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/atoms/LessThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/connectives/And.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/connectives/And.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/connectives/Not.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/connectives/Not.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/connectives/Or.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/connectives/Or.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/Result.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/Result.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/TupleCalculus.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/TupleCalculus.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/__init__.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/__init__.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/Formula.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/Formula.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/Variable.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/Variable.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/atoms/Equals.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/atoms/Equals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/connectives/And.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/connectives/And.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/connectives/Not.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/connectives/Not.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/connectives/Or.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/connectives/Or.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py` & `dbis-relational-calculus-1.0.9/src/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/tests/test_domain_calculus_sql.py` & `dbis-relational-calculus-1.0.9/tests/test_domain_calculus_sql.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/tests/test_domain_calculus_validity.py` & `dbis-relational-calculus-1.0.9/tests/test_domain_calculus_validity.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/tests/test_tuple_calculus_attribute_access.py` & `dbis-relational-calculus-1.0.9/tests/test_tuple_calculus_attribute_access.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/tests/test_tuple_calculus_sql.py` & `dbis-relational-calculus-1.0.9/tests/test_tuple_calculus_sql.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.8/tests/test_tuple_calculus_validity.py` & `dbis-relational-calculus-1.0.9/tests/test_tuple_calculus_validity.py`

 * *Files identical despite different names*

