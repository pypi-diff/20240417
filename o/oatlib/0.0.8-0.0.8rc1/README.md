# Comparing `tmp/oatlib-0.0.8.tar.gz` & `tmp/oatlib-0.0.8rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oatlib-0.0.8.tar", last modified: Wed Sep  7 14:08:18 2022, max compression
+gzip compressed data, was "oatlib-0.0.8rc1.tar", last modified: Thu Sep  8 08:27:08 2022, max compression
```

## Comparing `oatlib-0.0.8.tar` & `oatlib-0.0.8rc1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2022-09-07 14:08:18.987030 oatlib-0.0.8/
--rw-rw-r--   0 jovyan    (1000) users      (100)      956 2020-05-25 14:29:32.000000 oatlib-0.0.8/LICENSE
--rw-r--r--   0 jovyan    (1000) users      (100)     1782 2022-09-07 14:08:18.987030 oatlib-0.0.8/PKG-INFO
--rw-rw-r--   0 jovyan    (1000) users      (100)     1305 2022-08-05 12:38:14.000000 oatlib-0.0.8/README.md
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2022-09-07 14:08:18.983030 oatlib-0.0.8/oatlib/
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2022-09-07 14:08:18.983030 oatlib-0.0.8/oatlib/oatlib/
--rw-rw-r--   0 jovyan    (1000) users      (100)     2705 2022-09-07 14:02:38.000000 oatlib-0.0.8/oatlib/oatlib/__init__.py
--rw-rw-r--   0 jovyan    (1000) users      (100)    48664 2022-08-05 10:15:19.000000 oatlib-0.0.8/oatlib/oatlib/method.py
--rw-rw-r--   0 jovyan    (1000) users      (100)     8017 2020-05-25 14:29:32.000000 oatlib-0.0.8/oatlib/oatlib/oat_algorithms.py
--rw-rw-r--   0 jovyan    (1000) users      (100)    29948 2022-08-05 10:25:05.000000 oatlib-0.0.8/oatlib/oatlib/oat_utils.py
--rw-rw-r--   0 jovyan    (1000) users      (100)    51497 2022-04-24 17:53:56.000000 oatlib-0.0.8/oatlib/oatlib/sensor.py
--rw-rw-r--   0 jovyan    (1000) users      (100)    13753 2022-09-07 14:01:55.000000 oatlib-0.0.8/oatlib/oatlib/sos2sos.py
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2022-09-07 14:08:18.987030 oatlib-0.0.8/oatlib/oatlib.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)     1782 2022-09-07 14:08:18.000000 oatlib-0.0.8/oatlib/oatlib.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)      416 2022-09-07 14:08:18.000000 oatlib-0.0.8/oatlib/oatlib.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2022-09-07 14:08:18.000000 oatlib-0.0.8/oatlib/oatlib.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       66 2022-09-07 14:08:18.000000 oatlib-0.0.8/oatlib/oatlib.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        7 2022-09-07 14:08:18.000000 oatlib-0.0.8/oatlib/oatlib.egg-info/top_level.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2022-08-05 08:35:55.000000 oatlib-0.0.8/oatlib/oatlib.egg-info/zip-safe
--rw-rw-r--   0 jovyan    (1000) users      (100)       80 2022-08-05 12:23:31.000000 oatlib-0.0.8/pyproject.toml
--rw-rw-r--   0 jovyan    (1000) users      (100)      744 2022-09-07 14:08:18.987030 oatlib-0.0.8/setup.cfg
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2022-09-08 08:27:08.929427 oatlib-0.0.8rc1/
+-rw-rw-r--   0 jovyan    (1000) users      (100)      956 2020-05-25 14:29:32.000000 oatlib-0.0.8rc1/LICENSE
+-rw-r--r--   0 jovyan    (1000) users      (100)     1799 2022-09-08 08:27:08.929427 oatlib-0.0.8rc1/PKG-INFO
+-rw-rw-r--   0 jovyan    (1000) users      (100)     1319 2022-09-08 07:18:49.000000 oatlib-0.0.8rc1/README.md
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2022-09-08 08:27:08.925427 oatlib-0.0.8rc1/oatlib/
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2022-09-08 08:27:08.929427 oatlib-0.0.8rc1/oatlib/oatlib/
+-rw-rw-r--   0 jovyan    (1000) users      (100)     2708 2022-09-07 14:16:45.000000 oatlib-0.0.8rc1/oatlib/oatlib/__init__.py
+-rw-rw-r--   0 jovyan    (1000) users      (100)    48664 2022-08-05 10:15:19.000000 oatlib-0.0.8rc1/oatlib/oatlib/method.py
+-rw-rw-r--   0 jovyan    (1000) users      (100)     8017 2020-05-25 14:29:32.000000 oatlib-0.0.8rc1/oatlib/oatlib/oat_algorithms.py
+-rw-rw-r--   0 jovyan    (1000) users      (100)    29948 2022-08-05 10:25:05.000000 oatlib-0.0.8rc1/oatlib/oatlib/oat_utils.py
+-rw-rw-r--   0 jovyan    (1000) users      (100)    51497 2022-04-24 17:53:56.000000 oatlib-0.0.8rc1/oatlib/oatlib/sensor.py
+-rw-rw-r--   0 jovyan    (1000) users      (100)    14379 2022-09-08 07:24:20.000000 oatlib-0.0.8rc1/oatlib/oatlib/sos2sos.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2022-09-08 08:27:08.929427 oatlib-0.0.8rc1/oatlib/oatlib.egg-info/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1799 2022-09-08 08:27:08.000000 oatlib-0.0.8rc1/oatlib/oatlib.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)      416 2022-09-08 08:27:08.000000 oatlib-0.0.8rc1/oatlib/oatlib.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2022-09-08 08:27:08.000000 oatlib-0.0.8rc1/oatlib/oatlib.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       66 2022-09-08 08:27:08.000000 oatlib-0.0.8rc1/oatlib/oatlib.egg-info/requires.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        7 2022-09-08 08:27:08.000000 oatlib-0.0.8rc1/oatlib/oatlib.egg-info/top_level.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2022-08-05 08:35:55.000000 oatlib-0.0.8rc1/oatlib/oatlib.egg-info/zip-safe
+-rw-rw-r--   0 jovyan    (1000) users      (100)       80 2022-08-05 12:23:31.000000 oatlib-0.0.8rc1/pyproject.toml
+-rw-rw-r--   0 jovyan    (1000) users      (100)      744 2022-09-08 08:27:08.929427 oatlib-0.0.8rc1/setup.cfg
```

### Comparing `oatlib-0.0.8/LICENSE` & `oatlib-0.0.8rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `oatlib-0.0.8/PKG-INFO` & `oatlib-0.0.8rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oatlib
-Version: 0.0.8
+Version: 0.0.8rc1
 Summary: Observation Analysis Tool: library to handle time series
 Home-page: https://gitlab.com/ist-supsi/OAT
 Author: Massimiliano Cannata
 Author-email: massimiliano.cannata@gmail.com
 License: GPLv2+
 Keywords: example,setuptools
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
@@ -29,16 +29,17 @@
 
 ## Create pypi package
 
 modify the code and
 **change the VERSION in __init__.py**
 
 # run scipy-notebook docker
-docker run -p 10000:8888 -v /home/maxi/GIT/OAT/oatlib:/home/jovyan/work jupyter/scipy-notebook:807999a41207
+docker run -p 10000:8888 -v /home/maxi/GIT/OAT:/home/jovyan/work jupyter/scipy-notebook:807999a41207
 # in jupyter-lab terminal build the package
+cd /home/jovyan/work
 python -m pip install --upgrade setuptools
 python -m pip install --upgrade pip
 python -m pip install --upgrade build
 python -m build
 
 # test the package in your notebook
 pip install /home/jovyan/work/dist/oatlib-__YOUR_VERSION_HERE__-py3-none-any.whl
```

### Comparing `oatlib-0.0.8/README.md` & `oatlib-0.0.8rc1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 
 ## Create pypi package
 
 modify the code and
 **change the VERSION in __init__.py**
 
 # run scipy-notebook docker
-docker run -p 10000:8888 -v /home/maxi/GIT/OAT/oatlib:/home/jovyan/work jupyter/scipy-notebook:807999a41207
+docker run -p 10000:8888 -v /home/maxi/GIT/OAT:/home/jovyan/work jupyter/scipy-notebook:807999a41207
 # in jupyter-lab terminal build the package
+cd /home/jovyan/work
 python -m pip install --upgrade setuptools
 python -m pip install --upgrade pip
 python -m pip install --upgrade build
 python -m build
 
 # test the package in your notebook
 pip install /home/jovyan/work/dist/oatlib-__YOUR_VERSION_HERE__-py3-none-any.whl
```

### Comparing `oatlib-0.0.8/oatlib/oatlib/__init__.py` & `oatlib-0.0.8rc1/oatlib/oatlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,9 +72,9 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 #
 # ===============================================================================
 __all__ = ["sensor", "method", "oat_utils", "oat_algorithms","sos2sos"]
-__version__ = "0.0.8"
+__version__ = "0.0.8rc1"
```

### Comparing `oatlib-0.0.8/oatlib/oatlib/method.py` & `oatlib-0.0.8rc1/oatlib/oatlib/method.py`

 * *Files identical despite different names*

### Comparing `oatlib-0.0.8/oatlib/oatlib/oat_algorithms.py` & `oatlib-0.0.8rc1/oatlib/oatlib/oat_algorithms.py`

 * *Files identical despite different names*

### Comparing `oatlib-0.0.8/oatlib/oatlib/oat_utils.py` & `oatlib-0.0.8rc1/oatlib/oatlib/oat_utils.py`

 * *Files identical despite different names*

### Comparing `oatlib-0.0.8/oatlib/oatlib/sensor.py` & `oatlib-0.0.8rc1/oatlib/oatlib/sensor.py`

 * *Files identical despite different names*

### Comparing `oatlib-0.0.8/oatlib/oatlib/sos2sos.py` & `oatlib-0.0.8rc1/oatlib/oatlib/sos2sos.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,15 +79,16 @@
         'filter_qilist': [],
         'min_obs': 1,
         'nan_qi': 0,
         'nan_data': -999.9,
         'closed': 'right',
         'label': 'right',
         'tz': '+00:00',
-        'data_verbose': False
+        'data_verbose': False,
+        'test_only': False
     }
     forcePeriod = False
     # Set general settings merging general into default
     for k in list(def_settings.keys()):
         if k in gen_settings:
             def_settings[k] = gen_settings[k]
 
@@ -156,14 +157,18 @@
         settings = {}
         for k in list(gen_settings.keys()):
             if k in sen_settings:
                 settings[k] = sen_settings[k]
             else:
                 settings[k] = gen_settings[k]
 
+        if verbose:
+            print("|")
+            print("|----> aggregating with settings: %s" % settings)
+
         aggsens = {}
         for key, dest_proc in list(obs.items()):
 
             # set OAT.sensor from origin
             asen = sensor.Sensor.from_istsos(
                 service=origin_service,
                 procedure=dest_proc['origin_proc'],
@@ -242,19 +247,24 @@
                 observed_property=dest_proc['origin_obspro'],
                 event_time=period,
                 freq=frequency,
                 basic_auth=origin_auth
             )
             if verbose:
                 print("|----> %s timeSerie uploaded" % key.split(":")[-1])
-                #if (not asen.ts is None):
-                #    print("|----> STATS")
-                #    print("|----> %s" % asen.ts.describe())
-                #    print("|----> DATA")
-                #    print("|----> %s" % asen.ts)
+                if (not asen.ts is None) and (not asen.ts.empty):
+                    print("|----> %s origin timeSerie rows" % len(asen.ts))
+                else:
+                    print("|----> %s origin timeSerie is Empty" % len(asen.ts))
+
+                if (not asen.ts is None and settings['data_verbose']):
+                   print("|----> STATS")
+                   print("|----> %s" % asen.ts.describe())
+                   print("|----> DATA")
+                   print("|----> %s" % asen.ts)
 
             # print('asen:',asen)
             # print("AGG: ",dest_proc['origin_agg_method'])
 
             if (not asen.ts is None) and (not asen.ts.empty):
                 # aggregate serie (only if dest_proc['origin_agg_method']
                 if 'origin_agg_method' in dest_proc and 'origin_agg_freq' in dest_proc:
@@ -265,14 +275,16 @@
                                     qilist=settings['filter_qilist'] if 'filter_qilist' in settings else None,
                                     min_obs=settings['min_obs'] if 'min_obs' in settings else None,
                                     closed=settings['closed'] if 'closed' in settings else 'right',
                                     label=settings['label'] if 'label' in settings else 'right'
                                 )
                     if aggsens[key].ts.empty:
                         push = False
+                        if verbose:
+                            print("|----> %s dest timeSerie aggregated rows" % len(aggsens[key].ts))
                 else:
                     aggsens[key] = asen
 
                 if 'force_qi' in dest_proc and dest_proc['force_qi']:
                     aggsens[key].ts['quality'] = dest_proc['force_qi']
 
                 # FILL NO DATA WITH PROVIDED VLUES
@@ -289,16 +301,17 @@
             res = ou.sensors_to_istsos(
                 service=destination_service,
                 procedure=dest_sens,
                 obspro_sensor=aggsens,
                 qualityIndex=settings['updateQualityIndex'] if 'updateQualityIndex' in settings else True,
                 period=period if forcePeriod else None,
                 basic_auth=destination_auth,
-                verbose=def_settings['data_verbose'],
-                nan_qi=settings['nan_qi'] if 'nan_qi' in settings else 0  # TODO: use this for settings or dict in obsepro
+                verbose=settings['data_verbose'],
+                nan_qi=settings['nan_qi'] if 'nan_qi' in settings else 0,  # TODO: use this for settings or dict in obsepro
+                test_only=settings['test_only'] if 'test_only' in settings else False
             )
             if verbose or minlog:
                 print("|")
                 print("%s procedure successfully updated" % dest_sens)
                 print("=================================")
         else:
             if verbose or minlog:
```

### Comparing `oatlib-0.0.8/oatlib/oatlib.egg-info/PKG-INFO` & `oatlib-0.0.8rc1/oatlib/oatlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oatlib
-Version: 0.0.8
+Version: 0.0.8rc1
 Summary: Observation Analysis Tool: library to handle time series
 Home-page: https://gitlab.com/ist-supsi/OAT
 Author: Massimiliano Cannata
 Author-email: massimiliano.cannata@gmail.com
 License: GPLv2+
 Keywords: example,setuptools
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
@@ -29,16 +29,17 @@
 
 ## Create pypi package
 
 modify the code and
 **change the VERSION in __init__.py**
 
 # run scipy-notebook docker
-docker run -p 10000:8888 -v /home/maxi/GIT/OAT/oatlib:/home/jovyan/work jupyter/scipy-notebook:807999a41207
+docker run -p 10000:8888 -v /home/maxi/GIT/OAT:/home/jovyan/work jupyter/scipy-notebook:807999a41207
 # in jupyter-lab terminal build the package
+cd /home/jovyan/work
 python -m pip install --upgrade setuptools
 python -m pip install --upgrade pip
 python -m pip install --upgrade build
 python -m build
 
 # test the package in your notebook
 pip install /home/jovyan/work/dist/oatlib-__YOUR_VERSION_HERE__-py3-none-any.whl
```

### Comparing `oatlib-0.0.8/setup.cfg` & `oatlib-0.0.8rc1/setup.cfg`

 * *Files identical despite different names*

