# Comparing `tmp/winiel-rfid-sensor-0.0.6.tar.gz` & `tmp/winiel-rfid-sensor-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winiel-rfid-sensor-0.0.6.tar", last modified: Thu Apr 11 07:06:41 2024, max compression
+gzip compressed data, was "winiel-rfid-sensor-0.0.7.tar", last modified: Wed Apr 17 01:04:32 2024, max compression
```

## Comparing `winiel-rfid-sensor-0.0.6.tar` & `winiel-rfid-sensor-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-04-11 07:06:41.994812 winiel-rfid-sensor-0.0.6/
--rw-r--r--   0 yongjinsohn   (501) staff       (20)      501 2024-04-11 07:06:41.994373 winiel-rfid-sensor-0.0.6/PKG-INFO
--rw-r--r--   0 yongjinsohn   (501) staff       (20)       38 2024-04-11 07:06:41.994918 winiel-rfid-sensor-0.0.6/setup.cfg
--rw-r--r--   0 yongjinsohn   (501) staff       (20)      760 2024-04-11 07:04:14.000000 winiel-rfid-sensor-0.0.6/setup.py
-drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-04-11 07:06:41.990852 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor/
--rw-r--r--   0 yongjinsohn   (501) staff       (20)       22 2024-04-11 07:04:14.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor/__init__.py
--rw-r--r--   0 yongjinsohn   (501) staff       (20)     4620 2024-04-11 07:00:38.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor/rfid_sensor.py
-drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-04-11 07:06:41.993875 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor.egg-info/
--rw-r--r--   0 yongjinsohn   (501) staff       (20)      501 2024-04-11 07:06:41.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor.egg-info/PKG-INFO
--rw-r--r--   0 yongjinsohn   (501) staff       (20)      323 2024-04-11 07:06:41.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor.egg-info/SOURCES.txt
--rw-r--r--   0 yongjinsohn   (501) staff       (20)        1 2024-04-11 07:06:41.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor.egg-info/dependency_links.txt
--rw-r--r--   0 yongjinsohn   (501) staff       (20)        1 2024-03-29 04:23:22.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor.egg-info/not-zip-safe
--rw-r--r--   0 yongjinsohn   (501) staff       (20)       15 2024-04-11 07:06:41.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor.egg-info/requires.txt
--rw-r--r--   0 yongjinsohn   (501) staff       (20)       19 2024-04-11 07:06:41.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor.egg-info/top_level.txt
+drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-04-17 01:04:32.572453 winiel-rfid-sensor-0.0.7/
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)      501 2024-04-17 01:04:32.571998 winiel-rfid-sensor-0.0.7/PKG-INFO
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)       38 2024-04-17 01:04:32.572561 winiel-rfid-sensor-0.0.7/setup.cfg
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)      760 2024-04-11 07:04:14.000000 winiel-rfid-sensor-0.0.7/setup.py
+drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-04-17 01:04:32.567671 winiel-rfid-sensor-0.0.7/winiel_rfid_sensor/
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)       22 2024-04-17 01:04:30.000000 winiel-rfid-sensor-0.0.7/winiel_rfid_sensor/__init__.py
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)     4660 2024-04-17 01:03:56.000000 winiel-rfid-sensor-0.0.7/winiel_rfid_sensor/rfid_sensor.py
+drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-04-17 01:04:32.571437 winiel-rfid-sensor-0.0.7/winiel_rfid_sensor.egg-info/
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)      501 2024-04-17 01:04:32.000000 winiel-rfid-sensor-0.0.7/winiel_rfid_sensor.egg-info/PKG-INFO
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)      323 2024-04-17 01:04:32.000000 winiel-rfid-sensor-0.0.7/winiel_rfid_sensor.egg-info/SOURCES.txt
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)        1 2024-04-17 01:04:32.000000 winiel-rfid-sensor-0.0.7/winiel_rfid_sensor.egg-info/dependency_links.txt
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)        1 2024-03-29 04:23:22.000000 winiel-rfid-sensor-0.0.7/winiel_rfid_sensor.egg-info/not-zip-safe
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)       15 2024-04-17 01:04:32.000000 winiel-rfid-sensor-0.0.7/winiel_rfid_sensor.egg-info/requires.txt
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)       19 2024-04-17 01:04:32.000000 winiel-rfid-sensor-0.0.7/winiel_rfid_sensor.egg-info/top_level.txt
```

### Comparing `winiel-rfid-sensor-0.0.6/setup.py` & `winiel-rfid-sensor-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `winiel-rfid-sensor-0.0.6/winiel_rfid_sensor/rfid_sensor.py` & `winiel-rfid-sensor-0.0.7/winiel_rfid_sensor/rfid_sensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,14 +114,15 @@
             std_dev_rssi = np.std(rssi_values)  # RSSI 값의 표준 편차
             avg_rssi = np.mean(rssi_values)  # RSSI 평균 값
             # 거리 추정
             distance = 10 ** ((rssi_at_1m - avg_rssi) / (10 * path_loss_exponent))
             results[sensor_id] = {
                 "occurrence" : occurrence
                 , "std_dev_rssi" : std_dev_rssi
+                , "avg_rssi" : avg_rssi
                 , "distance" : distance
             }
         return results
 
 
     def getData(self):
         return self.results
```

