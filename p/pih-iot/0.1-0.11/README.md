# Comparing `tmp/pih-iot-0.1.tar.gz` & `tmp/pih-iot-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-iot-0.1.tar", last modified: Wed Apr 17 06:03:31 2024, max compression
+gzip compressed data, was "pih-iot-0.11.tar", last modified: Wed Apr 17 13:09:53 2024, max compression
```

## Comparing `pih-iot-0.1.tar` & `pih-iot-0.11.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 06:03:32.010944 pih-iot-0.1/
--rw-rw-rw-   0        0        0      295 2024-04-17 06:03:31.979689 pih-iot-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 06:03:31.948417 pih-iot-0.1/pih_iot.egg-info/
--rw-rw-rw-   0        0        0      295 2024-04-17 06:03:31.000000 pih-iot-0.1/pih_iot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2024-04-17 06:03:31.000000 pih-iot-0.1/pih_iot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 06:03:31.000000 pih-iot-0.1/pih_iot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-17 06:03:31.000000 pih-iot-0.1/pih_iot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-17 06:03:31.000000 pih-iot-0.1/pih_iot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-17 06:03:31.000000 pih-iot-0.1/pih_iot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 06:03:32.026592 pih-iot-0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 13:09:53.429665 pih-iot-0.11/
+-rw-rw-rw-   0        0        0      296 2024-04-17 13:09:53.398429 pih-iot-0.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 13:09:53.351541 pih-iot-0.11/pih_iot.egg-info/
+-rw-rw-rw-   0        0        0      296 2024-04-17 13:09:52.000000 pih-iot-0.11/pih_iot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2024-04-17 13:09:52.000000 pih-iot-0.11/pih_iot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 13:09:52.000000 pih-iot-0.11/pih_iot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-17 13:09:52.000000 pih-iot-0.11/pih_iot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-04-17 13:09:52.000000 pih-iot-0.11/pih_iot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-17 13:09:52.000000 pih-iot-0.11/pih_iot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 13:09:53.429665 pih-iot-0.11/setup.cfg
```

