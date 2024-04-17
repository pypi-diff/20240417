# Comparing `tmp/pycrossva-0.97.tar.gz` & `tmp/pycrossva-0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrossva-0.97.tar", last modified: Fri Aug 25 14:42:09 2023, max compression
+gzip compressed data, was "pycrossva-0.98.tar", last modified: Wed Apr 17 17:35:50 2024, max compression
```

## Comparing `pycrossva-0.97.tar` & `pycrossva-0.98.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-08-25 14:42:09.839938 pycrossva-0.97/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    35147 2022-07-12 21:13:08.000000 pycrossva-0.97/LICENSE
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      174 2023-08-25 14:03:12.000000 pycrossva-0.97/MANIFEST.in
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     7930 2023-08-25 14:42:09.839670 pycrossva-0.97/PKG-INFO
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     6997 2023-08-25 14:37:35.000000 pycrossva-0.97/README.rst
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-08-25 14:42:09.820610 pycrossva-0.97/pycrossva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       19 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    25626 2023-07-25 14:56:32.000000 pycrossva-0.97/pycrossva/configuration.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19825 2023-07-25 14:56:39.000000 pycrossva-0.97/pycrossva/mappings.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-08-25 14:42:09.816588 pycrossva-0.97/pycrossva/resources/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-08-25 14:42:09.831455 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    49398 2023-08-21 18:22:27.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2012WHO_to_InSilicoVA.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    32803 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2012WHO_to_InSilicoVA_2012.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    32803 2023-08-21 18:21:16.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2012WHO_to_InterVA4.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    49398 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2012WHO_to_InterVA5.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    66136 2023-08-25 12:31:03.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InSilicoVA.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    42538 2023-08-21 18:27:56.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InSilicoVA_2012.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    42538 2023-08-21 16:57:45.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InterVA4.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    66136 2023-08-25 12:32:48.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InterVA5.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    64818 2023-08-25 12:34:27.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InSilicoVA.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    42139 2023-08-21 18:29:58.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InSilicoVA_2012.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    42139 2023-08-21 16:57:45.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InterVA4.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    64781 2023-08-25 12:35:38.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InterVA5.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    34196 2023-08-21 19:00:22.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2021WHO_to_InSilicoVA.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    53080 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2021WHO_to_InterVA5.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    35344 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/PHRMCShort_to_InSilicoVA.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    47073 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/PHRMCShort_to_InterVA5.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088     2608 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/example_config_1.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088      575 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/mapping_configuration_files/example_config_2.csv
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-08-25 14:42:09.838414 pycrossva-0.97/pycrossva/resources/sample_data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5059 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/sample_data/2012WHO_mock_data_1.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   470310 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/sample_data/2016WHO_bad_data_1.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   617783 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/sample_data/2016WHO_mock_data_1.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   915332 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/sample_data/2016WHO_mock_data_2.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     6760 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/sample_data/Mock_PHRMC_Data.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     6824 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/sample_data/PHRMC_mock_data_1.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   921756 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/sample_data/mock_data_2.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    36142 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/sample_data/mock_data_2016WHO151.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   193579 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/sample_data/test_data1.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   136542 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/resources/sample_data/test_data2.csv
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-08-25 14:42:09.838863 pycrossva-0.97/pycrossva/scripts/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5170 2022-07-12 21:13:08.000000 pycrossva-0.97/pycrossva/scripts/pycrossva_transform.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    15323 2023-08-21 18:45:30.000000 pycrossva-0.97/pycrossva/transform.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     6445 2023-08-22 17:49:25.000000 pycrossva-0.97/pycrossva/utils.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    33042 2023-07-25 15:33:39.000000 pycrossva-0.97/pycrossva/validation.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-08-25 14:42:09.822997 pycrossva-0.97/pycrossva.egg-info/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     7930 2023-08-25 14:42:09.000000 pycrossva-0.97/pycrossva.egg-info/PKG-INFO
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2335 2023-08-25 14:42:09.000000 pycrossva-0.97/pycrossva.egg-info/SOURCES.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        1 2023-08-25 14:42:09.000000 pycrossva-0.97/pycrossva.egg-info/dependency_links.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       83 2023-08-25 14:42:09.000000 pycrossva-0.97/pycrossva.egg-info/entry_points.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       27 2023-08-25 14:42:09.000000 pycrossva-0.97/pycrossva.egg-info/requires.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       10 2023-08-25 14:42:09.000000 pycrossva-0.97/pycrossva.egg-info/top_level.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     1241 2023-08-25 14:17:28.000000 pycrossva-0.97/pyproject.toml
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       38 2023-08-25 14:42:09.840024 pycrossva-0.97/setup.cfg
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-08-25 14:42:09.839162 pycrossva-0.97/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     1171 2023-08-21 17:11:27.000000 pycrossva-0.97/tests/test.py
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-17 17:35:50.528615 pycrossva-0.98/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    35147 2022-07-12 21:13:08.000000 pycrossva-0.98/LICENSE
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      174 2023-08-25 14:03:12.000000 pycrossva-0.98/MANIFEST.in
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     8047 2024-04-17 17:35:50.527656 pycrossva-0.98/PKG-INFO
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     6997 2023-08-25 14:37:35.000000 pycrossva-0.98/Readme.rst
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-17 17:35:50.460976 pycrossva-0.98/pycrossva/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       19 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    25626 2024-04-17 15:49:57.000000 pycrossva-0.98/pycrossva/configuration.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    19825 2023-07-25 14:56:39.000000 pycrossva-0.98/pycrossva/mappings.py
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-17 17:35:50.451835 pycrossva-0.98/pycrossva/resources/
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-17 17:35:50.493029 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    49398 2023-08-21 18:22:27.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2012WHO_to_InSilicoVA.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    32803 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2012WHO_to_InSilicoVA_2012.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    32803 2023-08-21 18:21:16.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2012WHO_to_InterVA4.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    49398 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2012WHO_to_InterVA5.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    66136 2023-08-25 12:31:03.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InSilicoVA.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    42538 2023-08-21 18:27:56.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InSilicoVA_2012.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    42538 2023-08-21 16:57:45.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InterVA4.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    66136 2023-08-25 12:32:48.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InterVA5.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    64818 2023-08-25 12:34:27.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InSilicoVA.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    42139 2023-08-21 18:29:58.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InSilicoVA_2012.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    42139 2023-08-21 16:57:45.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InterVA4.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    64781 2023-08-25 12:35:38.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InterVA5.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    34196 2023-08-21 19:00:22.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2021WHO_to_InSilicoVA.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    53080 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2021WHO_to_InterVA5.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    35344 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/PHMRCShort_to_InSilicoVA.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    47073 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/PHMRCShort_to_InterVA5.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     2608 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/example_config_1.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      575 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/mapping_configuration_files/example_config_2.csv
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-17 17:35:50.520300 pycrossva-0.98/pycrossva/resources/sample_data/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     5059 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/sample_data/2012WHO_mock_data_1.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   470310 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/sample_data/2016WHO_bad_data_1.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   617783 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/sample_data/2016WHO_mock_data_1.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   915332 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/sample_data/2016WHO_mock_data_2.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     6760 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/sample_data/Mock_PHRMC_Data.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     6824 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/sample_data/PHMRC_mock_data_1.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   921756 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/sample_data/mock_data_2.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    36142 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/sample_data/mock_data_2016WHO151.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   193579 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/sample_data/test_data1.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   136542 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/resources/sample_data/test_data2.csv
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-17 17:35:50.522554 pycrossva-0.98/pycrossva/scripts/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     5170 2022-07-12 21:13:08.000000 pycrossva-0.98/pycrossva/scripts/pycrossva_transform.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    15323 2024-04-17 15:49:26.000000 pycrossva-0.98/pycrossva/transform.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     6445 2023-08-22 17:49:25.000000 pycrossva-0.98/pycrossva/utils.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    33042 2023-07-25 15:33:39.000000 pycrossva-0.98/pycrossva/validation.py
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-17 17:35:50.526499 pycrossva-0.98/pycrossva.egg-info/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     8047 2024-04-17 17:35:50.000000 pycrossva-0.98/pycrossva.egg-info/PKG-INFO
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     2335 2024-04-17 17:35:50.000000 pycrossva-0.98/pycrossva.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        1 2024-04-17 17:35:50.000000 pycrossva-0.98/pycrossva.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       83 2024-04-17 17:35:50.000000 pycrossva-0.98/pycrossva.egg-info/entry_points.txt
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       27 2024-04-17 17:35:50.000000 pycrossva-0.98/pycrossva.egg-info/requires.txt
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       10 2024-04-17 17:35:50.000000 pycrossva-0.98/pycrossva.egg-info/top_level.txt
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     1281 2024-04-17 16:10:00.000000 pycrossva-0.98/pyproject.toml
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       38 2024-04-17 17:35:50.529677 pycrossva-0.98/setup.cfg
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-17 17:35:50.523983 pycrossva-0.98/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     1171 2023-08-21 17:11:27.000000 pycrossva-0.98/tests/test.py
```

### Comparing `pycrossva-0.97/LICENSE` & `pycrossva-0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/PKG-INFO` & `pycrossva-0.98/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: pycrossva
-Version: 0.97
+Version: 0.98
 Summary: Prepare data from WHO and PHRMC instruments for verbal autopsy algorithms
 Author: ekarpinskiMITRE, pkmitre, owentrigueros, Peter Choi, Yue Chu, Jason Thomas
-Maintainer-email: Jason Thomas <jarathomas@gmail.com>
+Maintainer-email: openVA Team <help@openva.net>
 Project-URL: Homepage, https://github.com/verbal-autopsy-software/pyCrossVA
 Project-URL: Bug Tracker, https://github.com/verbal-autopsy-software/pyCrossVA/issues
 Keywords: verbal autopsy,data preparation
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: numpy>=1.22.0
+Requires-Dist: pandas
+Requires-Dist: Click
 
 pyCrossVA
 =========
 
 .. image:: https://img.shields.io/pypi/pyversions/pycrossva
     :target: https://pypi.org/project/pycrossva
 .. image:: http://readthedocs.org/projects/pycrossva/badge/
```

### Comparing `pycrossva-0.97/README.rst` & `pycrossva-0.98/Readme.rst`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/configuration.py` & `pycrossva-0.98/pycrossva/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from pycrossva.validation import Validation, Err, Warn
 
 
 class Configuration():
     """ Configuration class details the relationship between a set of input
     data and output data. It is composed of MapConditions that
     transform an input data source (2012 WHO, 2016 WHO 141, 2016 WHO 151,
-    PHRMC SHORT) into a different data form (PHRMC SHORT, InSilicoVA,
+    PHMRC SHORT) into a different data form (PHMRC SHORT, InSilicoVA,
     InterVA4, InterVA5, or Tarrif2) for verbal autopsy.
 
     Attributes:
         given_columns (Pandas Series): columns of mapping dataframe.
         required_columns (Pandas Series): required columns in mapping data.
         main_columns (list): the four main columns required in config_data.
         valid_relationships (Pandas Series): contains list of valid
```

### Comparing `pycrossva-0.97/pycrossva/mappings.py` & `pycrossva-0.98/pycrossva/mappings.py`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2012WHO_to_InSilicoVA.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2012WHO_to_InSilicoVA.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2012WHO_to_InSilicoVA_2012.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2012WHO_to_InSilicoVA_2012.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2012WHO_to_InterVA4.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2012WHO_to_InterVA4.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2012WHO_to_InterVA5.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2012WHO_to_InterVA5.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InSilicoVA.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InSilicoVA.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InSilicoVA_2012.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InSilicoVA_2012.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InterVA4.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InterVA4.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InterVA5.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InterVA5.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InSilicoVA.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InSilicoVA.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InSilicoVA_2012.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InSilicoVA_2012.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InterVA4.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InterVA4.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InterVA5.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InterVA5.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2021WHO_to_InSilicoVA.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2021WHO_to_InSilicoVA.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/2021WHO_to_InterVA5.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/2021WHO_to_InterVA5.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/PHRMCShort_to_InSilicoVA.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/PHMRCShort_to_InSilicoVA.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/PHRMCShort_to_InterVA5.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/PHMRCShort_to_InterVA5.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/example_config_1.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/example_config_1.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/mapping_configuration_files/example_config_2.csv` & `pycrossva-0.98/pycrossva/resources/mapping_configuration_files/example_config_2.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/sample_data/2012WHO_mock_data_1.csv` & `pycrossva-0.98/pycrossva/resources/sample_data/2012WHO_mock_data_1.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/sample_data/2016WHO_bad_data_1.csv` & `pycrossva-0.98/pycrossva/resources/sample_data/2016WHO_bad_data_1.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/sample_data/2016WHO_mock_data_1.csv` & `pycrossva-0.98/pycrossva/resources/sample_data/2016WHO_mock_data_1.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/sample_data/2016WHO_mock_data_2.csv` & `pycrossva-0.98/pycrossva/resources/sample_data/2016WHO_mock_data_2.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/sample_data/Mock_PHRMC_Data.csv` & `pycrossva-0.98/pycrossva/resources/sample_data/Mock_PHRMC_Data.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/sample_data/PHRMC_mock_data_1.csv` & `pycrossva-0.98/pycrossva/resources/sample_data/PHMRC_mock_data_1.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/sample_data/mock_data_2.csv` & `pycrossva-0.98/pycrossva/resources/sample_data/mock_data_2.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/sample_data/mock_data_2016WHO151.csv` & `pycrossva-0.98/pycrossva/resources/sample_data/mock_data_2016WHO151.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/sample_data/test_data1.csv` & `pycrossva-0.98/pycrossva/resources/sample_data/test_data1.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/resources/sample_data/test_data2.csv` & `pycrossva-0.98/pycrossva/resources/sample_data/test_data2.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/scripts/pycrossva_transform.py` & `pycrossva-0.98/pycrossva/scripts/pycrossva_transform.py`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/transform.py` & `pycrossva-0.98/pycrossva/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import pandas as pd
 import numpy as np
 
 from pycrossva.configuration import Configuration, CrossVA
 from pycrossva.utils import flexible_read
 
-SUPPORTED_INPUTS = ["2016WHOv151", "2016WHOv141", "2012WHO", "PHRMCShort"]
+SUPPORTED_INPUTS = ["2016WHOv151", "2016WHOv141", "2012WHO", "PHMRCShort"]
 SUPPORTED_OUTPUTS = ["InterVA5", "InterVA4", "InSilicoVA", "InSilicoVA_2012"]
 
 
 def transform(mapping, raw_data, raw_data_id=None, lower=False,
               verbose=2, preserve_na=True,
               result_values={"Present": "y", "Absent": "n", "NA": "."}):
     """transforms raw VA data (`raw_data`) into data suitable for use with a VA
@@ -119,37 +119,37 @@
         with new columns that are specified but missing source columns.
         These new columns will be created so that the final result has the correct
         expeted columns for the algorithm, but filled with NA values to indicate
         the lack of information. If `preserve_na` is set to `False`, then the NA
         values will also be `False`.
 
         This situation is common between certain questionnaire sources and algorithms.
-        For example, in the mapping between the PHRMC Short questionnaire
+        For example, in the mapping between the PHMRC Short questionnaire
         to InterVA5 mapping, there are 107 InterVA5
         variables that are listed in the mapping configuration to be created,
-        but have no corresponding question in PHRMC short.
+        but have no corresponding question in PHMRC short.
 
         For example, variables i004a and i004b have no specifications in the
         mapping below. They are still listed under "New Column Name" so
         CrossVA knows that they should be created in the final result, but
         because they have no logic defined, they will be left as their default
         value of NA.
 
-        >>> phrmc_to_interva5 = pd.read_csv('resources/mapping_configuration_files/PHRMCShort_to_InterVA5.csv')
+        >>> phrmc_to_interva5 = pd.read_csv('resources/mapping_configuration_files/PHMRCShort_to_InterVA5.csv')
         >>> phrmc_to_interva5.iloc[:5,[0,2,4,-1]]
           New Column Name Source Column ID Relationship Meta: Notes
         0           i004a              NaN          NaN   Not asked
         1           i004b              NaN          NaN   Not asked
         2           i019a          gen_5_2           eq         NaN
         3           i019b          gen_5_2           eq         NaN
         4           i022a         gen_5_4h           ge         NaN
 
         The `transform` function will warn the user of this behavior.
 
-        >>> transform(phrmc_to_interva5, "resources/sample_data/PHRMC_mock_data_1.csv").iloc[:5,:5]
+        >>> transform(phrmc_to_interva5, "resources/sample_data/PHMRC_mock_data_1.csv").iloc[:5,:5]
         Validating Mapping Configuration . . .
         <BLANKLINE>
          WARNINGS
         [?] 	 124 new column(s) listed but not defined in Mapping Configuration detected. These ('i004a', 'i004b', 'i059o', 'i082o', 'i087o', 'i091o', 'i092o', 'i093o', 'i094o', 'i095o', etc) will be treated as NA.
         Validating Mapping-Data Relationship . . .
         <BLANKLINE>
          WARNINGS
```

### Comparing `pycrossva-0.97/pycrossva/utils.py` & `pycrossva-0.98/pycrossva/utils.py`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva/validation.py` & `pycrossva-0.98/pycrossva/validation.py`

 * *Files identical despite different names*

### Comparing `pycrossva-0.97/pycrossva.egg-info/PKG-INFO` & `pycrossva-0.98/pycrossva.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: pycrossva
-Version: 0.97
+Version: 0.98
 Summary: Prepare data from WHO and PHRMC instruments for verbal autopsy algorithms
 Author: ekarpinskiMITRE, pkmitre, owentrigueros, Peter Choi, Yue Chu, Jason Thomas
-Maintainer-email: Jason Thomas <jarathomas@gmail.com>
+Maintainer-email: openVA Team <help@openva.net>
 Project-URL: Homepage, https://github.com/verbal-autopsy-software/pyCrossVA
 Project-URL: Bug Tracker, https://github.com/verbal-autopsy-software/pyCrossVA/issues
 Keywords: verbal autopsy,data preparation
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: numpy>=1.22.0
+Requires-Dist: pandas
+Requires-Dist: Click
 
 pyCrossVA
 =========
 
 .. image:: https://img.shields.io/pypi/pyversions/pycrossva
     :target: https://pypi.org/project/pycrossva
 .. image:: http://readthedocs.org/projects/pycrossva/badge/
```

### Comparing `pycrossva-0.97/pycrossva.egg-info/SOURCES.txt` & `pycrossva-0.98/pycrossva.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,23 @@
 pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InterVA5.csv
 pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InSilicoVA.csv
 pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InSilicoVA_2012.csv
 pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InterVA4.csv
 pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InterVA5.csv
 pycrossva/resources/mapping_configuration_files/2021WHO_to_InSilicoVA.csv
 pycrossva/resources/mapping_configuration_files/2021WHO_to_InterVA5.csv
-pycrossva/resources/mapping_configuration_files/PHRMCShort_to_InSilicoVA.csv
-pycrossva/resources/mapping_configuration_files/PHRMCShort_to_InterVA5.csv
+pycrossva/resources/mapping_configuration_files/PHMRCShort_to_InSilicoVA.csv
+pycrossva/resources/mapping_configuration_files/PHMRCShort_to_InterVA5.csv
 pycrossva/resources/mapping_configuration_files/example_config_1.csv
 pycrossva/resources/mapping_configuration_files/example_config_2.csv
 pycrossva/resources/sample_data/2012WHO_mock_data_1.csv
 pycrossva/resources/sample_data/2016WHO_bad_data_1.csv
 pycrossva/resources/sample_data/2016WHO_mock_data_1.csv
 pycrossva/resources/sample_data/2016WHO_mock_data_2.csv
 pycrossva/resources/sample_data/Mock_PHRMC_Data.csv
-pycrossva/resources/sample_data/PHRMC_mock_data_1.csv
+pycrossva/resources/sample_data/PHMRC_mock_data_1.csv
 pycrossva/resources/sample_data/mock_data_2.csv
 pycrossva/resources/sample_data/mock_data_2016WHO151.csv
 pycrossva/resources/sample_data/test_data1.csv
 pycrossva/resources/sample_data/test_data2.csv
 pycrossva/scripts/pycrossva_transform.py
 tests/test.py
```

### Comparing `pycrossva-0.97/pyproject.toml` & `pycrossva-0.98/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pycrossva"
 description = "Prepare data from WHO and PHRMC instruments for verbal autopsy algorithms"
-version = "0.97"
+version = "0.98"
 readme = "Readme.rst"
 requires-python = ">=3.8"
 dependencies = [
     "numpy >= 1.22.0",
     "pandas",
     "Click",
 ]
@@ -14,22 +14,23 @@
   {name = "pkmitre"},
   {name = "owentrigueros"},
   {name = "Peter Choi"},
   {name = "Yue Chu"},
   {name = "Jason Thomas"},
 ]
 maintainers = [
-  {name = "Jason Thomas", email = "jarathomas@gmail.com"},
+  {name = "openVA Team", email = "help@openva.net"},
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 keywords = ["verbal autopsy", "data preparation"]
 
 [project.urls]
 "Homepage" = "https://github.com/verbal-autopsy-software/pyCrossVA"
```

### Comparing `pycrossva-0.97/tests/test.py` & `pycrossva-0.98/tests/test.py`

 * *Files identical despite different names*

