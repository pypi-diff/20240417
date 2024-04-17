# Comparing `tmp/image-go-nord-0.1.7.tar.gz` & `tmp/image-go-nord-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-go-nord-0.1.7.tar", last modified: Wed Jul 26 18:58:56 2023, max compression
+gzip compressed data, was "image-go-nord-1.0.1.tar", last modified: Wed Apr 17 09:20:22 2024, max compression
```

## Comparing `image-go-nord-0.1.7.tar` & `image-go-nord-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:58:56.886544 image-go-nord-0.1.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:58:56.886544 image-go-nord-0.1.7/ImageGoNord/
--rwxr-xr-x   0 root         (0) root         (0)    21892 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/GoNord.py
--rw-r--r--   0 root         (0) root         (0)      768 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/GoNord_test.py
--rwxr-xr-x   0 root         (0) root         (0)       72 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:58:56.886544 image-go-nord-0.1.7/ImageGoNord/palettes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:58:56.886544 image-go-nord-0.1.7/ImageGoNord/palettes/Nord/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/palettes/Nord/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/palettes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:58:56.886544 image-go-nord-0.1.7/ImageGoNord/utility/
--rwxr-xr-x   0 root         (0) root         (0)     2330 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/utility/ConvertUtility.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/utility/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3368 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/utility/palette_loader.py
--rw-r--r--   0 root         (0) root         (0)      962 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/utility/quantize.py
--rw-r--r--   0 root         (0) root         (0)     1073 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)       16 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5904 2023-07-26 18:58:56.886544 image-go-nord-0.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4870 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:58:56.886544 image-go-nord-0.1.7/image_go_nord.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5904 2023-07-26 18:58:56.000000 image-go-nord-0.1.7/image_go_nord.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      506 2023-07-26 18:58:56.000000 image-go-nord-0.1.7/image_go_nord.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 18:58:56.000000 image-go-nord-0.1.7/image_go_nord.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-26 18:58:56.000000 image-go-nord-0.1.7/image_go_nord.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-26 18:58:56.000000 image-go-nord-0.1.7/image_go_nord.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 18:58:56.890544 image-go-nord-0.1.7/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1553 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:20:22.255963 image-go-nord-1.0.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:20:22.251963 image-go-nord-1.0.1/ImageGoNord/
+-rwxr-xr-x   0 root         (0) root         (0)    24849 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/ImageGoNord/GoNord.py
+-rw-r--r--   0 root         (0) root         (0)      768 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/ImageGoNord/GoNord_test.py
+-rwxr-xr-x   0 root         (0) root         (0)       72 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/ImageGoNord/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:20:22.255963 image-go-nord-1.0.1/ImageGoNord/models/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:20:22.255963 image-go-nord-1.0.1/ImageGoNord/models/PaletteNet/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/ImageGoNord/models/PaletteNet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/ImageGoNord/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:20:22.255963 image-go-nord-1.0.1/ImageGoNord/palettes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:20:22.255963 image-go-nord-1.0.1/ImageGoNord/palettes/Nord/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/ImageGoNord/palettes/Nord/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/ImageGoNord/palettes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:20:22.255963 image-go-nord-1.0.1/ImageGoNord/utility/
+-rwxr-xr-x   0 root         (0) root         (0)     2330 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/ImageGoNord/utility/ConvertUtility.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/ImageGoNord/utility/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5947 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/ImageGoNord/utility/model.py
+-rw-r--r--   0 root         (0) root         (0)     3368 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/ImageGoNord/utility/palette_loader.py
+-rw-r--r--   0 root         (0) root         (0)      962 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/ImageGoNord/utility/quantize.py
+-rw-r--r--   0 root         (0) root         (0)    34522 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/LICENSE
+-rwxr-xr-x   0 root         (0) root         (0)       31 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7009 2024-04-17 09:20:22.255963 image-go-nord-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5861 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:20:22.255963 image-go-nord-1.0.1/image_go_nord.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7009 2024-04-17 09:20:22.000000 image-go-nord-1.0.1/image_go_nord.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      608 2024-04-17 09:20:22.000000 image-go-nord-1.0.1/image_go_nord.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 09:20:22.000000 image-go-nord-1.0.1/image_go_nord.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-17 09:20:22.000000 image-go-nord-1.0.1/image_go_nord.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-17 09:20:22.000000 image-go-nord-1.0.1/image_go_nord.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 09:20:22.255963 image-go-nord-1.0.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1751 2024-04-17 09:20:06.000000 image-go-nord-1.0.1/setup.py
```

### Comparing `image-go-nord-0.1.7/ImageGoNord/GoNord.py` & `image-go-nord-1.0.1/ImageGoNord/GoNord.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,33 @@
 from PIL import Image, ImageFilter
 
 import numpy as np
 import ffmpeg
 import uuid
 import shutil
 
+import torch
+import skimage.io as io
+import skimage.color as convertor
+import torchvision.transforms as transforms
+
+
 try:
     import importlib.resources as pkg_resources
 except ImportError:
     # Try backported to PY<37 `importlib_resources`.
     import importlib_resources as pkg_resources
 
 from .palettes import Nord as nord_palette
+from .models import PaletteNet as palette_net
 
 from ImageGoNord.utility.quantize import quantize_to_palette
 import ImageGoNord.utility.palette_loader as pl
 from ImageGoNord.utility.ConvertUtility import ConvertUtility
+from ImageGoNord.utility.model import FeatureEncoder,RecoloringDecoder
 
 
 class NordPaletteFile:
     """
     A class used to map the nord color-scheme into files.
     Each file contains the hex of colors
 
@@ -413,52 +421,125 @@
                 colors_list = self.PALETTE_DATA[difference]
                 if (is_rgba and len(colors_list) == 3):
                     colors_list.append(color_to_check[3])
 
                 pixels[row, col] = tuple(colors_list)
         return pixels
 
-    def convert_image(self, image, save_path='', parallel_threading=False):
+    def convert_image_by_model(self, image, use_model_cpu=False):
+        """
+        Process a Pillow image by using a PyTorch model "PaletteNet" for recoloring the image
+
+        Parameters
+        ----------
+        image : pillow image
+            The source pillow image
+        use_model_cpu : bool, optional
+            true if using cpu power
+
+        Returns
+        -------
+        pillow image
+            processed image
+        """
+        FE = FeatureEncoder() # torch.Size([64, 3, 3, 3])
+        RD = RecoloringDecoder() # torch.Size([530, 256, 3, 3])
+
+        FE.load_state_dict(torch.load(pkg_resources.open_binary(palette_net, "FE.state_dict.pt")))
+        RD.load_state_dict(torch.load(pkg_resources.open_binary(palette_net, "RD.state_dict.pt")))
+
+        if use_model_cpu:
+            FE.to("cpu")
+            RD.to("cpu")
+
+        lab_image = ((convertor.rgb2lab(np.array(image))) - [50,0,0] ) / [50,127,127]
+
+        img = torch.Tensor(lab_image).permute(2,0,1)
+
+        h = 16*int(img.shape[1]/16)
+        w = 16*int(img.shape[2]/16)
+
+        T = transforms.Resize((h,w))
+
+        img = T(img)
+        img = img.unsqueeze(0)
+        palette = []
+        for hex, rgb_value in self.PALETTE_DATA.items():
+            a = []
+            for j in [2,4,6]:
+                a.append(int(hex[j-2:j],16))
+            palette.append(a)
+
+        try:
+            pal_np = np.array(palette).reshape(1,6,3)/255
+        except:
+            print("You have too many colors in your palette for the model, this feature is limited to 6 colours, now you have: ", len(palette), "! I'll take the first 6!")
+            pal_np = np.array(palette[0:6]).reshape(1,6,3)/255
+
+        pal = torch.Tensor((convertor.rgb2lab(pal_np) - [50,0,0] ) / [50,128,128]).unsqueeze(0)
+
+        image = img
+        palette = pal
+        illu = image[:,0:1,:,:]
+
+        with torch.no_grad():
+            c1,c2,c3,c4 = FE(image)
+            out = RD(c1, c2, c3, c4, palette, illu)
+            final_image = torch.cat([(illu+1)*50, out*128],axis = 1).permute(0,2,3,1)[0]
+            # need to convert float value returning in skimage to 0-255 range values for pillow (computer vision / training lib vs pixel operation lib)
+            return Image.fromarray((convertor.lab2rgb(final_image) * 255).astype(np.uint8))
+
+    def convert_image(self, image, save_path='', use_model=False, use_model_cpu=False, parallel_threading=False):
         """
         Process a Pillow image by replacing pixel or by avg algorithm
 
         Parameters
         ----------
         image : pillow image
             The source pillow image
         save_path : str, optional
             the path and the filename where to save the image
+        use_model : bool, optional
+            true if using ai model
+        use_model_cpu : bool, optional
+            true if using cpu power
+        parallel_threading : bool, optional
+            true to enable multi-thread conversion loop
 
         Returns
         -------
         pillow image
             processed image
         """
         self.get_palette_data()
         original_image = image.copy()
         original_pixels = self.load_pixel_image(original_image)
         original_image.close()
         pixels = self.load_pixel_image(image)
         is_rgba = (image.mode == 'RGBA')
-        if (parallel_threading == False):
-            self.converted_loop(is_rgba, pixels, original_pixels, image.size[0], image.size[1])
+
+        if use_model:
+            image = self.convert_image_by_model(image, use_model_cpu)
         else:
-            step = ceil(image.size[0] / self.MAX_THREADS)
-            threads = []
-            for row in range(step, image.size[0] + step, step):
-                args = (is_rgba, pixels, original_pixels, row, image.size[1], row - step, 0)
-                t = threading.Thread(target=self.converted_loop, args=args)
-                t.daemon = True
-                t.start()
-                threads.append(t)
+            if not parallel_threading:
+                self.converted_loop(is_rgba, pixels, original_pixels, image.size[0], image.size[1])
+            else:
+                step = ceil(image.size[0] / self.MAX_THREADS)
+                threads = []
+                for row in range(step, image.size[0] + step, step):
+                    args = (is_rgba, pixels, original_pixels, row, image.size[1], row - step, 0)
+                    t = threading.Thread(target=self.converted_loop, args=args)
+                    t.daemon = True
+                    t.start()
+                    threads.append(t)
 
-            for t in threads:
-                t.join(timeout=30)
+                for t in threads:
+                    t.join(timeout=30)
 
-        if (self.USE_GAUSSIAN_BLUR == True):
+        if self.USE_GAUSSIAN_BLUR:
             image = image.filter(ImageFilter.GaussianBlur(1))
 
         if (save_path != ''):
             self.save_image_to_file(image, save_path)
 
         return image
```

### Comparing `image-go-nord-0.1.7/ImageGoNord/GoNord_test.py` & `image-go-nord-1.0.1/ImageGoNord/GoNord_test.py`

 * *Files identical despite different names*

### Comparing `image-go-nord-0.1.7/ImageGoNord/utility/ConvertUtility.py` & `image-go-nord-1.0.1/ImageGoNord/utility/ConvertUtility.py`

 * *Files identical despite different names*

### Comparing `image-go-nord-0.1.7/ImageGoNord/utility/palette_loader.py` & `image-go-nord-1.0.1/ImageGoNord/utility/palette_loader.py`

 * *Files identical despite different names*

### Comparing `image-go-nord-0.1.7/ImageGoNord/utility/quantize.py` & `image-go-nord-1.0.1/ImageGoNord/utility/quantize.py`

 * *Files identical despite different names*

### Comparing `image-go-nord-0.1.7/PKG-INFO` & `image-go-nord-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,64 @@
 Metadata-Version: 2.1
 Name: image-go-nord
-Version: 0.1.7
-Summary: A tool for converting RGB image to Nordtheme palette
+Version: 1.0.1
+Summary: A tool to convert any RGB image or video to any theme or color palette input by the user
 Home-page: https://github.com/Schrodinger-Hat/ImageGoNord-pip
 Author: Schrodinger Hat
 Author-email: schrodinger.hat.show@gmail.com
-License: MIT
+License: AGPL-3.0
 Download-URL: https://github.com/Schrodinger-Hat/ImageGoNord-pip/releases
 Project-URL: Homepage, https://ign.schrodinger-hat.it
 Project-URL: Source, https://github.com/Schrodinger-Hat/ImageGoNord-pip
 Project-URL: Bug Reports, https://github.com/Schrodinger-Hat/ImageGoNord-pip/issues
-Keywords: nordtheme,pillow,image,conversion,rgb,color-scheme,color-palette
+Keywords: nordtheme,pillow,image,conversion,rgb,color-scheme,color-palette,linux-rice,gruvbox,catpuccin
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ImageGoNord - RGB image to Nordtheme palette
+# ImageGoNord - RGB image and video to any kind of palette or theme
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/image-go-nord)
 [![PyPI](https://img.shields.io/pypi/v/image-go-nord)](https://pypi.org/project/image-go-nord/)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
 [![Join the community on Spectrum](https://withspectrum.github.io/badge/badge.svg)](https://spectrum.chat/image-go-nord)
 
-A tool that can convert your rgb images to nordtheme palette.
+A tool that can convert your rgb images to nordtheme, gruvbox, catpuccin and many more palettes.
+Video included.
 
-This repository is a python package that can convert any sort of image into a [nordtheme](https://github.com/arcticicestudio/nord) palette image.
+This repository is a python package.
 
 You can find a demo on [the website](https://ign.schrodinger-hat.it) for testing out the package.
-
-We build also a little API hosted on Heroku to give to anyone the change to test it out by theirself. You can find the documentation on the website too.
-
 The main repository of this whole project is [ImageGoNord](https://github.com/Schrodinger-Hat/ImageGoNord).
 
+It's including an API layer, in case you'd like to set it up also for your project.
+
 ### Documentation
 
 You can find the [documentation into this repository](https://github.com/Schrodinger-Hat/ImageGoNord-pip/tree/master/docs) and also on the website.
-
-<!--
-@TODO
-- Describe very briefly but clearly what the project does.
-- State if it is out-of-the-box user-friendly, so it’s clear to the user.
-- List its most useful/innovative/noteworthy features.
-- State its goals/what problem(s) it solves.
-- Note and briefly describe any key concepts (technical, philosophical, or both) important to the user’s understanding.
-- Link to any supplementary blog posts or project main pages.
-- Note its development status.
-- If possible, include screenshots and demo videos.
--->
+If you have any questions, please reach us at us@schrodinger-hat.it
 
 ### Inspiration
 
 We are in love with Nordtheme, that is why we created this repository.
 
-[![Nord Color Palette Overview](https://raw.githubusercontent.com/arcticicestudio/nord-docs/develop/assets/images/nord/repository-color-palettes.svg?sanitize=true)](https://www.nordtheme.com/docs/colors-and-palettes)
-
-Our goal is to make a shortcut to convert anything into this theme, by starting from the images.
+Our goal is to make a shortcut to convert anything into any kind of themes, by starting from the images and going to videos.
 <br>An example could be an awesome wallpaper converted into the Nordtheme palette.
 
 We checked the commnunity and we did not find anything similar or any project that can accomplish this task. So, here we are.
 
+Of course, we resolved the issue for any kind of palette, theme and it's video supported.
+
 ### What you can do with this package
 
 You can convert any image into the nord palette (or others). Here are some examples:
 
 **Original**
 
 [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test.jpg)
@@ -87,14 +76,52 @@
 [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)
 
 
 **Processed with avg algorithm**
 
 [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-average.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-average.jpg)
 
+
+### ImageGoNord with AI - PaletteNet
+
+We implemented the PaletteNet model with PyTorch based on [this implementation](https://github.com/AakritiKinra/PaletteNet-Implementation).
+Inside that repository you could find the paper, in case you'd like to develop and train your model.
+
+There is a lot of room for improvement as the shape of the input is reduced to only 6 colors.
+
+Here are some results that you could compare with other. On our point of view, AI model it seems working great with wallpaper.
+
+**Original**
+
+[![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)
+
+**AI processed - Aurora palette from Nordtheme**
+
+[![Converted](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-ai-aurora.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-ai-aurora.jpg)
+
+-----
+
+**Original**
+
+[![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/sh.png)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/sh.png)
+
+**AI processed - Nordtheme**
+
+[![Converted](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-sh-ai.png)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-sh-ai.png)
+
+-----
+
+**Original**
+
+[![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/valley.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/valley.jpg)
+
+**AI processed - Nordtheme**
+
+[![Converted](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-valley-ai.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-valley-ai.jpg)
+
 -----
 
 You can also convert videos into the nord palette (or others). Here is an example:  
 **Original**  
 
 https://github.com/05Alston/ImageGoNord-pip/assets/89850018/76d4c4a6-9660-4a02-9f46-e5f3f6d0147a
 
@@ -121,27 +148,16 @@
 Then you can use [some example](https://github.com/Schrodinger-Hat/ImageGoNord-pip/tree/master/docs/example) to getting started properly!
 
 ### Contributing
 - Follow the contributor guidelines
 - Follow the code style / requirements
 - Format for commit messages
 
-### TODO
-- Testing
-- Improvements on image quality and supporting any image format
-- Make contributing guidelines
-
 # Authors
 
 [TheJoin95](https://github.com/TheJoin95) & [Wabri](https://github.com/Wabri)
 
-**NOTE**: we are not (yet) affiliated with the Nordtheme or [Arcticicestudio](https://github.com/arcticicestudio).
-
-# Credits
-
-[Nordtheme](https://www.nordtheme.com/)
-
 ### License
 
-[MIT license](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
+[AGPLv3 license](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `image-go-nord-0.1.7/image_go_nord.egg-info/PKG-INFO` & `image-go-nord-1.0.1/image_go_nord.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,64 @@
 Metadata-Version: 2.1
 Name: image-go-nord
-Version: 0.1.7
-Summary: A tool for converting RGB image to Nordtheme palette
+Version: 1.0.1
+Summary: A tool to convert any RGB image or video to any theme or color palette input by the user
 Home-page: https://github.com/Schrodinger-Hat/ImageGoNord-pip
 Author: Schrodinger Hat
 Author-email: schrodinger.hat.show@gmail.com
-License: MIT
+License: AGPL-3.0
 Download-URL: https://github.com/Schrodinger-Hat/ImageGoNord-pip/releases
 Project-URL: Homepage, https://ign.schrodinger-hat.it
 Project-URL: Source, https://github.com/Schrodinger-Hat/ImageGoNord-pip
 Project-URL: Bug Reports, https://github.com/Schrodinger-Hat/ImageGoNord-pip/issues
-Keywords: nordtheme,pillow,image,conversion,rgb,color-scheme,color-palette
+Keywords: nordtheme,pillow,image,conversion,rgb,color-scheme,color-palette,linux-rice,gruvbox,catpuccin
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ImageGoNord - RGB image to Nordtheme palette
+# ImageGoNord - RGB image and video to any kind of palette or theme
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/image-go-nord)
 [![PyPI](https://img.shields.io/pypi/v/image-go-nord)](https://pypi.org/project/image-go-nord/)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
 [![Join the community on Spectrum](https://withspectrum.github.io/badge/badge.svg)](https://spectrum.chat/image-go-nord)
 
-A tool that can convert your rgb images to nordtheme palette.
+A tool that can convert your rgb images to nordtheme, gruvbox, catpuccin and many more palettes.
+Video included.
 
-This repository is a python package that can convert any sort of image into a [nordtheme](https://github.com/arcticicestudio/nord) palette image.
+This repository is a python package.
 
 You can find a demo on [the website](https://ign.schrodinger-hat.it) for testing out the package.
-
-We build also a little API hosted on Heroku to give to anyone the change to test it out by theirself. You can find the documentation on the website too.
-
 The main repository of this whole project is [ImageGoNord](https://github.com/Schrodinger-Hat/ImageGoNord).
 
+It's including an API layer, in case you'd like to set it up also for your project.
+
 ### Documentation
 
 You can find the [documentation into this repository](https://github.com/Schrodinger-Hat/ImageGoNord-pip/tree/master/docs) and also on the website.
-
-<!--
-@TODO
-- Describe very briefly but clearly what the project does.
-- State if it is out-of-the-box user-friendly, so it’s clear to the user.
-- List its most useful/innovative/noteworthy features.
-- State its goals/what problem(s) it solves.
-- Note and briefly describe any key concepts (technical, philosophical, or both) important to the user’s understanding.
-- Link to any supplementary blog posts or project main pages.
-- Note its development status.
-- If possible, include screenshots and demo videos.
--->
+If you have any questions, please reach us at us@schrodinger-hat.it
 
 ### Inspiration
 
 We are in love with Nordtheme, that is why we created this repository.
 
-[![Nord Color Palette Overview](https://raw.githubusercontent.com/arcticicestudio/nord-docs/develop/assets/images/nord/repository-color-palettes.svg?sanitize=true)](https://www.nordtheme.com/docs/colors-and-palettes)
-
-Our goal is to make a shortcut to convert anything into this theme, by starting from the images.
+Our goal is to make a shortcut to convert anything into any kind of themes, by starting from the images and going to videos.
 <br>An example could be an awesome wallpaper converted into the Nordtheme palette.
 
 We checked the commnunity and we did not find anything similar or any project that can accomplish this task. So, here we are.
 
+Of course, we resolved the issue for any kind of palette, theme and it's video supported.
+
 ### What you can do with this package
 
 You can convert any image into the nord palette (or others). Here are some examples:
 
 **Original**
 
 [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test.jpg)
@@ -87,14 +76,52 @@
 [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)
 
 
 **Processed with avg algorithm**
 
 [![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-average.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-average.jpg)
 
+
+### ImageGoNord with AI - PaletteNet
+
+We implemented the PaletteNet model with PyTorch based on [this implementation](https://github.com/AakritiKinra/PaletteNet-Implementation).
+Inside that repository you could find the paper, in case you'd like to develop and train your model.
+
+There is a lot of room for improvement as the shape of the input is reduced to only 6 colors.
+
+Here are some results that you could compare with other. On our point of view, AI model it seems working great with wallpaper.
+
+**Original**
+
+[![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile.jpg)
+
+**AI processed - Aurora palette from Nordtheme**
+
+[![Converted](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-ai-aurora.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-profile-ai-aurora.jpg)
+
+-----
+
+**Original**
+
+[![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/sh.png)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/sh.png)
+
+**AI processed - Nordtheme**
+
+[![Converted](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-sh-ai.png)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-sh-ai.png)
+
+-----
+
+**Original**
+
+[![Original](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/valley.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/valley.jpg)
+
+**AI processed - Nordtheme**
+
+[![Converted](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-valley-ai.jpg)](https://raw.githubusercontent.com/Schrodinger-Hat/ImageGoNord-pip/master/images/test-valley-ai.jpg)
+
 -----
 
 You can also convert videos into the nord palette (or others). Here is an example:  
 **Original**  
 
 https://github.com/05Alston/ImageGoNord-pip/assets/89850018/76d4c4a6-9660-4a02-9f46-e5f3f6d0147a
 
@@ -121,27 +148,16 @@
 Then you can use [some example](https://github.com/Schrodinger-Hat/ImageGoNord-pip/tree/master/docs/example) to getting started properly!
 
 ### Contributing
 - Follow the contributor guidelines
 - Follow the code style / requirements
 - Format for commit messages
 
-### TODO
-- Testing
-- Improvements on image quality and supporting any image format
-- Make contributing guidelines
-
 # Authors
 
 [TheJoin95](https://github.com/TheJoin95) & [Wabri](https://github.com/Wabri)
 
-**NOTE**: we are not (yet) affiliated with the Nordtheme or [Arcticicestudio](https://github.com/arcticicestudio).
-
-# Credits
-
-[Nordtheme](https://www.nordtheme.com/)
-
 ### License
 
-[MIT license](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
+[AGPLv3 license](https://github.com/Schrodinger-Hat/ImageGoNord-pip/blob/master/LICENSE)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `image-go-nord-0.1.7/setup.py` & `image-go-nord-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 from setuptools import setup, find_packages
 
 ROOT = pathlib.Path('.')
 README = (ROOT / "README.md").read_text()
 
 setup(
     name="image-go-nord",
-    version="0.1.7",
-    description="A tool for converting RGB image to Nordtheme palette",
+    version="1.0.1",
+    description="A tool to convert any RGB image or video to any theme or color palette input by the user",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Schrodinger-Hat/ImageGoNord-pip",
     download_url = 'https://github.com/Schrodinger-Hat/ImageGoNord-pip/releases',
-    keywords = ['nordtheme', 'pillow', 'image', 'conversion', 'rgb', 'color-scheme', 'color-palette'], 
+    keywords = ['nordtheme', 'pillow', 'image', 'conversion', 'rgb', 'color-scheme', 'color-palette', 'linux-rice', 'gruvbox', 'catpuccin'], 
     author="Schrodinger Hat",
     author_email="schrodinger.hat.show@gmail.com",
-    license="MIT",
+    license="AGPL-3.0",
     classifiers=[
         'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.7"
     ],
     project_urls={
         "Homepage": "https://ign.schrodinger-hat.it",
         "Source": "https://github.com/Schrodinger-Hat/ImageGoNord-pip",
         "Bug Reports": "https://github.com/Schrodinger-Hat/ImageGoNord-pip/issues",
     },
     packages=find_packages(),
-    package_data={'': ['*.txt', 'palettes/*.txt']},
+    package_data={'': ['*.txt', 'palettes/*.txt', 'models/*.pt', '*.pt', '*.state_dict.*']},
     include_package_data=True,
-    install_requires=["Pillow", "ffmpeg-python", "numpy"],
+    install_requires=["Pillow", "ffmpeg-python", "numpy", "torch", "skimage", "torchvision"],
     python_requires=">=3.5"
 )
```

