# Comparing `tmp/modelisation-0.0.7-py3-none-any.whl.zip` & `tmp/modelisation-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4947 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    12075 b- defN 24-Feb-15 15:11 modelisation.py
--rw-rw-rw-  2.0 fat     2188 b- defN 24-Feb-15 15:20 modelisation-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-15 15:20 modelisation-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Feb-15 15:20 modelisation-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      391 b- defN 24-Feb-15 15:20 modelisation-0.0.7.dist-info/RECORD
-5 files, 14759 bytes uncompressed, 4219 bytes compressed:  71.4%
+Zip file size: 5078 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    12867 b- defN 24-Mar-24 17:50 modelisation.py
+-rw-rw-rw-  2.0 fat     2188 b- defN 24-Apr-17 10:22 modelisation-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-17 10:22 modelisation-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-17 10:22 modelisation-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      391 b- defN 24-Apr-17 10:22 modelisation-0.0.8.dist-info/RECORD
+5 files, 15551 bytes uncompressed, 4350 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: modelisation.py
 Comment: 
 
-Filename: modelisation-0.0.7.dist-info/METADATA
+Filename: modelisation-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: modelisation-0.0.7.dist-info/WHEEL
+Filename: modelisation-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: modelisation-0.0.7.dist-info/top_level.txt
+Filename: modelisation-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: modelisation-0.0.7.dist-info/RECORD
+Filename: modelisation-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## modelisation.py

```diff
@@ -1,9 +1,8 @@
-# Bibliothèque permettant de réaliser la modélisation de points expérimentaux 
-# © Stéphane LAURENT 2024
+# bibliothèque pour modéliser des graphiques : Stéphane LAURENT
 
 import matplotlib.pyplot as plt # importation d'un sous module (pyplot) de la bibliothèque matplotlib sous le nom plt
 import numpy as np # Importation du module numpy afin de lire le contenu du fichier csv
 from scipy.optimize import curve_fit
 from matplotlib.path import Path
 from matplotlib.widgets import LassoSelector
 from matplotlib.widgets import Cursor    # pour afficher un réticule
@@ -174,15 +173,18 @@
         
             
 
 def affichage_message_erreur():
     global message_erreur
     message_erreur=plt.figtext(0.6, 0.5, 'Modélisation impossible !',fontsize = 16, fontweight = 'bold', color = 'red', backgroundcolor = 'yellow',horizontalalignment = 'center', verticalalignment = 'center')
         
-
+def message_modele_inconnue():
+    global message_erreur
+    message_erreur=plt.figtext(0.6, 0.5, 'Modélisation impossible\nmodèle inconnu !',fontsize = 16, fontweight = 'bold', color = 'red', backgroundcolor = 'yellow',horizontalalignment = 'center', verticalalignment = 'center')
+  
 ### Modélisation ###
 
 def lineaire(x, a):
     return a * x
 
 def affine(x, a, b):
     return a * x + b
@@ -208,15 +210,15 @@
     else:
         couleur = "blue"
         
     points_modelisation.append(plt.plot(x_modelisation, y_modelisation, color=couleur, linestyle='solid', linewidth=1.5, label = caracteristiques_modele))
     
     legende = plt.legend(loc = 'upper left', title = titre_legende, title_fontsize='large')
     legende._legend_box.align = "left"
-    
+    plt.tight_layout() # ajuste automatiquement de l’espace autour du graphique
     
         
 def afficher_modele_affine(x1, y1):
     global titre_legende
     
     try:
         popt,pcov = curve_fit(affine, x1, y1) 
@@ -318,51 +320,64 @@
     canvas = plt.gca().figure.canvas
     
     plt.gcf().canvas.mpl_connect("key_press_event", touche_clavier)
     
     x_points = x1
     y_points = y1
     
-    if modele.lower() == "double-affine":
-        modele = "double_affine"
-        
+    modele = modele.strip() # supprime les espaces surperflus
     modele_choisi = modele.lower()
     
+    if modele_choisi == "exp croissante" or modele_choisi == "exp-croissante":
+        modele_choisi = "exp_croissante"
+       
+    if modele_choisi == "exp decroissante" or modele_choisi == "exp-decroissante" or modele_choisi =="exp décroissante" or modele_choisi == "exp-décroissante" or modele_choisi == "exp_décroissante":
+        modele_choisi = "exp_decroissante"
+        
+    if modele_choisi == "double-affine" or modele_choisi == "double affine":
+        modele_choisi = "double_affine"
+    
+    
     xmin, xmax = plt.gca().xaxis.get_view_interval() # valeurs extrêmes sur l'axe des x
     
     if modele_choisi == "lineaire" or modele_choisi == "linéaire":
         afficher_modele_lineaire(x_points, y_points)
         selection_lasso(x_points, y_points)        
-        return 
+         
         
-    if modele_choisi == "affine":
+    elif modele_choisi == "affine":
         afficher_modele_affine(x_points, y_points)
         selection_lasso(x_points, y_points)              
-        return
+        
     
     
-    if modele_choisi == "parabole":
+    elif modele_choisi == "parabole":
         afficher_modele_parabole(x_points, y_points)
         selection_lasso(x_points, y_points)
-        return
+        
     
-    if modele_choisi == "exp_decroissante" or modele_choisi == "exp-decroissante":
+    elif modele_choisi == "exp_decroissante":
         afficher_modele_exp_decroissante(x_points, y_points)
         selection_lasso(x_points, y_points)
-        return
+        
         
     
-    if modele_choisi == "exp_croissante" or modele_choisi == "exp-croissante":
+    elif modele_choisi == "exp_croissante":
         afficher_modele_exp_croissante(x_points, y_points)
         selection_lasso(x_points, y_points)
-        return 
+         
     
-    if modele_choisi == "double_affine":
+    elif modele_choisi == "double_affine":
         global nbr_modelisation # nombre de droite modélisées pour "double_affine"
         nbr_modelisation = 0
         selection_lasso(x_points, y_points)
+        
+    else:
+        message_modele_inconnue()
+        
+    
 
 reticule = Cursor(plt.gca(), useblit=True, color='black', linewidth=1, linestyle='dashed')
 reticule.visible = False
 
 warnings.filterwarnings(action='ignore') # empêcher l'affichage d'avertissement Python
```

## Comparing `modelisation-0.0.7.dist-info/METADATA` & `modelisation-0.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelisation
-Version: 0.0.7
+Version: 0.0.8
 Summary: Modéliser des points expérimentaux
 Home-page: https://urlz.fr/pu0X
 Author: LAURENT Stéphane
 License: MIT
 Keywords: modelisation physique chimie lycée linéaire affine linear regression physical chemistry modeling
 Platform: UNKNOWN
 Classifier: Topic :: Education
```

