# Comparing `tmp/xmlschema-3.2.1.tar.gz` & `tmp/xmlschema-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmlschema-3.2.1.tar", last modified: Sun Apr  7 16:36:35 2024, max compression
+gzip compressed data, was "xmlschema-3.3.0.tar", last modified: Wed Apr 17 17:34:43 2024, max compression
```

## Comparing `xmlschema-3.2.1.tar` & `xmlschema-3.3.0.tar`

### file list

```diff
@@ -1,572 +1,572 @@
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.223650 xmlschema-3.2.1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2023-03-05 21:16:57.000000 xmlschema-3.2.1/.coveragerc
--rw-r--r--   0 brunato   (1000) brunato   (1000)    28021 2024-04-07 16:34:58.000000 xmlschema-3.2.1/CHANGELOG.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2024-01-07 11:20:34.000000 xmlschema-3.2.1/LICENSE
--rw-r--r--   0 brunato   (1000) brunato   (1000)      330 2023-03-05 20:30:24.000000 xmlschema-3.2.1/MANIFEST.in
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8237 2024-04-07 16:36:35.223650 xmlschema-3.2.1/PKG-INFO
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6120 2024-02-18 21:08:04.000000 xmlschema-3.2.1/README.rst
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.043649 xmlschema-3.2.1/doc/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      606 2018-09-23 09:23:56.000000 xmlschema-3.2.1/doc/Makefile
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11907 2024-03-25 21:28:10.000000 xmlschema-3.2.1/doc/api.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    11273 2021-08-02 14:12:17.000000 xmlschema-3.2.1/doc/components.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5483 2024-04-07 16:34:58.000000 xmlschema-3.2.1/doc/conf.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5499 2022-06-24 14:13:22.000000 xmlschema-3.2.1/doc/converters.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4841 2022-06-24 14:13:22.000000 xmlschema-3.2.1/doc/extras.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9946 2024-03-25 21:28:10.000000 xmlschema-3.2.1/doc/features.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2021-02-05 09:05:33.000000 xmlschema-3.2.1/doc/index.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-05-28 20:30:12.000000 xmlschema-3.2.1/doc/intro.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)       82 2024-02-03 22:44:00.000000 xmlschema-3.2.1/doc/requirements.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5921 2021-04-11 20:19:21.000000 xmlschema-3.2.1/doc/testing.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)    31284 2024-03-25 21:28:10.000000 xmlschema-3.2.1/doc/usage.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-03-07 13:26:41.000000 xmlschema-3.2.1/mypy.ini
--rw-r--r--   0 brunato   (1000) brunato   (1000)       81 2023-09-23 04:52:41.000000 xmlschema-3.2.1/pyproject.toml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2024-03-13 05:27:13.000000 xmlschema-3.2.1/requirements-dev.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2024-04-07 16:36:35.223650 xmlschema-3.2.1/setup.cfg
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)     2765 2024-04-07 16:34:58.000000 xmlschema-3.2.1/setup.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.052649 xmlschema-3.2.1/tests/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-03 21:49:59.000000 xmlschema-3.2.1/tests/__init__.py
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)     6753 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/check_memory.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.020649 xmlschema-3.2.1/tests/templates/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.053649 xmlschema-3.2.1/tests/templates/demo/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-3.2.1/tests/templates/demo/demo_type_filter_test.jinja
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.055649 xmlschema-3.2.1/tests/templates/filters/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       34 2021-02-05 09:05:33.000000 xmlschema-3.2.1/tests/templates/filters/name_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-3.2.1/tests/templates/filters/namespace_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-3.2.1/tests/templates/filters/python_type_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       35 2021-02-05 09:05:33.000000 xmlschema-3.2.1/tests/templates/filters/qname_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       87 2021-02-05 09:05:33.000000 xmlschema-3.2.1/tests/templates/filters/sort_types_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-04-03 19:09:14.000000 xmlschema-3.2.1/tests/templates/filters/type_name_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       40 2021-02-05 09:05:33.000000 xmlschema-3.2.1/tests/templates/filters/type_qname_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       37 2021-04-05 21:38:16.000000 xmlschema-3.2.1/tests/templates/filters/unknown_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-3.2.1/tests/templates/filters/wrong-template.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3576 2024-03-25 21:28:10.000000 xmlschema-3.2.1/tests/test_all.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.055649 xmlschema-3.2.1/tests/test_cases/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.021649 xmlschema-3.2.1/tests/test_cases/examples/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.059649 xmlschema-3.2.1/tests/test_cases/examples/collection/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      925 2020-05-28 20:30:12.000000 xmlschema-3.2.1/tests/test_cases/examples/collection/collection-1_error.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      884 2022-08-26 15:33:28.000000 xmlschema-3.2.1/tests/test_cases/examples/collection/collection-default.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1171 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/examples/collection/collection-redef-xmlns.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      798 2024-04-07 16:30:20.000000 xmlschema-3.2.1/tests/test_cases/examples/collection/collection.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      923 2020-05-28 20:30:12.000000 xmlschema-3.2.1/tests/test_cases/examples/collection/collection.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1599 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/collection/collection.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      941 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/collection/collection2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1736 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/collection/collection2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/collection/collection3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1938 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/collection/collection3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1082 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/collection/collection3bis.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1979 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/collection/collection3bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1364 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/collection/collection4.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1743 2020-11-08 22:15:33.000000 xmlschema-3.2.1/tests/test_cases/examples/collection/collection4.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1658 2022-08-26 15:33:28.000000 xmlschema-3.2.1/tests/test_cases/examples/collection/collection5.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.061649 xmlschema-3.2.1/tests/test_cases/examples/menù/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      559 2023-07-27 19:52:28.000000 xmlschema-3.2.1/tests/test_cases/examples/menù/menù-ascii.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2023-07-27 19:52:28.000000 xmlschema-3.2.1/tests/test_cases/examples/menù/menù-ascii.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      532 2023-07-27 19:52:28.000000 xmlschema-3.2.1/tests/test_cases/examples/menù/menù-cp1252.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      509 2023-07-27 19:52:28.000000 xmlschema-3.2.1/tests/test_cases/examples/menù/menù-cp1252.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)        3 2023-07-27 19:52:28.000000 xmlschema-3.2.1/tests/test_cases/examples/menù/menù.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)      542 2023-07-27 19:52:28.000000 xmlschema-3.2.1/tests/test_cases/examples/menù/menù.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2023-07-27 19:52:28.000000 xmlschema-3.2.1/tests/test_cases/examples/menù/menù.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.062649 xmlschema-3.2.1/tests/test_cases/examples/stockquote/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1039 2020-11-08 22:15:33.000000 xmlschema-3.2.1/tests/test_cases/examples/stockquote/stockquote.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-11-08 22:15:33.000000 xmlschema-3.2.1/tests/test_cases/examples/stockquote/stockquote.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1230 2020-11-08 22:15:33.000000 xmlschema-3.2.1/tests/test_cases/examples/stockquote/stockquoteservice.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.070649 xmlschema-3.2.1/tests/test_cases/examples/vehicles/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/bikes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      469 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/cars.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      595 2022-10-01 13:42:01.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      361 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/types.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:30.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/vehicles-1_error.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/vehicles-1_error.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      475 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/vehicles-2_errors.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:33.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/vehicles-3_errors.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      491 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/vehicles-3_errors.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      557 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/vehicles-max.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/vehicles-redef.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1666 2020-11-15 16:10:20.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip
--rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/vehicles.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      543 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/vehicles.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2020-05-02 09:28:32.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/vehicles2.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      432 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/examples/vehicles/vehicles2.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.022649 xmlschema-3.2.1/tests/test_cases/features/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.071649 xmlschema-3.2.1/tests/test_cases/features/attributes/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      688 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/attributes/default_attributes-missing_group.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      910 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/attributes/default_attributes.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.071649 xmlschema-3.2.1/tests/test_cases/features/builtins/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      584 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/builtins/builtins.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      601 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/builtins/builtins.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.073649 xmlschema-3.2.1/tests/test_cases/features/decoder/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      781 2022-05-20 20:00:14.000000 xmlschema-3.2.1/tests/test_cases/features/decoder/data.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      725 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/decoder/data2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2021-04-01 09:07:37.000000 xmlschema-3.2.1/tests/test_cases/features/decoder/data3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      480 2021-04-05 21:38:16.000000 xmlschema-3.2.1/tests/test_cases/features/decoder/data4-mixed.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      691 2021-12-08 19:41:39.000000 xmlschema-3.2.1/tests/test_cases/features/decoder/long-sequence-1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      727 2021-04-05 21:38:16.000000 xmlschema-3.2.1/tests/test_cases/features/decoder/mixed-content.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5913 2022-05-20 20:00:14.000000 xmlschema-3.2.1/tests/test_cases/features/decoder/simple-types.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.076649 xmlschema-3.2.1/tests/test_cases/features/derivations/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1956 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/derivations/complex-extensions.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      662 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3949 2023-05-18 20:18:16.000000 xmlschema-3.2.1/tests/test_cases/features/derivations/complex11-restrictions.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      599 2023-05-18 20:18:16.000000 xmlschema-3.2.1/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2051 2023-05-18 20:18:16.000000 xmlschema-3.2.1/tests/test_cases/features/derivations/invalid-restrictions1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1027 2023-05-18 20:18:16.000000 xmlschema-3.2.1/tests/test_cases/features/derivations/invalid-restrictions2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      322 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/derivations/list_types.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      675 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/derivations/list_types.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.077649 xmlschema-3.2.1/tests/test_cases/features/elements/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      154 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/elements/test_alternatives-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1487 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/elements/type_alternatives-no-ns.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1543 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/elements/type_alternatives.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.084649 xmlschema-3.2.1/tests/test_cases/features/models/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5143 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/models/billion_laughs_model.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      301 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/models/circular_model.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      215 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/models/illegal-attributes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/models/illegal-declarations.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      523 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/models/illegal-occurs.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1192 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/models/invalid_models1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1541 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/models/invalid_models2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/models/model1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4794 2020-04-28 13:28:56.000000 xmlschema-3.2.1/tests/test_cases/features/models/models.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/models/other-ns.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      760 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/models/recursive-groups.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1062 2020-04-28 13:28:56.000000 xmlschema-3.2.1/tests/test_cases/features/models/valid_model1.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.096649 xmlschema-3.2.1/tests/test_cases/features/namespaces/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      151 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/chameleon1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/chameleon2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      272 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/chameleon3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/default_ns_invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      481 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/default_ns_valid1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      375 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/default_ns_valid2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      256 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/dynamic-case1-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      169 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/dynamic-case1-overlap.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/dynamic-case1-override.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      245 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/dynamic-case1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      448 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/dynamic-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/import-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/import-case2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      436 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/import-case3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      241 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/import-case4-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      316 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/import-case4-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/import-case4a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/import-case4b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      365 2022-09-08 10:16:11.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/import-case5a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      377 2022-09-08 10:16:11.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/import-case5b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      379 2022-09-08 10:16:11.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/import-case5c.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/include-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/include-case1bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/include-case2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      541 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/include-case2bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/include-case3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      490 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/include-case4.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      520 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/include-case5.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      499 2023-10-18 10:33:30.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/include-case6.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/include-case7.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      466 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/include-case8.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      261 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/included3-valid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      257 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/included4-invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      269 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/included5-valid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      211 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/included6-invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      169 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/included7-overlap.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      355 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/features/namespaces/included8-redefine.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.096649 xmlschema-3.2.1/tests/test_cases/features/patterns/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      833 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/features/patterns/patterns.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3276 2020-04-07 21:42:10.000000 xmlschema-3.2.1/tests/test_cases/features/patterns/patterns.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.102649 xmlschema-3.2.1/tests/test_cases/features/wsdl/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2089 2023-05-18 20:18:16.000000 xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example3.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1477 2023-05-18 20:18:16.000000 xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-05-18 20:18:16.000000 xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example3_types.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1954 2020-11-08 22:15:33.000000 xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2132 2020-11-08 22:15:33.000000 xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example4.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1962 2020-11-08 22:15:33.000000 xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2996 2020-11-08 22:15:33.000000 xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example5.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3163 2020-11-08 22:15:33.000000 xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3414 2020-11-08 22:15:33.000000 xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.031649 xmlschema-3.2.1/tests/test_cases/issues/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.102649 xmlschema-3.2.1/tests/test_cases/issues/issue_008/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      252 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_008/issue_008.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      533 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_008/issue_008.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.102649 xmlschema-3.2.1/tests/test_cases/issues/issue_009/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      303 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_009/issue_009.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.104649 xmlschema-3.2.1/tests/test_cases/issues/issue_013/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_013/issue_013-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      731 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_013/issue_013-1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_013/issue_013-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      184 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_013/issue_013.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      801 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_013/issue_013.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.104649 xmlschema-3.2.1/tests/test_cases/issues/issue_014/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      556 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_014/issue014.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.105649 xmlschema-3.2.1/tests/test_cases/issues/issue_018/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      193 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_018/issue_018-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1449 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_018/issue_018.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.106649 xmlschema-3.2.1/tests/test_cases/issues/issue_022/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1048 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_022/README.md
--rw-r--r--   0 brunato   (1000) brunato   (1000)      130 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_022/xml_string_1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      208 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_022/xml_string_2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_022/xsd_string.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.108649 xmlschema-3.2.1/tests/test_cases/issues/issue_026/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      229 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_026/issue_026-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      224 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_026/issue_026-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      213 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_026/issue_026-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_026/issue_026.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.109649 xmlschema-3.2.1/tests/test_cases/issues/issue_028/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_028/issue_028-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_028/issue_028-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      353 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_028/issue_028.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.110649 xmlschema-3.2.1/tests/test_cases/issues/issue_029/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_029/issue_029-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      159 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_029/issue_029-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_029/issue_029-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      363 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_029/issue_029.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.112649 xmlschema-3.2.1/tests/test_cases/issues/issue_035/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      869 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_035/dates.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1081 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_035/dates.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.113649 xmlschema-3.2.1/tests/test_cases/issues/issue_041/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      247 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_041/issue_041.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      708 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_041/issue_041.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.114649 xmlschema-3.2.1/tests/test_cases/issues/issue_045/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      275 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_045/issue_045.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.116649 xmlschema-3.2.1/tests/test_cases/issues/issue_046/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      354 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_046/issue_046.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      419 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_046/issue_046.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.117649 xmlschema-3.2.1/tests/test_cases/issues/issue_051/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      331 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_051/issue_051.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      824 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_051/issue_051.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.118649 xmlschema-3.2.1/tests/test_cases/issues/issue_073/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      327 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_073/issue_073-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      362 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_073/issue_073-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      685 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_073/issue_073.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.119649 xmlschema-3.2.1/tests/test_cases/issues/issue_086/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_086/issue_086-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_086/issue_086-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1328 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_086/issue_086.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.119649 xmlschema-3.2.1/tests/test_cases/issues/issue_105/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_105/issue_105.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.120649 xmlschema-3.2.1/tests/test_cases/issues/issue_111/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      698 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_111/issue_111.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.120649 xmlschema-3.2.1/tests/test_cases/issues/issue_115/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      620 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_115/Rotation.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.121649 xmlschema-3.2.1/tests/test_cases/issues/issue_171/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      535 2020-03-23 16:13:26.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_171/issue_171.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      580 2020-03-23 16:13:26.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_171/issue_171b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-08-14 19:07:25.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_171/issue_171c.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.122649 xmlschema-3.2.1/tests/test_cases/issues/issue_187/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-09-25 15:20:24.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_187/issue_187_1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      804 2020-09-25 15:20:24.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_187/issue_187_2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.123649 xmlschema-3.2.1/tests/test_cases/issues/issue_190/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      109 2020-05-28 20:30:12.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_190/issue_190.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      785 2020-05-28 20:30:12.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_190/issue_190.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.123649 xmlschema-3.2.1/tests/test_cases/issues/issue_200/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      310 2020-08-14 19:07:25.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_200/issue_200.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      752 2020-08-14 19:07:25.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_200/issue_200.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.124649 xmlschema-3.2.1/tests/test_cases/issues/issue_203/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      196 2020-09-19 06:08:01.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_203/issue_203.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-09-19 06:08:01.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_203/issue_203.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      964 2020-09-19 06:08:01.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_203/issue_203alt.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.125649 xmlschema-3.2.1/tests/test_cases/issues/issue_204/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      524 2020-09-25 15:20:24.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_204/issue_204.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      172 2020-09-25 15:20:24.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_204/issue_204_1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-09-25 15:20:24.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_204/issue_204_2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2020-09-25 15:20:24.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_204/issue_204_3.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.125649 xmlschema-3.2.1/tests/test_cases/issues/issue_208/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-11-08 22:15:33.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_208/issue_208.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1532 2020-11-08 22:15:33.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_208/issue_208.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.126649 xmlschema-3.2.1/tests/test_cases/issues/issue_222/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       66 2021-01-24 21:47:47.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_222/issue_222.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      569 2021-01-24 21:47:47.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_222/issue_222.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.126649 xmlschema-3.2.1/tests/test_cases/issues/issue_223/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       46 2021-01-24 21:47:47.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_223/issue_223.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      392 2021-03-30 11:13:45.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_223/issue_223.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.026649 xmlschema-3.2.1/tests/test_cases/issues/issue_237/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.128649 xmlschema-3.2.1/tests/test_cases/issues/issue_237/dir1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      191 2021-04-05 21:38:16.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_237/dir1/issue_237.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1249 2021-04-05 21:38:16.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.130649 xmlschema-3.2.1/tests/test_cases/issues/issue_237/dir2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      141 2021-04-05 21:38:16.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_237/dir2/issue_237a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      314 2021-04-05 21:38:16.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_237/dir2/issue_237b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1041 2021-04-05 21:38:16.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2021-04-05 21:38:16.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_237/dir2/stockquote.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.130649 xmlschema-3.2.1/tests/test_cases/issues/issue_243/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      283 2021-05-03 11:37:57.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_243/issue_243.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2021-05-03 11:37:57.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_243/issue_243.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.132649 xmlschema-3.2.1/tests/test_cases/issues/issue_245/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_245/issue_245-valid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_245/issue_245.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2021-05-03 11:37:57.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_245/issue_245.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.133649 xmlschema-3.2.1/tests/test_cases/issues/issue_259/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     2422 2021-09-02 10:52:43.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_259/issue_259-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1432 2021-09-02 10:52:43.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_259/issue_259-2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.134649 xmlschema-3.2.1/tests/test_cases/issues/issue_265/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3471 2021-10-20 14:14:48.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_265/issue_265-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1411 2021-10-20 14:14:48.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      454 2021-10-20 14:14:48.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_265/issue_265-2-override.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.136649 xmlschema-3.2.1/tests/test_cases/issues/issue_266/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_266/issue_266-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      538 2021-10-20 14:14:48.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_266/issue_266-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_266/issue_266-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      528 2021-10-20 14:14:48.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_266/issue_266-2.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      651 2021-11-11 15:30:24.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_266/issue_266b-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      551 2021-11-11 15:30:24.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_266/issue_266b-2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.137649 xmlschema-3.2.1/tests/test_cases/issues/issue_273/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      299 2021-12-08 19:41:39.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_273/issue_273.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      517 2021-12-08 19:41:39.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_273/issue_273.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.138649 xmlschema-3.2.1/tests/test_cases/issues/issue_276/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      122 2021-12-08 22:11:41.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_276/dummy.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      495 2021-12-08 22:11:41.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_276/schema.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.138649 xmlschema-3.2.1/tests/test_cases/issues/issue_298/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      114 2022-05-22 16:17:24.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_298/issue_298-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      240 2022-05-22 16:17:24.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_298/issue_298-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      792 2022-05-22 16:17:24.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_298/issue_298.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.140649 xmlschema-3.2.1/tests/test_cases/issues/issue_306/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      881 2022-06-24 14:13:22.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_306/issue_306-alt.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      203 2022-06-24 14:13:22.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_306/issue_306-invalid.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      182 2022-06-24 14:13:22.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_306/issue_306-valid.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      689 2022-06-24 14:13:22.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_306/issue_306.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.140649 xmlschema-3.2.1/tests/test_cases/issues/issue_311/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      786 2022-07-18 14:19:15.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_311/correct_no_list.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      788 2022-07-18 14:19:15.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_311/incorrect_with_list.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4013 2022-07-18 14:19:15.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.141649 xmlschema-3.2.1/tests/test_cases/issues/issue_314/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      267 2022-07-21 09:40:50.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_314/issue_314.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1153 2022-07-21 09:40:50.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_314/issue_314.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.143649 xmlschema-3.2.1/tests/test_cases/issues/issue_315/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       66 2022-07-18 14:19:15.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_315/issue_315-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       63 2022-07-18 14:19:15.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_315/issue_315-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_315/issue_315-3.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       76 2022-07-18 14:19:15.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_315/issue_315-4.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_315/issue_315-5.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      604 2022-07-18 14:19:15.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_315/issue_315_mixed.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      456 2022-07-18 14:19:15.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_315/issue_315_simple.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.144649 xmlschema-3.2.1/tests/test_cases/issues/issue_322/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      155 2022-08-26 15:33:28.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_322/issue_322.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      348 2022-08-26 15:33:28.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_322/issue_322.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.146649 xmlschema-3.2.1/tests/test_cases/issues/issue_324/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_324/issue_324-invalid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_324/issue_324-valid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      672 2022-08-28 05:56:41.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_324/issue_324.zip
--rw-r--r--   0 brunato   (1000) brunato   (1000)      384 2022-09-08 10:16:11.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_324/issue_324a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      190 2022-09-08 10:16:11.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_324/issue_324b.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.147649 xmlschema-3.2.1/tests/test_cases/issues/issue_334/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1814 2023-02-11 10:41:50.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_334/issue_334.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5149 2023-02-11 10:41:50.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_334/issue_334.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2663 2023-02-09 09:02:31.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_334/issue_334.zip
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.150649 xmlschema-3.2.1/tests/test_cases/issues/issue_341/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2070 2023-04-14 13:49:05.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_341/issue_341-ext.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      158 2023-04-14 13:49:05.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_341/issue_341.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1781 2023-04-14 13:49:05.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_341/issue_341.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.151649 xmlschema-3.2.1/tests/test_cases/issues/issue_349/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      329 2023-06-14 07:04:00.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_349/issue_349.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      574 2023-06-14 07:04:00.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_349/issue_349.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.151649 xmlschema-3.2.1/tests/test_cases/issues/issue_362/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.152649 xmlschema-3.2.1/tests/test_cases/issues/issue_362/dir1/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.152649 xmlschema-3.2.1/tests/test_cases/issues/issue_362/dir1/dir2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      433 2023-09-23 04:52:41.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_362/dir1/dir2/issue_362_2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      334 2023-09-23 04:52:41.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_362/dir1/issue_362_1.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.152649 xmlschema-3.2.1/tests/test_cases/issues/issue_362/dir2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      345 2023-09-23 04:52:41.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_362/dir2/issue_362_2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      816 2023-09-23 04:52:41.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_362/issue_362_1.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.154649 xmlschema-3.2.1/tests/test_cases/issues/issue_363/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      352 2023-09-23 04:52:41.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_363/issue_363-invalid-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      347 2023-09-23 04:52:41.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_363/issue_363-invalid-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-09-23 04:52:41.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_363/issue_363-invalid-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      323 2023-09-23 04:52:41.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_363/issue_363.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      544 2023-09-23 04:52:41.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_363/issue_363.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.156649 xmlschema-3.2.1/tests/test_cases/issues/issue_372/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       60 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_372/issue_372-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)       83 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_372/issue_372-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      549 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_372/issue_372.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.157649 xmlschema-3.2.1/tests/test_cases/issues/issue_386/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      371 2024-02-18 21:08:04.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_386/issue_386-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      370 2024-02-18 21:08:04.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_386/issue_386-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1392 2024-02-18 21:08:04.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_386/issue_386-2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1402 2024-02-18 21:08:04.000000 xmlschema-3.2.1/tests/test_cases/issues/issue_386/issue_386.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.159649 xmlschema-3.2.1/tests/test_cases/mypy/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      911 2022-05-20 16:16:20.000000 xmlschema-3.2.1/tests/test_cases/mypy/extra_validator.py
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)     3350 2024-03-13 05:27:13.000000 xmlschema-3.2.1/tests/test_cases/mypy/protocols.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)     1905 2023-05-05 12:33:46.000000 xmlschema-3.2.1/tests/test_cases/mypy/schema_source.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)      646 2021-11-11 15:30:24.000000 xmlschema-3.2.1/tests/test_cases/mypy/simple_types.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.163649 xmlschema-3.2.1/tests/test_cases/resources/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/resources/dummy file.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       26 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/resources/dummy file.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      171 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/resources/external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)       20 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/resources/malformed.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      308 2020-11-08 22:15:33.000000 xmlschema-3.2.1/tests/test_cases/resources/unparsed_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      170 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/resources/unused_external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      270 2020-11-08 22:15:33.000000 xmlschema-3.2.1/tests/test_cases/resources/unused_unparsed_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      129 2020-01-23 20:05:17.000000 xmlschema-3.2.1/tests/test_cases/resources/with_entity.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.167650 xmlschema-3.2.1/tests/test_cases/serialization/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4558 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/serialization/abdera.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5473 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/serialization/badgerfish.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3661 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/serialization/document.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5599 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/serialization/jsonml.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2264 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/serialization/parker.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6725 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_cases/testfiles
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.032649 xmlschema-3.2.1/tests/test_cases/translations/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.168650 xmlschema-3.2.1/tests/test_cases/translations/pl/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    22092 2023-07-27 19:52:28.000000 xmlschema-3.2.1/tests/test_cases/translations/pl/tw-1(5)8e.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6795 2023-07-27 19:52:28.000000 xmlschema-3.2.1/tests/test_cases/translations/pl/tytul_wykonawczy_niekompletny.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11960 2024-03-13 05:27:13.000000 xmlschema-3.2.1/tests/test_cli.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    26576 2023-02-11 10:41:50.000000 xmlschema-3.2.1/tests/test_codegen.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    32551 2024-03-13 05:27:13.000000 xmlschema-3.2.1/tests/test_converters.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    28876 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_dataobjects.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24798 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_documents.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16654 2024-03-25 21:28:10.000000 xmlschema-3.2.1/tests/test_exports.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3234 2021-02-05 08:47:55.000000 xmlschema-3.2.1/tests/test_files.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    30654 2024-03-25 21:28:10.000000 xmlschema-3.2.1/tests/test_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19738 2024-03-25 21:28:10.000000 xmlschema-3.2.1/tests/test_locations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5738 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_memory.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23506 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_namespaces.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4755 2023-09-20 10:58:25.000000 xmlschema-3.2.1/tests/test_package.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    58232 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_resources.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1785 2021-09-02 10:52:43.000000 xmlschema-3.2.1/tests/test_schemas.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5976 2023-09-23 04:52:41.000000 xmlschema-3.2.1/tests/test_translations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2336 2024-03-13 05:27:13.000000 xmlschema-3.2.1/tests/test_typing.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1806 2021-09-02 10:52:43.000000 xmlschema-3.2.1/tests/test_validation.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    27292 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/test_w3c_suite.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    44084 2023-05-18 20:18:16.000000 xmlschema-3.2.1/tests/test_wsdl.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15023 2024-02-18 21:08:04.000000 xmlschema-3.2.1/tests/test_xpath.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.170650 xmlschema-3.2.1/tests/validation/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-3.2.1/tests/validation/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    79224 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/validation/test_decoding.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33245 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/validation/test_encoding.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    29598 2024-04-07 16:34:58.000000 xmlschema-3.2.1/tests/validation/test_validation.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.175650 xmlschema-3.2.1/tests/validators/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-3.2.1/tests/validators/__init__.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    25878 2022-07-18 14:19:15.000000 xmlschema-3.2.1/tests/validators/test_attributes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14352 2020-12-23 12:38:37.000000 xmlschema-3.2.1/tests/validators/test_builtins.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    34334 2024-02-18 21:08:04.000000 xmlschema-3.2.1/tests/validators/test_complex_types.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4333 2022-06-24 14:13:22.000000 xmlschema-3.2.1/tests/validators/test_elements.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16414 2024-01-07 11:20:34.000000 xmlschema-3.2.1/tests/validators/test_exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    63262 2024-03-25 21:28:10.000000 xmlschema-3.2.1/tests/validators/test_facets.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5409 2023-10-27 20:18:56.000000 xmlschema-3.2.1/tests/validators/test_global_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15833 2024-02-18 21:08:04.000000 xmlschema-3.2.1/tests/validators/test_groups.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19335 2023-09-23 04:52:41.000000 xmlschema-3.2.1/tests/validators/test_identities.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    52694 2024-04-07 16:34:58.000000 xmlschema-3.2.1/tests/validators/test_models.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3447 2022-07-18 14:19:15.000000 xmlschema-3.2.1/tests/validators/test_notations.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     8625 2022-07-18 14:19:15.000000 xmlschema-3.2.1/tests/validators/test_particles.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    39368 2024-03-25 21:28:10.000000 xmlschema-3.2.1/tests/validators/test_schemas.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    10292 2024-03-23 21:43:51.000000 xmlschema-3.2.1/tests/validators/test_simple_types.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    34302 2022-07-18 14:19:15.000000 xmlschema-3.2.1/tests/validators/test_wildcards.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    38338 2024-03-25 21:28:10.000000 xmlschema-3.2.1/tests/validators/test_xsdbase.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1441 2024-03-13 05:41:48.000000 xmlschema-3.2.1/tox.ini
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.185649 xmlschema-3.2.1/xmlschema/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3089 2024-04-07 16:34:58.000000 xmlschema-3.2.1/xmlschema/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6145 2024-04-07 16:34:58.000000 xmlschema-3.2.1/xmlschema/aliases.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11866 2024-03-13 05:27:13.000000 xmlschema-3.2.1/xmlschema/cli.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.190650 xmlschema-3.2.1/xmlschema/converters/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      865 2024-03-13 05:27:13.000000 xmlschema-3.2.1/xmlschema/converters/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6640 2024-01-07 11:20:34.000000 xmlschema-3.2.1/xmlschema/converters/abdera.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6709 2024-03-13 05:27:13.000000 xmlschema-3.2.1/xmlschema/converters/badgerfish.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7855 2024-01-07 11:20:34.000000 xmlschema-3.2.1/xmlschema/converters/columnar.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24841 2024-01-07 11:20:34.000000 xmlschema-3.2.1/xmlschema/converters/default.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7977 2024-03-13 05:27:13.000000 xmlschema-3.2.1/xmlschema/converters/gdata.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5271 2024-01-07 11:20:34.000000 xmlschema-3.2.1/xmlschema/converters/jsonml.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6137 2024-01-07 11:20:34.000000 xmlschema-3.2.1/xmlschema/converters/parker.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6132 2024-01-07 11:20:34.000000 xmlschema-3.2.1/xmlschema/converters/unordered.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24831 2024-03-13 05:27:13.000000 xmlschema-3.2.1/xmlschema/dataobjects.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    38425 2024-01-07 11:20:34.000000 xmlschema-3.2.1/xmlschema/documents.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1235 2021-10-20 14:14:48.000000 xmlschema-3.2.1/xmlschema/exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15000 2024-04-07 16:34:58.000000 xmlschema-3.2.1/xmlschema/exports.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.190650 xmlschema-3.2.1/xmlschema/extras/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-02-05 09:05:33.000000 xmlschema-3.2.1/xmlschema/extras/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    21930 2023-05-18 20:18:16.000000 xmlschema-3.2.1/xmlschema/extras/codegen.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.034649 xmlschema-3.2.1/xmlschema/extras/templates/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.191650 xmlschema-3.2.1/xmlschema/extras/templates/python/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      997 2022-07-18 14:19:15.000000 xmlschema-3.2.1/xmlschema/extras/templates/python/bindings.py.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1116 2021-02-11 14:32:40.000000 xmlschema-3.2.1/xmlschema/extras/templates/python/sample.py.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24452 2024-01-07 11:20:34.000000 xmlschema-3.2.1/xmlschema/extras/wsdl.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16326 2024-03-25 21:28:10.000000 xmlschema-3.2.1/xmlschema/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      677 2020-11-10 10:13:55.000000 xmlschema-3.2.1/xmlschema/limits.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.035649 xmlschema-3.2.1/xmlschema/locale/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.034649 xmlschema-3.2.1/xmlschema/locale/en/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.192650 xmlschema-3.2.1/xmlschema/locale/en/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    45327 2022-05-20 20:00:14.000000 xmlschema-3.2.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo
--rw-r--r--   0 brunato   (1000) brunato   (1000)    64464 2024-03-19 14:02:56.000000 xmlschema-3.2.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.034649 xmlschema-3.2.1/xmlschema/locale/it/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.192650 xmlschema-3.2.1/xmlschema/locale/it/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    47535 2022-05-20 20:00:14.000000 xmlschema-3.2.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    67361 2022-05-20 20:00:14.000000 xmlschema-3.2.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.035649 xmlschema-3.2.1/xmlschema/locale/pl/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.193650 xmlschema-3.2.1/xmlschema/locale/pl/LC_MESSAGES/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    47395 2023-07-27 19:52:28.000000 xmlschema-3.2.1/xmlschema/locale/pl/LC_MESSAGES/xmlschema.mo
--rw-r--r--   0 brunato   (1000) brunato   (1000)    66282 2023-07-27 19:52:28.000000 xmlschema-3.2.1/xmlschema/locale/pl/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.035649 xmlschema-3.2.1/xmlschema/locale/ru/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.195650 xmlschema-3.2.1/xmlschema/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    60295 2022-06-11 14:29:39.000000 xmlschema-3.2.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    79497 2022-06-11 14:29:39.000000 xmlschema-3.2.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po
--rw-r--r--   0 brunato   (1000) brunato   (1000)    10643 2024-03-25 21:28:10.000000 xmlschema-3.2.1/xmlschema/locations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9653 2024-03-25 21:28:10.000000 xmlschema-3.2.1/xmlschema/names.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17001 2024-01-07 11:20:34.000000 xmlschema-3.2.1/xmlschema/namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)        0 2021-09-02 10:52:43.000000 xmlschema-3.2.1/xmlschema/py.typed
--rw-r--r--   0 brunato   (1000) brunato   (1000)    49667 2024-03-25 21:28:10.000000 xmlschema-3.2.1/xmlschema/resources.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.036649 xmlschema-3.2.1/xmlschema/schemas/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.196650 xmlschema-3.2.1/xmlschema/schemas/DSIG/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    10447 2023-07-27 19:52:28.000000 xmlschema-3.2.1/xmlschema/schemas/DSIG/xmldsig-core-schema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4664 2023-07-27 19:52:28.000000 xmlschema-3.2.1/xmlschema/schemas/DSIG/xmldsig11-schema.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.196650 xmlschema-3.2.1/xmlschema/schemas/HFP/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1534 2020-11-08 22:15:33.000000 xmlschema-3.2.1/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.197650 xmlschema-3.2.1/xmlschema/schemas/VC/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      984 2020-11-08 22:15:33.000000 xmlschema-3.2.1/xmlschema/schemas/VC/XMLSchema-versioning.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.198650 xmlschema-3.2.1/xmlschema/schemas/WSDL/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19204 2020-11-08 22:15:33.000000 xmlschema-3.2.1/xmlschema/schemas/WSDL/soap-encoding.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6061 2020-11-08 22:15:33.000000 xmlschema-3.2.1/xmlschema/schemas/WSDL/soap-envelope.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6005 2020-11-08 22:15:33.000000 xmlschema-3.2.1/xmlschema/schemas/WSDL/wsdl-soap.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11900 2020-11-08 22:15:33.000000 xmlschema-3.2.1/xmlschema/schemas/WSDL/wsdl.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.199650 xmlschema-3.2.1/xmlschema/schemas/XENC/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4360 2023-07-27 19:52:28.000000 xmlschema-3.2.1/xmlschema/schemas/XENC/xenc-schema-11.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6669 2023-07-27 19:52:28.000000 xmlschema-3.2.1/xmlschema/schemas/XENC/xenc-schema.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.200650 xmlschema-3.2.1/xmlschema/schemas/XHTML/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    65477 2020-11-08 22:15:33.000000 xmlschema-3.2.1/xmlschema/schemas/XHTML/xhtml1-strict.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.201650 xmlschema-3.2.1/xmlschema/schemas/XLINK/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8051 2020-11-08 22:15:33.000000 xmlschema-3.2.1/xmlschema/schemas/XLINK/xlink.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.201650 xmlschema-3.2.1/xmlschema/schemas/XML/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1277 2020-11-08 22:15:33.000000 xmlschema-3.2.1/xmlschema/schemas/XML/xml_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.202650 xmlschema-3.2.1/xmlschema/schemas/XSD_1.0/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    88033 2022-05-20 16:16:20.000000 xmlschema-3.2.1/xmlschema/schemas/XSD_1.0/XMLSchema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    44301 2020-11-08 22:15:33.000000 xmlschema-3.2.1/xmlschema/schemas/XSD_1.0/datatypes.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.204650 xmlschema-3.2.1/xmlschema/schemas/XSD_1.1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    67728 2022-09-25 07:58:42.000000 xmlschema-3.2.1/xmlschema/schemas/XSD_1.1/XMLSchema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17497 2020-11-08 22:15:33.000000 xmlschema-3.2.1/xmlschema/schemas/XSD_1.1/datatypes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3767 2022-09-12 09:59:59.000000 xmlschema-3.2.1/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.204650 xmlschema-3.2.1/xmlschema/schemas/XSI/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      385 2020-11-08 22:15:33.000000 xmlschema-3.2.1/xmlschema/schemas/XSI/XMLSchema-instance_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.206650 xmlschema-3.2.1/xmlschema/testing/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2023-07-27 19:52:28.000000 xmlschema-3.2.1/xmlschema/testing/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    31080 2024-03-13 05:27:13.000000 xmlschema-3.2.1/xmlschema/testing/_builders.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7950 2023-10-18 10:59:40.000000 xmlschema-3.2.1/xmlschema/testing/_case_class.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9443 2023-12-19 09:41:12.000000 xmlschema-3.2.1/xmlschema/testing/_factory.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7658 2024-01-07 11:20:34.000000 xmlschema-3.2.1/xmlschema/testing/_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4891 2023-05-18 20:18:16.000000 xmlschema-3.2.1/xmlschema/testing/_observers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2072 2023-02-11 10:41:50.000000 xmlschema-3.2.1/xmlschema/translation.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.216650 xmlschema-3.2.1/xmlschema/validators/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3677 2024-03-13 05:27:13.000000 xmlschema-3.2.1/xmlschema/validators/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7277 2024-03-13 05:27:13.000000 xmlschema-3.2.1/xmlschema/validators/assertions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    34229 2024-03-11 14:51:16.000000 xmlschema-3.2.1/xmlschema/validators/attributes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19881 2022-08-26 15:33:28.000000 xmlschema-3.2.1/xmlschema/validators/builtins.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    47513 2024-04-07 16:34:58.000000 xmlschema-3.2.1/xmlschema/validators/complex_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    66755 2024-03-13 05:27:13.000000 xmlschema-3.2.1/xmlschema/validators/elements.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17473 2024-04-07 16:34:58.000000 xmlschema-3.2.1/xmlschema/validators/exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    31285 2024-03-25 21:28:10.000000 xmlschema-3.2.1/xmlschema/validators/facets.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33583 2024-04-07 16:34:58.000000 xmlschema-3.2.1/xmlschema/validators/global_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    64343 2024-04-07 16:34:58.000000 xmlschema-3.2.1/xmlschema/validators/groups.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7108 2024-03-13 05:27:13.000000 xmlschema-3.2.1/xmlschema/validators/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19395 2024-03-13 05:27:13.000000 xmlschema-3.2.1/xmlschema/validators/identities.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23027 2024-04-07 16:34:58.000000 xmlschema-3.2.1/xmlschema/validators/models.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1611 2022-05-20 20:00:15.000000 xmlschema-3.2.1/xmlschema/validators/notations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7532 2024-04-07 16:34:58.000000 xmlschema-3.2.1/xmlschema/validators/particles.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)   107664 2024-04-06 05:40:10.000000 xmlschema-3.2.1/xmlschema/validators/schemas.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    62097 2024-03-25 21:28:10.000000 xmlschema-3.2.1/xmlschema/validators/simple_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    38068 2024-04-07 16:34:58.000000 xmlschema-3.2.1/xmlschema/validators/wildcards.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    42960 2024-03-30 06:19:36.000000 xmlschema-3.2.1/xmlschema/validators/xsdbase.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.219650 xmlschema-3.2.1/xmlschema/xpath/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      787 2024-03-13 05:27:13.000000 xmlschema-3.2.1/xmlschema/xpath/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1072 2024-02-18 21:08:04.000000 xmlschema-3.2.1/xmlschema/xpath/assertion_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1139 2024-02-18 21:08:04.000000 xmlschema-3.2.1/xmlschema/xpath/identity_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9622 2024-03-13 05:27:13.000000 xmlschema-3.2.1/xmlschema/xpath/mixin.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4101 2024-03-13 05:27:13.000000 xmlschema-3.2.1/xmlschema/xpath/proxy.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1231 2024-02-13 06:35:18.000000 xmlschema-3.2.1/xmlschema/xpath3.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-07 16:36:35.219650 xmlschema-3.2.1/xmlschema.egg-info/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8237 2024-04-07 16:36:34.000000 xmlschema-3.2.1/xmlschema.egg-info/PKG-INFO
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    19948 2024-04-07 16:36:35.000000 xmlschema-3.2.1/xmlschema.egg-info/SOURCES.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)        1 2024-04-07 16:36:34.000000 xmlschema-3.2.1/xmlschema.egg-info/dependency_links.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      150 2024-04-07 16:36:34.000000 xmlschema-3.2.1/xmlschema.egg-info/entry_points.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      256 2024-04-07 16:36:34.000000 xmlschema-3.2.1/xmlschema.egg-info/requires.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       10 2024-04-07 16:36:34.000000 xmlschema-3.2.1/xmlschema.egg-info/top_level.txt
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.723928 xmlschema-3.3.0/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2023-03-05 21:16:57.000000 xmlschema-3.3.0/.coveragerc
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    28284 2024-04-17 17:34:18.000000 xmlschema-3.3.0/CHANGELOG.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2024-01-07 11:20:34.000000 xmlschema-3.3.0/LICENSE
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      330 2023-03-05 20:30:24.000000 xmlschema-3.3.0/MANIFEST.in
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8237 2024-04-17 17:34:43.723928 xmlschema-3.3.0/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6120 2024-02-18 21:08:04.000000 xmlschema-3.3.0/README.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.570928 xmlschema-3.3.0/doc/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      606 2018-09-23 09:23:56.000000 xmlschema-3.3.0/doc/Makefile
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11907 2024-03-25 21:28:10.000000 xmlschema-3.3.0/doc/api.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    11273 2021-08-02 14:12:17.000000 xmlschema-3.3.0/doc/components.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5483 2024-04-17 17:34:18.000000 xmlschema-3.3.0/doc/conf.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5499 2022-06-24 14:13:22.000000 xmlschema-3.3.0/doc/converters.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4841 2022-06-24 14:13:22.000000 xmlschema-3.3.0/doc/extras.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9946 2024-03-25 21:28:10.000000 xmlschema-3.3.0/doc/features.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2021-02-05 09:05:33.000000 xmlschema-3.3.0/doc/index.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2024-04-08 08:13:09.000000 xmlschema-3.3.0/doc/intro.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       82 2024-02-03 22:44:00.000000 xmlschema-3.3.0/doc/requirements.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5921 2021-04-11 20:19:21.000000 xmlschema-3.3.0/doc/testing.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    31284 2024-03-25 21:28:10.000000 xmlschema-3.3.0/doc/usage.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-03-07 13:26:41.000000 xmlschema-3.3.0/mypy.ini
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       81 2023-09-23 04:52:41.000000 xmlschema-3.3.0/pyproject.toml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2024-03-13 05:27:13.000000 xmlschema-3.3.0/requirements-dev.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2024-04-17 17:34:43.724928 xmlschema-3.3.0/setup.cfg
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     2765 2024-04-17 17:34:18.000000 xmlschema-3.3.0/setup.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.579928 xmlschema-3.3.0/tests/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-03 21:49:59.000000 xmlschema-3.3.0/tests/__init__.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     6753 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/check_memory.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.541928 xmlschema-3.3.0/tests/templates/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.580928 xmlschema-3.3.0/tests/templates/demo/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/demo/demo_type_filter_test.jinja
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.582928 xmlschema-3.3.0/tests/templates/filters/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       34 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/filters/name_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/filters/namespace_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/filters/python_type_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       35 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/filters/qname_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       87 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/filters/sort_types_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-04-03 19:09:14.000000 xmlschema-3.3.0/tests/templates/filters/type_name_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       40 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/filters/type_qname_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       37 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/templates/filters/unknown_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/filters/wrong-template.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3576 2024-03-25 21:28:10.000000 xmlschema-3.3.0/tests/test_all.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.582928 xmlschema-3.3.0/tests/test_cases/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.541928 xmlschema-3.3.0/tests/test_cases/examples/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.586928 xmlschema-3.3.0/tests/test_cases/examples/collection/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      925 2020-05-28 20:30:12.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection-1_error.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      884 2022-08-26 15:33:28.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection-default.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1171 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection-redef-xmlns.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      798 2024-04-17 17:12:21.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      923 2020-05-28 20:30:12.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1599 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      941 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1736 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1938 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1082 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection3bis.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1979 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection3bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1364 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection4.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1743 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection4.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1658 2022-08-26 15:33:28.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection5.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.590928 xmlschema-3.3.0/tests/test_cases/examples/menù/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      559 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/examples/menù/menù-ascii.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/examples/menù/menù-ascii.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      532 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/examples/menù/menù-cp1252.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      509 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/examples/menù/menù-cp1252.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        3 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/examples/menù/menù.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      542 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/examples/menù/menù.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/examples/menù/menù.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.591928 xmlschema-3.3.0/tests/test_cases/examples/stockquote/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1039 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/examples/stockquote/stockquote.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/examples/stockquote/stockquote.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1230 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/examples/stockquote/stockquoteservice.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.596928 xmlschema-3.3.0/tests/test_cases/examples/vehicles/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/bikes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      469 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/cars.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      595 2022-10-01 13:42:01.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      361 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/types.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:30.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-1_error.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-1_error.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      475 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-2_errors.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:33.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-3_errors.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      491 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-3_errors.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      557 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-max.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-redef.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1666 2020-11-15 16:10:20.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      543 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2020-05-02 09:28:32.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles2.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      432 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles2.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.542928 xmlschema-3.3.0/tests/test_cases/features/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.597928 xmlschema-3.3.0/tests/test_cases/features/attributes/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      688 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/attributes/default_attributes-missing_group.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      910 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/attributes/default_attributes.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.597928 xmlschema-3.3.0/tests/test_cases/features/builtins/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      584 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/builtins/builtins.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      601 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/builtins/builtins.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.599928 xmlschema-3.3.0/tests/test_cases/features/decoder/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      781 2022-05-20 20:00:14.000000 xmlschema-3.3.0/tests/test_cases/features/decoder/data.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      725 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/decoder/data2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2021-04-01 09:07:37.000000 xmlschema-3.3.0/tests/test_cases/features/decoder/data3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      480 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/features/decoder/data4-mixed.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      691 2021-12-08 19:41:39.000000 xmlschema-3.3.0/tests/test_cases/features/decoder/long-sequence-1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      727 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/features/decoder/mixed-content.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5913 2022-05-20 20:00:14.000000 xmlschema-3.3.0/tests/test_cases/features/decoder/simple-types.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.601928 xmlschema-3.3.0/tests/test_cases/features/derivations/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1956 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/complex-extensions.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      662 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3949 2023-05-18 20:18:16.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/complex11-restrictions.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      599 2023-05-18 20:18:16.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2051 2023-05-18 20:18:16.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/invalid-restrictions1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1027 2023-05-18 20:18:16.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/invalid-restrictions2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      322 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/list_types.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      675 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/list_types.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.602928 xmlschema-3.3.0/tests/test_cases/features/elements/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      154 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/elements/test_alternatives-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1487 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/elements/type_alternatives-no-ns.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1543 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/elements/type_alternatives.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.609928 xmlschema-3.3.0/tests/test_cases/features/models/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5143 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/billion_laughs_model.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      301 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/circular_model.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      215 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/illegal-attributes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/illegal-declarations.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      523 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/illegal-occurs.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1192 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/invalid_models1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1541 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/invalid_models2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/model1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4794 2020-04-28 13:28:56.000000 xmlschema-3.3.0/tests/test_cases/features/models/models.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/other-ns.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      760 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/recursive-groups.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1062 2020-04-28 13:28:56.000000 xmlschema-3.3.0/tests/test_cases/features/models/valid_model1.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.618928 xmlschema-3.3.0/tests/test_cases/features/namespaces/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      151 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/chameleon1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/chameleon2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      272 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/chameleon3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/default_ns_invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      481 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/default_ns_valid1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      375 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/default_ns_valid2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      256 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/dynamic-case1-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      169 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/dynamic-case1-overlap.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/dynamic-case1-override.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      245 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/dynamic-case1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      448 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/dynamic-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      436 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      241 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case4-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      316 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case4-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case4a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case4b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      365 2022-09-08 10:16:11.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case5a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      377 2022-09-08 10:16:11.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case5b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      379 2022-09-08 10:16:11.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case5c.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case1bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      541 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case2bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      490 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case4.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      520 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case5.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      499 2023-10-18 10:33:30.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case6.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case7.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      466 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case8.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      261 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/included3-valid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      257 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/included4-invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      269 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/included5-valid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      211 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/included6-invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      169 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/included7-overlap.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      355 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/included8-redefine.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.619928 xmlschema-3.3.0/tests/test_cases/features/patterns/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      833 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/patterns/patterns.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3276 2020-04-07 21:42:10.000000 xmlschema-3.3.0/tests/test_cases/features/patterns/patterns.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.621928 xmlschema-3.3.0/tests/test_cases/features/wsdl/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2089 2023-05-18 20:18:16.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example3.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1477 2023-05-18 20:18:16.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-05-18 20:18:16.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example3_types.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1954 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2132 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example4.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1962 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2996 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example5.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3163 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3414 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.552928 xmlschema-3.3.0/tests/test_cases/issues/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.622928 xmlschema-3.3.0/tests/test_cases/issues/issue_008/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      252 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_008/issue_008.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      533 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_008/issue_008.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.622928 xmlschema-3.3.0/tests/test_cases/issues/issue_009/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      303 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_009/issue_009.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.623928 xmlschema-3.3.0/tests/test_cases/issues/issue_013/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_013/issue_013-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      731 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_013/issue_013-1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_013/issue_013-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      184 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_013/issue_013.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      801 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_013/issue_013.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.624928 xmlschema-3.3.0/tests/test_cases/issues/issue_014/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      556 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_014/issue014.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.624928 xmlschema-3.3.0/tests/test_cases/issues/issue_018/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      193 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_018/issue_018-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1449 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_018/issue_018.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.625928 xmlschema-3.3.0/tests/test_cases/issues/issue_022/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1048 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_022/README.md
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      130 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_022/xml_string_1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      208 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_022/xml_string_2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_022/xsd_string.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.627928 xmlschema-3.3.0/tests/test_cases/issues/issue_026/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      229 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_026/issue_026-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      224 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_026/issue_026-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      213 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_026/issue_026-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_026/issue_026.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.628928 xmlschema-3.3.0/tests/test_cases/issues/issue_028/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_028/issue_028-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_028/issue_028-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      353 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_028/issue_028.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.629928 xmlschema-3.3.0/tests/test_cases/issues/issue_029/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_029/issue_029-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      159 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_029/issue_029-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_029/issue_029-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      363 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_029/issue_029.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.630928 xmlschema-3.3.0/tests/test_cases/issues/issue_035/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      869 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_035/dates.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1081 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_035/dates.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.631928 xmlschema-3.3.0/tests/test_cases/issues/issue_041/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      247 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_041/issue_041.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      708 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_041/issue_041.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.631928 xmlschema-3.3.0/tests/test_cases/issues/issue_045/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      275 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_045/issue_045.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.631928 xmlschema-3.3.0/tests/test_cases/issues/issue_046/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      354 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_046/issue_046.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      419 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_046/issue_046.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.632928 xmlschema-3.3.0/tests/test_cases/issues/issue_051/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      331 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_051/issue_051.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      824 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_051/issue_051.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.633928 xmlschema-3.3.0/tests/test_cases/issues/issue_073/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      327 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_073/issue_073-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      362 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_073/issue_073-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      685 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_073/issue_073.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.634928 xmlschema-3.3.0/tests/test_cases/issues/issue_086/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_086/issue_086-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_086/issue_086-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1328 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_086/issue_086.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.634928 xmlschema-3.3.0/tests/test_cases/issues/issue_105/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_105/issue_105.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.634928 xmlschema-3.3.0/tests/test_cases/issues/issue_111/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      698 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_111/issue_111.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.635928 xmlschema-3.3.0/tests/test_cases/issues/issue_115/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      620 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_115/Rotation.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.636928 xmlschema-3.3.0/tests/test_cases/issues/issue_171/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      535 2020-03-23 16:13:26.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_171/issue_171.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      580 2020-03-23 16:13:26.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_171/issue_171b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-08-14 19:07:25.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_171/issue_171c.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.637928 xmlschema-3.3.0/tests/test_cases/issues/issue_187/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-09-25 15:20:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_187/issue_187_1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      804 2020-09-25 15:20:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_187/issue_187_2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.637928 xmlschema-3.3.0/tests/test_cases/issues/issue_190/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      109 2020-05-28 20:30:12.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_190/issue_190.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      785 2020-05-28 20:30:12.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_190/issue_190.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.638928 xmlschema-3.3.0/tests/test_cases/issues/issue_200/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      310 2020-08-14 19:07:25.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_200/issue_200.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      752 2020-08-14 19:07:25.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_200/issue_200.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.641928 xmlschema-3.3.0/tests/test_cases/issues/issue_203/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      196 2020-09-19 06:08:01.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_203/issue_203.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-09-19 06:08:01.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_203/issue_203.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      964 2020-09-19 06:08:01.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_203/issue_203alt.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.643928 xmlschema-3.3.0/tests/test_cases/issues/issue_204/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      524 2020-09-25 15:20:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_204/issue_204.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      172 2020-09-25 15:20:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_204/issue_204_1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-09-25 15:20:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_204/issue_204_2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2020-09-25 15:20:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_204/issue_204_3.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.643928 xmlschema-3.3.0/tests/test_cases/issues/issue_208/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_208/issue_208.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1532 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_208/issue_208.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.644928 xmlschema-3.3.0/tests/test_cases/issues/issue_222/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       66 2021-01-24 21:47:47.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_222/issue_222.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      569 2021-01-24 21:47:47.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_222/issue_222.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.645928 xmlschema-3.3.0/tests/test_cases/issues/issue_223/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       46 2021-01-24 21:47:47.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_223/issue_223.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      392 2021-03-30 11:13:45.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_223/issue_223.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.547928 xmlschema-3.3.0/tests/test_cases/issues/issue_237/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.645928 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      191 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir1/issue_237.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1249 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.646928 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      141 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir2/issue_237a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      314 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir2/issue_237b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1041 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.647928 xmlschema-3.3.0/tests/test_cases/issues/issue_243/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      283 2021-05-03 11:37:57.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_243/issue_243.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2021-05-03 11:37:57.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_243/issue_243.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.648928 xmlschema-3.3.0/tests/test_cases/issues/issue_245/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_245/issue_245-valid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_245/issue_245.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2021-05-03 11:37:57.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_245/issue_245.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.648928 xmlschema-3.3.0/tests/test_cases/issues/issue_259/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     2422 2021-09-02 10:52:43.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_259/issue_259-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1432 2021-09-02 10:52:43.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_259/issue_259-2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.649928 xmlschema-3.3.0/tests/test_cases/issues/issue_265/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3471 2021-10-20 14:14:48.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_265/issue_265-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1411 2021-10-20 14:14:48.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      454 2021-10-20 14:14:48.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_265/issue_265-2-override.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.650928 xmlschema-3.3.0/tests/test_cases/issues/issue_266/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      538 2021-10-20 14:14:48.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      528 2021-10-20 14:14:48.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266-2.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      651 2021-11-11 15:30:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266b-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      551 2021-11-11 15:30:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266b-2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.651928 xmlschema-3.3.0/tests/test_cases/issues/issue_273/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      299 2021-12-08 19:41:39.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_273/issue_273.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      517 2021-12-08 19:41:39.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_273/issue_273.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.651928 xmlschema-3.3.0/tests/test_cases/issues/issue_276/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      122 2021-12-08 22:11:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_276/dummy.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      495 2021-12-08 22:11:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_276/schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.652928 xmlschema-3.3.0/tests/test_cases/issues/issue_298/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      114 2022-05-22 16:17:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_298/issue_298-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      240 2022-05-22 16:17:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_298/issue_298-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      792 2022-05-22 16:17:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_298/issue_298.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.653928 xmlschema-3.3.0/tests/test_cases/issues/issue_306/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      881 2022-06-24 14:13:22.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_306/issue_306-alt.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      203 2022-06-24 14:13:22.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_306/issue_306-invalid.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      182 2022-06-24 14:13:22.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_306/issue_306-valid.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      689 2022-06-24 14:13:22.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_306/issue_306.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.654928 xmlschema-3.3.0/tests/test_cases/issues/issue_311/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      786 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_311/correct_no_list.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      788 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_311/incorrect_with_list.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4013 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.655928 xmlschema-3.3.0/tests/test_cases/issues/issue_314/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      267 2022-07-21 09:40:50.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_314/issue_314.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1153 2022-07-21 09:40:50.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_314/issue_314.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.656928 xmlschema-3.3.0/tests/test_cases/issues/issue_315/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       66 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       63 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315-3.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       76 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315-4.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315-5.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      604 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315_mixed.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      456 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315_simple.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.657928 xmlschema-3.3.0/tests/test_cases/issues/issue_322/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      155 2022-08-26 15:33:28.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_322/issue_322.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      348 2022-08-26 15:33:28.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_322/issue_322.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.658928 xmlschema-3.3.0/tests/test_cases/issues/issue_324/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_324/issue_324-invalid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_324/issue_324-valid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      672 2022-08-28 05:56:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_324/issue_324.zip
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      384 2022-09-08 10:16:11.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_324/issue_324a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      190 2022-09-08 10:16:11.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_324/issue_324b.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.659928 xmlschema-3.3.0/tests/test_cases/issues/issue_334/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1814 2023-02-11 10:41:50.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_334/issue_334.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5149 2023-02-11 10:41:50.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_334/issue_334.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2663 2023-02-09 09:02:31.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_334/issue_334.zip
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.660928 xmlschema-3.3.0/tests/test_cases/issues/issue_341/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2070 2023-04-14 13:49:05.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_341/issue_341-ext.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      158 2023-04-14 13:49:05.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_341/issue_341.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1781 2023-04-14 13:49:05.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_341/issue_341.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.661928 xmlschema-3.3.0/tests/test_cases/issues/issue_349/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      329 2023-06-14 07:04:00.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_349/issue_349.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      574 2023-06-14 07:04:00.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_349/issue_349.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.661928 xmlschema-3.3.0/tests/test_cases/issues/issue_362/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.661928 xmlschema-3.3.0/tests/test_cases/issues/issue_362/dir1/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.662928 xmlschema-3.3.0/tests/test_cases/issues/issue_362/dir1/dir2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      433 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_362/dir1/dir2/issue_362_2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      334 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_362/dir1/issue_362_1.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.662928 xmlschema-3.3.0/tests/test_cases/issues/issue_362/dir2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      345 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_362/dir2/issue_362_2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      816 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_362/issue_362_1.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.664928 xmlschema-3.3.0/tests/test_cases/issues/issue_363/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      352 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_363/issue_363-invalid-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      347 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_363/issue_363-invalid-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_363/issue_363-invalid-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      323 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_363/issue_363.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      544 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_363/issue_363.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.665928 xmlschema-3.3.0/tests/test_cases/issues/issue_372/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       60 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_372/issue_372-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       83 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_372/issue_372-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      549 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_372/issue_372.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.666928 xmlschema-3.3.0/tests/test_cases/issues/issue_386/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      371 2024-02-18 21:08:04.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_386/issue_386-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      370 2024-02-18 21:08:04.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_386/issue_386-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1392 2024-02-18 21:08:04.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_386/issue_386-2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1402 2024-02-18 21:08:04.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_386/issue_386.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.667928 xmlschema-3.3.0/tests/test_cases/mypy/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      911 2022-05-20 16:16:20.000000 xmlschema-3.3.0/tests/test_cases/mypy/extra_validator.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     3350 2024-03-13 05:27:13.000000 xmlschema-3.3.0/tests/test_cases/mypy/protocols.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)     1905 2023-05-05 12:33:46.000000 xmlschema-3.3.0/tests/test_cases/mypy/schema_source.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)      646 2021-11-11 15:30:24.000000 xmlschema-3.3.0/tests/test_cases/mypy/simple_types.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.669928 xmlschema-3.3.0/tests/test_cases/resources/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/resources/dummy file.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       26 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/resources/dummy file.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      171 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/resources/external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       20 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/resources/malformed.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      308 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/resources/unparsed_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      170 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/resources/unused_external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      270 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/resources/unused_unparsed_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      129 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/resources/with_entity.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.671928 xmlschema-3.3.0/tests/test_cases/serialization/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4558 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/serialization/abdera.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5473 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/serialization/badgerfish.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3661 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/serialization/document.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5599 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/serialization/jsonml.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2264 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/serialization/parker.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6725 2024-04-17 17:34:18.000000 xmlschema-3.3.0/tests/test_cases/testfiles
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.553928 xmlschema-3.3.0/tests/test_cases/translations/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.671928 xmlschema-3.3.0/tests/test_cases/translations/pl/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    22092 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/translations/pl/tw-1(5)8e.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6795 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/translations/pl/tytul_wykonawczy_niekompletny.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11960 2024-03-13 05:27:13.000000 xmlschema-3.3.0/tests/test_cli.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    26576 2023-02-11 10:41:50.000000 xmlschema-3.3.0/tests/test_codegen.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    32551 2024-03-13 05:27:13.000000 xmlschema-3.3.0/tests/test_converters.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    28876 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_dataobjects.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24798 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_documents.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16654 2024-03-25 21:28:10.000000 xmlschema-3.3.0/tests/test_exports.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3234 2021-02-05 08:47:55.000000 xmlschema-3.3.0/tests/test_files.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30654 2024-03-25 21:28:10.000000 xmlschema-3.3.0/tests/test_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19738 2024-03-25 21:28:10.000000 xmlschema-3.3.0/tests/test_locations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5738 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_memory.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23506 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_namespaces.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4755 2023-09-20 10:58:25.000000 xmlschema-3.3.0/tests/test_package.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    58232 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_resources.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1785 2021-09-02 10:52:43.000000 xmlschema-3.3.0/tests/test_schemas.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5976 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_translations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2336 2024-03-13 05:27:13.000000 xmlschema-3.3.0/tests/test_typing.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1806 2021-09-02 10:52:43.000000 xmlschema-3.3.0/tests/test_validation.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    27292 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_w3c_suite.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    44084 2024-04-16 19:49:32.000000 xmlschema-3.3.0/tests/test_wsdl.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15023 2024-02-18 21:08:04.000000 xmlschema-3.3.0/tests/test_xpath.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.677928 xmlschema-3.3.0/tests/validation/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-3.3.0/tests/validation/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    79224 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/validation/test_decoding.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    33245 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/validation/test_encoding.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    29598 2024-04-14 19:45:21.000000 xmlschema-3.3.0/tests/validation/test_validation.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.682928 xmlschema-3.3.0/tests/validators/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-3.3.0/tests/validators/__init__.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    25878 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/validators/test_attributes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14352 2020-12-23 12:38:37.000000 xmlschema-3.3.0/tests/validators/test_builtins.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    34334 2024-02-18 21:08:04.000000 xmlschema-3.3.0/tests/validators/test_complex_types.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4333 2022-06-24 14:13:22.000000 xmlschema-3.3.0/tests/validators/test_elements.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16509 2024-04-17 17:34:18.000000 xmlschema-3.3.0/tests/validators/test_exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    63262 2024-03-25 21:28:10.000000 xmlschema-3.3.0/tests/validators/test_facets.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5409 2023-10-27 20:18:56.000000 xmlschema-3.3.0/tests/validators/test_global_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15868 2024-04-17 17:34:18.000000 xmlschema-3.3.0/tests/validators/test_groups.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19335 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/validators/test_identities.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    55290 2024-04-17 17:34:18.000000 xmlschema-3.3.0/tests/validators/test_models.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3447 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/validators/test_notations.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     8625 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/validators/test_particles.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    39368 2024-03-25 21:28:10.000000 xmlschema-3.3.0/tests/validators/test_schemas.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    10292 2024-03-23 21:43:51.000000 xmlschema-3.3.0/tests/validators/test_simple_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    34306 2024-04-17 17:34:18.000000 xmlschema-3.3.0/tests/validators/test_wildcards.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    38338 2024-03-25 21:28:10.000000 xmlschema-3.3.0/tests/validators/test_xsdbase.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1441 2024-03-13 05:41:48.000000 xmlschema-3.3.0/tox.ini
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.687928 xmlschema-3.3.0/xmlschema/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3089 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6145 2024-04-07 16:34:58.000000 xmlschema-3.3.0/xmlschema/aliases.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11866 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/cli.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.692928 xmlschema-3.3.0/xmlschema/converters/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      865 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/converters/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6255 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/converters/abdera.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6372 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/converters/badgerfish.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7504 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/converters/columnar.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24133 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/converters/default.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7629 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/converters/gdata.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5271 2024-01-07 11:20:34.000000 xmlschema-3.3.0/xmlschema/converters/jsonml.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5824 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/converters/parker.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5409 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/converters/unordered.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24831 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/dataobjects.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    38425 2024-01-07 11:20:34.000000 xmlschema-3.3.0/xmlschema/documents.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1235 2021-10-20 14:14:48.000000 xmlschema-3.3.0/xmlschema/exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15000 2024-04-07 16:34:58.000000 xmlschema-3.3.0/xmlschema/exports.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.695928 xmlschema-3.3.0/xmlschema/extras/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-02-05 09:05:33.000000 xmlschema-3.3.0/xmlschema/extras/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    21930 2023-05-18 20:18:16.000000 xmlschema-3.3.0/xmlschema/extras/codegen.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.556928 xmlschema-3.3.0/xmlschema/extras/templates/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.697928 xmlschema-3.3.0/xmlschema/extras/templates/python/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      997 2022-07-18 14:19:15.000000 xmlschema-3.3.0/xmlschema/extras/templates/python/bindings.py.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1116 2021-02-11 14:32:40.000000 xmlschema-3.3.0/xmlschema/extras/templates/python/sample.py.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24452 2024-01-07 11:20:34.000000 xmlschema-3.3.0/xmlschema/extras/wsdl.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16326 2024-03-25 21:28:10.000000 xmlschema-3.3.0/xmlschema/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      677 2020-11-10 10:13:55.000000 xmlschema-3.3.0/xmlschema/limits.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.558928 xmlschema-3.3.0/xmlschema/locale/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.557928 xmlschema-3.3.0/xmlschema/locale/en/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.698928 xmlschema-3.3.0/xmlschema/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    45327 2022-05-20 20:00:14.000000 xmlschema-3.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    64464 2024-03-19 14:02:56.000000 xmlschema-3.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.557928 xmlschema-3.3.0/xmlschema/locale/it/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.699928 xmlschema-3.3.0/xmlschema/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    47535 2022-05-20 20:00:14.000000 xmlschema-3.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    67361 2022-05-20 20:00:14.000000 xmlschema-3.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.558928 xmlschema-3.3.0/xmlschema/locale/pl/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.700928 xmlschema-3.3.0/xmlschema/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    47395 2023-07-27 19:52:28.000000 xmlschema-3.3.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.mo
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    66282 2023-07-27 19:52:28.000000 xmlschema-3.3.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.558928 xmlschema-3.3.0/xmlschema/locale/ru/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.700928 xmlschema-3.3.0/xmlschema/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    60295 2022-06-11 14:29:39.000000 xmlschema-3.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    79497 2022-06-11 14:29:39.000000 xmlschema-3.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    10643 2024-03-25 21:28:10.000000 xmlschema-3.3.0/xmlschema/locations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9653 2024-03-25 21:28:10.000000 xmlschema-3.3.0/xmlschema/names.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17001 2024-01-07 11:20:34.000000 xmlschema-3.3.0/xmlschema/namespaces.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)        0 2021-09-02 10:52:43.000000 xmlschema-3.3.0/xmlschema/py.typed
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    49667 2024-03-25 21:28:10.000000 xmlschema-3.3.0/xmlschema/resources.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.561928 xmlschema-3.3.0/xmlschema/schemas/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.701928 xmlschema-3.3.0/xmlschema/schemas/DSIG/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    10447 2023-07-27 19:52:28.000000 xmlschema-3.3.0/xmlschema/schemas/DSIG/xmldsig-core-schema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4664 2023-07-27 19:52:28.000000 xmlschema-3.3.0/xmlschema/schemas/DSIG/xmldsig11-schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.702928 xmlschema-3.3.0/xmlschema/schemas/HFP/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1534 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.703928 xmlschema-3.3.0/xmlschema/schemas/VC/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      984 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/VC/XMLSchema-versioning.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.704928 xmlschema-3.3.0/xmlschema/schemas/WSDL/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19204 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/WSDL/soap-encoding.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6061 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/WSDL/soap-envelope.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6005 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/WSDL/wsdl-soap.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11900 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/WSDL/wsdl.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.706928 xmlschema-3.3.0/xmlschema/schemas/XENC/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4360 2023-07-27 19:52:28.000000 xmlschema-3.3.0/xmlschema/schemas/XENC/xenc-schema-11.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6669 2023-07-27 19:52:28.000000 xmlschema-3.3.0/xmlschema/schemas/XENC/xenc-schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.707928 xmlschema-3.3.0/xmlschema/schemas/XHTML/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    65477 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/XHTML/xhtml1-strict.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.708928 xmlschema-3.3.0/xmlschema/schemas/XLINK/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8051 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/XLINK/xlink.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.708928 xmlschema-3.3.0/xmlschema/schemas/XML/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1277 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/XML/xml_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.709928 xmlschema-3.3.0/xmlschema/schemas/XSD_1.0/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    88033 2022-05-20 16:16:20.000000 xmlschema-3.3.0/xmlschema/schemas/XSD_1.0/XMLSchema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    44301 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/XSD_1.0/datatypes.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.710928 xmlschema-3.3.0/xmlschema/schemas/XSD_1.1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67728 2022-09-25 07:58:42.000000 xmlschema-3.3.0/xmlschema/schemas/XSD_1.1/XMLSchema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17497 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/XSD_1.1/datatypes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3767 2022-09-12 09:59:59.000000 xmlschema-3.3.0/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.710928 xmlschema-3.3.0/xmlschema/schemas/XSI/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      385 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/XSI/XMLSchema-instance_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.712928 xmlschema-3.3.0/xmlschema/testing/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2023-07-27 19:52:28.000000 xmlschema-3.3.0/xmlschema/testing/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    31080 2024-04-16 10:58:59.000000 xmlschema-3.3.0/xmlschema/testing/_builders.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7950 2023-10-18 10:59:40.000000 xmlschema-3.3.0/xmlschema/testing/_case_class.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9443 2023-12-19 09:41:12.000000 xmlschema-3.3.0/xmlschema/testing/_factory.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7658 2024-01-07 11:20:34.000000 xmlschema-3.3.0/xmlschema/testing/_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4891 2023-05-18 20:18:16.000000 xmlschema-3.3.0/xmlschema/testing/_observers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2072 2023-02-11 10:41:50.000000 xmlschema-3.3.0/xmlschema/translation.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.718928 xmlschema-3.3.0/xmlschema/validators/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3677 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/validators/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7277 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/validators/assertions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    34229 2024-04-16 13:14:15.000000 xmlschema-3.3.0/xmlschema/validators/attributes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19881 2022-08-26 15:33:28.000000 xmlschema-3.3.0/xmlschema/validators/builtins.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    46820 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/validators/complex_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67446 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/validators/elements.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17473 2024-04-07 16:34:58.000000 xmlschema-3.3.0/xmlschema/validators/exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    31285 2024-03-25 21:28:10.000000 xmlschema-3.3.0/xmlschema/validators/facets.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    33583 2024-04-07 16:34:58.000000 xmlschema-3.3.0/xmlschema/validators/global_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    64335 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/validators/groups.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7108 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/validators/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19395 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/validators/identities.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    27717 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/validators/models.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1611 2022-05-20 20:00:15.000000 xmlschema-3.3.0/xmlschema/validators/notations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7924 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/validators/particles.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)   107664 2024-04-16 13:49:31.000000 xmlschema-3.3.0/xmlschema/validators/schemas.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    62097 2024-03-25 21:28:10.000000 xmlschema-3.3.0/xmlschema/validators/simple_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    37949 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/validators/wildcards.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    42960 2024-03-30 06:19:36.000000 xmlschema-3.3.0/xmlschema/validators/xsdbase.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.719928 xmlschema-3.3.0/xmlschema/xpath/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      787 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/xpath/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1072 2024-02-18 21:08:04.000000 xmlschema-3.3.0/xmlschema/xpath/assertion_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1139 2024-02-18 21:08:04.000000 xmlschema-3.3.0/xmlschema/xpath/identity_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9622 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/xpath/mixin.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4101 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/xpath/proxy.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1231 2024-02-13 06:35:18.000000 xmlschema-3.3.0/xmlschema/xpath3.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.719928 xmlschema-3.3.0/xmlschema.egg-info/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8237 2024-04-17 17:34:43.000000 xmlschema-3.3.0/xmlschema.egg-info/PKG-INFO
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    19948 2024-04-17 17:34:43.000000 xmlschema-3.3.0/xmlschema.egg-info/SOURCES.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)        1 2024-04-17 17:34:43.000000 xmlschema-3.3.0/xmlschema.egg-info/dependency_links.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      150 2024-04-17 17:34:43.000000 xmlschema-3.3.0/xmlschema.egg-info/entry_points.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      256 2024-04-17 17:34:43.000000 xmlschema-3.3.0/xmlschema.egg-info/requires.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       10 2024-04-17 17:34:43.000000 xmlschema-3.3.0/xmlschema.egg-info/top_level.txt
```

### Comparing `xmlschema-3.2.1/CHANGELOG.rst` & `xmlschema-3.3.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 *********
 CHANGELOG
 *********
 
+`v3.3.0`_ (2024-04-17)
+======================
+* Rewrite the validation of openContent using InterleavedModelVisitor and SuffixedModelVisitor
+* Fix validation of XSD 1.1 'all' nested models
+
 `v3.2.1`_ (2024-04-07)
 ======================
 * Improve ModelVisitor and particle occurs checking
 * Fix interleave mode with XSD 1.1 open content (issue #397)
 * Fix for export/download of XSD sources with commented-out imports/include (issue #387)
 
 `v3.2.0`_ (2024-03-25)
@@ -688,7 +693,8 @@
 .. _v2.5.1: https://github.com/brunato/xmlschema/compare/v2.5.0...v2.5.1
 .. _v3.0.0: https://github.com/brunato/xmlschema/compare/v2.5.1...v3.0.0
 .. _v3.0.1: https://github.com/brunato/xmlschema/compare/v3.0.0...v3.0.1
 .. _v3.0.2: https://github.com/brunato/xmlschema/compare/v3.0.1...v3.0.2
 .. _v3.1.0: https://github.com/brunato/xmlschema/compare/v3.0.2...v3.1.0
 .. _v3.2.0: https://github.com/brunato/xmlschema/compare/v3.1.0...v3.2.0
 .. _v3.2.1: https://github.com/brunato/xmlschema/compare/v3.2.0...v3.2.1
+.. _v3.3.0: https://github.com/brunato/xmlschema/compare/v3.2.1...v3.3.0
```

### Comparing `xmlschema-3.2.1/LICENSE` & `xmlschema-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/PKG-INFO` & `xmlschema-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlschema
-Version: 3.2.1
+Version: 3.3.0
 Summary: An XML Schema validator and decoder
 Home-page: https://github.com/sissaschool/xmlschema
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `xmlschema-3.2.1/README.rst` & `xmlschema-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/doc/Makefile` & `xmlschema-3.3.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/doc/api.rst` & `xmlschema-3.3.0/doc/api.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/doc/components.rst` & `xmlschema-3.3.0/doc/components.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/doc/conf.py` & `xmlschema-3.3.0/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,17 +75,17 @@
 author = 'Davide Brunato'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '3.2'
+version = '3.3'
 # The full version, including alpha/beta/rc tags.
-release = '3.2.1'
+release = '3.3.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 # language = None
```

### Comparing `xmlschema-3.2.1/doc/converters.rst` & `xmlschema-3.3.0/doc/converters.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/doc/extras.rst` & `xmlschema-3.3.0/doc/extras.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/doc/features.rst` & `xmlschema-3.3.0/doc/features.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/doc/testing.rst` & `xmlschema-3.3.0/doc/testing.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/doc/usage.rst` & `xmlschema-3.3.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/setup.py` & `xmlschema-3.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 with Path(__file__).parent.joinpath('README.rst').open() as readme:
     long_description = readme.read()
 
 
 setup(
     name='xmlschema',
-    version='3.2.1',
+    version='3.3.0',
     packages=find_packages(include=['xmlschema*']),
     package_data={
         'xmlschema': ['py.typed', 'locale/**/*.mo', 'locale/**/*.po', 'schemas/*/*.xsd'],
         'xmlschema.extras': ['templates/*/*.jinja'],
     },
     entry_points={
         'console_scripts': [
```

### Comparing `xmlschema-3.2.1/tests/check_memory.py` & `xmlschema-3.3.0/tests/check_memory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_all.py` & `xmlschema-3.3.0/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/collection/collection-1_error.xml` & `xmlschema-3.3.0/tests/test_cases/examples/collection/collection-1_error.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/collection/collection-default.xml` & `xmlschema-3.3.0/tests/test_cases/examples/collection/collection-default.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/collection/collection-redef-xmlns.xml` & `xmlschema-3.3.0/tests/test_cases/examples/collection/collection-redef-xmlns.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/collection/collection.py` & `xmlschema-3.3.0/tests/test_cases/examples/collection/collection.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/collection/collection.xml` & `xmlschema-3.3.0/tests/test_cases/examples/collection/collection.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/collection/collection.xsd` & `xmlschema-3.3.0/tests/test_cases/examples/collection/collection.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/collection/collection2.xml` & `xmlschema-3.3.0/tests/test_cases/examples/collection/collection2.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/collection/collection2.xsd` & `xmlschema-3.3.0/tests/test_cases/examples/collection/collection2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/collection/collection3.xml` & `xmlschema-3.3.0/tests/test_cases/examples/collection/collection3.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/collection/collection3.xsd` & `xmlschema-3.3.0/tests/test_cases/examples/collection/collection3.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/collection/collection3bis.xml` & `xmlschema-3.3.0/tests/test_cases/examples/collection/collection3bis.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/collection/collection3bis.xsd` & `xmlschema-3.3.0/tests/test_cases/examples/collection/collection3bis.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/collection/collection4.xml` & `xmlschema-3.3.0/tests/test_cases/examples/collection/collection4.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/collection/collection4.xsd` & `xmlschema-3.3.0/tests/test_cases/examples/collection/collection4.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/collection/collection5.xsd` & `xmlschema-3.3.0/tests/test_cases/examples/collection/collection5.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/menù/menù-ascii.xml` & `xmlschema-3.3.0/tests/test_cases/examples/menù/menù-ascii.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/menù/menù-ascii.xsd` & `xmlschema-3.3.0/tests/test_cases/examples/menù/menù-ascii.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/menù/menù-cp1252.xml` & `xmlschema-3.3.0/tests/test_cases/examples/menù/menù-cp1252.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/menù/menù.xml` & `xmlschema-3.3.0/tests/test_cases/examples/menù/menù.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/stockquote/stockquote.wsdl` & `xmlschema-3.3.0/tests/test_cases/examples/stockquote/stockquote.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/stockquote/stockquote.xsd` & `xmlschema-3.3.0/tests/test_cases/examples/stockquote/stockquote.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/stockquote/stockquoteservice.wsdl` & `xmlschema-3.3.0/tests/test_cases/examples/stockquote/stockquoteservice.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/vehicles/invalid.xsd` & `xmlschema-3.3.0/tests/test_cases/examples/vehicles/invalid.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/vehicles/vehicles-max.xsd` & `xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-max.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip` & `xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/examples/vehicles/vehicles.xsd` & `xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/attributes/default_attributes-missing_group.xsd` & `xmlschema-3.3.0/tests/test_cases/features/attributes/default_attributes-missing_group.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/attributes/default_attributes.xsd` & `xmlschema-3.3.0/tests/test_cases/features/attributes/default_attributes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/builtins/builtins.xml` & `xmlschema-3.3.0/tests/test_cases/features/builtins/builtins.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/builtins/builtins.xsd` & `xmlschema-3.3.0/tests/test_cases/features/builtins/builtins.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/decoder/data.xml` & `xmlschema-3.3.0/tests/test_cases/features/decoder/data.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/decoder/data2.xml` & `xmlschema-3.3.0/tests/test_cases/features/decoder/data2.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/decoder/data3.xml` & `xmlschema-3.3.0/tests/test_cases/features/decoder/data3.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/decoder/long-sequence-1.xsd` & `xmlschema-3.3.0/tests/test_cases/features/decoder/long-sequence-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/decoder/mixed-content.xsd` & `xmlschema-3.3.0/tests/test_cases/features/decoder/mixed-content.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/decoder/simple-types.xsd` & `xmlschema-3.3.0/tests/test_cases/features/decoder/simple-types.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/derivations/complex-extensions.xsd` & `xmlschema-3.3.0/tests/test_cases/features/derivations/complex-extensions.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd` & `xmlschema-3.3.0/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/derivations/complex11-restrictions.xsd` & `xmlschema-3.3.0/tests/test_cases/features/derivations/complex11-restrictions.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd` & `xmlschema-3.3.0/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/derivations/invalid-restrictions1.xsd` & `xmlschema-3.3.0/tests/test_cases/features/derivations/invalid-restrictions1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/derivations/invalid-restrictions2.xsd` & `xmlschema-3.3.0/tests/test_cases/features/derivations/invalid-restrictions2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/derivations/list_types.xsd` & `xmlschema-3.3.0/tests/test_cases/features/derivations/list_types.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/elements/type_alternatives-no-ns.xsd` & `xmlschema-3.3.0/tests/test_cases/features/elements/type_alternatives-no-ns.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/elements/type_alternatives.xsd` & `xmlschema-3.3.0/tests/test_cases/features/elements/type_alternatives.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/models/billion_laughs_model.xsd` & `xmlschema-3.3.0/tests/test_cases/features/models/billion_laughs_model.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/models/illegal-declarations.xsd` & `xmlschema-3.3.0/tests/test_cases/features/models/illegal-declarations.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/models/illegal-occurs.xsd` & `xmlschema-3.3.0/tests/test_cases/features/models/illegal-occurs.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/models/invalid_models1.xsd` & `xmlschema-3.3.0/tests/test_cases/features/models/invalid_models1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/models/invalid_models2.xsd` & `xmlschema-3.3.0/tests/test_cases/features/models/invalid_models2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/models/models.xsd` & `xmlschema-3.3.0/tests/test_cases/features/models/models.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/models/recursive-groups.xsd` & `xmlschema-3.3.0/tests/test_cases/features/models/recursive-groups.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/models/valid_model1.xsd` & `xmlschema-3.3.0/tests/test_cases/features/models/valid_model1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/namespaces/import-case1.xsd` & `xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/namespaces/import-case2.xsd` & `xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/namespaces/import-case4a.xsd` & `xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case4a.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/namespaces/import-case4b.xsd` & `xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case4b.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/namespaces/include-case2.xsd` & `xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/namespaces/include-case2bis.xsd` & `xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case2bis.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/namespaces/include-case3.xsd` & `xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case3.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/namespaces/include-case5.xsd` & `xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case5.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/patterns/patterns.xml` & `xmlschema-3.3.0/tests/test_cases/features/patterns/patterns.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/patterns/patterns.xsd` & `xmlschema-3.3.0/tests/test_cases/features/patterns/patterns.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example3.wsdl` & `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example3.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl` & `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl` & `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example4.wsdl` & `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example4.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl` & `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example5.wsdl` & `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example5.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl` & `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl` & `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_008/issue_008.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_008/issue_008.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_013/issue_013-1.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_013/issue_013-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_013/issue_013.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_013/issue_013.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_014/issue014.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_014/issue014.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_018/issue_018.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_018/issue_018.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_022/README.md` & `xmlschema-3.3.0/tests/test_cases/issues/issue_022/README.md`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_022/xsd_string.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_022/xsd_string.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_026/issue_026.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_026/issue_026.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_035/dates.xml` & `xmlschema-3.3.0/tests/test_cases/issues/issue_035/dates.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_035/dates.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_035/dates.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_041/issue_041.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_041/issue_041.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_051/issue_051.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_051/issue_051.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_073/issue_073.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_073/issue_073.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_086/issue_086.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_086/issue_086.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_105/issue_105.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_105/issue_105.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_111/issue_111.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_111/issue_111.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_115/Rotation.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_115/Rotation.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_171/issue_171.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_171/issue_171.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_171/issue_171b.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_171/issue_171b.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_187/issue_187_1.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_187/issue_187_1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_187/issue_187_2.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_187/issue_187_2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_190/issue_190.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_190/issue_190.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_200/issue_200.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_200/issue_200.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_203/issue_203.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_203/issue_203.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_203/issue_203alt.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_203/issue_203alt.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_204/issue_204.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_204/issue_204.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_208/issue_208.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_208/issue_208.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_222/issue_222.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_222/issue_222.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl` & `xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl` & `xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_237/dir2/stockquote.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_243/issue_243.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_243/issue_243.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_245/issue_245-valid.xml` & `xmlschema-3.3.0/tests/test_cases/issues/issue_245/issue_245-valid.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_245/issue_245.xml` & `xmlschema-3.3.0/tests/test_cases/issues/issue_245/issue_245.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_245/issue_245.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_245/issue_245.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_259/issue_259-1.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_259/issue_259-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_259/issue_259-2.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_259/issue_259-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_265/issue_265-1.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_265/issue_265-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_266/issue_266-1.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_266/issue_266-2.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_266/issue_266b-1.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266b-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_266/issue_266b-2.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266b-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_273/issue_273.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_273/issue_273.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_298/issue_298.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_298/issue_298.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_306/issue_306-alt.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_306/issue_306-alt.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_306/issue_306.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_306/issue_306.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_311/correct_no_list.xml` & `xmlschema-3.3.0/tests/test_cases/issues/issue_311/correct_no_list.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_311/incorrect_with_list.xml` & `xmlschema-3.3.0/tests/test_cases/issues/issue_311/incorrect_with_list.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_314/issue_314.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_314/issue_314.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_315/issue_315_mixed.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315_mixed.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_324/issue_324.zip` & `xmlschema-3.3.0/tests/test_cases/issues/issue_324/issue_324.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_334/issue_334.xml` & `xmlschema-3.3.0/tests/test_cases/issues/issue_334/issue_334.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_334/issue_334.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_334/issue_334.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_334/issue_334.zip` & `xmlschema-3.3.0/tests/test_cases/issues/issue_334/issue_334.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_341/issue_341-ext.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_341/issue_341-ext.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_341/issue_341.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_341/issue_341.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_349/issue_349.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_349/issue_349.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_362/issue_362_1.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_362/issue_362_1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_363/issue_363.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_363/issue_363.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_372/issue_372.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_372/issue_372.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_386/issue_386-2.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_386/issue_386-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/issues/issue_386/issue_386.xsd` & `xmlschema-3.3.0/tests/test_cases/issues/issue_386/issue_386.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/mypy/extra_validator.py` & `xmlschema-3.3.0/tests/test_cases/mypy/extra_validator.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/mypy/protocols.py` & `xmlschema-3.3.0/tests/test_cases/mypy/protocols.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/mypy/schema_source.py` & `xmlschema-3.3.0/tests/test_cases/mypy/schema_source.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/mypy/simple_types.py` & `xmlschema-3.3.0/tests/test_cases/mypy/simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/serialization/abdera.json` & `xmlschema-3.3.0/tests/test_cases/serialization/abdera.json`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/serialization/badgerfish.json` & `xmlschema-3.3.0/tests/test_cases/serialization/badgerfish.json`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/serialization/document.xml` & `xmlschema-3.3.0/tests/test_cases/serialization/document.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/serialization/jsonml.json` & `xmlschema-3.3.0/tests/test_cases/serialization/jsonml.json`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/serialization/parker.json` & `xmlschema-3.3.0/tests/test_cases/serialization/parker.json`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/testfiles` & `xmlschema-3.3.0/tests/test_cases/testfiles`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 issues/issue_018/issue_018-1.xml --version=1.1
 issues/issue_026/issue_026-1.xml
 issues/issue_026/issue_026-2.xml --errors=1
 issues/issue_026/issue_026-3.xml --errors=1
 issues/issue_028/issue_028-1.xml
 issues/issue_028/issue_028-2.xml --errors=1
 issues/issue_029/issue_029-1.xml
-issues/issue_029/issue_029-2.xml --errors=2
+issues/issue_029/issue_029-2.xml --errors=1
 issues/issue_029/issue_029-3.xml --errors=1
 issues/issue_035/dates.xsd
 issues/issue_035/dates.xml --errors=1
 issues/issue_041/issue_041.xsd
 issues/issue_041/issue_041.xml
 issues/issue_045/issue_045.xsd
 issues/issue_051/issue_051.xml
```

### Comparing `xmlschema-3.2.1/tests/test_cases/translations/pl/tw-1(5)8e.xsd` & `xmlschema-3.3.0/tests/test_cases/translations/pl/tw-1(5)8e.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cases/translations/pl/tytul_wykonawczy_niekompletny.xml` & `xmlschema-3.3.0/tests/test_cases/translations/pl/tytul_wykonawczy_niekompletny.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_cli.py` & `xmlschema-3.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_codegen.py` & `xmlschema-3.3.0/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_converters.py` & `xmlschema-3.3.0/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_dataobjects.py` & `xmlschema-3.3.0/tests/test_dataobjects.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_documents.py` & `xmlschema-3.3.0/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_exports.py` & `xmlschema-3.3.0/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_files.py` & `xmlschema-3.3.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_helpers.py` & `xmlschema-3.3.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_locations.py` & `xmlschema-3.3.0/tests/test_locations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_memory.py` & `xmlschema-3.3.0/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_namespaces.py` & `xmlschema-3.3.0/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_package.py` & `xmlschema-3.3.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_resources.py` & `xmlschema-3.3.0/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_schemas.py` & `xmlschema-3.3.0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_translations.py` & `xmlschema-3.3.0/tests/test_translations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_typing.py` & `xmlschema-3.3.0/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_validation.py` & `xmlschema-3.3.0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_w3c_suite.py` & `xmlschema-3.3.0/tests/test_w3c_suite.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_wsdl.py` & `xmlschema-3.3.0/tests/test_wsdl.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/test_xpath.py` & `xmlschema-3.3.0/tests/test_xpath.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/validation/test_decoding.py` & `xmlschema-3.3.0/tests/validation/test_decoding.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/validation/test_encoding.py` & `xmlschema-3.3.0/tests/validation/test_encoding.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/validation/test_validation.py` & `xmlschema-3.3.0/tests/validation/test_validation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/validators/test_attributes.py` & `xmlschema-3.3.0/tests/validators/test_attributes.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/validators/test_builtins.py` & `xmlschema-3.3.0/tests/validators/test_builtins.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/validators/test_complex_types.py` & `xmlschema-3.3.0/tests/validators/test_complex_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/validators/test_elements.py` & `xmlschema-3.3.0/tests/validators/test_elements.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/validators/test_exceptions.py` & `xmlschema-3.3.0/tests/validators/test_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,19 +372,20 @@
         invalid_child = ctx.exception.invalid_child
         self.assertTrue(is_etree_element(invalid_child))
         self.assertEqual(invalid_child.tag, 'c1')
 
         xml_source = '<a><b1></b1><b2><c1/><c1/></b2></a>'
         resource = XMLResource(xml_source, lazy=True)
         errors = list(schema.iter_errors(resource))
-        self.assertEqual(len(errors), 4)
+        self.assertEqual(len(errors), 3)
         self.assertIsNone(errors[0].invalid_child)
-        self.assertIsNone(errors[1].invalid_child)
-        self.assertIsNotNone(errors[2].invalid_child)
-        self.assertIsNotNone(errors[3].invalid_child)
+        self.assertTrue(is_etree_element(errors[1].invalid_child))
+        self.assertEqual(errors[1].invalid_child.tag, 'c1')
+        self.assertTrue(is_etree_element(errors[2].invalid_child))
+        self.assertEqual(errors[2].invalid_child.tag, 'b2')
 
 
 if __name__ == '__main__':
     import platform
     header_template = "Test xmlschema's validator exceptions with Python {} on {}"
     header = header_template.format(platform.python_version(), platform.platform())
     print('{0}\n{1}\n{0}'.format("*" * len(header), header))
```

### Comparing `xmlschema-3.2.1/tests/validators/test_facets.py` & `xmlschema-3.3.0/tests/validators/test_facets.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/validators/test_global_maps.py` & `xmlschema-3.3.0/tests/validators/test_global_maps.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/validators/test_groups.py` & `xmlschema-3.3.0/tests/validators/test_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     """A subclass for testing XSD models, that disables element parsing and schema bindings."""
 
     def __init__(self, model: str, min_occurs: int = 1, max_occurs: Optional[int] = 1) -> None:
         ParticleMixin.__init__(self, min_occurs, max_occurs)
         if model not in {'sequence', 'choice', 'all'}:
             raise XMLSchemaValueError("invalid model {!r} for a group".format(model))
         self._group: List[Union[ParticleMixin, 'ModelGroup']] = []
+        self.content = self._group
         self.model: str = model
 
     def __repr__(self) -> str:
         return '%s(model=%r, occurs=%r)' % (self.__class__.__name__, self.model, self.occurs)
 
     @property
     def xsd_version(self) -> str:
```

### Comparing `xmlschema-3.2.1/tests/validators/test_identities.py` & `xmlschema-3.3.0/tests/validators/test_identities.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/validators/test_models.py` & `xmlschema-3.3.0/tests/validators/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
 """Tests concerning model groups validation"""
 import unittest
 import os.path
+import warnings
 from textwrap import dedent
 from typing import Any, Union, List, Optional
 
 from xmlschema import XMLSchema10, XMLSchema11
 from xmlschema.exceptions import XMLSchemaValueError
 from xmlschema.validators.exceptions import XMLSchemaValidationError
 from xmlschema.validators.particles import ParticleMixin
@@ -29,14 +30,15 @@
     """A subclass for testing XSD models, that disables element parsing and schema bindings."""
 
     def __init__(self, model: str, min_occurs: int = 1, max_occurs: Optional[int] = 1) -> None:
         ParticleMixin.__init__(self, min_occurs, max_occurs)
         if model not in {'sequence', 'choice', 'all'}:
             raise XMLSchemaValueError("invalid model {!r} for a group".format(model))
         self._group: List[Union[ParticleMixin, 'ModelGroup']] = []
+        self.content = self._group
         self.model: str = model
 
     def __repr__(self) -> str:
         return '%s(model=%r, occurs=%r)' % (self.__class__.__name__, self.model, self.occurs)
 
     append: Any
 
@@ -170,15 +172,17 @@
         self.check_advance_true(model)     # <car>
         self.check_advance_true(model)     # <car>
         self.check_advance_true(model)     # <car>
         self.check_advance_false(model)    # (end)
         self.assertIsNone(model.element)
 
         model = ModelVisitor(group)
-        self.check_advance_false(model, [(group[0], 0, [group[0]])])  # <not-a-car>
+        self.check_advance_false(
+            model, [(group[0], 0, [group[0]]), (group, 0, [group[0]])]
+        )  # <not-a-car>
         self.assertIsNone(model.element)
 
     def test_person_type_model(self):
         # Sequence with four single elements, last two are also emptiable.
         group = self.col_schema.types['personType'].content
 
         model = ModelVisitor(group)
@@ -539,15 +543,17 @@
         self.assertIsNone(model.element)
 
     def test_model_group7(self):
         group = self.models_schema.types['complexType7'].content
 
         model = ModelVisitor(group)
         self.assertEqual(model.element, group[0][0])
-        self.check_stop(model, [(group[0], 0, [group[0][0]])])
+        self.check_stop(
+            model, [(group[0][0], 0, [group[0][0]]), (group, 0, [group[0][0]])]
+        )
 
         group = self.models_schema.types['complexType7_emptiable'].content
 
         model = ModelVisitor(group)
         self.assertEqual(model.element, group[0][0])
         self.check_stop(model)
 
@@ -1067,30 +1073,20 @@
                     <xs:element name="B6" minOccurs="0" />
                     <xs:element name="B7" />
                 </xs:sequence>
             </xs:complexType>
             """)
 
         group = schema.types['A_type'].content
-        model = ModelVisitor(group)
-
         content = [('B3', 10), ('B4', None), ('B5', True), ('B6', 'alpha'), ('B7', 20)]
-        model.restart()
-        self.assertListEqual(
-            list(model.iter_collapsed_content(content)), content
-        )
         self.assertListEqual(
             list(iter_collapsed_content(content, group)), content
         )
 
         content = [('B3', 10), ('B5', True), ('B6', 'alpha'), ('B7', 20)]  # Missing B4
-        model.restart()
-        self.assertListEqual(
-            list(model.iter_collapsed_content(content)), content
-        )
         self.assertListEqual(
             list(iter_collapsed_content(content, group)), content
         )
 
     def test_iter_collapsed_content_with_repeated_elements(self):
         schema = self.get_schema("""
             <xs:element name="A" type="A_type" />
@@ -1193,14 +1189,72 @@
 
         content = [('B1', 'abc'), ('B2', 10), ('X', None)]
         self.assertListEqual(list(iter_collapsed_content(content, group)), content)
 
         content = [('X', None), ('B1', 'abc'), ('B2', 10), ('B3', False)]
         self.assertListEqual(list(iter_collapsed_content(content, group)), content)
 
+    def test_deprecated_methods(self):
+        schema = self.get_schema("""
+            <xs:element name="A" type="A_type" />
+            <xs:complexType name="A_type">
+                <xs:sequence maxOccurs="10">
+                    <xs:element name="B1" minOccurs="0" />
+                    <xs:element name="B2" minOccurs="0" />
+                </xs:sequence>
+            </xs:complexType>
+            """)
+
+        group = schema.types['A_type'].content
+        model = ModelVisitor(group)
+        default_namespace = 'http://xmlschema.test/ns'
+        content = [('B1', 1), ('B1', 2), ('B2', 3)]
+
+        with warnings.catch_warnings(record=True) as ctx:
+            warnings.   simplefilter("always")
+            self.assertListEqual(
+                list(model.iter_collapsed_content(content)),
+                [('B1', 1), ('B2', 3), ('B1', 2)]
+            )
+            self.assertEqual(len(ctx), 1, "Expected one deprecation warning")
+            self.assertIn("use iter_collapsed_content()", str(ctx[0].message))
+            self.assertNotIn("Don't provide default_namespace", str(ctx[0].message))
+
+        with warnings.catch_warnings(record=True) as ctx:
+            warnings.simplefilter("always")
+            self.assertListEqual(
+                list(model.iter_collapsed_content(content, default_namespace)),
+                [('B1', 1), ('B2', 3), ('B1', 2)]
+            )
+            self.assertEqual(len(ctx), 1, "Expected one deprecation warning")
+            self.assertIn("use iter_collapsed_content()", str(ctx[0].message))
+            self.assertIn("Don't provide default_namespace", str(ctx[0].message))
+
+        content = [('B2', 1), ('B1', 2), ('B2', 3), ('B1', 4)]
+
+        with warnings.catch_warnings(record=True) as ctx:
+            warnings.   simplefilter("always")
+            self.assertListEqual(
+                list(model.iter_unordered_content(content)),
+                [('B1', 2), ('B2', 1), ('B1', 4), ('B2', 3)]
+            )
+            self.assertEqual(len(ctx), 1, "Expected one deprecation warning")
+            self.assertIn("use iter_unordered_content()", str(ctx[0].message))
+            self.assertNotIn("Don't provide default_namespace", str(ctx[0].message))
+
+        with warnings.catch_warnings(record=True) as ctx:
+            warnings.simplefilter("always")
+            self.assertListEqual(
+                list(model.iter_unordered_content(content, default_namespace)),
+                [('B1', 2), ('B2', 1), ('B1', 4), ('B2', 3)]
+            )
+            self.assertEqual(len(ctx), 1, "Expected one deprecation warning")
+            self.assertIn("use iter_unordered_content()", str(ctx[0].message))
+            self.assertIn("Don't provide default_namespace", str(ctx[0].message))
+
 
 class TestModelPaths(unittest.TestCase):
 
     def test_distinguishable_paths_one_level(self):
         group = ModelGroup('sequence', min_occurs=0)
         group.append(ModelGroup('sequence'))
         group.append(ModelGroup('sequence'))
```

### Comparing `xmlschema-3.2.1/tests/validators/test_notations.py` & `xmlschema-3.3.0/tests/validators/test_notations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/validators/test_particles.py` & `xmlschema-3.3.0/tests/validators/test_particles.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/validators/test_schemas.py` & `xmlschema-3.3.0/tests/validators/test_schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/validators/test_simple_types.py` & `xmlschema-3.3.0/tests/validators/test_simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tests/validators/test_wildcards.py` & `xmlschema-3.3.0/tests/validators/test_wildcards.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,16 +378,16 @@
               <xs:element name="Date" type="xs:gYear"/>
               <xs:element name="ISBN" type="xs:string"/>
               <xs:element name="Publisher" type="xs:string"/>
             </xs:sequence>
           </xs:complexType>
         </xs:element>""")
         self.assertEqual(schema.elements['Book'].type.open_content.mode, 'interleave')
-        self.assertEqual(schema.elements['Book'].type.open_content.any_element.min_occurs, 0)
-        self.assertIsNone(schema.elements['Book'].type.open_content.any_element.max_occurs)
+        self.assertEqual(schema.elements['Book'].type.open_content.any_element.min_occurs, 1)
+        self.assertEqual(schema.elements['Book'].type.open_content.any_element.max_occurs, 1)
 
         schema = self.check_schema("""
         <xs:complexType name="name">
           <xs:openContent>
             <xs:any namespace="##other" processContents="skip"/>
           </xs:openContent>
           <xs:sequence>
@@ -417,16 +417,16 @@
           <xs:sequence>
             <xs:element name="given" type="xs:string"/>
             <xs:element name="middle" type="xs:string" minOccurs="0"/>
             <xs:element name="family" type="xs:string"/>
           </xs:sequence>
         </xs:complexType>""")
         self.assertEqual(schema.types['name'].open_content.mode, 'suffix')
-        self.assertEqual(schema.types['name'].open_content.any_element.min_occurs, 0)
-        self.assertIsNone(schema.types['name'].open_content.any_element.max_occurs)
+        self.assertEqual(schema.types['name'].open_content.any_element.min_occurs, 1)
+        self.assertEqual(schema.types['name'].open_content.any_element.max_occurs, 1)
 
         self.check_schema("""
         <xs:complexType name="name">
           <xs:openContent mode="suffix"/>
           <xs:sequence>
             <xs:element name="given" type="xs:string"/>
             <xs:element name="middle" type="xs:string" minOccurs="0"/>
```

### Comparing `xmlschema-3.2.1/tests/validators/test_xsdbase.py` & `xmlschema-3.3.0/tests/validators/test_xsdbase.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/tox.ini` & `xmlschema-3.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/__init__.py` & `xmlschema-3.3.0/xmlschema/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     XMLSchemaModelError, XMLSchemaModelDepthError, XMLSchemaValidationError,
     XMLSchemaDecodeError, XMLSchemaEncodeError, XMLSchemaChildrenValidationError,
     XMLSchemaStopValidation, XMLSchemaIncludeWarning, XMLSchemaImportWarning,
     XMLSchemaTypeTableWarning, XMLSchemaAssertPathWarning, XsdGlobals, XMLSchemaBase,
     XMLSchema, XMLSchema10, XMLSchema11, XsdComponent, XsdType, XsdElement, XsdAttribute
 )
 
-__version__ = '3.2.1'
+__version__ = '3.3.0'
 __author__ = "Davide Brunato"
 __contact__ = "brunato@sissa.it"
 __copyright__ = "Copyright 2016-2024, SISSA"
 __license__ = "MIT"
 __status__ = "Production/Stable"
 
 __all__ = [
```

### Comparing `xmlschema-3.2.1/xmlschema/aliases.py` & `xmlschema-3.3.0/xmlschema/aliases.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/cli.py` & `xmlschema-3.3.0/xmlschema/cli.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/converters/__init__.py` & `xmlschema-3.3.0/xmlschema/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/converters/abdera.py` & `xmlschema-3.3.0/xmlschema/converters/abdera.py`

 * *Files 10% similar despite different names*

```diff
@@ -140,25 +140,18 @@
                     if not isinstance(value, MutableSequence) or not value:
                         content.append((self.unmap_qname(name), value))
                     elif isinstance(value[0], (MutableMapping, MutableSequence)):
                         ns_name = self.unmap_qname(name)
                         for item in value:
                             content.append((ns_name, item))
                     else:
-                        xsd_group = xsd_element.type.model_group
-                        if xsd_group is None:
-                            xsd_group = xsd_element.any_type.model_group
-                            assert xsd_group is not None
-
                         ns_name = self.unmap_qname(name)
-                        for xsd_child in xsd_group.iter_elements():
-                            matched_element = xsd_child.match(ns_name, resolve=True)
-                            if matched_element is not None:
-                                if matched_element.type and matched_element.type.is_list():
-                                    content.append((ns_name, value))
-                                else:
-                                    content.extend((ns_name, item) for item in value)
-                                break
+                        xsd_child = xsd_element.match_child(ns_name)
+                        if xsd_child is not None:
+                            if xsd_child.type and xsd_child.type.is_list():
+                                content.append((ns_name, value))
+                            else:
+                                content.extend((ns_name, item) for item in value)
                         else:
-                            content.append((ns_name, value))
+                            content.extend((ns_name, item) for item in value)
 
             return ElementData(tag, None, content, attributes, None)
```

### Comparing `xmlschema-3.2.1/xmlschema/converters/badgerfish.py` & `xmlschema-3.3.0/xmlschema/converters/badgerfish.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,25 +136,18 @@
                 ns_name = self.unmap_qname(name, xmlns=self.get_xmlns_from_data(value))
                 content.append((ns_name, value))
             elif isinstance(value[0], (MutableMapping, MutableSequence)):
                 ns_name = self.unmap_qname(name, xmlns=self.get_xmlns_from_data(value[0]))
                 for item in value:
                     content.append((ns_name, item))
             else:
-                xsd_group = xsd_element.type.model_group
-                if xsd_group is None:
-                    xsd_group = xsd_element.any_type.model_group
-                    assert xsd_group is not None
-
                 ns_name = self.unmap_qname(name)
-                for xsd_child in xsd_group.iter_elements():
-                    matched_element = xsd_child.match(ns_name, resolve=True)
-                    if matched_element is not None:
-                        if matched_element.type and matched_element.type.is_list():
-                            content.append((ns_name, value))
-                        else:
-                            content.extend((ns_name, item) for item in value)
-                        break
+                xsd_child = xsd_element.match_child(ns_name)
+                if xsd_child is not None:
+                    if xsd_child.type and xsd_child.type.is_list():
+                        content.append((ns_name, value))
+                    else:
+                        content.extend((ns_name, item) for item in value)
                 else:
-                    content.append((ns_name, value))
+                    content.extend((ns_name, item) for item in value)
 
         return ElementData(tag, text, content, attributes, xmlns)
```

### Comparing `xmlschema-3.2.1/xmlschema/converters/columnar.py` & `xmlschema-3.3.0/xmlschema/converters/columnar.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,25 +156,18 @@
                 attributes[ns_name] = value
             elif not isinstance(value, MutableSequence) or not value:
                 content.append((self.unmap_qname(name), value))
             elif isinstance(value[0], (MutableMapping, MutableSequence)):
                 ns_name = self.unmap_qname(name)
                 content.extend((ns_name, item) for item in value)
             else:
-                xsd_group = xsd_element.type.model_group
-                if xsd_group is None:
-                    xsd_group = xsd_element.any_type.model_group
-                    assert xsd_group is not None
-
                 ns_name = self.unmap_qname(name)
-                for xsd_child in xsd_group.iter_elements():
-                    matched_element = xsd_child.match(ns_name, resolve=True)
-                    if matched_element is not None:
-                        if matched_element.type and matched_element.type.is_list():
-                            content.append((xsd_child.name, value))
-                        else:
-                            content.extend((xsd_child.name, item) for item in value)
-                        break
+                xsd_child = xsd_element.match_child(ns_name)
+                if xsd_child is not None:
+                    if xsd_child.type and xsd_child.type.is_list():
+                        content.append((ns_name, value))
+                    else:
+                        content.extend((ns_name, item) for item in value)
                 else:
-                    content.append((ns_name, value))
+                    content.extend((ns_name, item) for item in value)
 
         return ElementData(xsd_element.name, text, content, attributes, None)
```

### Comparing `xmlschema-3.2.1/xmlschema/converters/default.py` & `xmlschema-3.3.0/xmlschema/converters/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -500,34 +500,20 @@
             elif not isinstance(value, MutableSequence) or not value:
                 ns_name = self.unmap_qname(name, xmlns=self.get_xmlns_from_data(value))
                 content.append((ns_name, value))
             elif isinstance(value[0], (MutableMapping, MutableSequence)):
                 ns_name = self.unmap_qname(name, xmlns=self.get_xmlns_from_data(value[0]))
                 content.extend((ns_name, item) for item in value)
             else:
-                xsd_group = xsd_element.type.model_group
-                if xsd_group is None:
-                    # fallback to xs:anyType encoder
-                    xsd_group = xsd_element.any_type.model_group
-                    assert xsd_group is not None
-
                 ns_name = self.unmap_qname(name)
-                for xsd_child in xsd_group.iter_elements():
-                    matched_element = xsd_child.match(ns_name, resolve=True)
-                    if matched_element is not None:
-                        if matched_element.type and matched_element.type.is_list():
-                            content.append((ns_name, value))
-                        else:
-                            content.extend((ns_name, item) for item in value)
-                        break
-                else:
-                    if self.attr_prefix == '' and ns_name not in attributes:
-                        for key, xsd_attribute in xsd_element.attributes.items():
-                            if key and xsd_attribute.is_matching(ns_name):
-                                attributes[key] = value
-                                break
-                        else:
-                            content.append((ns_name, value))
-                    else:
+                xsd_child = xsd_element.match_child(ns_name)
+                if xsd_child is not None:
+                    if xsd_child.type and xsd_child.type.is_list():
                         content.append((ns_name, value))
+                    else:
+                        content.extend((ns_name, item) for item in value)
+                elif self.attr_prefix == '' and ns_name in xsd_element.attributes:
+                    attributes[ns_name] = value
+                else:
+                    content.extend((ns_name, item) for item in value)
 
         return ElementData(xsd_element.name, text, content, attributes, xmlns)
```

### Comparing `xmlschema-3.2.1/xmlschema/converters/gdata.py` & `xmlschema-3.3.0/xmlschema/converters/gdata.py`

 * *Files 6% similar despite different names*

```diff
@@ -155,32 +155,25 @@
                 ns_name = self.unmap_qname(name, xmlns=self.get_xmlns_from_data(value))
                 content.append((ns_name, value))
             elif isinstance(value[0], (MutableMapping, MutableSequence)):
                 ns_name = self.unmap_qname(name, xmlns=self.get_xmlns_from_data(value[0]))
                 for item in value:
                     content.append((ns_name, item))
             else:
-                xsd_group = xsd_element.type.model_group
-                if xsd_group is None:
-                    xsd_group = xsd_element.any_type.model_group
-                    assert xsd_group is not None
-
                 ns_name = self.unmap_qname(name)
-                for xsd_child in xsd_group.iter_elements():
-                    matched_element = xsd_child.match(ns_name, resolve=True)
-                    if matched_element is not None:
-                        if matched_element.type and matched_element.type.is_list():
-                            content.append((ns_name, value))
-                        else:
-                            content.extend((ns_name, item) for item in value)
-                        break
+                xsd_child = xsd_element.match_child(ns_name)
+                if xsd_child is not None:
+                    if xsd_child.type and xsd_child.type.is_list():
+                        content.append((ns_name, value))
+                    else:
+                        content.extend((ns_name, item) for item in value)
                 else:
                     if isinstance(value, MutableSequence):
                         # Fallback tentative to an attribute if no element match
-                        ns_name = self.unmap_qname(name, xsd_element.attributes)
-                        if ns_name in xsd_element.attributes:
-                            attributes[ns_name] = value
+                        attr_name = self.unmap_qname(name, xsd_element.attributes)
+                        if attr_name in xsd_element.attributes:
+                            attributes[attr_name] = value
                             continue
 
                     content.append((ns_name, value))
 
         return ElementData(tag, text, content, attributes, xmlns)
```

### Comparing `xmlschema-3.2.1/xmlschema/converters/jsonml.py` & `xmlschema-3.3.0/xmlschema/converters/jsonml.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/converters/parker.py` & `xmlschema-3.3.0/xmlschema/converters/parker.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,36 +112,30 @@
                     items = obj[self.map_qname(name)]
                 except KeyError:
                     return ElementData(xsd_element.name, None, None, {}, None)
             else:
                 items = obj
 
             try:
-                xsd_group = xsd_element.type.model_group
-                if xsd_group is None:
-                    xsd_group = xsd_element.any_type.model_group
-                    assert xsd_group is not None
-
                 content = []
                 for name, value in obj.items():
                     ns_name = self.unmap_qname(name)
                     if not isinstance(value, MutableSequence) or not value:
                         content.append((ns_name, value))
                     elif any(isinstance(v, MutableSequence) for v in value):
                         for item in value:
                             content.append((ns_name, item))
                     else:
-                        for xsd_child in xsd_group.iter_elements():
-                            matched_element = xsd_child.match(ns_name, resolve=True)
-                            if matched_element is not None:
-                                if matched_element.type and matched_element.type.is_list():
-                                    content.append((ns_name, value))
-                                else:
-                                    content.extend((ns_name, item) for item in value)
-                                break
+                        ns_name = self.unmap_qname(name)
+                        xsd_child = xsd_element.match_child(ns_name)
+                        if xsd_child is not None:
+                            if xsd_child.type and xsd_child.type.is_list():
+                                content.append((ns_name, value))
+                            else:
+                                content.extend((ns_name, item) for item in value)
                         else:
                             content.extend((ns_name, item) for item in value)
 
             except AttributeError:
                 return ElementData(xsd_element.name, items, None, {}, None)
             else:
                 return ElementData(xsd_element.name, None, content, {}, None)
```

### Comparing `xmlschema-3.2.1/xmlschema/converters/unordered.py` & `xmlschema-3.3.0/xmlschema/converters/unordered.py`

 * *Files 9% similar despite different names*

```diff
@@ -94,34 +94,21 @@
             elif not isinstance(value, MutableSequence) or not value:
                 ns_name = self.unmap_qname(name, xmlns=self.get_xmlns_from_data(value))
                 content_lu[ns_name] = [value]
             elif isinstance(value[0], (MutableMapping, MutableSequence)):
                 ns_name = self.unmap_qname(name, xmlns=self.get_xmlns_from_data(value[0]))
                 content_lu[ns_name] = value
             else:
-                xsd_group = xsd_element.type.model_group
-                if xsd_group is None:
-                    xsd_group = xsd_element.any_type.model_group
-                    assert xsd_group is not None
-
                 # `value` is a list but not a list of lists or list of dicts.
                 ns_name = self.unmap_qname(name)
-                for xsd_child in xsd_group.iter_elements():
-                    matched_element = xsd_child.match(ns_name, resolve=True)
-                    if matched_element is not None:
-                        if matched_element.type and matched_element.type.is_list():
-                            content_lu[self.unmap_qname(name)] = [value]
-                        else:
-                            content_lu[self.unmap_qname(name)] = value
-                        break
-                else:
-                    if self.attr_prefix == '' and ns_name not in attributes:
-                        for xsd_attribute in xsd_element.attributes.values():
-                            if xsd_attribute.is_matching(ns_name):
-                                attributes[ns_name] = value
-                                break
-                        else:
-                            content_lu[self.unmap_qname(name)] = [value]
+                xsd_child = xsd_element.match_child(ns_name)
+                if xsd_child is not None:
+                    if xsd_child.type and xsd_child.type.is_list():
+                        content_lu[ns_name] = [value]
                     else:
-                        content_lu[self.unmap_qname(name)] = [value]
+                        content_lu[ns_name] = value
+                elif self.attr_prefix == '' and ns_name in xsd_element.attributes:
+                    attributes[ns_name] = value
+                else:
+                    content_lu[ns_name] = value
 
         return ElementData(xsd_element.name, text, content_lu, attributes, xmlns)
```

### Comparing `xmlschema-3.2.1/xmlschema/dataobjects.py` & `xmlschema-3.3.0/xmlschema/dataobjects.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/documents.py` & `xmlschema-3.3.0/xmlschema/documents.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/exceptions.py` & `xmlschema-3.3.0/xmlschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/exports.py` & `xmlschema-3.3.0/xmlschema/exports.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/extras/codegen.py` & `xmlschema-3.3.0/xmlschema/extras/codegen.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/extras/templates/python/bindings.py.jinja` & `xmlschema-3.3.0/xmlschema/extras/templates/python/bindings.py.jinja`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/extras/templates/python/sample.py.jinja` & `xmlschema-3.3.0/xmlschema/extras/templates/python/sample.py.jinja`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/extras/wsdl.py` & `xmlschema-3.3.0/xmlschema/extras/wsdl.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/helpers.py` & `xmlschema-3.3.0/xmlschema/helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/limits.py` & `xmlschema-3.3.0/xmlschema/limits.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo` & `xmlschema-3.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.po` & `xmlschema-3.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo` & `xmlschema-3.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.po` & `xmlschema-3.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/locale/pl/LC_MESSAGES/xmlschema.mo` & `xmlschema-3.3.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/locale/pl/LC_MESSAGES/xmlschema.po` & `xmlschema-3.3.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo` & `xmlschema-3.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po` & `xmlschema-3.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/locations.py` & `xmlschema-3.3.0/xmlschema/locations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/names.py` & `xmlschema-3.3.0/xmlschema/names.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/namespaces.py` & `xmlschema-3.3.0/xmlschema/namespaces.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/resources.py` & `xmlschema-3.3.0/xmlschema/resources.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/DSIG/xmldsig-core-schema.xsd` & `xmlschema-3.3.0/xmlschema/schemas/DSIG/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/DSIG/xmldsig11-schema.xsd` & `xmlschema-3.3.0/xmlschema/schemas/DSIG/xmldsig11-schema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd` & `xmlschema-3.3.0/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/VC/XMLSchema-versioning.xsd` & `xmlschema-3.3.0/xmlschema/schemas/VC/XMLSchema-versioning.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/WSDL/soap-encoding.xsd` & `xmlschema-3.3.0/xmlschema/schemas/WSDL/soap-encoding.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/WSDL/soap-envelope.xsd` & `xmlschema-3.3.0/xmlschema/schemas/WSDL/soap-envelope.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/WSDL/wsdl-soap.xsd` & `xmlschema-3.3.0/xmlschema/schemas/WSDL/wsdl-soap.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/WSDL/wsdl.xsd` & `xmlschema-3.3.0/xmlschema/schemas/WSDL/wsdl.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/XENC/xenc-schema-11.xsd` & `xmlschema-3.3.0/xmlschema/schemas/XENC/xenc-schema-11.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/XENC/xenc-schema.xsd` & `xmlschema-3.3.0/xmlschema/schemas/XENC/xenc-schema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/XHTML/xhtml1-strict.xsd` & `xmlschema-3.3.0/xmlschema/schemas/XHTML/xhtml1-strict.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/XLINK/xlink.xsd` & `xmlschema-3.3.0/xmlschema/schemas/XLINK/xlink.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/XML/xml_minimal.xsd` & `xmlschema-3.3.0/xmlschema/schemas/XML/xml_minimal.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/XSD_1.0/XMLSchema.xsd` & `xmlschema-3.3.0/xmlschema/schemas/XSD_1.0/XMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/XSD_1.0/datatypes.xsd` & `xmlschema-3.3.0/xmlschema/schemas/XSD_1.0/datatypes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/XSD_1.1/XMLSchema.xsd` & `xmlschema-3.3.0/xmlschema/schemas/XSD_1.1/XMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/XSD_1.1/datatypes.xsd` & `xmlschema-3.3.0/xmlschema/schemas/XSD_1.1/datatypes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd` & `xmlschema-3.3.0/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/testing/__init__.py` & `xmlschema-3.3.0/xmlschema/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/testing/_builders.py` & `xmlschema-3.3.0/xmlschema/testing/_builders.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/testing/_case_class.py` & `xmlschema-3.3.0/xmlschema/testing/_case_class.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/testing/_factory.py` & `xmlschema-3.3.0/xmlschema/testing/_factory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/testing/_helpers.py` & `xmlschema-3.3.0/xmlschema/testing/_helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/testing/_observers.py` & `xmlschema-3.3.0/xmlschema/testing/_observers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/translation.py` & `xmlschema-3.3.0/xmlschema/translation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/validators/__init__.py` & `xmlschema-3.3.0/xmlschema/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/validators/assertions.py` & `xmlschema-3.3.0/xmlschema/validators/assertions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/validators/attributes.py` & `xmlschema-3.3.0/xmlschema/validators/attributes.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/validators/builtins.py` & `xmlschema-3.3.0/xmlschema/validators/builtins.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/validators/complex_types.py` & `xmlschema-3.3.0/xmlschema/validators/complex_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-import copy
 from typing import cast, Any, Callable, Iterator, List, Optional, Tuple, Union
 
 from elementpath.datatypes import AnyAtomicType
 
 from ..exceptions import XMLSchemaValueError
 from ..names import XSD_GROUP, XSD_ATTRIBUTE_GROUP, XSD_SEQUENCE, XSD_OVERRIDE, \
     XSD_ALL, XSD_CHOICE, XSD_ANY_ATTRIBUTE, XSD_ATTRIBUTE, XSD_COMPLEX_CONTENT, \
@@ -767,17 +766,15 @@
         try:
             name, value = obj
         except ValueError:
             name = obj.name
             value = obj
 
         xsd_type: BaseXsdType
-        if isinstance(value, list):
-            xsd_type = self.any_simple_type
-        elif isinstance(value, AnyAtomicType):
+        if isinstance(value, AnyAtomicType):
             xsd_type = self.any_atomic_type
         else:
             xsd_type = self.any_type
 
         xsd_element = self.schema.create_element(name, parent=xsd_type, form='unqualified')
         xsd_element.type = xsd_type
         yield from xsd_element.iter_encode(value, validation, **kwargs)
@@ -845,30 +842,19 @@
             # See: http://www.w3.org/TR/xmlschema11-1/#Simple_Type_Definition_details
             msg = _("the simple content of {!r} is not a valid simple type in XSD 1.1")
             self.parse_error(msg.format(self.base_type))
 
         # Add open content to a complex content type
         if isinstance(self.content, XsdGroup):
             if self.open_content is None:
-                if self.content.interleave is not None or self.content.suffix is not None:
+                if self.content.open_content is not None:
                     msg = _("openContent mismatch between type and model group")
                     self.parse_error(msg)
-            elif self.open_content.mode == 'interleave':
-                interleave = self.schema.create_empty_content_group(
-                    parent=self, model='all'
-                )
-                interleave.append(self.content)
-                wildcard = copy.copy(self.open_content.any_element)
-                wildcard.min_occurs = 0
-                wildcard.max_occurs = None
-                wildcard.parent = self.content.interleave
-                interleave.append(wildcard)
-                self.content.interleave = interleave
-            elif self.open_content.mode == 'suffix':
-                self.content.suffix = self.open_content.any_element
+            elif self.open_content:
+                self.content.open_content = self.open_content
 
         # Add inheritable attributes
         if isinstance(self.base_type, XsdComplexType):
             for name, attr in self.base_type.attributes.items():
                 if attr.inheritable:
                     if name not in self.attributes:
                         self.attributes[name] = attr
```

### Comparing `xmlschema-3.2.1/xmlschema/validators/elements.py` & `xmlschema-3.3.0/xmlschema/validators/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1106,14 +1106,30 @@
             return self
         else:
             for xsd_element in self.iter_substitutes():
                 if name == xsd_element.name:
                     return xsd_element
         return None
 
+    def match_child(self, name: str) -> Optional['XsdElement']:
+        xsd_group = self.type.model_group
+        if xsd_group is None:
+            # fallback to xs:anyType encoder for matching extra content
+            xsd_group = self.any_type.model_group
+            assert xsd_group is not None
+
+        for xsd_child in xsd_group.iter_elements():
+            matched_element = xsd_child.match(name, resolve=True)
+            if isinstance(matched_element, XsdElement):
+                return matched_element
+        else:
+            if name in self.maps.elements and xsd_group.open_content_mode != 'none':
+                return self.maps.lookup_element(name)
+            return None
+
     def is_restriction(self, other: ModelParticleType, check_occurs: bool = True) -> bool:
         e: ModelParticleType
 
         if isinstance(other, XsdAnyElement):
             if self.min_occurs == self.max_occurs == 0:
                 return True
             if check_occurs and not self.has_occurs_restriction(other):
```

### Comparing `xmlschema-3.2.1/xmlschema/validators/exceptions.py` & `xmlschema-3.3.0/xmlschema/validators/exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/validators/facets.py` & `xmlschema-3.3.0/xmlschema/validators/facets.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/validators/global_maps.py` & `xmlschema-3.3.0/xmlschema/validators/global_maps.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/validators/groups.py` & `xmlschema-3.3.0/xmlschema/validators/groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,17 @@
 
 from .exceptions import XMLSchemaModelError, XMLSchemaModelDepthError, \
     XMLSchemaValidationError, XMLSchemaChildrenValidationError, \
     XMLSchemaTypeTableWarning
 from .xsdbase import ValidationMixin, XsdComponent, XsdType
 from .particles import ParticleMixin, OccursCalculator
 from .elements import XsdElement, XsdAlternative
-from .wildcards import XsdAnyElement, Xsd11AnyElement
-from .models import ModelVisitor, iter_unordered_content, iter_collapsed_content
+from .wildcards import XsdAnyElement, Xsd11AnyElement, XsdOpenContent
+from .models import ModelVisitor, InterleavedModelVisitor, SuffixedModelVisitor, \
+    iter_unordered_content, iter_collapsed_content
 
 if TYPE_CHECKING:
     from .complex_types import XsdComplexType
 
 ANY_ELEMENT = ElementTree.Element(
     XSD_ANY,
     attrib={
@@ -91,28 +92,29 @@
           {any attributes with non-schema namespace . . .}>
           Content: (annotation?, (element | group | choice | sequence | any)*)
         </sequence>
     """
     parent: Optional[Union['XsdComplexType', 'XsdGroup']]
     model: str
     mixed: bool = False
-    ref: Optional['XsdGroup']
+    ref: Optional['XsdGroup']  # Not None if the instance is a ref to a global group
+    content: List[ModelParticleType]  # Direct access to children also from a ref group
     restriction: Optional['XsdGroup'] = None
 
     # For XSD 1.1 openContent processing
-    interleave: Optional['XsdGroup'] = None  # if openContent with mode='interleave'
-    suffix: Optional[Xsd11AnyElement] = None  # if openContent with mode='suffix'/'interleave'
+    open_content: Optional[XsdOpenContent] = None
 
     _ADMITTED_TAGS = {XSD_GROUP, XSD_SEQUENCE, XSD_ALL, XSD_CHOICE}
 
     def __init__(self, elem: ElementType,
                  schema: SchemaType,
                  parent: Optional[Union['XsdComplexType', 'XsdGroup']] = None) -> None:
 
         self._group: List[ModelParticleType] = []
+        self.content = self._group
         self.oid = (self,)
         if parent is not None and parent.mixed:
             self.mixed = parent.mixed
         super(XsdGroup, self).__init__(elem, schema, parent)
 
     def __repr__(self) -> str:
         if self.name is None:
@@ -191,14 +193,18 @@
             return False
         elif self.model == 'choice' and parent.model != 'choice':
             return False
         else:
             return True
 
     @property
+    def open_content_mode(self) -> str:
+        return 'none' if self.open_content is None else self.open_content.mode
+
+    @property
     def effective_min_occurs(self) -> int:
         if not self.min_occurs or not self:
             return 0
 
         effective_items: List[Any]
         min_occurs: int
         effective_items = [e for e in self.iter_model() if e.effective_max_occurs != 0]
@@ -342,16 +348,19 @@
 
         iterators: List[Iterator[ModelParticleType]] = []
         particles = iter(self)
 
         while True:
             for item in particles:
                 if isinstance(item, XsdGroup):
+                    if item.max_occurs == 0:
+                        continue
+
                     iterators.append(particles)
-                    particles = iter(item)
+                    particles = iter(item.content)
                     if len(iterators) > limits.MAX_MODEL_DEPTH:
                         raise XMLSchemaModelDepthError(self)
                     break
                 else:
                     yield item
             else:
                 try:
@@ -449,14 +458,16 @@
         return expected
 
     def copy(self) -> 'XsdGroup':
         group: XsdGroup = object.__new__(self.__class__)
         group.__dict__.update(self.__dict__)
         group.errors = self.errors[:]
         group._group = self._group[:]
+        if self.ref is None:
+            group.content = group._group
         return group
 
     __copy__ = copy
 
     def _parse(self) -> None:
         self.clear()
         self._parse_particle(self.elem)
@@ -486,14 +497,15 @@
                         msg = _("minOccurs must be (0 | 1) for 'all' model groups")
                         self.parse_error(msg)
                     if self.xsd_version == '1.0' and isinstance(self.parent, XsdGroup):
                         msg = _("in XSD 1.0 an 'all' model group cannot be nested")
                         self.parse_error(msg)
                 self._group.append(xsd_group)
                 self.ref = xsd_group
+                self.content = xsd_group._group
             else:
                 # Disallowed circular definition, substitute with any content group.
                 msg = _("Circular definition detected for group %r")
                 self.parse_error(msg % self.name, xsd_group[0])
                 self.model = 'sequence'
                 self.mixed = True
                 self._group.append(self.schema.xsd_any_class(ANY_ELEMENT, self.schema, self))
@@ -980,35 +992,34 @@
         except KeyError:
             converter = self._get_converter(obj, kwargs)
 
         errors: List[Tuple[int, ModelParticleType, int, Optional[List[SchemaElementType]]]]
         xsd_element: Optional[SchemaElementType]
         expected: Optional[List[SchemaElementType]]
 
-        model = ModelVisitor(self.interleave or self)
+        if self.open_content is None:
+            model = ModelVisitor(self)
+        elif self.open_content.mode == 'interleave':
+            model = InterleavedModelVisitor(self, self.open_content.any_element)
+        else:
+            model = SuffixedModelVisitor(self, self.open_content.any_element)
+
         errors = []
         broken_model = False
         namespaces = converter.namespaces
 
         for index, child in enumerate(obj):
             if callable(child.tag):
                 continue  # child is a comment or PI
 
             converter.set_context(child, level)
-            default_namespace = converter.default_namespace
             name = converter.map_qname(child.tag)
 
             while model.element is not None:
-                if model.element.max_occurs == 0:
-                    xsd_element = None
-                else:
-                    xsd_element = model.element.match(
-                        child.tag, group=self, occurs=model.occurs
-                    )
-
+                xsd_element = model.match_element(child.tag)
                 if xsd_element is None:
                     for particle, occurs, expected in model.advance(False):
                         errors.append((index, particle, occurs, expected))
                         model.clear()
                         broken_model = True  # the model is broken, continues with raw decoding.
                         xsd_element = self.match_element(child.tag)
                         break
@@ -1021,25 +1032,21 @@
                 except XMLSchemaValidationError as err:
                     yield self.validation_error(validation, err, obj, **kwargs)
 
                 for particle, occurs, expected in model.advance(True):
                     errors.append((index, particle, occurs, expected))
                 break
             else:
-                if self.suffix is not None and \
-                        self.suffix.is_matching(child.tag, default_namespace, self):
-                    xsd_element = self.suffix
-                else:
-                    xsd_element = self.match_element(child.tag)
-                    if xsd_element is None:
-                        errors.append((index, self, 0, None))
-                        broken_model = True
-                    elif not broken_model:
-                        errors.append((index, xsd_element, 0, []))
-                        broken_model = True
+                xsd_element = self.match_element(child.tag)
+                if xsd_element is None:
+                    errors.append((index, self, 0, None))
+                    broken_model = True
+                elif not broken_model:
+                    errors.append((index, xsd_element, 0, []))
+                    broken_model = True
 
             if xsd_element is None:
                 if kwargs.get('keep_unknown'):
                     for result in self.any_type.iter_decode(child, validation, **kwargs):
                         result_list.append((name, result, None))
                 continue
             elif over_max_depth:
@@ -1064,14 +1071,15 @@
                         result_list.append((cdata_index, tail, None))
                         cdata_index += 1
 
         if model.element is not None:
             index = len(obj)
             for particle, occurs, expected in model.stop():
                 errors.append((index, particle, occurs, expected))
+                break
 
         if errors:
             source = kwargs.get('source')
             namespaces = converter.namespaces
 
             for index, particle, occurs, expected in errors:
                 error = XMLSchemaChildrenValidationError(
@@ -1109,100 +1117,98 @@
             level = kwargs['level'] = kwargs['level'] + 1
         except KeyError:
             level = kwargs['level'] = 1
 
         converter = kwargs['converter']
         padding = '\n' + ' ' * converter.indent * level
         default_namespace = converter.get('')
-        model = ModelVisitor(self.interleave or self)
+
+        if self.open_content is None:
+            model = ModelVisitor(self)
+        elif self.open_content.mode == 'interleave':
+            model = InterleavedModelVisitor(self, self.open_content.any_element)
+        else:
+            model = SuffixedModelVisitor(self, self.open_content.any_element)
+
         index = cdata_index = 0
         wrong_content_type = False
         over_max_depth = 'max_depth' in kwargs and kwargs['max_depth'] <= level
 
         content: Iterable[Any]
         if not obj.content:
             content = []
         elif isinstance(obj.content, MutableMapping) or kwargs.get('unordered'):
-            content = iter_unordered_content(obj.content, self, default_namespace)
+            content = iter_unordered_content(obj.content, self)
         elif not isinstance(obj.content, MutableSequence):
             wrong_content_type = True
             content = []
         elif not isinstance(obj.content[0], tuple):
             if len(obj.content) > 1 or text is not None:
                 wrong_content_type = True
             else:
                 text = raw_xml_encode(obj.content[0])
             content = []
         elif converter.losslessly:
             content = obj.content
         else:
-            content = iter_collapsed_content(obj.content, self, default_namespace)
+            content = iter_collapsed_content(obj.content, self)
 
         for index, (name, value) in enumerate(content):
             if isinstance(name, int):
                 if not children:
                     text = padding + value if text is None else text + value + padding
                 elif children[-1].tail is None:
                     children[-1].tail = padding + value
                 else:
                     children[-1].tail += value + padding
                 cdata_index += 1
                 continue
 
             xsd_element: Optional[SchemaElementType]
             while model.element is not None:
-                if model.element.max_occurs == 0:
-                    xsd_element = None
-                else:
-                    xsd_element = model.element.match(
-                        name, group=self, occurs=model.occurs
-                    )
-
+                xsd_element = model.match_element(name)
                 if xsd_element is None:
                     for particle, occurs, expected in model.advance():
                         errors.append((index - cdata_index, particle, occurs, expected))
                     continue
                 elif isinstance(xsd_element, XsdAnyElement):
                     value = get_qname(default_namespace, name), value
 
                 for particle, occurs, expected in model.advance(True):
                     errors.append((index - cdata_index, particle, occurs, expected))
                 break
             else:
-                if self.suffix and self.suffix.is_matching(name, default_namespace, group=self):
-                    xsd_element = self.suffix
+                errors.append((index - cdata_index, self, 0, []))
+                xsd_element = self.match_element(name)
+                if isinstance(xsd_element, XsdAnyElement):
                     value = get_qname(default_namespace, name), value
-                else:
-                    errors.append((index - cdata_index, self, 0, []))
-                    xsd_element = self.match_element(name)
-                    if isinstance(xsd_element, XsdAnyElement):
-                        value = get_qname(default_namespace, name), value
-                    elif xsd_element is None:
-                        if name.startswith('{') or ':' not in name:
-                            reason = _('{!r} does not match any declared element '
-                                       'of the model group').format(name)
-                        else:
-                            reason = _('{0} has an unknown prefix {1!r}').format(
-                                name, name.split(':')[0]
-                            )
-                        yield self.validation_error(validation, reason, value, **kwargs)
-                        continue
+                elif xsd_element is None:
+                    if name.startswith('{') or ':' not in name:
+                        reason = _('{!r} does not match any declared element '
+                                   'of the model group').format(name)
+                    else:
+                        reason = _('{0} has an unknown prefix {1!r}').format(
+                            name, name.split(':')[0]
+                        )
+                    yield self.validation_error(validation, reason, value, **kwargs)
+                    continue
 
             if over_max_depth:
                 continue
 
             for result in xsd_element.iter_encode(value, validation, **kwargs):
                 if isinstance(result, XMLSchemaValidationError):
                     yield result
                 else:
                     children.append(result)
 
         if model.element is not None:
             for particle, occurs, expected in model.stop():
                 errors.append((index - cdata_index + 1, particle, occurs, expected))
+                break
 
         if children:
             if children[-1].tail is None:
                 children[-1].tail = padding[:-converter.indent] or '\n'
             else:
                 children[-1].tail = children[-1].tail.strip() + (
                         padding[:-converter.indent] or '\n'
```

### Comparing `xmlschema-3.2.1/xmlschema/validators/helpers.py` & `xmlschema-3.3.0/xmlschema/validators/helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/validators/identities.py` & `xmlschema-3.3.0/xmlschema/validators/identities.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/validators/models.py` & `xmlschema-3.3.0/xmlschema/validators/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 This module contains a function and a class for validating XSD content models,
 plus a set of functions for manipulating encoded content.
 """
 from collections import defaultdict, deque, Counter
 from operator import attrgetter
 from typing import Any, Dict, Iterable, Iterator, List, \
     MutableMapping, MutableSequence, Optional, Tuple, Union
+import warnings
 
 from ..exceptions import XMLSchemaValueError
 from ..aliases import ModelGroupType, ModelParticleType, SchemaElementType, \
     OccursCounterType
 from ..translation import gettext as _
 from .. import limits
 from .exceptions import XMLSchemaModelError, XMLSchemaModelDepthError
@@ -241,20 +242,38 @@
     def stop(self) -> Iterator[AdvanceYieldedType]:
         while self.element is not None:
             for e in self.advance():
                 yield e
 
     def iter_group(self) -> Iterator[ModelParticleType]:
         """Returns an iterator for the current model group."""
-        if self.group.max_occurs == 0:
-            return iter(())
-        elif self.group.model != 'all':
-            return iter(self.group)
+        if self.group.model == 'all':
+            for e in self.group.iter_elements():
+                if not e.is_over(self.occurs):
+                    yield e
+        elif self.group.max_occurs == 0:
+            return
         else:
-            return (e for e in self.group.iter_elements() if not e.is_over(self.occurs))
+            yield from self.group.content
+
+    def match_element(self, tag: str) -> Optional[SchemaElementType]:
+        if self.element is None:
+            raise XMLSchemaValueError("cannot match, %r is ended!" % self)
+        elif self.element.max_occurs == 0:
+            return None
+        elif self.element.name is None:
+            return self.element.match(tag, group=self.root, occurs=self.occurs)
+        elif tag == self.element.name:
+            return self.element
+        else:
+            for xsd_element in self.element.iter_substitutes():
+                if tag == xsd_element.name:
+                    return xsd_element
+            else:
+                return None
 
     def advance(self, match: bool = False) -> Iterator[AdvanceYieldedType]:
         """
         Generator function for advance to the next element. Yields tuples with
         particles information when occurrence violation is found.
 
         :param match: provides current element match.
@@ -310,22 +329,23 @@
                 return stop_item()
             elif self.group.is_missing(occurs):
                 return True
             else:
                 item = self.group
                 return stop_item()
 
-            if item is self.group[-1]:
-                for k, item2 in enumerate(self.group, start=1):  # pragma: no cover
+            if item is self.group.content[-1]:
+                for k, item2 in enumerate(self.group.content, start=1):  # pragma: no cover
                     low_occurs = occurs[item2]
                     if not low_occurs:
                         continue
 
                     high_occurs = occurs[item2.oid] or low_occurs
-                    if high_occurs == 1 or any(not x.is_emptiable() for x in self.group[k:]):
+                    if high_occurs == 1 or \
+                            any(not x.is_emptiable() for x in self.group.content[k:]):
                         occurs[self.group] += 1
                         occurs[self.group.oid] += 1
                         break
 
                     occurs[self.group] += (low_occurs // (item2.max_occurs or low_occurs)) or 1
                     occurs[self.group.oid] += (high_occurs // (item2.min_occurs or 1)) or 1
                     break
@@ -349,100 +369,213 @@
         occurs = self.occurs
         item_occurs = occurs[item]
 
         if match:
             occurs[item] += 1
             self.match = True
             if self.group.model == 'all':
-                self.items = (e for e in self.group.iter_elements() if not e.is_over(occurs))
-            elif not item.is_over(occurs):
-                return
-            elif self.group.model == 'choice' and item.is_ambiguous():
+                self.items = self.iter_group()
+            elif not item.is_over(occurs) or \
+                    self.group.model == 'choice' and item.is_ambiguous():
                 return
 
-        obj = None
         try:
             if stop_item():
                 yield model_error_tuple()
 
             while True:
                 while self.group.is_over(occurs):
                     item = self.group
                     stop_item()
 
-                obj = next(self.items, None)
-                if isinstance(obj, groups.XsdGroup):
-                    # inner 'sequence' or 'choice' XsdGroup
-                    self._groups.append((self.group, self.items, self.match))
-                    self.group = obj
-                    self.items = self.iter_group()
-                    self.match = False
-                    occurs[obj] = occurs[obj.oid] = 0
-
-                elif obj is not None:
-                    # XsdElement or XsdAnyElement
-                    self.element = obj
-                    if self.group.model == 'sequence':
-                        occurs[obj] = 0
-                    return
-
-                elif not self.match:
-                    if self.group.model == 'all':
-                        if all(e.min_occurs <= occurs[e] for e in self.group.iter_elements()):
-                            occurs[self.group] = 1
-
-                    item = self.group
-                    if stop_item():
-                        yield model_error_tuple()
-
-                elif self.group.model != 'all':
-                    self.items, self.match = self.iter_group(), False
-                elif any(e.min_occurs > occurs[e] for e in self.group.iter_elements()):
-                    if not self.group.min_occurs:
-                        yield self.group, occurs[self.group], self.expected
-                    self.group, self.items, self.match = self._groups.pop()
-                elif any(not e.is_over(occurs) for e in self.group):
-                    self.items = self.iter_group()
-                    self.match = False
+                for obj in self.items:
+                    if isinstance(obj, groups.XsdGroup):
+                        # inner 'sequence' or 'choice' XsdGroup
+                        self._groups.append((self.group, self.items, self.match))
+                        self.group = obj
+                        self.items = self.iter_group()
+                        self.match = False
+                        occurs[obj] = occurs[obj.oid] = 0
+                        break
+                    else:
+                        # XsdElement or XsdAnyElement
+                        self.element = obj
+                        if self.group.model == 'sequence':
+                            occurs[obj] = 0
+                        return
                 else:
-                    occurs[self.group] = 1
+                    if self.match:
+                        self.items, self.match = self.iter_group(), False
+                    elif self.group.model == 'all':
+                        self.group, self.items, self.match = self._groups.pop()
+                    else:
+                        item = self.group
+                        if stop_item():
+                            yield model_error_tuple()
 
         except IndexError:
             # Model visit ended
             self.element = None
-            if self.group.is_missing(occurs):
-                if self.group.model == 'choice':
-                    yield self.group, occurs[self.group], self.expected
-                elif self.group.model == 'sequence':
-                    if obj is not None:
-                        yield self.group, occurs[self.group], self.expected
-                elif any(e.min_occurs > occurs[e] for e in self.group):
-                    yield self.group, occurs[self.group], self.expected
-            elif self.group.max_occurs is not None and self.group.max_occurs < occurs[self.group]:
+            if self.group.model == 'all':
+                yield from self._iter_all_model_errors(occurs)
+            elif self.group.is_missing(occurs) or self.group.is_exceeded(occurs):
                 yield self.group, occurs[self.group], self.expected
 
+    def _iter_all_model_errors(self, occurs: OccursCounterType) -> Iterator[AdvanceYieldedType]:
+        """Validate occurrences in an 'all' model, yielding error tuples."""
+        stack: List[Tuple[groups.XsdGroup, Iterator[ModelParticleType]]] = []
+        group, particles = self.group, iter(self.group)
+        zero_missing: List[Tuple[groups.XsdGroup, ModelParticleType]] = []
+
+        while True:
+            for item in particles:
+                if occurs[item]:
+                    occurs[group] = 1
+
+                if isinstance(item, groups.XsdGroup):
+                    if item.max_occurs == 0:
+                        continue
+
+                    stack.append((group, particles))
+                    particles = iter(item.content)
+                    if len(stack) > limits.MAX_MODEL_DEPTH:
+                        raise XMLSchemaModelDepthError(self.group)
+                    break
+
+                if item.is_missing(occurs) or item.is_exceeded(occurs):
+                    if occurs[item]:
+                        yield item, occurs[item], item.get_expected(occurs)
+                    else:
+                        zero_missing.append((group, item))
+            else:
+                if group.is_missing(occurs) or group.is_exceeded(occurs):
+                    if occurs[group] or not stack:
+                        yield group, occurs[group], group.get_expected(occurs)
+                    else:
+                        zero_missing.append((stack[-1][0], group))
+
+                if not stack:
+                    break
+                group, particles = stack.pop()
+
+        # Late check on missing items that never occurs
+        for group, item in zero_missing:
+            if occurs[group]:
+                yield item, occurs[item], item.get_expected(occurs)
+
     # Kept for backward compatibility
     def iter_unordered_content(
             self, content: EncodedContentType,
             default_namespace: Optional[str] = None) -> Iterator[ContentItemType]:
-        return iter_unordered_content(content, self.root, default_namespace)
+
+        msg = f"{self.__class__.__name__}.iter_unordered_content() method will " \
+              "be removed in v4.0, use iter_unordered_content() function instead."
+        if default_namespace is not None:
+            msg += " Don't provide default_namespace argument, it's ignored."
+        warnings.warn(msg, DeprecationWarning, stacklevel=2)
+
+        return iter_unordered_content(content, self.root)
 
     def iter_collapsed_content(
             self, content: Iterable[ContentItemType],
             default_namespace: Optional[str] = None) -> Iterator[ContentItemType]:
-        return iter_collapsed_content(content, self.root, default_namespace)
+
+        msg = f"{self.__class__.__name__}.iter_collapsed_content() method will " \
+              "be removed in v4.0, use iter_collapsed_content() function instead."
+        if default_namespace is not None:
+            msg += " Don't provide default_namespace argument, it's ignored."
+        warnings.warn(msg, DeprecationWarning, stacklevel=2)
+
+        return iter_collapsed_content(content, self.root)
+
+
+class InterleavedModelVisitor(ModelVisitor):
+    """
+    A visitor for openContent interleaved models. Memorizes an internal state
+    for deciding when to advance the model. The model doesn't advance if the
+    last match_element() call is with the wildcard.
+    """
+    __slots__ = 'wildcard', '_advance_model'
+
+    def __init__(self, root: ModelGroupType, wildcard: XsdAnyElement) -> None:
+        super().__init__(root)
+        self.wildcard = wildcard
+        self._advance_model = True
+        if self.element is None:
+            self.element = wildcard
+
+    def clear(self) -> None:
+        super().clear()
+        self._advance_model = True
+        if self.element is None:
+            self.element = self.wildcard
+
+    def match_element(self, tag: str) -> Optional[SchemaElementType]:
+        xsd_element = super().match_element(tag)
+        if xsd_element is not None or self.element is self.wildcard:
+            return xsd_element
+        elif not self.wildcard.is_matching(tag, group=self.root, occurs=self.occurs):
+            return None
+
+        for xsd_element in self.group.iter_elements():
+            if xsd_element.is_matching(tag, group=self.root, occurs=self.occurs):
+                if not xsd_element.is_over(self.occurs):
+                    return None
+        else:
+            if self.wildcard.process_contents != 'strict' or tag in self.root.maps.elements:
+                self._advance_model = False
+                return self.wildcard
+            return None
+
+    def advance(self, match: bool = False) -> Iterator[AdvanceYieldedType]:
+        if self.element is None:
+            yield from super().advance(match)
+        elif self.element is self.wildcard:
+            if not match:
+                self.element = None
+        elif not self._advance_model:
+            self._advance_model = True
+        else:
+            yield from super().advance(match)
+            if self.element is None:
+                self.element = self.wildcard
+
+
+class SuffixedModelVisitor(ModelVisitor):
+    """A visitor for openContent suffixed models."""
+
+    __slots__ = 'wildcard',
+
+    def __init__(self, root: ModelGroupType, wildcard: XsdAnyElement) -> None:
+        super().__init__(root)
+        self.wildcard = wildcard
+        if self.element is None:
+            self.element = wildcard
+
+    def clear(self) -> None:
+        super().clear()
+        if self.element is None:
+            self.element = self.wildcard
+
+    def advance(self, match: bool = False) -> Iterator[AdvanceYieldedType]:
+        if self.element is None:
+            yield from super().advance(match)
+        elif self.element is not self.wildcard:
+            yield from super().advance(match)
+            if self.element is None:
+                self.element = self.wildcard
+        elif not match:
+            self.element = None
 
 
 #
 # Functions for manipulating encoded content
 
-def iter_unordered_content(
-        content: EncodedContentType,
-        group: ModelGroupType,
-        default_namespace: Optional[str] = None) -> Iterator[ContentItemType]:
+def iter_unordered_content(content: EncodedContentType, group: ModelGroupType) \
+        -> Iterator[ContentItemType]:
     """
     Takes an unordered content stored in a dictionary of lists and yields the
     content elements sorted with the ordering defined by the model group. Character
     data parts are yielded at start and between child elements.
 
     Ordering is inferred from ModelVisitor instance with any elements that
     don't fit the schema placed at the end of the returned sequence. Checking
@@ -450,15 +583,14 @@
     of class :class:`XsdGroup`.
 
     :param content: a dictionary of element names to list of element contents \
     or an iterable composed of couples of name and value. In case of a \
     dictionary the values must be lists where each item is the content \
     of a single element.
     :param group: the model group related to content.
-    :param default_namespace: the default namespace to apply for matching names.
     """
     consumable_content: Dict[str, Any]
 
     if isinstance(content, MutableMapping):
         cdata_content = sorted(
             ((k, v) for k, v in content.items() if isinstance(k, int)), reverse=True
         )
@@ -500,38 +632,34 @@
             if cdata_content:
                 yield cdata_content.pop()
 
     while cdata_content:
         yield cdata_content.pop()
 
 
-def sort_content(content: EncodedContentType,
-                 group: ModelGroupType,
-                 default_namespace: Optional[str] = None) -> List[ContentItemType]:
-    return [x for x in iter_unordered_content(content, group, default_namespace)]
+def sort_content(content: EncodedContentType, group: ModelGroupType) \
+        -> List[ContentItemType]:
+    return [x for x in iter_unordered_content(content, group)]
 
 
-def iter_collapsed_content(
-        content: Iterable[ContentItemType],
-        group: ModelGroupType,
-        default_namespace: Optional[str] = None) -> Iterator[ContentItemType]:
+def iter_collapsed_content(content: Iterable[ContentItemType], group: ModelGroupType) \
+        -> Iterator[ContentItemType]:
     """
     Iterates a content stored in a sequence of couples *(name, value)*, yielding
     items in the same order of the sequence, except for repetitions of the same
     tag that don't match with the current element of the :class:`ModelVisitor`
     instance. These items are included in an unsorted buffer and yielded asap
     when there is a match with the model's element or at the end of the iteration.
 
     This iteration mode, in cooperation with the method *iter_encode* of the class
     XsdGroup, facilitates the encoding of content formatted with a convention that
-    collapses the children with the same tag into a list (eg. BadgerFish).
+    collapses the children with the same tag into a list (e.g. BadgerFish).
 
     :param content: an iterable containing couples of names and values.
     :param group: the model group related to content.
-    :param default_namespace: the default namespace to apply for matching names.
     """
     prev_name = None
     unordered_content: Dict[str, Any] = defaultdict(deque)
 
     model = ModelVisitor(group)
     for name, value in content:
         if isinstance(name, int) or model.element is None:
@@ -565,11 +693,11 @@
             else:
                 for _err in model.advance(True):
                     pass
         else:
             yield name, value
             prev_name = name
 
-    # Add the remaining consumable content onto the end of the data.
+    # Yields the remaining consumable content after the end of the data.
     for name, values in unordered_content.items():
         for v in values:
             yield name, v
```

### Comparing `xmlschema-3.2.1/xmlschema/validators/notations.py` & `xmlschema-3.3.0/xmlschema/validators/notations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/validators/particles.py` & `xmlschema-3.3.0/xmlschema/validators/particles.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,23 +102,31 @@
         """Tests if the particle occurrences are under the minimum."""
         try:
             return self.min_occurs > occurs[self]  # type: ignore[index]
         except TypeError:
             return self.min_occurs > occurs  # type: ignore[operator]
 
     def is_over(self, occurs: Union[OccursCounterType, int]) -> bool:
-        """Tests if particle occurrences are over the maximum."""
+        """Tests if particle occurrences are equal or over the maximum."""
         if self.max_occurs is None:
             return False
-
         try:
             return self.max_occurs <= occurs[self]  # type: ignore[index]
         except TypeError:
             return self.max_occurs <= occurs  # type: ignore[operator]
 
+    def is_exceeded(self, occurs: Union[OccursCounterType, int]) -> bool:
+        """Tests if particle occurrences are over the maximum."""
+        if self.max_occurs is None:
+            return False
+        try:
+            return self.max_occurs < occurs[self]  # type: ignore[index]
+        except TypeError:
+            return self.max_occurs < occurs  # type: ignore[operator]
+
     def get_expected(self, occurs: OccursCounterType) -> List[SchemaElementType]:
         return [cast(SchemaElementType, self)] if self.min_occurs > occurs[self] else []
 
     def has_occurs_restriction(self, other: Union[ModelParticleType, 'OccursCalculator']) -> bool:
         if self.min_occurs < other.min_occurs:
             return False
         elif self.max_occurs == 0:
```

### Comparing `xmlschema-3.2.1/xmlschema/validators/schemas.py` & `xmlschema-3.3.0/xmlschema/validators/schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/validators/simple_types.py` & `xmlschema-3.3.0/xmlschema/validators/simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/validators/wildcards.py` & `xmlschema-3.3.0/xmlschema/validators/wildcards.py`

 * *Files 1% similar despite different names*

```diff
@@ -887,18 +887,15 @@
             if child is not None and child.tag == XSD_ANY:
                 msg = _("an openContent with mode='none' cannot "
                         "have an <xs:any> child declaration")
                 self.parse_error(msg)
         elif child is None or child.tag != XSD_ANY:
             self.parse_error(_("an <xs:any> child declaration is required"))
         else:
-            any_element = Xsd11AnyElement(child, self.schema, self)
-            any_element.min_occurs = 0
-            any_element.max_occurs = None
-            self.any_element = any_element
+            self.any_element = Xsd11AnyElement(child, self.schema, self)
 
     @property
     def built(self) -> bool:
         return True
 
     def is_restriction(self, other: 'XsdOpenContent') -> bool:
         if other is None or other.mode == 'none':
```

### Comparing `xmlschema-3.2.1/xmlschema/validators/xsdbase.py` & `xmlschema-3.3.0/xmlschema/validators/xsdbase.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/xpath/__init__.py` & `xmlschema-3.3.0/xmlschema/xpath/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/xpath/assertion_parser.py` & `xmlschema-3.3.0/xmlschema/xpath/assertion_parser.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/xpath/identity_parser.py` & `xmlschema-3.3.0/xmlschema/xpath/identity_parser.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/xpath/mixin.py` & `xmlschema-3.3.0/xmlschema/xpath/mixin.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/xpath/proxy.py` & `xmlschema-3.3.0/xmlschema/xpath/proxy.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema/xpath3.py` & `xmlschema-3.3.0/xmlschema/xpath3.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.2.1/xmlschema.egg-info/PKG-INFO` & `xmlschema-3.3.0/xmlschema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlschema
-Version: 3.2.1
+Version: 3.3.0
 Summary: An XML Schema validator and decoder
 Home-page: https://github.com/sissaschool/xmlschema
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `xmlschema-3.2.1/xmlschema.egg-info/SOURCES.txt` & `xmlschema-3.3.0/xmlschema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

