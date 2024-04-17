# Comparing `tmp/reviutils-1.4.0a4.tar.gz` & `tmp/reviutils-1.4.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reviutils-1.4.0a4.tar", last modified: Tue Apr 16 08:17:44 2024, max compression
+gzip compressed data, was "reviutils-1.4.0a5.tar", last modified: Tue Apr 16 09:00:59 2024, max compression
```

## Comparing `reviutils-1.4.0a4.tar` & `reviutils-1.4.0a5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.691166 reviutils-1.4.0a4/
--rw-rw-rw-   0        0        0    11558 2024-03-14 03:50:07.000000 reviutils-1.4.0a4/LICENSE
--rw-rw-rw-   0        0        0     2872 2024-04-16 08:17:44.691166 reviutils-1.4.0a4/PKG-INFO
--rw-rw-rw-   0        0        0     2546 2024-04-11 07:45:45.000000 reviutils-1.4.0a4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.650165 reviutils-1.4.0a4/reviutils/
-drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.664165 reviutils-1.4.0a4/reviutils/api/
--rw-rw-rw-   0        0        0       57 2024-03-27 06:31:11.000000 reviutils-1.4.0a4/reviutils/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.666166 reviutils-1.4.0a4/reviutils/api/amap/
--rw-rw-rw-   0        0        0     2497 2024-04-11 08:50:46.000000 reviutils-1.4.0a4/reviutils/api/amap/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-11 08:36:43.000000 reviutils-1.4.0a4/reviutils/api/amap/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.669167 reviutils-1.4.0a4/reviutils/audio/
--rw-rw-rw-   0        0        0      116 2024-03-20 03:20:30.000000 reviutils-1.4.0a4/reviutils/audio/__init__.py
--rw-rw-rw-   0        0        0     3232 2024-03-18 03:19:04.000000 reviutils-1.4.0a4/reviutils/audio/clipper.py
--rw-rw-rw-   0        0        0     1534 2024-03-20 03:42:36.000000 reviutils-1.4.0a4/reviutils/audio/reader.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.671166 reviutils-1.4.0a4/reviutils/common/
--rw-rw-rw-   0        0        0     3467 2024-03-15 02:38:48.000000 reviutils-1.4.0a4/reviutils/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.674166 reviutils-1.4.0a4/reviutils/gis/
--rw-rw-rw-   0        0        0      106 2024-04-11 06:29:44.000000 reviutils-1.4.0a4/reviutils/gis/__init__.py
--rw-rw-rw-   0        0        0     6807 2024-04-11 08:35:09.000000 reviutils-1.4.0a4/reviutils/gis/convertor.py
--rw-rw-rw-   0        0        0      558 2024-04-11 06:29:44.000000 reviutils-1.4.0a4/reviutils/gis/main.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.682166 reviutils-1.4.0a4/reviutils/noisepollution/
--rw-rw-rw-   0        0        0      314 2024-03-20 03:21:45.000000 reviutils-1.4.0a4/reviutils/noisepollution/__init__.py
--rw-rw-rw-   0        0        0     1994 2024-03-14 08:34:09.000000 reviutils-1.4.0a4/reviutils/noisepollution/evaluation.py
--rw-rw-rw-   0        0        0     4114 2024-03-19 08:00:42.000000 reviutils-1.4.0a4/reviutils/noisepollution/funcarea.py
--rw-rw-rw-   0        0        0     1043 2024-03-20 03:33:29.000000 reviutils-1.4.0a4/reviutils/noisepollution/hourhelper.py
--rw-rw-rw-   0        0        0     7313 2024-03-15 02:38:48.000000 reviutils-1.4.0a4/reviutils/noisepollution/splhelper.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.684166 reviutils-1.4.0a4/reviutils/omap/
--rw-rw-rw-   0        0        0       22 2024-04-16 08:13:41.000000 reviutils-1.4.0a4/reviutils/omap/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.685167 reviutils-1.4.0a4/reviutils/omap/constants/
--rw-rw-rw-   0        0        0     3723 2024-04-16 01:26:46.000000 reviutils-1.4.0a4/reviutils/omap/constants/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.689165 reviutils-1.4.0a4/reviutils/omap/samples/
--rw-rw-rw-   0        0        0     1131 2024-04-16 02:18:53.000000 reviutils-1.4.0a4/reviutils/omap/samples/Base.py
--rw-rw-rw-   0        0        0       19 2024-04-16 08:13:29.000000 reviutils-1.4.0a4/reviutils/omap/samples/__init__.py
--rw-rw-rw-   0        0        0    12530 2024-04-16 08:00:15.000000 reviutils-1.4.0a4/reviutils/omap/samples/main.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.662165 reviutils-1.4.0a4/reviutils.egg-info/
--rw-rw-rw-   0        0        0     2872 2024-04-16 08:17:44.000000 reviutils-1.4.0a4/reviutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      843 2024-04-16 08:17:44.000000 reviutils-1.4.0a4/reviutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 08:17:44.000000 reviutils-1.4.0a4/reviutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 08:17:44.000000 reviutils-1.4.0a4/reviutils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       91 2024-04-16 08:17:44.000000 reviutils-1.4.0a4/reviutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-16 08:17:44.000000 reviutils-1.4.0a4/reviutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 08:17:44.692165 reviutils-1.4.0a4/setup.cfg
--rw-rw-rw-   0        0        0     1688 2024-04-16 08:17:24.000000 reviutils-1.4.0a4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:00:59.760003 reviutils-1.4.0a5/
+-rw-rw-rw-   0        0        0    11558 2024-03-14 03:50:07.000000 reviutils-1.4.0a5/LICENSE
+-rw-rw-rw-   0        0        0     2872 2024-04-16 09:00:59.759003 reviutils-1.4.0a5/PKG-INFO
+-rw-rw-rw-   0        0        0     2546 2024-04-11 07:45:45.000000 reviutils-1.4.0a5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 09:00:59.719003 reviutils-1.4.0a5/reviutils/
+drwxrwxrwx   0        0        0        0 2024-04-16 09:00:59.732004 reviutils-1.4.0a5/reviutils/api/
+-rw-rw-rw-   0        0        0       57 2024-03-27 06:31:11.000000 reviutils-1.4.0a5/reviutils/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:00:59.735004 reviutils-1.4.0a5/reviutils/api/amap/
+-rw-rw-rw-   0        0        0     2497 2024-04-11 08:50:46.000000 reviutils-1.4.0a5/reviutils/api/amap/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-11 08:36:43.000000 reviutils-1.4.0a5/reviutils/api/amap/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:00:59.739005 reviutils-1.4.0a5/reviutils/audio/
+-rw-rw-rw-   0        0        0      116 2024-03-20 03:20:30.000000 reviutils-1.4.0a5/reviutils/audio/__init__.py
+-rw-rw-rw-   0        0        0     3232 2024-03-18 03:19:04.000000 reviutils-1.4.0a5/reviutils/audio/clipper.py
+-rw-rw-rw-   0        0        0     1534 2024-03-20 03:42:36.000000 reviutils-1.4.0a5/reviutils/audio/reader.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:00:59.740005 reviutils-1.4.0a5/reviutils/common/
+-rw-rw-rw-   0        0        0     3467 2024-03-15 02:38:48.000000 reviutils-1.4.0a5/reviutils/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:00:59.744004 reviutils-1.4.0a5/reviutils/gis/
+-rw-rw-rw-   0        0        0      106 2024-04-11 06:29:44.000000 reviutils-1.4.0a5/reviutils/gis/__init__.py
+-rw-rw-rw-   0        0        0     6807 2024-04-11 08:35:09.000000 reviutils-1.4.0a5/reviutils/gis/convertor.py
+-rw-rw-rw-   0        0        0      558 2024-04-11 06:29:44.000000 reviutils-1.4.0a5/reviutils/gis/main.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:00:59.751004 reviutils-1.4.0a5/reviutils/noisepollution/
+-rw-rw-rw-   0        0        0      314 2024-03-20 03:21:45.000000 reviutils-1.4.0a5/reviutils/noisepollution/__init__.py
+-rw-rw-rw-   0        0        0     1994 2024-03-14 08:34:09.000000 reviutils-1.4.0a5/reviutils/noisepollution/evaluation.py
+-rw-rw-rw-   0        0        0     4114 2024-03-19 08:00:42.000000 reviutils-1.4.0a5/reviutils/noisepollution/funcarea.py
+-rw-rw-rw-   0        0        0     1043 2024-03-20 03:33:29.000000 reviutils-1.4.0a5/reviutils/noisepollution/hourhelper.py
+-rw-rw-rw-   0        0        0     7313 2024-03-15 02:38:48.000000 reviutils-1.4.0a5/reviutils/noisepollution/splhelper.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:00:59.753005 reviutils-1.4.0a5/reviutils/omap/
+-rw-rw-rw-   0        0        0       22 2024-04-16 08:13:41.000000 reviutils-1.4.0a5/reviutils/omap/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:00:59.754003 reviutils-1.4.0a5/reviutils/omap/constants/
+-rw-rw-rw-   0        0        0     3723 2024-04-16 01:26:46.000000 reviutils-1.4.0a5/reviutils/omap/constants/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:00:59.758003 reviutils-1.4.0a5/reviutils/omap/samples/
+-rw-rw-rw-   0        0        0     1131 2024-04-16 02:18:53.000000 reviutils-1.4.0a5/reviutils/omap/samples/Base.py
+-rw-rw-rw-   0        0        0       19 2024-04-16 08:13:29.000000 reviutils-1.4.0a5/reviutils/omap/samples/__init__.py
+-rw-rw-rw-   0        0        0    12592 2024-04-16 08:42:36.000000 reviutils-1.4.0a5/reviutils/omap/samples/main.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:00:59.731003 reviutils-1.4.0a5/reviutils.egg-info/
+-rw-rw-rw-   0        0        0     2872 2024-04-16 09:00:59.000000 reviutils-1.4.0a5/reviutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      843 2024-04-16 09:00:59.000000 reviutils-1.4.0a5/reviutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 09:00:59.000000 reviutils-1.4.0a5/reviutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 09:00:59.000000 reviutils-1.4.0a5/reviutils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       91 2024-04-16 09:00:59.000000 reviutils-1.4.0a5/reviutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-16 09:00:59.000000 reviutils-1.4.0a5/reviutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 09:00:59.760003 reviutils-1.4.0a5/setup.cfg
+-rw-rw-rw-   0        0        0     1688 2024-04-16 09:00:56.000000 reviutils-1.4.0a5/setup.py
```

### Comparing `reviutils-1.4.0a4/LICENSE` & `reviutils-1.4.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a4/PKG-INFO` & `reviutils-1.4.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviutils
-Version: 1.4.0a4
+Version: 1.4.0a5
 Summary: A common library frequently used on python
 Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI
 Author-email: reviy-top@outlook.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: audio
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reviutils Version: 1.4.0a4 Summary: A common
+Metadata-Version: 2.1 Name: reviutils Version: 1.4.0a5 Summary: A common
 library frequently used on python Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
 Description-Content-Type: text/markdown Provides-Extra: audio License-File:
 LICENSE
                             ************ rreevviiuuttiillss ************
                            ä¸ä¸ªå¸¸ç¨çPythonåº
                             _ç_®__ä_½__ä_¸_­_æ__ï½ _E_n_g_l_i_s_h
```

### Comparing `reviutils-1.4.0a4/README.md` & `reviutils-1.4.0a5/README.md`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a4/reviutils/api/amap/__init__.py` & `reviutils-1.4.0a5/reviutils/api/amap/__init__.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a4/reviutils/audio/clipper.py` & `reviutils-1.4.0a5/reviutils/audio/clipper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a4/reviutils/audio/reader.py` & `reviutils-1.4.0a5/reviutils/audio/reader.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a4/reviutils/common/__init__.py` & `reviutils-1.4.0a5/reviutils/common/__init__.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a4/reviutils/gis/convertor.py` & `reviutils-1.4.0a5/reviutils/gis/convertor.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a4/reviutils/gis/main.py` & `reviutils-1.4.0a5/reviutils/gis/main.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a4/reviutils/noisepollution/evaluation.py` & `reviutils-1.4.0a5/reviutils/noisepollution/evaluation.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a4/reviutils/noisepollution/funcarea.py` & `reviutils-1.4.0a5/reviutils/noisepollution/funcarea.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a4/reviutils/noisepollution/hourhelper.py` & `reviutils-1.4.0a5/reviutils/noisepollution/hourhelper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a4/reviutils/noisepollution/splhelper.py` & `reviutils-1.4.0a5/reviutils/noisepollution/splhelper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a4/reviutils/omap/constants/__init__.py` & `reviutils-1.4.0a5/reviutils/omap/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a4/reviutils/omap/samples/Base.py` & `reviutils-1.4.0a5/reviutils/omap/samples/Base.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a4/reviutils/omap/samples/main.py` & `reviutils-1.4.0a5/reviutils/omap/samples/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,21 +183,23 @@
 class Text(ItemBase):
     def __init__(
         self,
         name: str,
         lng: float,
         lat: float,
         is_gcj02: bool,
+        font_size:int = 16,
         color: Colors = Colors.Default,
         rotation: int = 0,
         parent_id: int = 1,
     ):
         extinfo = ExtInfoObject(
             FontClr=color.value.id,
-            FontRotateAngle=rotation
+            FontRotateAngle=rotation,
+            FontSize=font_size
         )
         detail = TextDetail(Lng=lng, Lat=lat, Gcj02=is_gcj02, ExtInfo=extinfo)
         obj = ObjectBase(
             name=name, obj_detail=detail, type_id=ObjectTypes.Point.value.id
         )
         super().__init__(
             obj=obj,
```

### Comparing `reviutils-1.4.0a4/reviutils.egg-info/PKG-INFO` & `reviutils-1.4.0a5/reviutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviutils
-Version: 1.4.0a4
+Version: 1.4.0a5
 Summary: A common library frequently used on python
 Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI
 Author-email: reviy-top@outlook.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: audio
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reviutils Version: 1.4.0a4 Summary: A common
+Metadata-Version: 2.1 Name: reviutils Version: 1.4.0a5 Summary: A common
 library frequently used on python Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
 Description-Content-Type: text/markdown Provides-Extra: audio License-File:
 LICENSE
                             ************ rreevviiuuttiillss ************
                            ä¸ä¸ªå¸¸ç¨çPythonåº
                             _ç_®__ä_½__ä_¸_­_æ__ï½ _E_n_g_l_i_s_h
```

### Comparing `reviutils-1.4.0a4/reviutils.egg-info/SOURCES.txt` & `reviutils-1.4.0a5/reviutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a4/setup.py` & `reviutils-1.4.0a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                 del_pycache(os.path.join(root, dir))
 
 
 del_pycache("reviutils")  # 删除reviutils下的每个子文件夹的__pycache__文件夹
 
 setup(
     name="reviutils",
-    version="1.4.0a4",
+    version="1.4.0a5",
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="A common library frequently used on python",
     url="https://github.com/Viyyy/viutils",
     author="Re.VI",
     author_email="reviy-top@outlook.com",
     license="Apache License 2.0",
```

