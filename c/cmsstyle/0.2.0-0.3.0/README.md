# Comparing `tmp/cmsstyle-0.2.0.tar.gz` & `tmp/cmsstyle-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Feb  8 17:13:51 2024, max compression
+gzip compressed data, last modified: Wed Apr 17 20:59:02 2024, max compression
```

## Comparing `cmsstyle-0.2.0.tar` & `cmsstyle-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       24 2024-02-08 17:13:51.000000 cmsstyle-0.2.0/src/cmsstyle/__init__.py
--rw-r--r--   0        0        0      411 2024-02-08 17:13:51.000000 cmsstyle-0.2.0/src/cmsstyle/_version.py
--rw-r--r--   0        0        0    22514 2024-02-08 17:13:51.000000 cmsstyle-0.2.0/src/cmsstyle/cmsstyle.py
--rw-r--r--   0        0        0     1246 2024-02-08 17:13:51.000000 cmsstyle-0.2.0/.gitignore
--rw-r--r--   0        0        0     1082 2024-02-08 17:13:51.000000 cmsstyle-0.2.0/LICENSE
--rw-r--r--   0        0        0      192 2024-02-08 17:13:51.000000 cmsstyle-0.2.0/README.md
--rw-r--r--   0        0        0     1524 2024-02-08 17:13:51.000000 cmsstyle-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1446 2024-02-08 17:13:51.000000 cmsstyle-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       24 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/src/cmsstyle/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/src/cmsstyle/_version.py
+-rw-r--r--   0        0        0    23845 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/src/cmsstyle/cmsstyle.py
+-rw-r--r--   0        0        0     1246 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1082 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/LICENSE
+-rw-r--r--   0        0        0      192 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/README.md
+-rw-r--r--   0        0        0     1524 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1446 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/PKG-INFO
```

### Comparing `cmsstyle-0.2.0/src/cmsstyle/cmsstyle.py` & `cmsstyle-0.3.0/src/cmsstyle/cmsstyle.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 import ROOT as rt
 from array import array
 
 rt.gROOT.SetBatch(rt.kTRUE)
 
 cms_lumi = "Run 2, 138 fb^{#minus1}"
-cms_energy = "13"
+cms_energy = "13 TeV"
 
 
-def SetEnergy(energy):
+def SetEnergy(energy, unit = "TeV"):
     global cms_energy
-    cms_energy = str(energy)
+    cms_energy = str(energy) + " " + unit
 
 
 def SetLumi(lumi, unit="fb", round_lumi=False):
     global cms_lumi
     if lumi != "":
         cms_lumi = f"{lumi:.0f}" if round_lumi else f"{lumi}"
         cms_lumi += f" {unit}^{{#minus1}}"
@@ -64,14 +64,44 @@
 kRectangular = False
 
 # Petroff color schemes for 6, 8 and 10 colors, respectively
 petroff_6 = ["#5790fc", "#f89c20", "#e42536", "#964a8b", "#9c9ca1", "#7a21dd"]
 petroff_8 = ["#1845fb", "#ff5e02", "#c91f16", "#c849a9", "#adad7d", "#86c8dd", "#578dff", "#656364"]
 petroff_10 = ["#3f90da", "#ffa90e", "#bd1f01", "#94a4a2", "#832db6", "#a96b59", "#e76300", "#b9ac70", "#717581", "#92dadd"]
 
+class p6:
+    kBlue = rt.TColor.GetColor("#5790fc")
+    kYellow = rt.TColor.GetColor("#f89c20")
+    kRed = rt.TColor.GetColor("#e42536")
+    kGrape = rt.TColor.GetColor("#964a8b")
+    kGray = rt.TColor.GetColor("#9c9ca1")
+    kViolet = rt.TColor.GetColor("#7a21dd")
+
+class p8:
+    kBlue = rt.TColor.GetColor("#1845fb")
+    kOrange = rt.TColor.GetColor("#ff5e02")
+    kRed = rt.TColor.GetColor("#c91f16")
+    kPink = rt.TColor.GetColor("#c849a9")
+    kGreen = rt.TColor.GetColor("#adad7d")
+    kCyan = rt.TColor.GetColor("#86c8dd")
+    kAzure = rt.TColor.GetColor("#578dff")
+    kGray = rt.TColor.GetColor("#656364")
+
+class p10:
+    kBlue = rt.TColor.GetColor("#3f90da")
+    kYellow = rt.TColor.GetColor("#ffa90e")
+    kRed = rt.TColor.GetColor("#bd1f01")
+    kGray = rt.TColor.GetColor("#94a4a2")
+    kViolet = rt.TColor.GetColor("#832db6")
+    kBrown = rt.TColor.GetColor("#a96b59")
+    kOrange = rt.TColor.GetColor("#e76300")
+    kGreen = rt.TColor.GetColor("#b9ac70")
+    kAsh = rt.TColor.GetColor("#717581")
+    kCyan = rt.TColor.GetColor("#92dadd")
+
 # Define an alternative color palette and a function to set it
 MyPalette = None
 
 
 def CreateAlternativePalette(alpha=1):
     red_values = array("d", [0.00, 0.00, 1.00, 0.70])
     green_values = array("d", [0.30, 0.50, 0.70, 0.00])
@@ -296,15 +326,15 @@
     r = pad.GetRightMargin()
     b = pad.GetBottomMargin()
     outOfFrame_posY = 1 - t + lumiTextOffset * t
     pad.cd()
     lumiText = ""
     lumiText += cms_lumi
     if cms_energy != "":
-        lumiText += " (" + cms_energy + " TeV)"
+        lumiText += " (" + cms_energy + ")"
     if scaleLumi:
         lumiText = ScaleText(lumiText, scale=scaleLumi)
 
     def drawText(text, posX, posY, font, align, size):
         latex.SetTextFont(font)
         latex.SetTextAlign(align)
         latex.SetTextSize(size)
@@ -680,15 +710,15 @@
 
 def is_valid_hex_color(hex_color):
     hex_color_pattern = re.compile(r'^#(?:[0-9a-fA-F]{3}){1,2}$')
     
     return bool(hex_color_pattern.match(hex_color))
 
 
-def cmsDrawStack(stack, legend, MC,  data = None, palette = None):
+def cmsDrawStack(stack, legend, MC, data = None, palette = None, invertLegendEntries = True):
     """Draws stacked histograms and data on a pre-defined stackplot and fills a pre-defined legend, using a user-defined or default list (palette) of hex colors"""
     
     is_user_palette_valid = False
 
     if palette != None:
         is_user_palette_valid = all(is_valid_hex_color(color) for color in palette)
         if is_user_palette_valid:
@@ -704,19 +734,24 @@
         elif len(MC.keys()) < 9:
             palette_ = petroff_8
         else:
             palette_ = petroff_10
             if len(MC.keys()) > len(palette_):
                 print("Length of largest default palette is smaller than the number of histograms to be drawn, wrap around is enabled")
 
+    # Add legend entries in inverse order
+    if invertLegendEntries:
+        for n, item in reversed(list(enumerate(MC.items()))):
+            legend.AddEntry(item[1], item[0], "f")
     for n, item in enumerate(MC.items()):
         item[1].SetLineColor(rt.TColor.GetColor(palette_[n%len(palette_)]))
         item[1].SetFillColor(rt.TColor.GetColor(palette_[n%len(palette_)]))
-        stack.Add(item[1]) 
-        legend.AddEntry(item[1], item[0], "f")
+        stack.Add(item[1])
+        if not invertLegendEntries:
+            legend.AddEntry(item[1], item[0], "f")
         stack.Draw("HIST SAME")
     
     if data != None:
         cmsDraw(data, "P", mcolor=rt.kBlack)
         legend.AddEntry(data, "Data", "lp")
```

### Comparing `cmsstyle-0.2.0/.gitignore` & `cmsstyle-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cmsstyle-0.2.0/LICENSE` & `cmsstyle-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmsstyle-0.2.0/pyproject.toml` & `cmsstyle-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cmsstyle-0.2.0/PKG-INFO` & `cmsstyle-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: cmsstyle
-Version: 0.2.0
+Version: 0.3.0
 Project-URL: Homepage, https://github.com/cms-cat/cms-root-style
 Project-URL: Documentation, https://github.com/cms-cat/cms-root-style
 Project-URL: Bug Tracker, https://github.com/cms-cat/cms-root-style/issues
 Project-URL: Discussions, https://github.com/cms-cat/cms-root-style/discussions
 Author-email: Andrzej Novak <andrzej.novak@cern.ch>, Tommaso Tedeschi <tommaso.tedeschi@cern.ch>, Clemens Lange <clemens.lange@cern.ch>, Piergiulio Lenzi <piergiulio.lenzi@cern.ch>, Andrea Malara <andrea.malara@cern.ch>
 Maintainer-email: CMS CAT Group <cms-phys-conveners-CAT@cern.ch>
 License-File: LICENSE
```

