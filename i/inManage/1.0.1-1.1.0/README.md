# Comparing `tmp/inManage-1.0.1.tar.gz` & `tmp/inManage-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inManage-1.0.1.tar", last modified: Thu Apr 11 02:31:46 2024, max compression
+gzip compressed data, was "dist/inManage-1.1.0.tar", last modified: Wed Apr 17 07:40:26 2024, max compression
```

## Comparing `inManage-1.0.1.tar` & `inManage-1.1.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      785 2024-04-11 02:22:49.000000 inManage-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-11 02:31:46.000000 inManage-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      228 2024-04-11 02:22:49.000000 inManage-1.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-11 02:22:49.000000 inManage-1.0.1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inManage.egg-info/
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-11 02:31:46.000000 inManage-1.0.1/inManage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2493 2024-04-11 02:31:46.000000 inManage-1.0.1/inManage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 02:31:46.000000 inManage-1.0.1/inManage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2024-04-11 02:31:46.000000 inManage-1.0.1/inManage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-11 02:31:46.000000 inManage-1.0.1/inManage.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5228 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inmanage_sdk/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inmanage_sdk/command/
--rw-r--r--   0 root         (0) root         (0)    49818 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/IpmiFunc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2857 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/biosPostEventStr.py
--rw-r--r--   0 root         (0) root         (0)    16391 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/commonInfoStr.py
--rw-r--r--   0 root         (0) root         (0)      693 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/eventLogString.py
--rw-r--r--   0 root         (0) root         (0)     3787 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/sensorEventStr.py
--rw-r--r--   0 root         (0) root         (0)    51098 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/sensorSpecificEventStr.py
--rw-r--r--   0 root         (0) root         (0)     5697 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/M5Log/showSensorDesc.py
--rw-r--r--   0 root         (0) root         (0)    21216 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/RedfishFunc.py
--rw-r--r--   0 root         (0) root         (0)   304005 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/RestFunc.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12150 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/backup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inmanage_sdk/command/bios/
--rw-r--r--   0 root         (0) root         (0)    44672 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/A7.xml
--rw-r--r--   0 root         (0) root         (0)    18001 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/M4.xml
--rw-r--r--   0 root         (0) root         (0)    54050 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/M5.xml
--rw-r--r--   0 root         (0) root         (0)    84400 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/M6-N.xml
--rw-r--r--   0 root         (0) root         (0)    81680 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/M6.xml
--rw-r--r--   0 root         (0) root         (0)    46082 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/M7.xml
--rw-r--r--   0 root         (0) root         (0)   117980 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/M7_5.10.00.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/NF3180A6.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/NF3280A6.xml
--rw-r--r--   0 root         (0) root         (0)   354128 2024-04-11 02:22:53.000000 inManage-1.0.1/inmanage_sdk/command/bios/NF5180M5.xml
--rw-r--r--   0 root         (0) root         (0)   354211 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/bios/NF5280M5.xml
--rw-r--r--   0 root         (0) root         (0)    36922 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/bios/NF5468A5.xml
--rw-r--r--   0 root         (0) root         (0)    29961 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/bios/NF5488A5.xml
--rw-r--r--   0 root         (0) root         (0)   354291 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/bios/SA5112M5.xml
--rw-r--r--   0 root         (0) root         (0)   354213 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/bios/SA5212M5.xml
--rw-r--r--   0 root         (0) root         (0)    66016 2024-04-11 02:22:52.000000 inManage-1.0.1/inmanage_sdk/command/restore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inmanage_sdk/interface/
--rw-r--r--   0 root         (0) root         (0)    44314 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/Base.py
--rw-r--r--   0 root         (0) root         (0)     2588 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonA5.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonA6.py
--rw-r--r--   0 root         (0) root         (0)     6330 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonA7.py
--rw-r--r--   0 root         (0) root         (0)      315 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonA7_11308.py
--rw-r--r--   0 root         (0) root         (0)   744214 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonM5.py
--rw-r--r--   0 root         (0) root         (0)   608244 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonM6.py
--rw-r--r--   0 root         (0) root         (0)    18026 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonM6_41401.py
--rw-r--r--   0 root         (0) root         (0)    16472 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonM6_4140a.py
--rw-r--r--   0 root         (0) root         (0)   271855 2024-04-11 02:22:51.000000 inManage-1.0.1/inmanage_sdk/interface/CommonM7.py
--rw-r--r--   0 root         (0) root         (0)      311 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/CommonM7_13505.py
--rw-r--r--   0 root         (0) root         (0)    45789 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/I24M6.py
--rw-r--r--   0 root         (0) root         (0)     8558 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/IBase.py
--rw-r--r--   0 root         (0) root         (0)    14823 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/NF5180M5.py
--rw-r--r--   0 root         (0) root         (0)      338 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/NF5180M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    15213 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/NF5280M5.py
--rw-r--r--   0 root         (0) root         (0)      509 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/NF5280M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    59692 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/NF5280M5_435.py
--rw-r--r--   0 root         (0) root         (0)     2190 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/NF5280M5_436.py
--rw-r--r--   0 root         (0) root         (0)    47112 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/NS5160M6.py
--rw-r--r--   0 root         (0) root         (0)   123026 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/ResEntity.py
--rw-r--r--   0 root         (0) root         (0)      511 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/SA5212M5Impl.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inmanage_sdk/route/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/route/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5516 2024-04-11 02:22:50.000000 inManage-1.0.1/inmanage_sdk/route/route.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:31:46.000000 inManage-1.0.1/inmanage_sdk/util/
--rw-r--r--   0 root         (0) root         (0)     4716 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/HostTypeJudge.py
--rw-r--r--   0 root         (0) root         (0)     4788 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/RedfishClient.py
--rw-r--r--   0 root         (0) root         (0)    10339 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/RegularCheckUtil.py
--rw-r--r--   0 root         (0) root         (0)     7686 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/RequestClient.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7550 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/configUtil.py
--rw-r--r--   0 root         (0) root         (0)     1812 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/fileUtil.py
--rw-r--r--   0 root         (0) root         (0)     7590 2024-04-11 02:22:49.000000 inManage-1.0.1/inmanage_sdk/util/parameterConversion.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 02:31:46.000000 inManage-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1438 2024-04-11 02:22:49.000000 inManage-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:40:26.000000 inManage-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      785 2024-04-17 07:39:06.000000 inManage-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-17 07:40:26.000000 inManage-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      228 2024-04-17 07:39:06.000000 inManage-1.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-17 07:39:06.000000 inManage-1.1.0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:40:26.000000 inManage-1.1.0/inManage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-17 07:40:25.000000 inManage-1.1.0/inManage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2493 2024-04-17 07:40:25.000000 inManage-1.1.0/inManage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 07:40:25.000000 inManage-1.1.0/inManage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2024-04-17 07:40:25.000000 inManage-1.1.0/inManage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-17 07:40:25.000000 inManage-1.1.0/inManage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5228 2024-04-17 07:39:11.000000 inManage-1.1.0/inmanage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:40:26.000000 inManage-1.1.0/inmanage_sdk/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 07:39:07.000000 inManage-1.1.0/inmanage_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:40:26.000000 inManage-1.1.0/inmanage_sdk/command/
+-rw-r--r--   0 root         (0) root         (0)    49818 2024-04-17 07:39:10.000000 inManage-1.1.0/inmanage_sdk/command/IpmiFunc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:40:26.000000 inManage-1.1.0/inmanage_sdk/command/M5Log/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 07:39:10.000000 inManage-1.1.0/inmanage_sdk/command/M5Log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2024-04-17 07:39:10.000000 inManage-1.1.0/inmanage_sdk/command/M5Log/biosPostEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    16391 2024-04-17 07:39:10.000000 inManage-1.1.0/inmanage_sdk/command/M5Log/commonInfoStr.py
+-rw-r--r--   0 root         (0) root         (0)      693 2024-04-17 07:39:10.000000 inManage-1.1.0/inmanage_sdk/command/M5Log/eventLogString.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2024-04-17 07:39:10.000000 inManage-1.1.0/inmanage_sdk/command/M5Log/sensorEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    51098 2024-04-17 07:39:10.000000 inManage-1.1.0/inmanage_sdk/command/M5Log/sensorSpecificEventStr.py
+-rw-r--r--   0 root         (0) root         (0)     5697 2024-04-17 07:39:10.000000 inManage-1.1.0/inmanage_sdk/command/M5Log/showSensorDesc.py
+-rw-r--r--   0 root         (0) root         (0)    21216 2024-04-17 07:39:10.000000 inManage-1.1.0/inmanage_sdk/command/RedfishFunc.py
+-rw-r--r--   0 root         (0) root         (0)   304005 2024-04-17 07:39:10.000000 inManage-1.1.0/inmanage_sdk/command/RestFunc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 07:39:10.000000 inManage-1.1.0/inmanage_sdk/command/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12150 2024-04-17 07:39:11.000000 inManage-1.1.0/inmanage_sdk/command/backup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:40:26.000000 inManage-1.1.0/inmanage_sdk/command/bios/
+-rw-r--r--   0 root         (0) root         (0)    44672 2024-04-17 07:39:11.000000 inManage-1.1.0/inmanage_sdk/command/bios/A7.xml
+-rw-r--r--   0 root         (0) root         (0)    18001 2024-04-17 07:39:11.000000 inManage-1.1.0/inmanage_sdk/command/bios/M4.xml
+-rw-r--r--   0 root         (0) root         (0)    54050 2024-04-17 07:39:11.000000 inManage-1.1.0/inmanage_sdk/command/bios/M5.xml
+-rw-r--r--   0 root         (0) root         (0)    84400 2024-04-17 07:39:11.000000 inManage-1.1.0/inmanage_sdk/command/bios/M6-N.xml
+-rw-r--r--   0 root         (0) root         (0)    81680 2024-04-17 07:39:11.000000 inManage-1.1.0/inmanage_sdk/command/bios/M6.xml
+-rw-r--r--   0 root         (0) root         (0)    46082 2024-04-17 07:39:11.000000 inManage-1.1.0/inmanage_sdk/command/bios/M7.xml
+-rw-r--r--   0 root         (0) root         (0)   117980 2024-04-17 07:39:11.000000 inManage-1.1.0/inmanage_sdk/command/bios/M7_5.10.00.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2024-04-17 07:39:11.000000 inManage-1.1.0/inmanage_sdk/command/bios/NF3180A6.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2024-04-17 07:39:11.000000 inManage-1.1.0/inmanage_sdk/command/bios/NF3280A6.xml
+-rw-r--r--   0 root         (0) root         (0)   354128 2024-04-17 07:39:11.000000 inManage-1.1.0/inmanage_sdk/command/bios/NF5180M5.xml
+-rw-r--r--   0 root         (0) root         (0)   354211 2024-04-17 07:39:11.000000 inManage-1.1.0/inmanage_sdk/command/bios/NF5280M5.xml
+-rw-r--r--   0 root         (0) root         (0)    36922 2024-04-17 07:39:11.000000 inManage-1.1.0/inmanage_sdk/command/bios/NF5468A5.xml
+-rw-r--r--   0 root         (0) root         (0)    29961 2024-04-17 07:39:11.000000 inManage-1.1.0/inmanage_sdk/command/bios/NF5488A5.xml
+-rw-r--r--   0 root         (0) root         (0)   354291 2024-04-17 07:39:10.000000 inManage-1.1.0/inmanage_sdk/command/bios/SA5112M5.xml
+-rw-r--r--   0 root         (0) root         (0)   354213 2024-04-17 07:39:10.000000 inManage-1.1.0/inmanage_sdk/command/bios/SA5212M5.xml
+-rw-r--r--   0 root         (0) root         (0)    66016 2024-04-17 07:39:10.000000 inManage-1.1.0/inmanage_sdk/command/restore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:40:26.000000 inManage-1.1.0/inmanage_sdk/interface/
+-rw-r--r--   0 root         (0) root         (0)    44314 2024-04-17 07:39:09.000000 inManage-1.1.0/inmanage_sdk/interface/Base.py
+-rw-r--r--   0 root         (0) root         (0)     2588 2024-04-17 07:39:09.000000 inManage-1.1.0/inmanage_sdk/interface/CommonA5.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-04-17 07:39:09.000000 inManage-1.1.0/inmanage_sdk/interface/CommonA6.py
+-rw-r--r--   0 root         (0) root         (0)     6330 2024-04-17 07:39:09.000000 inManage-1.1.0/inmanage_sdk/interface/CommonA7.py
+-rw-r--r--   0 root         (0) root         (0)      315 2024-04-17 07:39:09.000000 inManage-1.1.0/inmanage_sdk/interface/CommonA7_11308.py
+-rw-r--r--   0 root         (0) root         (0)   744309 2024-04-17 07:39:09.000000 inManage-1.1.0/inmanage_sdk/interface/CommonM5.py
+-rw-r--r--   0 root         (0) root         (0)   608302 2024-04-17 07:39:09.000000 inManage-1.1.0/inmanage_sdk/interface/CommonM6.py
+-rw-r--r--   0 root         (0) root         (0)    18064 2024-04-17 07:39:09.000000 inManage-1.1.0/inmanage_sdk/interface/CommonM6_41401.py
+-rw-r--r--   0 root         (0) root         (0)    16472 2024-04-17 07:39:09.000000 inManage-1.1.0/inmanage_sdk/interface/CommonM6_4140a.py
+-rw-r--r--   0 root         (0) root         (0)   271874 2024-04-17 07:39:09.000000 inManage-1.1.0/inmanage_sdk/interface/CommonM7.py
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-17 07:39:08.000000 inManage-1.1.0/inmanage_sdk/interface/CommonM7_13505.py
+-rw-r--r--   0 root         (0) root         (0)    45789 2024-04-17 07:39:08.000000 inManage-1.1.0/inmanage_sdk/interface/I24M6.py
+-rw-r--r--   0 root         (0) root         (0)     8558 2024-04-17 07:39:08.000000 inManage-1.1.0/inmanage_sdk/interface/IBase.py
+-rw-r--r--   0 root         (0) root         (0)    14823 2024-04-17 07:39:08.000000 inManage-1.1.0/inmanage_sdk/interface/NF5180M5.py
+-rw-r--r--   0 root         (0) root         (0)      338 2024-04-17 07:39:08.000000 inManage-1.1.0/inmanage_sdk/interface/NF5180M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    15213 2024-04-17 07:39:08.000000 inManage-1.1.0/inmanage_sdk/interface/NF5280M5.py
+-rw-r--r--   0 root         (0) root         (0)      509 2024-04-17 07:39:08.000000 inManage-1.1.0/inmanage_sdk/interface/NF5280M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    59692 2024-04-17 07:39:08.000000 inManage-1.1.0/inmanage_sdk/interface/NF5280M5_435.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2024-04-17 07:39:08.000000 inManage-1.1.0/inmanage_sdk/interface/NF5280M5_436.py
+-rw-r--r--   0 root         (0) root         (0)    47112 2024-04-17 07:39:08.000000 inManage-1.1.0/inmanage_sdk/interface/NS5160M6.py
+-rw-r--r--   0 root         (0) root         (0)   123026 2024-04-17 07:39:08.000000 inManage-1.1.0/inmanage_sdk/interface/ResEntity.py
+-rw-r--r--   0 root         (0) root         (0)      511 2024-04-17 07:39:08.000000 inManage-1.1.0/inmanage_sdk/interface/SA5212M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 07:39:08.000000 inManage-1.1.0/inmanage_sdk/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:40:26.000000 inManage-1.1.0/inmanage_sdk/route/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 07:39:07.000000 inManage-1.1.0/inmanage_sdk/route/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2024-04-17 07:39:07.000000 inManage-1.1.0/inmanage_sdk/route/route.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:40:26.000000 inManage-1.1.0/inmanage_sdk/util/
+-rw-r--r--   0 root         (0) root         (0)     4716 2024-04-17 07:39:07.000000 inManage-1.1.0/inmanage_sdk/util/HostTypeJudge.py
+-rw-r--r--   0 root         (0) root         (0)     4788 2024-04-17 07:39:07.000000 inManage-1.1.0/inmanage_sdk/util/RedfishClient.py
+-rw-r--r--   0 root         (0) root         (0)    10339 2024-04-17 07:39:07.000000 inManage-1.1.0/inmanage_sdk/util/RegularCheckUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7686 2024-04-17 07:39:07.000000 inManage-1.1.0/inmanage_sdk/util/RequestClient.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 07:39:07.000000 inManage-1.1.0/inmanage_sdk/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7550 2024-04-17 07:39:07.000000 inManage-1.1.0/inmanage_sdk/util/configUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2024-04-17 07:39:07.000000 inManage-1.1.0/inmanage_sdk/util/fileUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2024-04-17 07:39:07.000000 inManage-1.1.0/inmanage_sdk/util/parameterConversion.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 07:40:26.000000 inManage-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1438 2024-04-17 07:39:06.000000 inManage-1.1.0/setup.py
```

### Comparing `inManage-1.0.1/MANIFEST.in` & `inManage-1.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/PKG-INFO` & `inManage-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inManage
-Version: 1.0.1
+Version: 1.1.0
 Summary: ieisystem server manager api
 Home-page: https://github.com/ieisystem/inManage
 Author: Wangbaoshan
 Author-email: wangbaoshan@ieisystem.com
 License: Expat License
 Description: # InManage
         inManage is a support tool for ansible.ieisystem.inmanage
```

### Comparing `inManage-1.0.1/inManage.egg-info/PKG-INFO` & `inManage-1.1.0/inManage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inManage
-Version: 1.0.1
+Version: 1.1.0
 Summary: ieisystem server manager api
 Home-page: https://github.com/ieisystem/inManage
 Author: Wangbaoshan
 Author-email: wangbaoshan@ieisystem.com
 License: Expat License
 Description: # InManage
         inManage is a support tool for ansible.ieisystem.inmanage
```

### Comparing `inManage-1.0.1/inManage.egg-info/SOURCES.txt` & `inManage-1.1.0/inManage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage.py` & `inManage-1.1.0/inmanage.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except ImportError:
     INMANAGE_EXIST = False
 sys.path.append(os.path.join(sys.path[0], "interface"))
 current_time = time.strftime(
     '%Y-%m-%d   %H:%M:%S',
     time.localtime(
         time.time()))
-__version__ = '1.0.1'
+__version__ = '1.1.0'
 
 
 ERR_dict = {
     'ERR_CODE_CMN_FAIL': 'data acquisition exception',
     'ERR_CODE_PARAM_NULL': 'parameter is null',
     'ERR_CODE_INPUT_ERROR': 'parameter error',
     'ERR_CODE_INTF_FAIL': 'create link exception',
```

### Comparing `inManage-1.0.1/inmanage_sdk/command/IpmiFunc.py` & `inManage-1.1.0/inmanage_sdk/command/IpmiFunc.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/M5Log/biosPostEventStr.py` & `inManage-1.1.0/inmanage_sdk/command/M5Log/biosPostEventStr.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/M5Log/commonInfoStr.py` & `inManage-1.1.0/inmanage_sdk/command/M5Log/commonInfoStr.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/M5Log/eventLogString.py` & `inManage-1.1.0/inmanage_sdk/command/M5Log/eventLogString.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/M5Log/sensorEventStr.py` & `inManage-1.1.0/inmanage_sdk/command/M5Log/sensorEventStr.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/M5Log/sensorSpecificEventStr.py` & `inManage-1.1.0/inmanage_sdk/command/M5Log/sensorSpecificEventStr.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/M5Log/showSensorDesc.py` & `inManage-1.1.0/inmanage_sdk/command/M5Log/showSensorDesc.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/RedfishFunc.py` & `inManage-1.1.0/inmanage_sdk/command/RedfishFunc.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/RestFunc.py` & `inManage-1.1.0/inmanage_sdk/command/RestFunc.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/backup.py` & `inManage-1.1.0/inmanage_sdk/command/backup.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/bios/A7.xml` & `inManage-1.1.0/inmanage_sdk/command/bios/A7.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/bios/M4.xml` & `inManage-1.1.0/inmanage_sdk/command/bios/M4.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/bios/M5.xml` & `inManage-1.1.0/inmanage_sdk/command/bios/M5.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/bios/M6-N.xml` & `inManage-1.1.0/inmanage_sdk/command/bios/M6-N.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/bios/M6.xml` & `inManage-1.1.0/inmanage_sdk/command/bios/M6.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/bios/M7.xml` & `inManage-1.1.0/inmanage_sdk/command/bios/M7.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/bios/M7_5.10.00.xml` & `inManage-1.1.0/inmanage_sdk/command/bios/M7_5.10.00.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/bios/NF3180A6.xml` & `inManage-1.1.0/inmanage_sdk/command/bios/NF3180A6.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/bios/NF3280A6.xml` & `inManage-1.1.0/inmanage_sdk/command/bios/NF3280A6.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/bios/NF5180M5.xml` & `inManage-1.1.0/inmanage_sdk/command/bios/NF5180M5.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/bios/NF5280M5.xml` & `inManage-1.1.0/inmanage_sdk/command/bios/NF5280M5.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/bios/NF5468A5.xml` & `inManage-1.1.0/inmanage_sdk/command/bios/NF5468A5.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/bios/NF5488A5.xml` & `inManage-1.1.0/inmanage_sdk/command/bios/NF5488A5.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/bios/SA5112M5.xml` & `inManage-1.1.0/inmanage_sdk/command/bios/SA5112M5.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/bios/SA5212M5.xml` & `inManage-1.1.0/inmanage_sdk/command/bios/SA5212M5.xml`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/command/restore.py` & `inManage-1.1.0/inmanage_sdk/command/restore.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/interface/Base.py` & `inManage-1.1.0/inmanage_sdk/interface/Base.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/interface/CommonA5.py` & `inManage-1.1.0/inmanage_sdk/interface/CommonA5.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/interface/CommonA6.py` & `inManage-1.1.0/inmanage_sdk/interface/CommonA6.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/interface/CommonA7.py` & `inManage-1.1.0/inmanage_sdk/interface/CommonA7.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/interface/CommonM5.py` & `inManage-1.1.0/inmanage_sdk/interface/CommonM5.py`

 * *Files 0% similar despite different names*

```diff
@@ -11750,15 +11750,15 @@
                 px[item['slotNum']] = item['devId']
         return pd, pv, px
     else:
         return [], {}, {}
 
 
 def createVirtualDrive(client, args):
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         result = showpdInfo(client, args)
         return result
     result = ResultBean()
     if args.ctrlId is None or args.access is None or args.cache is None or args.init is None \
             or args.rlevel is None or args.slot is None or args.size is None or args.r is None or \
             args.w is None or args.io is None or args.select is None:
         result.State('Failure')
@@ -12102,15 +12102,15 @@
         result.State('Failure')
         result.Message(
             ["Device information Not Available (Device absent or failed to get)!"])
         return result
     elif raidtype == '00' or raidtype == '02' or raidtype == '03':
         result = setLogicalDrive_LSI(args, client)
     elif raidtype == 'ff':
-        if args.Info is not None:
+        if 'Info' in args and args.Info is not None:
             raidDict = {}
             LSIresult = showLogicalInfo_LSI(client, args)
             if LSIresult.State == 'Success':
                 LSI = LSIresult.Message
                 raidDict['LSI'] = LSI
             else:
                 return LSIresult
@@ -12133,15 +12133,15 @@
                 'Failure: failed to establish connection to the host, please check the user/passcode/host/port',
                 'usage: isrest [-h] [-V] -H HOST -U USERNAME -P PASSWORD -p PORT subcommand ...'])
         return result
     return result
 
 
 def setLogicalDrive_LSI(args, client):
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         result = showLogicalInfo_LSI(client, args)
         return result
     else:
         cid, vd = getLogicalInfo_LSI(client, args)
 
     result = ResultBean()
     if args.ctrlId is None or args.ldiskId is None or args.option is None:
@@ -12397,15 +12397,15 @@
         result.State('Failure')
         result.Message(
             ["Device information Not Available (Device absent or failed to get)!"])
         return result
     elif raidtype == '00' or raidtype == '02' or raidtype == '03':
         result = setPhysicalDrive_LSI(args, client)
     elif raidtype == 'ff':
-        if args.Info is not None:
+        if 'Info' in args and args.Info is not None:
             raidDict = {}
             LSIresult = showPhysicalInfo_LSI(args, client)
             if LSIresult.State == 'Success':
                 LSI = LSIresult.Message
                 raidDict['LSI'] = LSI
             else:
                 return LSIresult
@@ -12425,15 +12425,15 @@
         result.Message(["get raid type error."])
         return result
     return result
 
 
 def setPhysicalDrive_LSI(args, client):
     result = ResultBean()
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         result = showPhysicalInfo_LSI(client, args)
         return result
     else:
         cid, pd = getPhysicalInfo_LSI(client, args)
     if args.ctrlId is None or args.deviceId is None or args.option is None:
         result.State('Failure')
         result.Message(["argument ctrl_id, device_id or option is missing"])
```

### Comparing `inManage-1.0.1/inmanage_sdk/interface/CommonM6.py` & `inManage-1.1.0/inmanage_sdk/interface/CommonM6.py`

 * *Files 0% similar despite different names*

```diff
@@ -11350,15 +11350,15 @@
         return ncsiinfo
 
     def setncsi(self, client, args):
         ncsiinfo = ResultBean()
         if args.mode == "auto" and args.channel_number is not None:
             ncsiinfo.State('Failure')
             ncsiinfo.Message('port cannot be set when NCSI mode is auto')
-            return ncsiinfo
+            return ncsiinfoa
         if args.mode == "disable" and (args.nic_type is not None or args.channel_number is not None):
             ncsiinfo.State('Failure')
             ncsiinfo.Message('port and nicname cannot be set when NCSI mode is disable')
             return ncsiinfo
         if args.mode == "disable":
             set_cmd = " 0x3c 0x13 0x01 0x00 0x0f"
             set_res = IpmiFunc.sendRawByIpmi(client, set_cmd)
@@ -12031,15 +12031,15 @@
             if pd['ControllerName'] not in ctrl_list_dict:
                 ctrl_list_dict[pd['ControllerName']] = []
             ctrl_list_dict[pd['ControllerName']].append(pd.get('DeviceID', pd.get('slotNum')))
     else:
         result.State("Failure")
         result.Message(['get physical disk information failed!' + res.get('data')])
         return result
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         for pd in ctrl_list_dict:
             ctrl_list_dict.get(pd).sort()
         LSI_flag = False
         raidList = []
         for ctrlid in ctrl_id_name_dict:
             raidDict = collections.OrderedDict()
             raidDict['Controller ID'] = ctrlid
@@ -12407,15 +12407,15 @@
         result.State("Failure")
         result.Message([res.get('data')])
         return result
 
     for pd in ctrl_ld_list_dict:
         ctrl_ld_list_dict.get(pd).sort()
 
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         LSI_flag = False
         raidList = []
         for ctrlid in ctrl_id_name_dict:
             raidDict = collections.OrderedDict()
             raidDict['Controller ID'] = ctrlid
             raidDict['Controller Name'] = ctrl_id_name_dict.get(ctrlid)
             raidDict['Virtual Drive ID'] = ctrl_ld_list_dict.get(ctrl_id_name_dict.get(ctrlid))
@@ -12570,15 +12570,15 @@
     else:
         result.State("Failure")
         result.Message([res.get('data')])
 
     for pd in ctrl_list_dict:
         ctrl_list_dict.get(pd).sort()
 
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         LSI_flag = False
         raidList = []
         for ctrlid in ctrl_id_name_dict:
             raidDict = collections.OrderedDict()
             raidDict['Controller ID'] = ctrlid
             raidDict['Controller Name'] = ctrl_id_name_dict.get(ctrlid)
             pdiskList = []
```

### Comparing `inManage-1.0.1/inmanage_sdk/interface/CommonM6_41401.py` & `inManage-1.1.0/inmanage_sdk/interface/CommonM6_41401.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     else:
         result.State("Failure")
         result.Message([res.get('data')])
 
     for pd in ctrl_list_dict:
         ctrl_list_dict.get(pd).sort()
 
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         LSI_flag = False
         raidList = []
         for ctrlid in ctrl_id_name_dict:
             raidDict = collections.OrderedDict()
             raidDict['Controller ID'] = ctrlid
             raidDict['Controller Name'] = ctrl_id_name_dict.get(ctrlid)
             pdiskList = []
@@ -258,15 +258,15 @@
         result.State("Failure")
         result.Message([res.get('data')])
         return result
 
     for pd in ctrl_ld_list_dict:
         ctrl_ld_list_dict.get(pd).sort()
 
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         LSI_flag = False
         raidList = []
         for ctrlid in ctrl_id_name_dict:
             raidDict = collections.OrderedDict()
             raidDict['Controller ID'] = ctrlid
             raidDict['Controller Name'] = ctrl_id_name_dict.get(ctrlid)
             raidDict['Virtual Drive ID'] = ctrl_ld_list_dict.get(ctrl_id_name_dict.get(ctrlid))
```

### Comparing `inManage-1.0.1/inmanage_sdk/interface/CommonM6_4140a.py` & `inManage-1.1.0/inmanage_sdk/interface/CommonM6_4140a.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/interface/CommonM7.py` & `inManage-1.1.0/inmanage_sdk/interface/CommonM7.py`

 * *Files 0% similar despite different names*

```diff
@@ -5475,15 +5475,15 @@
             if pd['ControllerName'] not in ctrl_list_dict:
                 ctrl_list_dict[pd['ControllerName']] = []
             ctrl_list_dict[pd['ControllerName']].append(pd['DeviceID'])
     else:
         result.State("Failure")
         result.Message(['get physical disk information failed!' + res.get('data')])
         return result
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         for pd in ctrl_list_dict:
             ctrl_list_dict.get(pd).sort()
         LSI_flag = False
         raidList = []
         for ctrlid in ctrl_id_name_dict:
             raidDict = collections.OrderedDict()
             raidDict['Controller ID'] = ctrlid
```

### Comparing `inManage-1.0.1/inmanage_sdk/interface/I24M6.py` & `inManage-1.1.0/inmanage_sdk/interface/I24M6.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/interface/IBase.py` & `inManage-1.1.0/inmanage_sdk/interface/IBase.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/interface/NF5180M5.py` & `inManage-1.1.0/inmanage_sdk/interface/NF5180M5.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/interface/NF5280M5.py` & `inManage-1.1.0/inmanage_sdk/interface/NF5280M5.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/interface/NF5280M5_435.py` & `inManage-1.1.0/inmanage_sdk/interface/NF5280M5_435.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/interface/NF5280M5_436.py` & `inManage-1.1.0/inmanage_sdk/interface/NF5280M5_436.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/interface/NS5160M6.py` & `inManage-1.1.0/inmanage_sdk/interface/NS5160M6.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/interface/ResEntity.py` & `inManage-1.1.0/inmanage_sdk/interface/ResEntity.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/util/HostTypeJudge.py` & `inManage-1.1.0/inmanage_sdk/util/HostTypeJudge.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/util/RedfishClient.py` & `inManage-1.1.0/inmanage_sdk/util/RedfishClient.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/util/RegularCheckUtil.py` & `inManage-1.1.0/inmanage_sdk/util/RegularCheckUtil.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/util/RequestClient.py` & `inManage-1.1.0/inmanage_sdk/util/RequestClient.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/util/configUtil.py` & `inManage-1.1.0/inmanage_sdk/util/configUtil.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/util/fileUtil.py` & `inManage-1.1.0/inmanage_sdk/util/fileUtil.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/inmanage_sdk/util/parameterConversion.py` & `inManage-1.1.0/inmanage_sdk/util/parameterConversion.py`

 * *Files identical despite different names*

### Comparing `inManage-1.0.1/setup.py` & `inManage-1.1.0/setup.py`

 * *Files identical despite different names*

