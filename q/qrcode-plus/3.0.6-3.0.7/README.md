# Comparing `tmp/qrcode_plus-3.0.6.tar.gz` & `tmp/qrcode_plus-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrcode_plus-3.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "qrcode_plus-3.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `qrcode_plus-3.0.6.tar` & `qrcode_plus-3.0.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1505 2024-04-13 16:10:05.922714 qrcode_plus-3.0.6/LICENSE
--rw-r--r--   0        0        0     1003 2024-03-14 15:29:45.816329 qrcode_plus-3.0.6/README.rst
--rw-r--r--   0        0        0     1783 2024-04-17 13:36:39.410389 qrcode_plus-3.0.6/pyproject.toml
--rw-r--r--   0        0        0    15986 2024-04-17 10:59:40.398335 qrcode_plus-3.0.6/qrcode_plus.py
--rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 qrcode_plus-3.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1505 2024-04-13 16:10:05.922714 qrcode_plus-3.0.7/LICENSE
+-rw-r--r--   0        0        0     1003 2024-03-14 15:29:45.816329 qrcode_plus-3.0.7/README.rst
+-rw-r--r--   0        0        0     1783 2024-04-17 13:42:35.012655 qrcode_plus-3.0.7/pyproject.toml
+-rw-r--r--   0        0        0    16882 2024-04-17 13:42:18.875023 qrcode_plus-3.0.7/qrcode_plus.py
+-rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 qrcode_plus-3.0.7/PKG-INFO
```

### Comparing `qrcode_plus-3.0.6/LICENSE` & `qrcode_plus-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qrcode_plus-3.0.6/README.rst` & `qrcode_plus-3.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `qrcode_plus-3.0.6/pyproject.toml` & `qrcode_plus-3.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 
 [project]
 name = "qrcode-plus"
 description = "Advance Artistic (Micro) QR Code plugin for Segno"
-version = "3.0.6"
+version = "3.0.7"
 readme = "README.rst"
 license = {file = "LICENSE"}
 authors = [{"name" = "Kyle Bradley", email = "kbradley53@gmail.com"}]
 requires-python = ">= 3.5"
 keywords = ["QR Code", "Micro QR Code", "ISO/IEC 18004", "ISO/IEC 18004:2006(E)",
     "ISO/IEC 18004:2015(E)", "qrcode", "QR", "barcode", "matrix", "2D",]
 classifiers = [
```

### Comparing `qrcode_plus-3.0.6/qrcode_plus.py` & `qrcode_plus-3.0.7/qrcode_plus.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                 timing_dark=timing_dark, timing_light=timing_light,
                 separator=separator, dark_module=dark_module, quiet_zone=quiet_zone)
     buff.seek(0)
     return Image.open(buff)
 
 
 def write_artistic(qrcode, background, target, mode=None, format=None, kind=None,
-                   scale=3, boxSize=4, fullSize=0, border=None, dark='#000', light='#fff',
+                   scale=3, boxSize=9, dotSize=1, fullSize=0, border=None, dark='#000', light='#fff',
                    finder_dark=False, finder_light=False, data_dark=False,
                    data_light=False, version_dark=False, version_light=False,
                    format_dark=False, format_light=False, alignment_dark=False,
                    alignment_light=False, timing_dark=False, timing_light=False,
                    separator=False, dark_module=False, quiet_zone=False):
     """\
     Saves the QR code with the background image into target.
@@ -157,14 +157,15 @@
                        quiet_zone=quiet_zone).convert('RGBA')
     
     # Maximal dimensions of the background image(s)
     # The background image is not drawn at the quiet zone of the QR Code, therefore border=0
     max_bg_width = max_bg_width*boxSize
     max_bg_height = max_bg_height*boxSize
 
+    print(max_bg_width)
     if format:
         import warnings
         warnings.warn('Using format is deprecated, use "kind"', DeprecationWarning)
         kind = format
     try:
         bg_img = Image.open(background)
     except UnidentifiedImageError:
@@ -214,15 +215,15 @@
 
     rect_functions = [ImageDraw.Draw(img).rectangle for img in bg_images]
     ecllipse_functions = [ImageDraw.Draw(img).ellipse for img in bg_images]
 
     keep_modules = (consts.TYPE_FINDER_PATTERN_DARK, consts.TYPE_FINDER_PATTERN_LIGHT, consts.TYPE_SEPARATOR,
                     consts.TYPE_ALIGNMENT_PATTERN_DARK, consts.TYPE_ALIGNMENT_PATTERN_LIGHT)#, consts.TYPE_TIMING_DARK,
                     #consts.TYPE_TIMING_LIGHT)
-    d = scale // 3 # e.g. 1 | 10
+    d = scale // 3 
     
     # x x x x x x x x x 
     # x x x x x x x x x 
     # x x x x x x x x x 
     # x x x x x x x x x 
     # x x x x x x x x x 
     # x x x x x x x x x 
@@ -232,34 +233,40 @@
     
     #bg_images[0].paste(new_canvas, (0, 0))
 
     for i, row in enumerate(qrcode.matrix_iter(scale=scale, border=0, verbose=True)):
         for j, m in enumerate(row):
             if m in keep_modules:
                 for img_idx, img in enumerate(bg_images):
-                    rect_functions[img_idx](pixel_box(border_nonBox, boxSize, i, j, False), qr_img.getpixel((i+border_nonBox, j+border_nonBox)))
+                    rect_functions[img_idx](pixel_box(border_nonBox, boxSize, i, j), qr_img.getpixel((i+border_nonBox, j+border_nonBox)))
 
                 #ImageDraw.Draw(new_canvas).rectangle(pixel_box(border_nonBox, boxSize, i, j, False), qr_img.getpixel((i+border_nonBox, j+border_nonBox)))   
                 continue
             if not (((i // d) % 3 == 1) and ((j // d) % 3 == 1)):
+                #print ("("+str(i)+", "+str(j) +") - skip" + str((i // d) % 3 == 1))
                 for img_idx, img in enumerate(bg_images):
                     fill = img.getpixel((i, j))
                     #if not fill[3]:
                     #    ImageDraw.Draw(new_canvas).ellipse(pixel_box(border, scale, i, j, False), qr_img.getpixel((i+border, j+border))) 
             else:
                 if((i % d == 0) and (j % d == 0)):
                     for img_idx, img in enumerate(bg_images):
-                        ecllipse_functions[img_idx](pixel_box(border_nonBox, boxSize, i, j, False, scale=d), qr_img.getpixel((i+border_nonBox, j+border_nonBox)))  
+                        ecllipse_functions[img_idx](pixel_eclipse_box(border_nonBox, boxSize, i, j, True, width=d, enlarge = dotSize), qr_img.getpixel((i+border_nonBox, j+border_nonBox)))                  
+                #else:
+                    #print ("("+str(i)+", "+str(j) +") - draw skip")
                     # fill = qr_img.getpixel((i+border_nonBox, j+border_nonBox))
                     # transparency = fill[:3]+opacity(0)
                                             
                     # ImageDraw.Draw(new_canvas).ellipse(pixel_box(border_nonBox, boxSize, i, j, True, scale=d),transparency)   
                 
     #new_canvas.save("new-test-2.png", format=kind)
     
+    print(qr_img.width*boxSize)
+    print(border_offset)
+
     if fullSize != 0:
         bg_width, bg_height = max_bg_width, max_bg_height
         adjustment = fullSize / max_bg_width
         bg_width, bg_height = int(bg_width * adjustment), int(bg_height * adjustment)
         bg_images = [img.resize((bg_width, bg_height), LANCZOS) for img in bg_images]
     elif scale != requested_scale:
         bg_width, bg_height = max_bg_width, max_bg_height
@@ -303,28 +310,48 @@
     w, h = int(svg_width * ratio), int(svg_height * ratio)
     out = io.BytesIO()
     with open(source, 'rb') as f:
         cairosvg.svg2png(file_obj=f, write_to=out, output_width=w, output_height=h)
     out.seek(0)
     return Image.open(out)
 
-def pixel_box(border, boxsize, col, row, show, scale = 1):
+def pixel_eclipse_box(border, boxsize, col, row, show, width, enlarge):
         """
         A helper method for pixel-based image generators that specifies the
         four pixel coordinates for a single rect.
         """
 
         x = (col + border)*boxsize 
         y = (row + border)*boxsize 
         
+        rectRadius = boxsize*width
+        largerRadius = rectRadius*(enlarge - 1)/2
+
         if(show):
-            print (str(x) + " " + str(y) + " " + str(boxsize))
+           print ("("+str(x - rectRadius) + "," + str(y - rectRadius) +") " + "("+str(x + rectRadius) + "," + str(y + rectRadius)+")")
+
+        return (
+            (x - largerRadius, y - largerRadius),
+            (x + rectRadius+largerRadius, y + rectRadius+largerRadius),
+        )
+
+def pixel_box(border, boxsize, col, row):
+        """
+        A helper method for pixel-based image generators that specifies the
+        four pixel coordinates for a single rect.
+        """
+
+        x = (col + border)*boxsize 
+        y = (row + border)*boxsize 
+        
+        rectRadius = boxsize
 
         return (
             (x, y),
-            (x + boxsize*scale - scale, y + boxsize*scale - scale),
+            (x + rectRadius, y + rectRadius),
         )
 
 
+
 if not _SVG_SUPPORT:
     def _svg_to_png(source, width=None, height=None):  # noqa: F811
         raise ValueError('cairosvg is required for SVG support')
```

### Comparing `qrcode_plus-3.0.6/PKG-INFO` & `qrcode_plus-3.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrcode-plus
-Version: 3.0.6
+Version: 3.0.7
 Summary: Advance Artistic (Micro) QR Code plugin for Segno
 Keywords: QR Code,Micro QR Code,ISO/IEC 18004,ISO/IEC 18004:2006(E),ISO/IEC 18004:2015(E),qrcode,QR,barcode,matrix,2D
 Author-email: Kyle Bradley <kbradley53@gmail.com>
 Requires-Python: >= 3.5
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

