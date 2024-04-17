# Comparing `tmp/qrcode_plus-3.0.4.tar.gz` & `tmp/qrcode_plus-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrcode_plus-3.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "qrcode_plus-3.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `qrcode_plus-3.0.4.tar` & `qrcode_plus-3.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1505 2024-04-13 16:10:05.922714 qrcode_plus-3.0.4/LICENSE
--rw-r--r--   0        0        0     1003 2024-03-14 15:29:45.816329 qrcode_plus-3.0.4/README.rst
--rw-r--r--   0        0        0     1783 2024-04-14 09:55:34.990994 qrcode_plus-3.0.4/pyproject.toml
--rw-r--r--   0        0        0    15807 2024-04-14 09:44:36.362449 qrcode_plus-3.0.4/qrcode_plus.py
--rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 qrcode_plus-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1505 2024-04-13 16:10:05.922714 qrcode_plus-3.0.6/LICENSE
+-rw-r--r--   0        0        0     1003 2024-03-14 15:29:45.816329 qrcode_plus-3.0.6/README.rst
+-rw-r--r--   0        0        0     1783 2024-04-17 13:36:39.410389 qrcode_plus-3.0.6/pyproject.toml
+-rw-r--r--   0        0        0    15986 2024-04-17 10:59:40.398335 qrcode_plus-3.0.6/qrcode_plus.py
+-rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 qrcode_plus-3.0.6/PKG-INFO
```

### Comparing `qrcode_plus-3.0.4/LICENSE` & `qrcode_plus-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qrcode_plus-3.0.4/README.rst` & `qrcode_plus-3.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `qrcode_plus-3.0.4/pyproject.toml` & `qrcode_plus-3.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 
 [project]
 name = "qrcode-plus"
 description = "Advance Artistic (Micro) QR Code plugin for Segno"
-version = "3.0.4"
+version = "3.0.6"
 readme = "README.rst"
 license = {file = "LICENSE"}
 authors = [{"name" = "Kyle Bradley", email = "kbradley53@gmail.com"}]
 requires-python = ">= 3.5"
 keywords = ["QR Code", "Micro QR Code", "ISO/IEC 18004", "ISO/IEC 18004:2006(E)",
     "ISO/IEC 18004:2015(E)", "qrcode", "QR", "barcode", "matrix", "2D",]
 classifiers = [
```

### Comparing `qrcode_plus-3.0.4/qrcode_plus.py` & `qrcode_plus-3.0.6/qrcode_plus.py`

 * *Files 6% similar despite different names*

```diff
@@ -156,16 +156,14 @@
                        timing_light=timing_light, separator=separator, dark_module=dark_module,
                        quiet_zone=quiet_zone).convert('RGBA')
     
     # Maximal dimensions of the background image(s)
     # The background image is not drawn at the quiet zone of the QR Code, therefore border=0
     max_bg_width = max_bg_width*boxSize
     max_bg_height = max_bg_height*boxSize
-    print (max_bg_width)
-    print (max_bg_height)
 
     if format:
         import warnings
         warnings.warn('Using format is deprecated, use "kind"', DeprecationWarning)
         kind = format
     try:
         bg_img = Image.open(background)
@@ -218,14 +216,24 @@
     ecllipse_functions = [ImageDraw.Draw(img).ellipse for img in bg_images]
 
     keep_modules = (consts.TYPE_FINDER_PATTERN_DARK, consts.TYPE_FINDER_PATTERN_LIGHT, consts.TYPE_SEPARATOR,
                     consts.TYPE_ALIGNMENT_PATTERN_DARK, consts.TYPE_ALIGNMENT_PATTERN_LIGHT)#, consts.TYPE_TIMING_DARK,
                     #consts.TYPE_TIMING_LIGHT)
     d = scale // 3 # e.g. 1 | 10
     
+    # x x x x x x x x x 
+    # x x x x x x x x x 
+    # x x x x x x x x x 
+    # x x x x x x x x x 
+    # x x x x x x x x x 
+    # x x x x x x x x x 
+    # x x x x x x x x x 
+    # x x x x x x x x x 
+    # x x x x x x x x x 
+    
     #bg_images[0].paste(new_canvas, (0, 0))
 
     for i, row in enumerate(qrcode.matrix_iter(scale=scale, border=0, verbose=True)):
         for j, m in enumerate(row):
             if m in keep_modules:
                 for img_idx, img in enumerate(bg_images):
                     rect_functions[img_idx](pixel_box(border_nonBox, boxSize, i, j, False), qr_img.getpixel((i+border_nonBox, j+border_nonBox)))
```

### Comparing `qrcode_plus-3.0.4/PKG-INFO` & `qrcode_plus-3.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrcode-plus
-Version: 3.0.4
+Version: 3.0.6
 Summary: Advance Artistic (Micro) QR Code plugin for Segno
 Keywords: QR Code,Micro QR Code,ISO/IEC 18004,ISO/IEC 18004:2006(E),ISO/IEC 18004:2015(E),qrcode,QR,barcode,matrix,2D
 Author-email: Kyle Bradley <kbradley53@gmail.com>
 Requires-Python: >= 3.5
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

