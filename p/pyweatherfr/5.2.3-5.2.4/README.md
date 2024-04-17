# Comparing `tmp/pyweatherfr-5.2.3.tar.gz` & `tmp/pyweatherfr-5.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-5.2.3.tar", last modified: Tue Apr 16 07:23:47 2024, max compression
+gzip compressed data, was "pyweatherfr-5.2.4.tar", last modified: Tue Apr 16 20:01:34 2024, max compression
```

## Comparing `pyweatherfr-5.2.3.tar` & `pyweatherfr-5.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:23:47.135275 pyweatherfr-5.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 07:23:47.135275 pyweatherfr-5.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:23:47.135275 pyweatherfr-5.2.3/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    44338 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:23:47.135275 pyweatherfr-5.2.3/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 07:23:47.000000 pyweatherfr-5.2.3/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 07:23:47.000000 pyweatherfr-5.2.3/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:23:47.000000 pyweatherfr-5.2.3/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 07:23:47.000000 pyweatherfr-5.2.3/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:23:08.000000 pyweatherfr-5.2.3/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-16 07:23:47.000000 pyweatherfr-5.2.3/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 07:23:47.000000 pyweatherfr-5.2.3/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:23:47.135275 pyweatherfr-5.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:01:34.448013 pyweatherfr-5.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 20:00:34.000000 pyweatherfr-5.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 20:01:34.444013 pyweatherfr-5.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-16 20:00:34.000000 pyweatherfr-5.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 20:00:34.000000 pyweatherfr-5.2.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:01:34.444013 pyweatherfr-5.2.4/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-16 20:00:34.000000 pyweatherfr-5.2.4/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-16 20:00:34.000000 pyweatherfr-5.2.4/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44873 2024-04-16 20:00:34.000000 pyweatherfr-5.2.4/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-16 20:00:34.000000 pyweatherfr-5.2.4/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:01:34.444013 pyweatherfr-5.2.4/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 20:01:34.000000 pyweatherfr-5.2.4/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 20:01:34.000000 pyweatherfr-5.2.4/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:01:34.000000 pyweatherfr-5.2.4/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 20:01:34.000000 pyweatherfr-5.2.4/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:00:38.000000 pyweatherfr-5.2.4/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-16 20:01:34.000000 pyweatherfr-5.2.4/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 20:01:34.000000 pyweatherfr-5.2.4/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:01:34.448013 pyweatherfr-5.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-16 20:00:34.000000 pyweatherfr-5.2.4/setup.py
```

### Comparing `pyweatherfr-5.2.3/LICENSE.txt` & `pyweatherfr-5.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.2.3/PKG-INFO` & `pyweatherfr-5.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.2.3
+Version: 5.2.4
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.2.3/README.md` & `pyweatherfr-5.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.2.3/pyweatherfr/args.py` & `pyweatherfr-5.2.4/pyweatherfr/args.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.2.3/pyweatherfr/pyweatherfr.py` & `pyweatherfr-5.2.4/pyweatherfr/pyweatherfr.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,22 +47,24 @@
 WARM = "\U0001F321"
 HOME = "\U0001F3E0"
 BOUSSOLE = "\U0001F9ED"
 CLOCK = "\U000023F0"
 THERMO = "\U0001F321"
 HUMIDITE = "\U0001F4A7"
 PLUIE = "\U0001F327"
-FLECHE_N = "\U00002B07"
+
+FLECHE_N = "\U00002193"
 FLECHE_NO = "\U00002198"
-FLECHE_O = "\U000027A1"
+FLECHE_O = "\U00002192"
 FLECHE_SO = "\U00002197"
-FLECHE_S = "\U00002B06"
+FLECHE_S = "\U00002191"
 FLECHE_SE = "\U00002196"
-FLECHE_E = "\U00002B05"
+FLECHE_E = "\U00002190"
 FLECHE_NE = "\U00002199"
+
 ELEPHANT = "\U0001F418"
 PLUME = "\U0001FAB6"
 PC ="\U0001f4bb"
 LUNETTES= "\U0001F60E"
 WARNING_WARM=30
 WARNING_FROID=0
 WARNING_SNOW=0.1
@@ -794,39 +796,40 @@
     others = ','.join(parties[1:])
     print_debug(town)
     print_debug(others)
     ctx = ssl.create_default_context(cafile=certifi.where())
     geopy.geocoders.options.default_ssl_context = ctx
     geolocator = geopy.geocoders.Nominatim(user_agent="my_geocoder")
     if compute_args().lang:
-        locations = geolocator.geocode(town+","+others,featuretype="city",exactly_one=False,addressdetails=True,limit=9999)
+        locations = geolocator.geocode(town+","+others,exactly_one=False,addressdetails=True,limit=9999)
     else:
-        locations = geolocator.geocode(town+","+others,featuretype="city",exactly_one=False,addressdetails=True,language="fr",limit=9999)    
+        locations = geolocator.geocode(town+","+others,exactly_one=False,addressdetails=True,language="fr",limit=9999)    
     choix = []
     if locations is None:
         print(my_colored("erreur : aucune ville trouvée", "red"))
         exit(1)  
     world=False
     print_debug(str(len(locations)) +" villes trouvées")    
     for location in locations:
         print_debug(json.dumps(location.raw, indent=4,ensure_ascii=False))
-        if ((location.raw.get("addresstype")=="postcode" and location.raw.get("address").get("country")=="France") or location.raw.get("addresstype")=="hamlet" or location.raw.get("addresstype")=="town" or location.raw.get("addresstype")=="city" or location.raw.get("addresstype")=="municipality" or location.raw.get("addresstype")=="village" or location.raw.get("addresstype")=="province"):   
+        if ((location.raw.get("addresstype")=="postcode" and location.raw.get("address").get("country")=="France") or (location.raw.get("addresstype")=="hamlet" and location.raw.get("address").get("country")!="France") or location.raw.get("addresstype")=="town" or location.raw.get("addresstype")=="city" or location.raw.get("addresstype")=="municipality" or location.raw.get("addresstype")=="village" or (location.raw.get("addresstype")=="province" and location.raw.get("address").get("country_code")=="jp")):   
             ville = None
             if ville is None and (location.raw.get("address").get("province") is not None and (clean_string(location.raw.get("address").get("province").lower())==clean_string(town.lower()))):
                 ville = location.raw.get("address").get("province")                 
             if ville is None and (location.raw.get("address").get("city") is not None and (clean_string(location.raw.get("address").get("city").lower())==clean_string(town.lower()))):
                 ville = location.raw.get("address").get("city") 
             if ville is None and (location.raw.get("address").get("town") is not None and (clean_string(location.raw.get("address").get("town").lower())==clean_string(town.lower()))):
                 ville = location.raw.get("address").get("town")               
             if ville is None and (location.raw.get("address").get("municipality") is not None and (clean_string(location.raw.get("address").get("municipality").lower())==clean_string(town.lower()))):
                 ville = location.raw.get("address").get("municipality")
             if ville is None and (location.raw.get("address").get("village") is not None and (clean_string(location.raw.get("address").get("village").lower())==clean_string(town.lower()))):
                 ville = location.raw.get("address").get("village")
             if ville is None and (location.raw.get("address").get("hamlet") is not None and (clean_string(location.raw.get("address").get("hamlet").lower())==clean_string(town.lower()))):
                 ville = location.raw.get("address").get("hamlet")
+
             dpt = ""
             if location.raw.get("address").get("county") is not None:        
                 dpt = location.raw.get("address").get("county")
             if location.raw.get("address").get("state") is not None:
                 if dpt =="":
                     dpt = location.raw.get("address").get("state")  
                 else:
@@ -848,28 +851,30 @@
                     ville = location.raw.get("address").get("town")               
                 if ville is None and (location.raw.get("address").get("city") is not None):
                     ville = location.raw.get("address").get("city")                 
             else:
                 cp = ""
             lat = location.raw.get("lat")
             long = location.raw.get("lon")
+            if location.raw.get("address").get("country")=="France" and ((location.raw.get("address").get("municipality") is not None and location.raw.get("address").get("village") is not None and location.raw.get("address").get("city") is not None) or (location.raw.get("address").get("municipality") is not None and location.raw.get("address").get("town") is not None and location.raw.get("address").get("city") is not None)):
+                ville=None
             if ville is not None:
                 print_debug(ville+"-"+dpt+"-"+lat+"-"+long+"-"+country)
                 if (clean_string(ville.lower()) == clean_string(town.lower()) or cp.lower() == town.lower()):
                     if ville+"-"+dpt not in [item[0] for item in choix]:  
                         if country=="France":
                             choix.append([ville+"-"+dpt, ville, dpt, country,lat, long])
                         else:
                             if compute_args().world:
                                 choix.append([ville+"-"+dpt, ville, dpt, country,lat, long])
                             else:
                                 world=True    
     if not compute_args().world and world:
         print("")
-        print(my_colored("warning : il existe des villes hors France disponibles pour wotre recherche. Relancez la avec --world pour y acceder", "yellow"))
+        print(my_colored("warning : il existe des villes hors France disponibles pour wotre recherche. Relancez la avec -w pour y acceder", "yellow"))
     if len(choix)==1:
         choice = choix[0]
         ville = choice[1]
         dpt = choice[2]
         country = choice[3]
         lat = choice[4]
         long = choice[5]
```

### Comparing `pyweatherfr-5.2.3/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-5.2.4/pyweatherfr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.2.3
+Version: 5.2.4
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.2.3/setup.py` & `pyweatherfr-5.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="5.2.3",
+    version="5.2.4",
     description="pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

