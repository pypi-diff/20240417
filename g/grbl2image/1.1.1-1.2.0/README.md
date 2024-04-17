# Comparing `tmp/grbl2image-1.1.1.tar.gz` & `tmp/grbl2image-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grbl2image-1.1.1.tar", last modified: Fri Apr 21 13:13:43 2023, max compression
+gzip compressed data, was "grbl2image-1.2.0.tar", last modified: Wed Apr 17 09:12:03 2024, max compression
```

## Comparing `grbl2image-1.1.1.tar` & `grbl2image-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2023-04-21 13:13:43.870754 grbl2image-1.1.1/
--rw-rw-r--   0 alan      (1000) alan      (1000)     1070 2023-04-17 08:15:45.000000 grbl2image-1.1.1/LICENSE
--rw-rw-r--   0 alan      (1000) alan      (1000)     4523 2023-04-21 13:13:43.870754 grbl2image-1.1.1/PKG-INFO
--rw-rw-r--   0 alan      (1000) alan      (1000)     3880 2023-04-21 13:12:19.000000 grbl2image-1.1.1/README.md
--rw-rw-r--   0 alan      (1000) alan      (1000)      742 2023-04-21 13:13:06.000000 grbl2image-1.1.1/pyproject.toml
--rw-rw-r--   0 alan      (1000) alan      (1000)       38 2023-04-21 13:13:43.870754 grbl2image-1.1.1/setup.cfg
-drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2023-04-21 13:13:43.866754 grbl2image-1.1.1/src/
-drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2023-04-21 13:13:43.866754 grbl2image-1.1.1/src/grbl2image/
--rw-rw-r--   0 alan      (1000) alan      (1000)        0 2023-04-21 05:24:54.000000 grbl2image-1.1.1/src/grbl2image/__init__.py
--rw-rw-r--   0 alan      (1000) alan      (1000)     6336 2023-04-21 13:05:52.000000 grbl2image-1.1.1/src/grbl2image/grbl2image.py
-drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2023-04-21 13:13:43.870754 grbl2image-1.1.1/src/grbl2image.egg-info/
--rw-rw-r--   0 alan      (1000) alan      (1000)     4523 2023-04-21 13:13:43.000000 grbl2image-1.1.1/src/grbl2image.egg-info/PKG-INFO
--rw-rw-r--   0 alan      (1000) alan      (1000)      331 2023-04-21 13:13:43.000000 grbl2image-1.1.1/src/grbl2image.egg-info/SOURCES.txt
--rw-rw-r--   0 alan      (1000) alan      (1000)        1 2023-04-21 13:13:43.000000 grbl2image-1.1.1/src/grbl2image.egg-info/dependency_links.txt
--rw-rw-r--   0 alan      (1000) alan      (1000)       12 2023-04-21 13:13:43.000000 grbl2image-1.1.1/src/grbl2image.egg-info/requires.txt
--rw-rw-r--   0 alan      (1000) alan      (1000)       11 2023-04-21 13:13:43.000000 grbl2image-1.1.1/src/grbl2image.egg-info/top_level.txt
-drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2023-04-21 13:13:43.870754 grbl2image-1.1.1/tests/
--rw-rw-r--   0 alan      (1000) alan      (1000)      774 2023-04-21 12:54:56.000000 grbl2image-1.1.1/tests/tests.py
--rw-rw-r--   0 alan      (1000) alan      (1000)      758 2023-04-21 13:04:07.000000 grbl2image-1.1.1/tests/tests_all.py
--rw-rw-r--   0 alan      (1000) alan      (1000)      679 2023-04-21 13:06:56.000000 grbl2image-1.1.1/tests/tests_size.py
+drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2024-04-17 09:12:03.802031 grbl2image-1.2.0/
+-rw-rw-r--   0 alan      (1000) alan      (1000)     1070 2023-04-17 08:15:45.000000 grbl2image-1.2.0/LICENSE
+-rw-r--r--   0 alan      (1000) alan      (1000)     5092 2024-04-17 09:12:03.798031 grbl2image-1.2.0/PKG-INFO
+-rw-rw-r--   0 alan      (1000) alan      (1000)     4422 2024-04-17 09:00:23.000000 grbl2image-1.2.0/README.md
+-rw-rw-r--   0 alan      (1000) alan      (1000)      742 2024-04-17 09:04:38.000000 grbl2image-1.2.0/pyproject.toml
+-rw-rw-r--   0 alan      (1000) alan      (1000)       38 2024-04-17 09:12:03.802031 grbl2image-1.2.0/setup.cfg
+drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2024-04-17 09:12:03.798031 grbl2image-1.2.0/src/
+drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2024-04-17 09:12:03.798031 grbl2image-1.2.0/src/grbl2image/
+-rw-rw-r--   0 alan      (1000) alan      (1000)        0 2023-04-21 05:24:54.000000 grbl2image-1.2.0/src/grbl2image/__init__.py
+-rw-rw-r--   0 alan      (1000) alan      (1000)     7663 2024-04-17 08:55:27.000000 grbl2image-1.2.0/src/grbl2image/grbl2image.py
+drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2024-04-17 09:12:03.798031 grbl2image-1.2.0/src/grbl2image.egg-info/
+-rw-r--r--   0 alan      (1000) alan      (1000)     5092 2024-04-17 09:12:03.000000 grbl2image-1.2.0/src/grbl2image.egg-info/PKG-INFO
+-rw-rw-r--   0 alan      (1000) alan      (1000)      331 2024-04-17 09:12:03.000000 grbl2image-1.2.0/src/grbl2image.egg-info/SOURCES.txt
+-rw-rw-r--   0 alan      (1000) alan      (1000)        1 2024-04-17 09:12:03.000000 grbl2image-1.2.0/src/grbl2image.egg-info/dependency_links.txt
+-rw-rw-r--   0 alan      (1000) alan      (1000)       12 2024-04-17 09:12:03.000000 grbl2image-1.2.0/src/grbl2image.egg-info/requires.txt
+-rw-rw-r--   0 alan      (1000) alan      (1000)       11 2024-04-17 09:12:03.000000 grbl2image-1.2.0/src/grbl2image.egg-info/top_level.txt
+drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2024-04-17 09:12:03.798031 grbl2image-1.2.0/tests/
+-rw-rw-r--   0 alan      (1000) alan      (1000)      774 2024-04-17 08:54:22.000000 grbl2image-1.2.0/tests/tests.py
+-rw-rw-r--   0 alan      (1000) alan      (1000)      767 2024-04-17 09:00:41.000000 grbl2image-1.2.0/tests/tests_all.py
+-rw-rw-r--   0 alan      (1000) alan      (1000)      679 2023-04-21 13:06:56.000000 grbl2image-1.2.0/tests/tests_size.py
```

### Comparing `grbl2image-1.1.1/LICENSE` & `grbl2image-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grbl2image-1.1.1/PKG-INFO` & `grbl2image-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: grbl2image
-Version: 1.1.1
+Version: 1.2.0
 Summary: Generates an image (PNG, JPEG, etc.) from a GRBL file (.NC, .GC, ...) in Python using pillow (python3)
 Author: AlanFromJapan
 Project-URL: Homepage, https://github.com/AlanFromJapan/grbl2image
 Project-URL: Bug Tracker, https://github.com/AlanFromJapan/grbl2image/issues
 Project-URL: Parent project, https://github.com/AlanFromJapan/GrblWebStreamer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Pillow>=9.0
 
 # grbl2image
 Generates an **image** (PNG, JPEG, etc.) from a **GRBL** file (.NC, .GC, ...), in Python using pillow (python3 PIL fork). It is to be used as a reusable standalone component, initially for the **parent project [GRBL WebStreamer](https://github.com/AlanFromJapan/GrblWebStreamer)** that is a webinterface for laser cutters running on Raspi or similar SBC.
 
 ![Turns GRBL code into PNG](https://github.com/AlanFromJapan/grbl2image/blob/main/grbl2image.png?raw=true)
 
 The target is to generate a simply a top view of a GRBL job for my Laser (see *limitations* below). As of now only a subset of the GRBL commands are recognized, and more will be added along the way when their need arise. This is not meant to be the complete solution for all GRBL files, but I'll be taking requests on GitHub so don't hesitate. 
 
 ## What it does
 - [x] Generates image from a GRBL file for a Laser job
 - [x] Calculates estimated bounds of the job
+- [x] Supports color blending for "greyscale" jobs 
 - [ ] Calculates an estimated time of completion of the job
 
 ## Limitations 
 This is made to support a ***laser*** cutter/engraver, *not CNC*, and this is out of scope even of the end scope of library. There are already good solutions that handle the 3D component of your CNC. This is just a top view of a GRBL file, so if it works with yours CNC good for you!
 
 Therefore GRBL codes that don't make sense for a laser will be ignored and not implemented, but if you have time fork this project!
 
@@ -89,10 +91,27 @@
 
 #final flip because the image 0,0 is top left and for us human it's at the bottom left
 img = img.transpose(Image.FLIP_TOP_BOTTOM)
 
 #save
 img.save("laser_job_001.png")
 ```
+
+### Customize the rendering
+```python
+import grbl2image.grbl2image as G2I
+from PIL import Image
+
+# don't blend, just laser ON/OFF : makes you see the whole work but make greyscale images a big blotch
+G2I.NO_BLENDING = True
+# change default background color
+G2I.BG_COLOR = "whitesmoke"
+
+#Generate the PIL Image object based on sample code and overwrite the default values
+img, _ = G2I.processFile("sample.gcode/Test gcode 1.nc", color="blue", bg_color="yellow", noblending=False)
+
+...
+```
+
 ## Source code
 - Source is MIT licensed on GitHub : https://github.com/AlanFromJapan/grbl2image
 - Parent project [GRBL WebStreamer](https://github.com/AlanFromJapan/GrblWebStreamer) is also on GitHub under MIT license
```

### Comparing `grbl2image-1.1.1/README.md` & `grbl2image-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 ![Turns GRBL code into PNG](https://github.com/AlanFromJapan/grbl2image/blob/main/grbl2image.png?raw=true)
 
 The target is to generate a simply a top view of a GRBL job for my Laser (see *limitations* below). As of now only a subset of the GRBL commands are recognized, and more will be added along the way when their need arise. This is not meant to be the complete solution for all GRBL files, but I'll be taking requests on GitHub so don't hesitate. 
 
 ## What it does
 - [x] Generates image from a GRBL file for a Laser job
 - [x] Calculates estimated bounds of the job
+- [x] Supports color blending for "greyscale" jobs 
 - [ ] Calculates an estimated time of completion of the job
 
 ## Limitations 
 This is made to support a ***laser*** cutter/engraver, *not CNC*, and this is out of scope even of the end scope of library. There are already good solutions that handle the 3D component of your CNC. This is just a top view of a GRBL file, so if it works with yours CNC good for you!
 
 Therefore GRBL codes that don't make sense for a laser will be ignored and not implemented, but if you have time fork this project!
 
@@ -74,10 +75,27 @@
 
 #final flip because the image 0,0 is top left and for us human it's at the bottom left
 img = img.transpose(Image.FLIP_TOP_BOTTOM)
 
 #save
 img.save("laser_job_001.png")
 ```
+
+### Customize the rendering
+```python
+import grbl2image.grbl2image as G2I
+from PIL import Image
+
+# don't blend, just laser ON/OFF : makes you see the whole work but make greyscale images a big blotch
+G2I.NO_BLENDING = True
+# change default background color
+G2I.BG_COLOR = "whitesmoke"
+
+#Generate the PIL Image object based on sample code and overwrite the default values
+img, _ = G2I.processFile("sample.gcode/Test gcode 1.nc", color="blue", bg_color="yellow", noblending=False)
+
+...
+```
+
 ## Source code
 - Source is MIT licensed on GitHub : https://github.com/AlanFromJapan/grbl2image
 - Parent project [GRBL WebStreamer](https://github.com/AlanFromJapan/GrblWebStreamer) is also on GitHub under MIT license
```

### Comparing `grbl2image-1.1.1/pyproject.toml` & `grbl2image-1.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "grbl2image"
-version = "1.1.1"
+version = "1.2.0"
 authors = [
   { name="AlanFromJapan" },
 ]
 description = "Generates an image (PNG, JPEG, etc.) from a GRBL file (.NC, .GC, ...) in Python using pillow (python3)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `grbl2image-1.1.1/src/grbl2image/grbl2image.py` & `grbl2image-1.2.0/src/grbl2image/grbl2image.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os, io
 import re
 from enum import Enum, auto
 
 from PIL import Image
 from PIL import ImageDraw
-from PIL import ImageFont
+from PIL import ImageColor
 
 PIXELS_PER_MM = 10
 AREA_W_MM = 200
 AREA_H_MM = 200
+BG_COLOR = (255,255,255,255)
+NO_BLENDING = False #if True, the laser power will be ignored and the line will be drawn without alpha blending (ON/OFF mode)
 
 DEBUG=False
 
 class PositionsCalculation(Enum):
     ABSOLUTE = auto()
     RELATIVE = auto()
 
@@ -21,39 +23,42 @@
 r = re.compile(GRBL_REGEX)
 
 
 #laser with its coordinates in REAL world (assume MM unit)
 class Laser:
     X = 0.0
     Y = 0.0
-    PowerOn = False
+    Power = 0.0 #[0..100]
     positionsCalculation = PositionsCalculation.ABSOLUTE
 
-    def __init__(self, x=0.0, y=0.0, power=False) -> None:
+    def __init__(self, x=0.0, y=0.0, power=0.0) -> None:
         self.X = x
         self.Y = y
-        self.PowerOn = power
+        self.Power = power
         self.positionsCalculation = PositionsCalculation.ABSOLUTE
 
     def fromLaser(template:"Laser") -> "Laser":
         newLaser = Laser()
         newLaser.X = template.X
         newLaser.Y = template.Y
-        newLaser.PowerOn = template.PowerOn
+        newLaser.Power = template.Power
         newLaser.positionsCalculation = template.positionsCalculation
         return newLaser
 
 
     def __str__(self) -> str:
-        return f"X={self.X}, Y={self.Y}, Power={self.PowerOn}, Calculations={self.positionsCalculation.name}"
+        return f"X={self.X}, Y={self.Y}, Power={self.Power}, Calculations={self.positionsCalculation.name}"
     
     #Get the positions IN THE IMAGE of the laser
     def toImageXY(self, xoffset:int = 0, yoffset:int = 0):
         return (self.X * PIXELS_PER_MM + xoffset, self.Y * PIXELS_PER_MM + yoffset)
 
+    def powerOn(self):      
+        #reminder power is [0..100] 
+        return self.Power > 0.1
 
 
 #size of a job in mm, estimated time, etc.
 class JobStats:
     pointFromMM = []
     pointToMM = []
     estimatedDurationSec = 0
@@ -98,42 +103,55 @@
         y = float(match.group("Y"))
         if l.positionsCalculation == PositionsCalculation.ABSOLUTE:
             l.Y = y
         else:
             l.Y = l.Y + y
 
 
-def processFile(filepath:str, targetImage:Image = None, xoffset:int = 0, yoffset:int = 0, color="red", lineWidth:float=2):        
+def getColorWithAlpha (color, power, noblending = NO_BLENDING):
+    if noblending:
+        return color
+    
+    #power is [0..100] so convert to [0..255]
+    return (color[0], color[1], color[2], int(power / 100.0 * 255.0))
+
+
+def processFile(filepath:str, targetImage:Image = None, xoffset:int = 0, yoffset:int = 0, color="red", lineWidth:float=2, bg_color=BG_COLOR, noblending = NO_BLENDING):
     """ Based on a GRBL file content, generates an Image.
     Not every GRBL commands are supported so go ahead and test, fix, contribute.
 
     The image will be UPSIDE DOWN so remember to flip it (img = img.transpose(Image.FLIP_TOP_BOTTOM))
 
     :param filepath: FULL PATH to the source GRBL file
     :param targetImage: provide an image to write into, or function will make one based on the PIXELS_PER_MM, AREA_W_MM and AREA_H_MM
     :param xoffset: if you need to write in the image shifted by x pixels (default 0)
     :param yoffset: if you need to write in the image shifted by y pixels (default 0)
     :param color: which color you want the line, ie : "red" or (0,0,255,128) for semi-transparent blue (default "red")
     :param lineWidth: which width you want the line (default 2)
+    :param bg_color: which color you want the background (default BG_COLOR)
+    :param noblending: if True, the laser power will be ignored and the line will be drawn without alpha blending (ON/OFF mode) (default False=NO_BLENDING)
 
     
     """
     laser = Laser()
 
     contents = None
     with open(filepath, "r") as f:
         contents = f.readlines()
 
     stats = JobStats(os.path.basename(filepath))
 
-    img = targetImage
-    if targetImage == None:
-        img = Image.new("RGBA", (AREA_H_MM * PIXELS_PER_MM, AREA_W_MM * PIXELS_PER_MM), (255,255,255))
 
-    draw = ImageDraw.Draw(img, "RGBA")
+    #img is a calque we'll be drawing on
+    calque = Image.new("RGBA", (AREA_H_MM * PIXELS_PER_MM, AREA_W_MM * PIXELS_PER_MM), (255,255,255,0))
+
+    draw = ImageDraw.Draw(calque, "RGBA")
+
+    #convert color to RGBA ("blue" => (0,0,255,255))
+    K = ImageColor.getrgb(color)
         
     for l in contents:
         l = l.strip()
 
         if l.startswith(";"):
             #skip comments
             continue
@@ -155,22 +173,24 @@
         #------------------------ G1 : move (and trace) -------------------------
         if m.group("cmd") == "G1":
             #newlaser Power is same as previous by default (so continue what you were doing in sort)
             newlaser = Laser.fromLaser(laser)
 
             #sometimes when filling G1 is used as a G0 depending on the S value
             if m.group("S") != None:                
-                newlaser.PowerOn = int(m.group("S")) != 0
+                #if S is 0, it's a move without power.
+                #Convert power to percentage [0..100] (in the file it's per thousand)
+                newlaser.Power = float(m.group("S")) / 10.0
 
             __processLine(newlaser, match=m)
 
 
             #Draw a line?
-            if newlaser.PowerOn:
-                draw.line((laser.toImageXY(xoffset, yoffset), newlaser.toImageXY(xoffset, yoffset)), fill=color, width=lineWidth)
+            if newlaser.powerOn():
+                draw.line((laser.toImageXY(xoffset, yoffset), newlaser.toImageXY(xoffset, yoffset)), fill=getColorWithAlpha(K, newlaser.Power, noblending), width=lineWidth)
 
             #update pos
             laser = newlaser
 
 
         #------------------------ G90 : Positions are ABSOLUTE from 0,0 -------------------------     
         if m.group("cmd") == "G90":       
@@ -182,9 +202,17 @@
 
         #------------------------ Done. Next line. -------------------------
         #Update the stats
         stats.updateStats(laser)
 
         if DEBUG: print(f"DBG: laser is at { laser }")
     
+
+    #make a (default white) background and paste the drawing calque on it
+    if targetImage == None:
+        background = Image.new("RGBA", (AREA_H_MM * PIXELS_PER_MM, AREA_W_MM * PIXELS_PER_MM), bg_color)
+    else:
+        background = targetImage.copy()
+    background.paste(calque, (0,0), calque)
+
     #finished
-    return img, stats
+    return background, stats
```

### Comparing `grbl2image-1.1.1/src/grbl2image.egg-info/PKG-INFO` & `grbl2image-1.2.0/src/grbl2image.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: grbl2image
-Version: 1.1.1
+Version: 1.2.0
 Summary: Generates an image (PNG, JPEG, etc.) from a GRBL file (.NC, .GC, ...) in Python using pillow (python3)
 Author: AlanFromJapan
 Project-URL: Homepage, https://github.com/AlanFromJapan/grbl2image
 Project-URL: Bug Tracker, https://github.com/AlanFromJapan/grbl2image/issues
 Project-URL: Parent project, https://github.com/AlanFromJapan/GrblWebStreamer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Pillow>=9.0
 
 # grbl2image
 Generates an **image** (PNG, JPEG, etc.) from a **GRBL** file (.NC, .GC, ...), in Python using pillow (python3 PIL fork). It is to be used as a reusable standalone component, initially for the **parent project [GRBL WebStreamer](https://github.com/AlanFromJapan/GrblWebStreamer)** that is a webinterface for laser cutters running on Raspi or similar SBC.
 
 ![Turns GRBL code into PNG](https://github.com/AlanFromJapan/grbl2image/blob/main/grbl2image.png?raw=true)
 
 The target is to generate a simply a top view of a GRBL job for my Laser (see *limitations* below). As of now only a subset of the GRBL commands are recognized, and more will be added along the way when their need arise. This is not meant to be the complete solution for all GRBL files, but I'll be taking requests on GitHub so don't hesitate. 
 
 ## What it does
 - [x] Generates image from a GRBL file for a Laser job
 - [x] Calculates estimated bounds of the job
+- [x] Supports color blending for "greyscale" jobs 
 - [ ] Calculates an estimated time of completion of the job
 
 ## Limitations 
 This is made to support a ***laser*** cutter/engraver, *not CNC*, and this is out of scope even of the end scope of library. There are already good solutions that handle the 3D component of your CNC. This is just a top view of a GRBL file, so if it works with yours CNC good for you!
 
 Therefore GRBL codes that don't make sense for a laser will be ignored and not implemented, but if you have time fork this project!
 
@@ -89,10 +91,27 @@
 
 #final flip because the image 0,0 is top left and for us human it's at the bottom left
 img = img.transpose(Image.FLIP_TOP_BOTTOM)
 
 #save
 img.save("laser_job_001.png")
 ```
+
+### Customize the rendering
+```python
+import grbl2image.grbl2image as G2I
+from PIL import Image
+
+# don't blend, just laser ON/OFF : makes you see the whole work but make greyscale images a big blotch
+G2I.NO_BLENDING = True
+# change default background color
+G2I.BG_COLOR = "whitesmoke"
+
+#Generate the PIL Image object based on sample code and overwrite the default values
+img, _ = G2I.processFile("sample.gcode/Test gcode 1.nc", color="blue", bg_color="yellow", noblending=False)
+
+...
+```
+
 ## Source code
 - Source is MIT licensed on GitHub : https://github.com/AlanFromJapan/grbl2image
 - Parent project [GRBL WebStreamer](https://github.com/AlanFromJapan/GrblWebStreamer) is also on GitHub under MIT license
```

### Comparing `grbl2image-1.1.1/tests/tests.py` & `grbl2image-1.2.0/tests/tests.py`

 * *Files identical despite different names*

### Comparing `grbl2image-1.1.1/tests/tests_all.py` & `grbl2image-1.2.0/tests/tests_all.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import os
 
 from PIL import Image
 
 samplesPath = os.path.join("tests", "sample.gcode")
 #list of files
-l = [l for l in os.listdir(samplesPath) if os.path.isfile(os.path.join(samplesPath, l)) and l.lower()[-3:] == '.nc']
+l = [l for l in os.listdir(samplesPath) if os.path.isfile(os.path.join(samplesPath, l)) and l.lower()[-3:] in ['.nc', '.gc']]
 
 for f in l:
     print (f)
     img, stats = G2I.processFile(os.path.join(samplesPath, f), color="blue")
     print(stats)
     
     img = img.transpose(Image.FLIP_TOP_BOTTOM)
```

### Comparing `grbl2image-1.1.1/tests/tests_size.py` & `grbl2image-1.2.0/tests/tests_size.py`

 * *Files identical despite different names*

