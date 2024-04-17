# Comparing `tmp/geodynamic-0.0.5.tar.gz` & `tmp/geodynamic-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodynamic-0.0.5.tar", last modified: Mon Apr 15 15:43:39 2024, max compression
+gzip compressed data, was "geodynamic-0.0.6.tar", last modified: Wed Apr 17 10:50:39 2024, max compression
```

## Comparing `geodynamic-0.0.5.tar` & `geodynamic-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-15 15:43:39.168465 geodynamic-0.0.5/
--rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.5/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-15 15:43:39.168392 geodynamic-0.0.5/PKG-INFO
--rw-------   0 mac        (501) staff       (20)      415 2024-04-09 12:57:37.000000 geodynamic-0.0.5/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-15 15:43:39.162651 geodynamic-0.0.5/geodynamic/
--rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.5/geodynamic/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-15 15:43:39.165729 geodynamic-0.0.5/geodynamic/geo/
--rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.5/geodynamic/geo/__init__.py
--rw-------   0 mac        (501) staff       (20)    10547 2024-04-13 15:38:56.000000 geodynamic-0.0.5/geodynamic/geo/construction.py
--rw-------   0 mac        (501) staff       (20)    24312 2024-04-15 15:34:01.000000 geodynamic-0.0.5/geodynamic/geo/lib_commands.py
--rw-------   0 mac        (501) staff       (20)    12974 2024-04-13 14:52:57.000000 geodynamic-0.0.5/geodynamic/geo/lib_elements.py
--rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.5/geodynamic/geo/lib_vars.py
--rw-------   0 mac        (501) staff       (20)    30062 2024-04-15 14:48:54.000000 geodynamic-0.0.5/geodynamic/manim_dynamic.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-15 15:43:39.167544 geodynamic-0.0.5/geodynamic/parsers/
--rw-rw-r--   0 mac        (501) staff       (20)      411 2024-04-08 16:07:59.000000 geodynamic-0.0.5/geodynamic/parsers/__init__.py
--rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.5/geodynamic/parsers/ggb_generator.py
--rw-------   0 mac        (501) staff       (20)     7314 2024-04-15 15:20:08.000000 geodynamic-0.0.5/geodynamic/parsers/ggb_parser.py
--rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.5/geodynamic/parsers/short_parser.py
--rw-rw-r--   0 mac        (501) staff       (20)     6043 2024-04-09 12:06:03.000000 geodynamic-0.0.5/geodynamic/parsers/svg_parser.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-15 15:43:39.168103 geodynamic-0.0.5/geodynamic.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-15 15:43:39.000000 geodynamic-0.0.5/geodynamic.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      575 2024-04-15 15:43:39.000000 geodynamic-0.0.5/geodynamic.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-15 15:43:39.000000 geodynamic-0.0.5/geodynamic.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       60 2024-04-15 15:43:39.000000 geodynamic-0.0.5/geodynamic.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-15 15:43:39.000000 geodynamic-0.0.5/geodynamic.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-15 15:43:39.168777 geodynamic-0.0.5/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      951 2024-04-15 15:42:42.000000 geodynamic-0.0.5/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-17 10:50:39.565636 geodynamic-0.0.6/
+-rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.6/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-17 10:50:39.565562 geodynamic-0.0.6/PKG-INFO
+-rw-------   0 mac        (501) staff       (20)      415 2024-04-09 12:57:37.000000 geodynamic-0.0.6/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-17 10:50:39.559301 geodynamic-0.0.6/geodynamic/
+-rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.6/geodynamic/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-17 10:50:39.562104 geodynamic-0.0.6/geodynamic/geo/
+-rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.6/geodynamic/geo/__init__.py
+-rw-------   0 mac        (501) staff       (20)    10547 2024-04-13 15:38:56.000000 geodynamic-0.0.6/geodynamic/geo/construction.py
+-rw-------   0 mac        (501) staff       (20)    24312 2024-04-15 15:34:01.000000 geodynamic-0.0.6/geodynamic/geo/lib_commands.py
+-rw-------   0 mac        (501) staff       (20)    12974 2024-04-13 14:52:57.000000 geodynamic-0.0.6/geodynamic/geo/lib_elements.py
+-rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.6/geodynamic/geo/lib_vars.py
+-rw-------   0 mac        (501) staff       (20)    31572 2024-04-17 10:49:55.000000 geodynamic-0.0.6/geodynamic/manim_dynamic.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-17 10:50:39.564345 geodynamic-0.0.6/geodynamic/parsers/
+-rw-rw-r--   0 mac        (501) staff       (20)      411 2024-04-08 16:07:59.000000 geodynamic-0.0.6/geodynamic/parsers/__init__.py
+-rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.6/geodynamic/parsers/ggb_generator.py
+-rw-------   0 mac        (501) staff       (20)     7314 2024-04-15 15:20:08.000000 geodynamic-0.0.6/geodynamic/parsers/ggb_parser.py
+-rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.6/geodynamic/parsers/short_parser.py
+-rw-rw-r--   0 mac        (501) staff       (20)     6043 2024-04-09 12:06:03.000000 geodynamic-0.0.6/geodynamic/parsers/svg_parser.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-17 10:50:39.565091 geodynamic-0.0.6/geodynamic.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-17 10:50:39.000000 geodynamic-0.0.6/geodynamic.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      575 2024-04-17 10:50:39.000000 geodynamic-0.0.6/geodynamic.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-17 10:50:39.000000 geodynamic-0.0.6/geodynamic.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       60 2024-04-17 10:50:39.000000 geodynamic-0.0.6/geodynamic.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-17 10:50:39.000000 geodynamic-0.0.6/geodynamic.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-17 10:50:39.566226 geodynamic-0.0.6/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      951 2024-04-17 10:50:27.000000 geodynamic-0.0.6/setup.py
```

### Comparing `geodynamic-0.0.5/PKG-INFO` & `geodynamic-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.5
+Version: 0.0.6
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geodynamic-0.0.5/geodynamic/geo/construction.py` & `geodynamic-0.0.6/geodynamic/geo/construction.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.5/geodynamic/geo/lib_commands.py` & `geodynamic-0.0.6/geodynamic/geo/lib_commands.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.5/geodynamic/geo/lib_elements.py` & `geodynamic-0.0.6/geodynamic/geo/lib_elements.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.5/geodynamic/geo/lib_vars.py` & `geodynamic-0.0.6/geodynamic/geo/lib_vars.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.5/geodynamic/manim_dynamic.py` & `geodynamic-0.0.6/geodynamic/manim_dynamic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import json
 import numpy as np
 
 from .geo import construction as geo
 from manim import *
 from .parsers.svg_parser import *
 from .parsers import short_parser, ggb_parser
 
@@ -39,37 +40,56 @@
 style_pandora['color']['black'] = '#000000'
 style_pandora['color']['main'] = '#2581b5'
 style_pandora['color']['light'] = '#bef3fc'
 style_pandora['color']['aux'] = '#000000'
 style_pandora['color']['acc'] = '#ef60ab'
 style_pandora['color']['acc_light'] = '#ffd2ee'
 
+def isnan(x):
+    if isinstance(x, str):
+        try:
+            y = float(x)
+            return False
+        except:
+            return True
+    else:
+        return not isinstance(x, (int, float))
+
 def CorrectSVG(svg_path):
     #tree = ET.parse(svg_path)
 
     #for elem in tree.findall(f'.//{xmlns}text'):
     #    elem.set('font-style', 'italic')
 
     #tree.write(svg_path, encoding = "UTF-8", xml_declaration = False)
     return
 
 class GeoStyle:
-    def __init__(self, scheme = 'book', color = 'blue', theme = 'light', px_size = [1920, 1080]):
+    def __init__(self, style_json_file = None, scheme = None, color = 'blue', theme = 'light', px_size = [1920, 1080], crop_padding = None):
         self.dot_size = 0.17   
         self.line_width = 6   
         self.ang_width = 0.75 * self.line_width
         self.strich_rshift = 0.14
         self.ang_rshift = 0.75 * self.strich_rshift
         self.strich_len = 0.45
         self.strich_width = 6
         self.ang_rdefault = 0.8
         self.ang_right = 0.65
         
         self.background = WHITE
         self.strong = BLACK
+        
+        if style_json_file is not None:
+            style_json = json.loads(open(style_json_file, 'r').read())
+            scheme = style_json['name']
+            
+            if scheme == 'pandora':
+                global style_pandora
+                style_pandora = style_json['style']
+                #print(style_pandora)
 
         if scheme == 'pandora':            
             self.convert_pandora_to_manim()
             
         else:
             if theme == 'dark':
                 self.background = BLACK
@@ -137,34 +157,45 @@
         
         self.background = '#ffffff'
         self.col = style_pandora['color']['main']
         self.col_light = style_pandora['color']['light']
         self.col_accent = style_pandora['color']['acc']
         self.col_accent_light = style_pandora['color']['acc_light']
         self.col_gray = '#eeeeee'
-        
+
     def setViewByGeo(self, geoView):
         w0, h0 = self.view['width'], self.view['height']
         w, h = geoView['width'], geoView['height']
+        if isnan(w0) & isnan(h0): 
+            print("ERROR: width and heigth haven't been set")
+        elif isnan(w0):
+            #print(w0, h0, w, h)
+            w0 = float(h0) * w / h
+            self.view['width'] = w0
+        elif isnan(h0):
+            #print(w0, h0, w, h)
+            h0 = float(w0) * h / w
+            self.view['height'] = h0
+            
         q = min(w0/w, h0/h)
         
         self.view['scale'] = geoView['scale'] * q
         self.view['xZero'] = geoView['xZero'] * q + (w0 - q * w) / 2
         self.view['yZero'] = geoView['yZero'] * q + (h0 - q * h) / 2
 
 #--------------------------------------------------------------------------
 
 class GeoDynamic(MovingCameraScene):
-    style_default = GeoStyle('purple', 'dark')
+    style_default = GeoStyle(color = 'blue', theme = 'light')
 
     def __init__(self):
         super().__init__()
         self.obj = {}                       #хранение объектов сцены mobjects obj[name] = MObject
         self.geo = geo.Construction()
-        self.style = GeoStyle('blue')
+        self.style = GeoStyle(color = 'blue')
 
         self._styles_back = {}
         self._gray_mobjects = {}
 
         self.cuts = 0
 
     def mobject(self, name):
@@ -193,14 +224,24 @@
             [geo.Circle, geo.Arc, geo.Segment],
             [geo.Point]
         ]
 
         for el_types in element_types:
             for el in self.geo.elements: 
                 if type(el.data) in el_types: self.addGeoElement(el, show) 
+ 
+    def getAllGeometryBounds(self):
+        bounds = [None,None,None,None]
+        for elem in self.geo.elements: 
+            if elem.visible:
+                mobj = CreateMObject(elem, z_auto = True)
+                if mobj is not None:
+                    #!здесь нужно проверить границы элемента и расширить bounds по необходимости
+                    x = 0
+                    
 
     #пауза для обрезки видео + отображение ярлыка слева
     def waitCut(self, msg = None, **kwargs):
         self.cuts += 1
 
         rect = Rectangle(color = RED, fill_opacity = 1, height = self.camera.frame_height, width = self.camera.frame_width/4).move_to(self.camera.frame_center).shift( (3/8) * self.camera.frame_width * LEFT)
         txt = Text(str(msg) if msg is not None else str(self.cuts)).set_color(BLACK).scale(3).move_to(rect)
@@ -243,31 +284,32 @@
             if not el.visible: 
                 mobj.set_opacity(0)
 
     def loadGeometry(self, filepath, update = False, debug = False):
         short_parser.loadCode(self.geo, filepath, update = update, debug = debug)
         self.geo.rebuild(debug = debug)
 
-    def loadGeoGebra(self, filepath, scheme = 'pandora', px_size = None, update = False, debug = False):
+    def loadGeoGebra(self, filepath, style_json_file = None, scheme = 'pandora', px_size = None, crop_padding = None, debug = False):
         self.geo = ggb_parser.load(filepath, debug = debug) 
         self.geo.rebuild(debug = debug)
         
-        style = GeoStyle(scheme = scheme, px_size = px_size)
+        style = GeoStyle(style_json_file = style_json_file, scheme = scheme, px_size = px_size, crop_padding = crop_padding)
+        
+        if crop_padding is not None:
+            print('This method is going to be realized soon.')    
         
         if px_size is not None:
             style.setViewByGeo(self.geo.style['view'])
         else:
             style.view = self.geo.style['view']
 
         view = style.view
         scale = view['scale']
         for key in ['dot_size', 'line_width', 'ang_width', 'ang_rdefault', 'ang_right', 'ang_rshift', 'strich_rshift', 'strich_len']:
-            print(f'{key} BEFORE: {getattr(style, key)}')
             style.__setattr__(key, getattr(style, key) * 50 / scale)
-            print(f'{key} AFTER: {getattr(style, key)}')
 
         self.camera.frame.set(width = view['width'] / scale)
         dx = self.camera.frame.width / 2 - view['xZero'] / scale
         dy = view['height'] / (2 * scale) - view['yZero'] / scale      
         self.camera.frame.shift(dx * RIGHT + dy * DOWN)
 
         self.setStyle(style)
```

### Comparing `geodynamic-0.0.5/geodynamic/parsers/ggb_generator.py` & `geodynamic-0.0.6/geodynamic/parsers/ggb_generator.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.5/geodynamic/parsers/ggb_parser.py` & `geodynamic-0.0.6/geodynamic/parsers/ggb_parser.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.5/geodynamic/parsers/short_parser.py` & `geodynamic-0.0.6/geodynamic/parsers/short_parser.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.5/geodynamic/parsers/svg_parser.py` & `geodynamic-0.0.6/geodynamic/parsers/svg_parser.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.5/geodynamic.egg-info/PKG-INFO` & `geodynamic-0.0.6/geodynamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.5
+Version: 0.0.6
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geodynamic-0.0.5/geodynamic.egg-info/SOURCES.txt` & `geodynamic-0.0.6/geodynamic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.5/setup.py` & `geodynamic-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='geodynamic',
-  version='0.0.5',
+  version='0.0.6',
   author='ivaleo',
   author_email='ivaleotion@gmail.com',
   description='Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://gitlab.mathem.ru/',
   packages=find_packages(),
```

