# Comparing `tmp/Velkoz-0.0.59.tar.gz` & `tmp/Velkoz-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Velkoz-0.0.59.tar", last modified: Tue Apr 16 16:29:01 2024, max compression
+gzip compressed data, was "Velkoz-0.0.6.tar", last modified: Tue Apr 16 21:13:35 2024, max compression
```

## Comparing `Velkoz-0.0.59.tar` & `Velkoz-0.0.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 16:29:01.326945 Velkoz-0.0.59/
--rw-rw-rw-   0        0        0      563 2024-04-16 16:29:01.325945 Velkoz-0.0.59/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 16:29:01.267907 Velkoz-0.0.59/Velkoz/
--rw-rw-rw-   0        0        0      785 2024-04-16 11:13:15.000000 Velkoz-0.0.59/Velkoz/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 16:29:01.288920 Velkoz-0.0.59/Velkoz/data/
--rw-rw-rw-   0        0        0       48 2024-04-13 20:58:45.000000 Velkoz-0.0.59/Velkoz/data/__init__.py
--rw-rw-rw-   0        0        0     2832 2024-04-16 16:28:25.000000 Velkoz-0.0.59/Velkoz/data/champion.py
--rw-rw-rw-   0        0        0     2193 2024-04-16 16:26:49.000000 Velkoz-0.0.59/Velkoz/data/common.py
-drwxrwxrwx   0        0        0        0 2024-04-16 16:29:01.298017 Velkoz-0.0.59/Velkoz/eye/
--rw-rw-rw-   0        0        0      150 2024-03-23 23:06:35.000000 Velkoz-0.0.59/Velkoz/eye/__init__.py
--rw-rw-rw-   0        0        0      523 2024-04-10 19:31:41.000000 Velkoz-0.0.59/Velkoz/eye/account.py
--rw-rw-rw-   0        0        0      591 2024-04-09 19:37:05.000000 Velkoz-0.0.59/Velkoz/eye/champion_mastery.py
--rw-rw-rw-   0        0        0        8 2024-03-22 13:50:02.000000 Velkoz-0.0.59/Velkoz/eye/common.py
--rw-rw-rw-   0        0        0     7581 2024-04-12 12:51:42.000000 Velkoz-0.0.59/Velkoz/eye/match.py
--rw-rw-rw-   0        0        0     1976 2024-04-10 19:31:40.000000 Velkoz-0.0.59/Velkoz/eye/summoner.py
--rw-rw-rw-   0        0        0     3276 2024-04-16 15:09:23.000000 Velkoz-0.0.59/Velkoz/settings.py
--rw-rw-rw-   0        0        0     1032 2024-04-16 16:28:55.000000 Velkoz-0.0.59/Velkoz/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 16:29:01.309141 Velkoz-0.0.59/Velkoz/supp/
--rw-rw-rw-   0        0        0      154 2024-04-16 10:08:55.000000 Velkoz-0.0.59/Velkoz/supp/__init__.py
--rw-rw-rw-   0        0        0      601 2024-04-10 19:50:35.000000 Velkoz-0.0.59/Velkoz/supp/account.py
--rw-rw-rw-   0        0        0      280 2024-04-16 11:05:52.000000 Velkoz-0.0.59/Velkoz/supp/champion.py
--rw-rw-rw-   0        0        0     1165 2024-04-11 21:19:17.000000 Velkoz-0.0.59/Velkoz/supp/champion_mastery.py
--rw-rw-rw-   0        0        0      270 2024-04-11 21:19:18.000000 Velkoz-0.0.59/Velkoz/supp/match.py
--rw-rw-rw-   0        0        0     1681 2024-04-10 19:50:14.000000 Velkoz-0.0.59/Velkoz/supp/summoner.py
-drwxrwxrwx   0        0        0        0 2024-04-16 16:29:01.322830 Velkoz-0.0.59/Velkoz/tentacles/
--rw-rw-rw-   0        0        0      213 2024-04-11 21:19:17.000000 Velkoz-0.0.59/Velkoz/tentacles/__init__.py
--rw-rw-rw-   0        0        0     1224 2024-03-22 11:07:43.000000 Velkoz-0.0.59/Velkoz/tentacles/account.py
--rw-rw-rw-   0        0        0     3340 2024-04-11 21:19:18.000000 Velkoz-0.0.59/Velkoz/tentacles/champion_mastery.py
--rw-rw-rw-   0        0        0     4543 2024-04-12 22:57:44.000000 Velkoz-0.0.59/Velkoz/tentacles/common.py
--rw-rw-rw-   0        0        0       60 2024-04-05 19:09:48.000000 Velkoz-0.0.59/Velkoz/tentacles/config.py
--rw-rw-rw-   0        0        0     1650 2024-03-22 13:51:43.000000 Velkoz-0.0.59/Velkoz/tentacles/match.py
--rw-rw-rw-   0        0        0     1416 2024-03-22 11:06:12.000000 Velkoz-0.0.59/Velkoz/tentacles/summoner.py
--rw-rw-rw-   0        0        0     6667 2024-04-16 16:28:23.000000 Velkoz-0.0.59/Velkoz/velkoz.py
-drwxrwxrwx   0        0        0        0 2024-04-16 16:29:01.324934 Velkoz-0.0.59/Velkoz.egg-info/
--rw-rw-rw-   0        0        0      563 2024-04-16 16:29:01.000000 Velkoz-0.0.59/Velkoz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      780 2024-04-16 16:29:01.000000 Velkoz-0.0.59/Velkoz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 16:29:01.000000 Velkoz-0.0.59/Velkoz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-16 16:29:01.000000 Velkoz-0.0.59/Velkoz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-16 16:29:01.000000 Velkoz-0.0.59/Velkoz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 16:29:01.326945 Velkoz-0.0.59/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 21:13:35.504926 Velkoz-0.0.6/
+-rw-rw-rw-   0        0        0      562 2024-04-16 21:13:35.503417 Velkoz-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 21:13:35.231120 Velkoz-0.0.6/Velkoz/
+-rw-rw-rw-   0        0        0      816 2024-04-16 21:12:33.000000 Velkoz-0.0.6/Velkoz/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 21:13:35.272931 Velkoz-0.0.6/Velkoz/data/
+-rw-rw-rw-   0        0        0       48 2024-04-13 20:58:45.000000 Velkoz-0.0.6/Velkoz/data/__init__.py
+-rw-rw-rw-   0        0        0     2832 2024-04-16 16:28:25.000000 Velkoz-0.0.6/Velkoz/data/champion.py
+-rw-rw-rw-   0        0        0     2197 2024-04-16 20:27:43.000000 Velkoz-0.0.6/Velkoz/data/common.py
+drwxrwxrwx   0        0        0        0 2024-04-16 21:13:35.340978 Velkoz-0.0.6/Velkoz/eye/
+-rw-rw-rw-   0        0        0      150 2024-03-23 23:06:35.000000 Velkoz-0.0.6/Velkoz/eye/__init__.py
+-rw-rw-rw-   0        0        0      523 2024-04-10 19:31:41.000000 Velkoz-0.0.6/Velkoz/eye/account.py
+-rw-rw-rw-   0        0        0      591 2024-04-09 19:37:05.000000 Velkoz-0.0.6/Velkoz/eye/champion_mastery.py
+-rw-rw-rw-   0        0        0        8 2024-03-22 13:50:02.000000 Velkoz-0.0.6/Velkoz/eye/common.py
+-rw-rw-rw-   0        0        0     7581 2024-04-12 12:51:42.000000 Velkoz-0.0.6/Velkoz/eye/match.py
+-rw-rw-rw-   0        0        0     1976 2024-04-10 19:31:40.000000 Velkoz-0.0.6/Velkoz/eye/summoner.py
+-rw-rw-rw-   0        0        0     3276 2024-04-16 15:09:23.000000 Velkoz-0.0.6/Velkoz/settings.py
+-rw-rw-rw-   0        0        0     1031 2024-04-16 21:13:18.000000 Velkoz-0.0.6/Velkoz/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 21:13:35.415203 Velkoz-0.0.6/Velkoz/supp/
+-rw-rw-rw-   0        0        0      154 2024-04-16 10:08:55.000000 Velkoz-0.0.6/Velkoz/supp/__init__.py
+-rw-rw-rw-   0        0        0      601 2024-04-10 19:50:35.000000 Velkoz-0.0.6/Velkoz/supp/account.py
+-rw-rw-rw-   0        0        0      280 2024-04-16 11:05:52.000000 Velkoz-0.0.6/Velkoz/supp/champion.py
+-rw-rw-rw-   0        0        0     1165 2024-04-11 21:19:17.000000 Velkoz-0.0.6/Velkoz/supp/champion_mastery.py
+-rw-rw-rw-   0        0        0      270 2024-04-11 21:19:18.000000 Velkoz-0.0.6/Velkoz/supp/match.py
+-rw-rw-rw-   0        0        0     1681 2024-04-10 19:50:14.000000 Velkoz-0.0.6/Velkoz/supp/summoner.py
+drwxrwxrwx   0        0        0        0 2024-04-16 21:13:35.500416 Velkoz-0.0.6/Velkoz/tentacles/
+-rw-rw-rw-   0        0        0      213 2024-04-11 21:19:17.000000 Velkoz-0.0.6/Velkoz/tentacles/__init__.py
+-rw-rw-rw-   0        0        0     1224 2024-03-22 11:07:43.000000 Velkoz-0.0.6/Velkoz/tentacles/account.py
+-rw-rw-rw-   0        0        0     3340 2024-04-11 21:19:18.000000 Velkoz-0.0.6/Velkoz/tentacles/champion_mastery.py
+-rw-rw-rw-   0        0        0     4543 2024-04-12 22:57:44.000000 Velkoz-0.0.6/Velkoz/tentacles/common.py
+-rw-rw-rw-   0        0        0       60 2024-04-05 19:09:48.000000 Velkoz-0.0.6/Velkoz/tentacles/config.py
+-rw-rw-rw-   0        0        0     1650 2024-03-22 13:51:43.000000 Velkoz-0.0.6/Velkoz/tentacles/match.py
+-rw-rw-rw-   0        0        0     1416 2024-03-22 11:06:12.000000 Velkoz-0.0.6/Velkoz/tentacles/summoner.py
+-rw-rw-rw-   0        0        0     6814 2024-04-16 21:13:06.000000 Velkoz-0.0.6/Velkoz/velkoz.py
+drwxrwxrwx   0        0        0        0 2024-04-16 21:13:35.503417 Velkoz-0.0.6/Velkoz.egg-info/
+-rw-rw-rw-   0        0        0      562 2024-04-16 21:13:35.000000 Velkoz-0.0.6/Velkoz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2024-04-16 21:13:35.000000 Velkoz-0.0.6/Velkoz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 21:13:35.000000 Velkoz-0.0.6/Velkoz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-16 21:13:35.000000 Velkoz-0.0.6/Velkoz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-16 21:13:35.000000 Velkoz-0.0.6/Velkoz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 21:13:35.504926 Velkoz-0.0.6/setup.cfg
```

### Comparing `Velkoz-0.0.59/PKG-INFO` & `Velkoz-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.59
+Version: 0.0.6
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
 Keywords: python,riotapi,api,velkoz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `Velkoz-0.0.59/Velkoz/__init__.py` & `Velkoz-0.0.6/Velkoz/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,16 @@
         get_match,
         get_all_masteries,
         get_champion_mastery,
         get_top_masteries,
         get_masteryscore,
         get_champion,
         get_champ_image,
-        get_champName_by_key
+        get_champName_by_key,
+        get_key_by_champName
 
         )
 
 from .settings import *
```

### Comparing `Velkoz-0.0.59/Velkoz/data/champion.py` & `Velkoz-0.0.6/Velkoz/data/champion.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.59/Velkoz/data/common.py` & `Velkoz-0.0.6/Velkoz/data/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
     def _get_champion_image(self, **kwargs):
         get_type = kwargs.get('get_type', 'splash')
         num = kwargs.get('num', 0)
         champ = kwargs.get('champion', 'Aatrox')
         wants_url = kwargs.get('return_url', False)
-        path = f'https://ddragon.leagueoflegends.com/cdn/img/champion/splash/{champ}_{num}.jpg'
+        path = f'https://ddragon.leagueoflegends.com/cdn/img/champion/{get_type}/{champ}_{num}.jpg'
         if wants_url == True:
             return path
         else:
             response = requests.get(path)
             return ImageLoader.open(BytesIO(response.content))
         # return data
```

### Comparing `Velkoz-0.0.59/Velkoz/eye/account.py` & `Velkoz-0.0.6/Velkoz/eye/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.59/Velkoz/eye/champion_mastery.py` & `Velkoz-0.0.6/Velkoz/eye/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.59/Velkoz/eye/match.py` & `Velkoz-0.0.6/Velkoz/eye/match.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.59/Velkoz/eye/summoner.py` & `Velkoz-0.0.6/Velkoz/eye/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.59/Velkoz/settings.py` & `Velkoz-0.0.6/Velkoz/settings.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.59/Velkoz/setup.py` & `Velkoz-0.0.6/Velkoz/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
  #python setup.py sdist bdist_wheel
-VERSION = '0.0.59' 
+VERSION = '0.0.6' 
 DESCRIPTION = 'Velkoz Riot Api package'
 LONG_DESCRIPTION = 'Package that uses RiotApi to get information.\n Made to gain experience so it is not something as advanced as the other packages that do the same. Would not recommend.'
 
 # Setting up
 setup(
         name="Velkoz", 
         version=VERSION,
```

### Comparing `Velkoz-0.0.59/Velkoz/supp/account.py` & `Velkoz-0.0.6/Velkoz/supp/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.59/Velkoz/supp/champion_mastery.py` & `Velkoz-0.0.6/Velkoz/supp/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.59/Velkoz/supp/summoner.py` & `Velkoz-0.0.6/Velkoz/supp/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.59/Velkoz/tentacles/account.py` & `Velkoz-0.0.6/Velkoz/tentacles/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.59/Velkoz/tentacles/champion_mastery.py` & `Velkoz-0.0.6/Velkoz/tentacles/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.59/Velkoz/tentacles/common.py` & `Velkoz-0.0.6/Velkoz/tentacles/common.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.59/Velkoz/tentacles/match.py` & `Velkoz-0.0.6/Velkoz/tentacles/match.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.59/Velkoz/tentacles/summoner.py` & `Velkoz-0.0.6/Velkoz/tentacles/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.59/Velkoz/velkoz.py` & `Velkoz-0.0.6/Velkoz/velkoz.py`

 * *Files 5% similar despite different names*

```diff
@@ -220,15 +220,17 @@
 
     return image
 
 
 def get_champName_by_key(champId:int):
     return all_champion_id.get(champId, None)
 
-
+def get_key_by_champName(champName:str):
+    return (list(all_champion_id.keys())[list(all_champion_id.values()).index(champName)]) 
+            
 
 #############
 # DEBUGGING #
 #############
 
 if __name__ == '__main__':
     pass
```

### Comparing `Velkoz-0.0.59/Velkoz.egg-info/PKG-INFO` & `Velkoz-0.0.6/Velkoz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.59
+Version: 0.0.6
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
 Keywords: python,riotapi,api,velkoz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `Velkoz-0.0.59/Velkoz.egg-info/SOURCES.txt` & `Velkoz-0.0.6/Velkoz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

