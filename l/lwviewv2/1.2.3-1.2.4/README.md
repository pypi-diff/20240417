# Comparing `tmp/lwviewv2-1.2.3-py3-none-any.whl.zip` & `tmp/lwviewv2-1.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 27567 bytes, number of entries: 12
+Zip file size: 27568 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-05 13:02 lwviewv2/__init__.py
 -rw-r--r--  2.0 unx     8629 b- defN 24-Apr-12 15:12 lwviewv2/landmark.py
 -rw-r--r--  2.0 unx     1091 b- defN 24-Mar-19 17:18 lwviewv2/lw_babel.py
 -rw-r--r--  2.0 unx     6985 b- defN 22-Oct-25 20:11 lwviewv2/lw_image.py
 -rw-r--r--  2.0 unx     1797 b- defN 24-Mar-19 17:18 lwviewv2/lw_nrrd.py
 -rw-r--r--  2.0 unx    43131 b- defN 24-Mar-15 20:11 lwviewv2/lw_view copy.py
--rw-r--r--  2.0 unx    58671 b- defN 24-Apr-11 14:11 lwviewv2/lw_view.py
+-rw-r--r--  2.0 unx    58698 b- defN 24-Apr-17 17:06 lwviewv2/lw_view.py
 -rw-r--r--  2.0 unx      285 b- defN 24-Mar-14 21:01 lwviewv2/util.py
--rw-r--r--  2.0 unx      618 b- defN 24-Apr-12 15:12 lwviewv2-1.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 15:12 lwviewv2-1.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-12 15:12 lwviewv2-1.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      912 b- defN 24-Apr-12 15:12 lwviewv2-1.2.3.dist-info/RECORD
-12 files, 122220 bytes uncompressed, 26053 bytes compressed:  78.7%
+-rw-r--r--  2.0 unx      618 b- defN 24-Apr-17 17:06 lwviewv2-1.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 17:06 lwviewv2-1.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-17 17:06 lwviewv2-1.2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      912 b- defN 24-Apr-17 17:06 lwviewv2-1.2.4.dist-info/RECORD
+12 files, 122247 bytes uncompressed, 26054 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: lwviewv2/lw_view.py
 Comment: 
 
 Filename: lwviewv2/util.py
 Comment: 
 
-Filename: lwviewv2-1.2.3.dist-info/METADATA
+Filename: lwviewv2-1.2.4.dist-info/METADATA
 Comment: 
 
-Filename: lwviewv2-1.2.3.dist-info/WHEEL
+Filename: lwviewv2-1.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: lwviewv2-1.2.3.dist-info/top_level.txt
+Filename: lwviewv2-1.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: lwviewv2-1.2.3.dist-info/RECORD
+Filename: lwviewv2-1.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lwviewv2/lw_view.py

```diff
@@ -525,19 +525,19 @@
             self.canvas_cor.bind('<Shift-Button-5>', self.cor_shift_mousewheel_callback)
             self.canvas_sag.bind('<Button-4>', self.sag_mousewheel_callback)
             self.canvas_sag.bind('<Shift-Button-4>', self.sag_shift_mousewheel_callback)
             self.canvas_sag.bind('<Button-5>', self.sag_mousewheel_callback)
             self.canvas_sag.bind('<Shift-Button-5>', self.sag_shift_mousewheel_callback)
         else:
             self.canvas_axi.bind('<MouseWheel>', self.axi_mousewheel_callback)
-            self.canvas_axi.bind('<Shift-MouseWheel>', self.axi_shift_mousewheel_callback)
+            self.canvas_axi.bind(f'<{mod_key_jog}-MouseWheel>', self.axi_shift_mousewheel_callback)
             self.canvas_cor.bind('<MouseWheel>', self.cor_mousewheel_callback)
-            self.canvas_cor.bind('<Shift-MouseWheel>', self.cor_shift_mousewheel_callback)
+            self.canvas_cor.bind(f'<{mod_key_jog}-MouseWheel>', self.cor_shift_mousewheel_callback)
             self.canvas_sag.bind('<MouseWheel>', self.sag_mousewheel_callback)
-            self.canvas_sag.bind('<Shift-MouseWheel>', self.sag_shift_mousewheel_callback)
+            self.canvas_sag.bind(f'<{mod_key_jog}-MouseWheel>', self.sag_shift_mousewheel_callback)
             
             mod_key = "Command" if sys.platform == "darwin" else "Control"
             self.canvas_axi.bind(f'<{mod_key}-MouseWheel>', self.handle_zoom)
             
             self.canvas_axi.bind(f"<{mod_key}-ButtonPress-1>", self.on_mouse_down)
             self.canvas_axi.bind(f"<{mod_key}-B1-Motion>", self.on_mouse_move)
             self.canvas_axi.bind(f"<{mod_key}-ButtonRelease-1>", self.on_mouse_up)
```

## Comparing `lwviewv2-1.2.3.dist-info/METADATA` & `lwviewv2-1.2.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lwviewv2
-Version: 1.2.3
+Version: 1.2.4
 Summary: Viewer of images in python.
 Home-page: https://github.com/ReubenDo/lightweight-viewer
 Author: Sandy Wells
 Author-email: sw@bwh.harvard.edu
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

## Comparing `lwviewv2-1.2.3.dist-info/RECORD` & `lwviewv2-1.2.4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lwviewv2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lwviewv2/landmark.py,sha256=i-WZxHsCm0CpWhh7Opcfm0-eH6BhZZIx_Yz-Es9fIQA,8629
 lwviewv2/lw_babel.py,sha256=H84MF8uh4ADDiWK9e56iedtPdM3qGvbpTVDCpb_lLhQ,1091
 lwviewv2/lw_image.py,sha256=LH6hCzmyvssVseI0dM2gNkoN8XunDLBd84TTXtLFMiA,6985
 lwviewv2/lw_nrrd.py,sha256=2LxfO86sbjAbLyDKY41uPtrN7x6j6QUVhBv30_RsThM,1797
 lwviewv2/lw_view copy.py,sha256=A_4gWXB0SzufNiS-67erhvuF8y2qYYk0PSp0nvXnoRE,43131
-lwviewv2/lw_view.py,sha256=2yJD1OR4eFis5wzmSq22oxsivTiUDBae-csuBCu650k,58671
+lwviewv2/lw_view.py,sha256=lOMkx7wbXlVM-5sIvaai87Ppi9ApOvKP6G5e4L7Sy3U,58698
 lwviewv2/util.py,sha256=pTAX578rsDylPGfFEHew73-3578bp4GSVbnnNKTA-U0,285
-lwviewv2-1.2.3.dist-info/METADATA,sha256=GlwFJEe1Vaw1wP9cxysACJx2OQNTtj4_jtP7VYzf6OA,618
-lwviewv2-1.2.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-lwviewv2-1.2.3.dist-info/top_level.txt,sha256=UBxEML6xSOAmiPwcH66C4QPfPW3Bid1w25rLoIdLKLM,9
-lwviewv2-1.2.3.dist-info/RECORD,,
+lwviewv2-1.2.4.dist-info/METADATA,sha256=O3vt6lSkippm7mvhD3pwj8J2a1Lem3jBMcHn53aiw58,618
+lwviewv2-1.2.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+lwviewv2-1.2.4.dist-info/top_level.txt,sha256=UBxEML6xSOAmiPwcH66C4QPfPW3Bid1w25rLoIdLKLM,9
+lwviewv2-1.2.4.dist-info/RECORD,,
```

