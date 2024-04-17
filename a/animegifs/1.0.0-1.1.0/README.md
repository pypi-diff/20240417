# Comparing `tmp/animegifs-1.0.0.tar.gz` & `tmp/animegifs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animegifs-1.0.0.tar", last modified: Tue Mar 26 16:24:04 2024, max compression
+gzip compressed data, was "animegifs-1.1.0.tar", last modified: Wed Apr 17 14:55:42 2024, max compression
```

## Comparing `animegifs-1.0.0.tar` & `animegifs-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 16:24:04.163013 animegifs-1.0.0/
--rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4917 2024-03-26 16:24:04.161014 animegifs-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4100 2024-03-26 16:22:49.000000 animegifs-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 16:24:04.144014 animegifs-1.0.0/animegifs/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-1.0.0/animegifs/__init__.py
--rw-rw-rw-   0        0        0     3115 2024-03-26 16:07:32.000000 animegifs-1.0.0/animegifs/animegifs.py
-drwxrwxrwx   0        0        0        0 2024-03-26 16:24:04.159013 animegifs-1.0.0/animegifs/distutils/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-1.0.0/animegifs/distutils/__init__.py
--rw-rw-rw-   0        0        0      923 2024-03-23 00:30:19.000000 animegifs-1.0.0/animegifs/distutils/errors.py
-drwxrwxrwx   0        0        0        0 2024-03-26 16:24:04.155012 animegifs-1.0.0/animegifs.egg-info/
--rw-rw-rw-   0        0        0     4917 2024-03-26 16:24:03.000000 animegifs-1.0.0/animegifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2024-03-26 16:24:04.000000 animegifs-1.0.0/animegifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 16:24:03.000000 animegifs-1.0.0/animegifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-03-26 16:24:03.000000 animegifs-1.0.0/animegifs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-26 16:24:03.000000 animegifs-1.0.0/animegifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-26 16:24:04.163013 animegifs-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1242 2024-03-26 16:19:54.000000 animegifs-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:55:42.402300 animegifs-1.1.0/
+-rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4834 2024-04-17 14:55:42.401300 animegifs-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4025 2024-04-17 14:45:36.000000 animegifs-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 14:55:42.386299 animegifs-1.1.0/animegifs/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-1.1.0/animegifs/__init__.py
+-rw-rw-rw-   0        0        0     3753 2024-04-17 14:52:28.000000 animegifs-1.1.0/animegifs/animegifs.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:55:42.399299 animegifs-1.1.0/animegifs/distutils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-1.1.0/animegifs/distutils/__init__.py
+-rw-rw-rw-   0        0        0      923 2024-03-23 00:30:19.000000 animegifs-1.1.0/animegifs/distutils/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:55:42.396299 animegifs-1.1.0/animegifs.egg-info/
+-rw-rw-rw-   0        0        0     4834 2024-04-17 14:55:42.000000 animegifs-1.1.0/animegifs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2024-04-17 14:55:42.000000 animegifs-1.1.0/animegifs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 14:55:42.000000 animegifs-1.1.0/animegifs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-17 14:55:42.000000 animegifs-1.1.0/animegifs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-17 14:55:42.000000 animegifs-1.1.0/animegifs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 14:55:42.402300 animegifs-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2024-04-17 14:55:23.000000 animegifs-1.1.0/setup.py
```

### Comparing `animegifs-1.0.0/LICENSE` & `animegifs-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `animegifs-1.0.0/PKG-INFO` & `animegifs-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 1.0.0
+Version: 1.1.0
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gifs,discord
 Classifier: Programming Language :: Python :: 3.8
@@ -36,32 +36,24 @@
 Version below v1.0 will not have the gifs library updated anymore and the gifs may return 404 as they were hosted on Discord.
 For troubleshoots, known errors and categories list, check below.
 
 `pip install animegifs`
 
 # HOW TO USE
 ```py
-#v0.5.3>
-from animegifs import animegifs
-
-gifs = animegifs.Animegifs()
-
-gif = gifs.get_gif(category) #return the url of the gif.
-```
-
-```py
-#v0.6>
+#v1.1.0>
 from animegifs import animegifs
 
 gifs = animegifs.Animegifs()
 
 gif = gifs.get_gif(category) #gifs.get_gif('hug') and return the url of the gif.
 mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
 title = gifs.get_animetitle(gif) #get the title of the gif's anime.
 malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page.
+categories = gifs.get_categories() #get a list of available ctegories.
 ```
 
 ```py
 #v0.6>
 from animegifs import animegifs
 
 gifs = animegifs.Animegifs()
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: animegifs Version: 1.0.0 Summary: Get random anime
+Metadata-Version: 2.1 Name: animegifs Version: 1.1.0 Summary: Get random anime
 gifs by category. Home-page: https://github.com/MarcoSa-2000/animegifs Author:
 Marco-Sa2000 Author-email: grest0grest@gmail.com License: MIT Keywords:
 anime,gif,python,anime-gifs,discord Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Requires-Python: >=3.8 Description-
@@ -10,27 +10,26 @@
 _[_P_y_P_i_ _D_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_ _S_e_r_v_e_r_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_][PyPI - Python
                            Version][GitHub watchers]
 API wrapper for animegifs. Get random anime gifs by category. Use Python
 (intended (for now) for Discord). WIP - updated in time to time. Versions below
 v0.5.3 aren't expected to work flawlessly or at all. Version below v1.0 will
 not have the gifs library updated anymore and the gifs may return 404 as they
 were hosted on Discord. For troubleshoots, known errors and categories list,
-check below. `pip install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs
+check below. `pip install animegifs` # HOW TO USE ```py #v1.1.0> from animegifs
 import animegifs gifs = animegifs.Animegifs() gif = gifs.get_gif(category)
-#return the url of the gif. ``` ```py #v0.6> from animegifs import animegifs
-gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug')
-and return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's
-anime myanimelist page. title = gifs.get_animetitle(gif) #get the title of the
-gif's anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime
-myanimelist page. ``` ```py #v0.6> from animegifs import animegifs gifs =
-animegifs.Animegifs() user_input = input() #let user send any input and search
-if that input matches a category. #if user_input == "nom": #nom as category
-doesn't exist, but is similar to bite (as example) # user_input = "bite" try:
-gif = gifs.get_gif(user_input) #return the url of the gif if the category
-exists. except animegifs.errors.CategoryError: print("not a valid gif
+#gifs.get_gif('hug') and return the url of the gif. mal = gifs.get_mal(gif)
+#get url of the gif's anime myanimelist page. title = gifs.get_animetitle(gif)
+#get the title of the gif's anime. malid = gifs.get_malId(gif) #get the ID of
+the gif's anime myanimelist page. categories = gifs.get_categories() #get a
+list of available ctegories. ``` ```py #v0.6> from animegifs import animegifs
+gifs = animegifs.Animegifs() user_input = input() #let user send any input and
+search if that input matches a category. #if user_input == "nom": #nom as
+category doesn't exist, but is similar to bite (as example) # user_input =
+"bite" try: gif = gifs.get_gif(user_input) #return the url of the gif if the
+category exists. except animegifs.errors.CategoryError: print("not a valid gif
 category.") ``` ## Category list: **A** * Attack **B** * Bite, Bloodsuck,
 Blush, Bonk, Brofist **C** * Cry, Cuddle **D** * Dance, Disgust **E** *
 Exploding **F** * Facedesk, Facepalm, Flick, Flirt **H** * Handhold, Happy,
 Harass, Highfive, Hug **I** * Icecream, Insult **K** * Kill, Kiss **L** * Lick,
 Love **M** * Marry **N** * Nod, Nosebleed, Note, Nuzzle **P** * Pat, Peck,
 Poke, Popcorn, Pout, Punch, Punish **R** * Run **S** * Sad, Scared, Shoot,
 Shrug, Sip, Slap, Smirk, Sorry, Spank, Stare **T** * Tease, Threat, Tickle,
```

### Comparing `animegifs-1.0.0/README.md` & `animegifs-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,32 +16,24 @@
 Version below v1.0 will not have the gifs library updated anymore and the gifs may return 404 as they were hosted on Discord.
 For troubleshoots, known errors and categories list, check below.
 
 `pip install animegifs`
 
 # HOW TO USE
 ```py
-#v0.5.3>
-from animegifs import animegifs
-
-gifs = animegifs.Animegifs()
-
-gif = gifs.get_gif(category) #return the url of the gif.
-```
-
-```py
-#v0.6>
+#v1.1.0>
 from animegifs import animegifs
 
 gifs = animegifs.Animegifs()
 
 gif = gifs.get_gif(category) #gifs.get_gif('hug') and return the url of the gif.
 mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
 title = gifs.get_animetitle(gif) #get the title of the gif's anime.
 malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page.
+categories = gifs.get_categories() #get a list of available ctegories.
 ```
 
 ```py
 #v0.6>
 from animegifs import animegifs
 
 gifs = animegifs.Animegifs()
```

#### html2text {}

```diff
@@ -2,27 +2,26 @@
 _[_P_y_P_i_ _D_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_ _S_e_r_v_e_r_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_][PyPI - Python
                            Version][GitHub watchers]
 API wrapper for animegifs. Get random anime gifs by category. Use Python
 (intended (for now) for Discord). WIP - updated in time to time. Versions below
 v0.5.3 aren't expected to work flawlessly or at all. Version below v1.0 will
 not have the gifs library updated anymore and the gifs may return 404 as they
 were hosted on Discord. For troubleshoots, known errors and categories list,
-check below. `pip install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs
+check below. `pip install animegifs` # HOW TO USE ```py #v1.1.0> from animegifs
 import animegifs gifs = animegifs.Animegifs() gif = gifs.get_gif(category)
-#return the url of the gif. ``` ```py #v0.6> from animegifs import animegifs
-gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug')
-and return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's
-anime myanimelist page. title = gifs.get_animetitle(gif) #get the title of the
-gif's anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime
-myanimelist page. ``` ```py #v0.6> from animegifs import animegifs gifs =
-animegifs.Animegifs() user_input = input() #let user send any input and search
-if that input matches a category. #if user_input == "nom": #nom as category
-doesn't exist, but is similar to bite (as example) # user_input = "bite" try:
-gif = gifs.get_gif(user_input) #return the url of the gif if the category
-exists. except animegifs.errors.CategoryError: print("not a valid gif
+#gifs.get_gif('hug') and return the url of the gif. mal = gifs.get_mal(gif)
+#get url of the gif's anime myanimelist page. title = gifs.get_animetitle(gif)
+#get the title of the gif's anime. malid = gifs.get_malId(gif) #get the ID of
+the gif's anime myanimelist page. categories = gifs.get_categories() #get a
+list of available ctegories. ``` ```py #v0.6> from animegifs import animegifs
+gifs = animegifs.Animegifs() user_input = input() #let user send any input and
+search if that input matches a category. #if user_input == "nom": #nom as
+category doesn't exist, but is similar to bite (as example) # user_input =
+"bite" try: gif = gifs.get_gif(user_input) #return the url of the gif if the
+category exists. except animegifs.errors.CategoryError: print("not a valid gif
 category.") ``` ## Category list: **A** * Attack **B** * Bite, Bloodsuck,
 Blush, Bonk, Brofist **C** * Cry, Cuddle **D** * Dance, Disgust **E** *
 Exploding **F** * Facedesk, Facepalm, Flick, Flirt **H** * Handhold, Happy,
 Harass, Highfive, Hug **I** * Icecream, Insult **K** * Kill, Kiss **L** * Lick,
 Love **M** * Marry **N** * Nod, Nosebleed, Note, Nuzzle **P** * Pat, Peck,
 Poke, Popcorn, Pout, Punch, Punish **R** * Run **S** * Sad, Scared, Shoot,
 Shrug, Sip, Slap, Smirk, Sorry, Spank, Stare **T** * Tease, Threat, Tickle,
```

### Comparing `animegifs-1.0.0/animegifs/animegifs.py` & `animegifs-1.1.0/animegifs/animegifs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from animegifs.distutils import errors
 import requests
 import urllib.parse
 
 version = "v3"
 
 def request_api(type, arg):
-    arg = urllib.parse.quote(arg)
+    try:
+        arg = urllib.parse.quote(arg)
+    except TypeError:
+        arg = None
     if type == "get_gif":
         gif_url = requests.get(f"https://animegifs-enkidu.koyeb.app/{version}/api/?category={arg}")
         if gif_url.status_code != 200:
             raise errors.CategoryError
         data = gif_url.json()
         gif = data['gif']
         return gif
@@ -24,14 +27,19 @@
         mal_id = data['mal_id']
         return mal_id
     elif type == "get_animetitle":
         gif_animetitle = requests.get(f"https://animegifs-enkidu.koyeb.app/{version}/get_animetitle/?gif={arg}")
         data = gif_animetitle.json()
         animetitle = data['animetitle']
         return animetitle
+    elif type == "get_categories":
+        categories = requests.get(f"https://animegifs-enkidu.koyeb.app/{version}/get_categories")
+        data = categories.json()
+        categories = data['categories']
+        return categories
 
 class Animegifs:
 
     def __init__(self):
         self.category = None
 
     def get_gif(self, category: str) -> str:
@@ -71,15 +79,15 @@
         """
         Return the myanimelist ID of the gif's anime.
 
         Args:
             gif (url: str)
 
         Returns:
-            malid: malId -> int
+            mal_id: mal_id -> int
         """
         mal_id = request_api("get_mal_id", gif)
         if mal_id == "null":
             raise errors.CategoryError
         return mal_id
 
     def get_animetitle(self, gif) -> str:
@@ -92,7 +100,18 @@
         Returns:
             title: title -> str
         """
         animetitle = request_api("get_animetitle", gif)
         if animetitle == "null":
             raise errors.CategoryError
         return animetitle
+    def get_categories(self) -> list:
+        """
+        Return the list of the available categories.
+
+        Returns:
+            categories: categories -> list
+        """
+        categories = request_api("get_categories", None)
+        if categories == "null":
+            raise errors.CategoryError
+        return categories
```

### Comparing `animegifs-1.0.0/animegifs/distutils/errors.py` & `animegifs-1.1.0/animegifs/distutils/errors.py`

 * *Files identical despite different names*

### Comparing `animegifs-1.0.0/animegifs.egg-info/PKG-INFO` & `animegifs-1.1.0/animegifs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 1.0.0
+Version: 1.1.0
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gifs,discord
 Classifier: Programming Language :: Python :: 3.8
@@ -36,32 +36,24 @@
 Version below v1.0 will not have the gifs library updated anymore and the gifs may return 404 as they were hosted on Discord.
 For troubleshoots, known errors and categories list, check below.
 
 `pip install animegifs`
 
 # HOW TO USE
 ```py
-#v0.5.3>
-from animegifs import animegifs
-
-gifs = animegifs.Animegifs()
-
-gif = gifs.get_gif(category) #return the url of the gif.
-```
-
-```py
-#v0.6>
+#v1.1.0>
 from animegifs import animegifs
 
 gifs = animegifs.Animegifs()
 
 gif = gifs.get_gif(category) #gifs.get_gif('hug') and return the url of the gif.
 mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
 title = gifs.get_animetitle(gif) #get the title of the gif's anime.
 malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page.
+categories = gifs.get_categories() #get a list of available ctegories.
 ```
 
 ```py
 #v0.6>
 from animegifs import animegifs
 
 gifs = animegifs.Animegifs()
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: animegifs Version: 1.0.0 Summary: Get random anime
+Metadata-Version: 2.1 Name: animegifs Version: 1.1.0 Summary: Get random anime
 gifs by category. Home-page: https://github.com/MarcoSa-2000/animegifs Author:
 Marco-Sa2000 Author-email: grest0grest@gmail.com License: MIT Keywords:
 anime,gif,python,anime-gifs,discord Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Requires-Python: >=3.8 Description-
@@ -10,27 +10,26 @@
 _[_P_y_P_i_ _D_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_ _S_e_r_v_e_r_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_][PyPI - Python
                            Version][GitHub watchers]
 API wrapper for animegifs. Get random anime gifs by category. Use Python
 (intended (for now) for Discord). WIP - updated in time to time. Versions below
 v0.5.3 aren't expected to work flawlessly or at all. Version below v1.0 will
 not have the gifs library updated anymore and the gifs may return 404 as they
 were hosted on Discord. For troubleshoots, known errors and categories list,
-check below. `pip install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs
+check below. `pip install animegifs` # HOW TO USE ```py #v1.1.0> from animegifs
 import animegifs gifs = animegifs.Animegifs() gif = gifs.get_gif(category)
-#return the url of the gif. ``` ```py #v0.6> from animegifs import animegifs
-gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug')
-and return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's
-anime myanimelist page. title = gifs.get_animetitle(gif) #get the title of the
-gif's anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime
-myanimelist page. ``` ```py #v0.6> from animegifs import animegifs gifs =
-animegifs.Animegifs() user_input = input() #let user send any input and search
-if that input matches a category. #if user_input == "nom": #nom as category
-doesn't exist, but is similar to bite (as example) # user_input = "bite" try:
-gif = gifs.get_gif(user_input) #return the url of the gif if the category
-exists. except animegifs.errors.CategoryError: print("not a valid gif
+#gifs.get_gif('hug') and return the url of the gif. mal = gifs.get_mal(gif)
+#get url of the gif's anime myanimelist page. title = gifs.get_animetitle(gif)
+#get the title of the gif's anime. malid = gifs.get_malId(gif) #get the ID of
+the gif's anime myanimelist page. categories = gifs.get_categories() #get a
+list of available ctegories. ``` ```py #v0.6> from animegifs import animegifs
+gifs = animegifs.Animegifs() user_input = input() #let user send any input and
+search if that input matches a category. #if user_input == "nom": #nom as
+category doesn't exist, but is similar to bite (as example) # user_input =
+"bite" try: gif = gifs.get_gif(user_input) #return the url of the gif if the
+category exists. except animegifs.errors.CategoryError: print("not a valid gif
 category.") ``` ## Category list: **A** * Attack **B** * Bite, Bloodsuck,
 Blush, Bonk, Brofist **C** * Cry, Cuddle **D** * Dance, Disgust **E** *
 Exploding **F** * Facedesk, Facepalm, Flick, Flirt **H** * Handhold, Happy,
 Harass, Highfive, Hug **I** * Icecream, Insult **K** * Kill, Kiss **L** * Lick,
 Love **M** * Marry **N** * Nod, Nosebleed, Note, Nuzzle **P** * Pat, Peck,
 Poke, Popcorn, Pout, Punch, Punish **R** * Run **S** * Sad, Scared, Shoot,
 Shrug, Sip, Slap, Smirk, Sorry, Spank, Stare **T** * Tease, Threat, Tickle,
```

### Comparing `animegifs-1.0.0/setup.py` & `animegifs-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 LONG_DESCRIPTION = long_description
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 
 setup(
     name='animegifs',
     package_dir={"anime_gifs": "animegifs"},
     packages=["animegifs", "animegifs.distutils"],
     version=VERSION,
     description='Get random anime gifs by category.',
```

