# Comparing `tmp/starrailcard-2.1.2.tar.gz` & `tmp/starrailcard-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailcard-2.1.2.tar", max compression
+gzip compressed data, was "starrailcard-2.1.3.tar", max compression
```

## Comparing `starrailcard-2.1.2.tar` & `starrailcard-2.1.3.tar`

### file list

```diff
@@ -1,48 +1,51 @@
--rw-r--r--   0        0        0     1721 2024-03-20 15:38:40.776791 starrailcard-2.1.2/LICENSE
--rw-r--r--   0        0        0     1147 2024-04-06 19:08:26.820420 starrailcard-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     3642 2024-03-18 20:36:48.857949 starrailcard-2.1.2/README.md
--rw-r--r--   0        0        0       75 2024-03-15 20:07:42.107466 starrailcard-2.1.2/starrailcard/__init__.py
--rw-r--r--   0        0        0     9736 2024-04-02 12:01:15.004451 starrailcard-2.1.2/starrailcard/client.py
--rw-r--r--   0        0        0      106 2024-03-20 15:35:34.777763 starrailcard-2.1.2/starrailcard/requirements.txt
--rw-r--r--   0        0        0     1049 2024-04-06 18:57:38.219761 starrailcard-2.1.2/starrailcard/src/api/api.py
--rw-r--r--   0        0        0   201292 2023-10-12 08:13:59.547042 starrailcard-2.1.2/starrailcard/src/assets/font/font_hsr.ttf
--rw-r--r--   0        0        0     1751 2024-03-28 18:26:38.347683 starrailcard-2.1.2/starrailcard/src/data/avatar.json
--rw-r--r--   0        0        0      252 2024-03-28 18:26:38.460098 starrailcard-2.1.2/starrailcard/src/data/element.json
--rw-r--r--   0        0        0       70 2024-03-28 18:26:38.462097 starrailcard-2.1.2/starrailcard/src/data/keys.json
--rw-r--r--   0        0        0      293 2024-03-28 18:26:38.423267 starrailcard-2.1.2/starrailcard/src/data/paths.json
--rw-r--r--   0        0        0     1915 2024-03-28 18:26:38.386139 starrailcard-2.1.2/starrailcard/src/data/relict_sets.json
--rw-r--r--   0        0        0     4947 2024-03-28 18:26:38.266305 starrailcard-2.1.2/starrailcard/src/data/stats.json
--rw-r--r--   0        0        0     4738 2024-03-28 18:26:38.308097 starrailcard-2.1.2/starrailcard/src/data/weapons.json
--rw-r--r--   0        0        0     6696 2024-04-06 18:31:53.629800 starrailcard-2.1.2/starrailcard/src/generator/style_profile_phone.py
--rw-r--r--   0        0        0    23968 2024-03-24 23:40:49.094126 starrailcard-2.1.2/starrailcard/src/generator/style_relict_score.py
--rw-r--r--   0        0        0    29882 2024-04-06 19:07:58.575836 starrailcard-2.1.2/starrailcard/src/generator/style_ticket.py
--rw-r--r--   0        0        0     8410 2024-03-13 13:47:49.948737 starrailcard-2.1.2/starrailcard/src/model/api_mihomo.py
--rw-r--r--   0        0        0     4757 2024-03-27 19:18:51.084890 starrailcard-2.1.2/starrailcard/src/model/StarRailCard.py
--rw-r--r--   0        0        0     4065 2024-03-13 13:47:58.864230 starrailcard-2.1.2/starrailcard/src/model/style.py
--rw-r--r--   0        0        0      493 2024-03-13 13:48:02.345029 starrailcard-2.1.2/starrailcard/src/model/ukrainization_model.py
--rw-r--r--   0        0        0      845 2024-03-13 13:48:07.469416 starrailcard-2.1.2/starrailcard/src/model/utils_model.py
--rw-r--r--   0        0        0      373 2024-04-06 18:51:59.632223 starrailcard-2.1.2/starrailcard/src/tools/calculator/src/assets/max.json
--rw-r--r--   0        0        0       49 2024-04-06 18:52:00.222443 starrailcard-2.1.2/starrailcard/src/tools/calculator/src/assets/relic_id.json
--rw-r--r--   0        0        0     3434 2024-04-06 18:52:00.479448 starrailcard-2.1.2/starrailcard/src/tools/calculator/src/assets/rolls.json
--rw-r--r--   0        0        0    92881 2024-04-06 18:52:01.246844 starrailcard-2.1.2/starrailcard/src/tools/calculator/src/assets/score.json
--rw-r--r--   0        0        0     1959 2024-03-13 13:47:21.923389 starrailcard-2.1.2/starrailcard/src/tools/calculator/src/utils.py
--rw-r--r--   0        0        0     5747 2024-04-01 14:16:17.689304 starrailcard-2.1.2/starrailcard/src/tools/calculator/stats.py
--rw-r--r--   0        0        0     2526 2024-02-22 12:56:12.220916 starrailcard-2.1.2/starrailcard/src/tools/cashe.py
--rw-r--r--   0        0        0      563 2024-03-28 16:30:39.886551 starrailcard-2.1.2/starrailcard/src/tools/enums.py
--rw-r--r--   0        0        0    10136 2024-02-23 21:20:24.125982 starrailcard-2.1.2/starrailcard/src/tools/git.py
--rw-r--r--   0        0        0     6100 2024-03-28 17:26:04.740937 starrailcard-2.1.2/starrailcard/src/tools/http.py
--rw-r--r--   0        0        0      940 2024-03-28 18:26:46.684860 starrailcard-2.1.2/starrailcard/src/tools/json_data.py
--rw-r--r--   0        0        0     6345 2024-04-06 18:55:54.476858 starrailcard-2.1.2/starrailcard/src/tools/options.py
--rw-r--r--   0        0        0      199 2024-02-18 13:46:16.566296 starrailcard-2.1.2/starrailcard/src/tools/pill/__init__.py
--rw-r--r--   0        0        0     3854 2024-02-22 12:55:07.451038 starrailcard-2.1.2/starrailcard/src/tools/pill/color.py
--rw-r--r--   0        0        0     2330 2024-02-22 13:03:49.291296 starrailcard-2.1.2/starrailcard/src/tools/pill/color_controle.py
--rw-r--r--   0        0        0     5518 2024-02-25 12:31:53.901150 starrailcard-2.1.2/starrailcard/src/tools/pill/grandiend_v2.py
--rw-r--r--   0        0        0     3284 2024-02-22 12:55:28.873148 starrailcard-2.1.2/starrailcard/src/tools/pill/grandient_v1.py
--rw-r--r--   0        0        0     3833 2024-04-06 18:31:03.220838 starrailcard-2.1.2/starrailcard/src/tools/pill/image_controle.py
--rw-r--r--   0        0        0     5106 2024-02-22 12:55:59.845148 starrailcard-2.1.2/starrailcard/src/tools/pill/style_editor.py
--rw-r--r--   0        0        0     2116 2024-02-22 13:01:14.697378 starrailcard-2.1.2/starrailcard/src/tools/pill/text_controle.py
--rw-r--r--   0        0        0     2360 2024-03-13 13:31:40.291343 starrailcard-2.1.2/starrailcard/src/tools/translator.py
--rw-r--r--   0        0        0     6585 2024-02-22 12:57:06.983609 starrailcard-2.1.2/starrailcard/src/tools/treePaths.py
--rw-r--r--   0        0        0     1748 2024-03-28 18:26:54.868269 starrailcard-2.1.2/starrailcard/src/tools/ukrainization.py
--rw-r--r--   0        0        0     6884 2024-03-18 20:19:11.991157 starrailcard-2.1.2/starrailcard/utils.py
--rw-r--r--   0        0        0     4999 1970-01-01 00:00:00.000000 starrailcard-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1721 2024-03-20 15:38:40.776791 starrailcard-2.1.3/LICENSE
+-rw-r--r--   0        0        0     1165 2024-04-17 16:14:22.125126 starrailcard-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3642 2024-03-18 20:36:48.857949 starrailcard-2.1.3/README.md
+-rw-r--r--   0        0        0       75 2024-03-15 20:07:42.107466 starrailcard-2.1.3/starrailcard/__init__.py
+-rw-r--r--   0        0        0    11836 2024-04-17 16:12:22.105894 starrailcard-2.1.3/starrailcard/client.py
+-rw-r--r--   0        0        0      106 2024-03-20 15:35:34.777763 starrailcard-2.1.3/starrailcard/requirements.txt
+-rw-r--r--   0        0        0     2461 2024-04-14 21:56:24.992763 starrailcard-2.1.3/starrailcard/src/api/api.py
+-rw-r--r--   0        0        0     3487 2024-04-14 22:43:00.884583 starrailcard-2.1.3/starrailcard/src/api/enka.py
+-rw-r--r--   0        0        0    25187 2024-04-14 22:52:21.950058 starrailcard-2.1.3/starrailcard/src/api/enka_parsed.py
+-rw-r--r--   0        0        0      487 2024-04-09 16:19:13.263140 starrailcard-2.1.3/starrailcard/src/api/error.py
+-rw-r--r--   0        0        0   201292 2023-10-12 08:13:59.547042 starrailcard-2.1.3/starrailcard/src/assets/font/font_hsr.ttf
+-rw-r--r--   0        0        0     1751 2024-03-28 18:26:38.347683 starrailcard-2.1.3/starrailcard/src/data/avatar.json
+-rw-r--r--   0        0        0      252 2024-03-28 18:26:38.460098 starrailcard-2.1.3/starrailcard/src/data/element.json
+-rw-r--r--   0        0        0       70 2024-03-28 18:26:38.462097 starrailcard-2.1.3/starrailcard/src/data/keys.json
+-rw-r--r--   0        0        0      293 2024-03-28 18:26:38.423267 starrailcard-2.1.3/starrailcard/src/data/paths.json
+-rw-r--r--   0        0        0     1915 2024-03-28 18:26:38.386139 starrailcard-2.1.3/starrailcard/src/data/relict_sets.json
+-rw-r--r--   0        0        0     4947 2024-03-28 18:26:38.266305 starrailcard-2.1.3/starrailcard/src/data/stats.json
+-rw-r--r--   0        0        0     4738 2024-03-28 18:26:38.308097 starrailcard-2.1.3/starrailcard/src/data/weapons.json
+-rw-r--r--   0        0        0     6696 2024-04-06 18:31:53.629800 starrailcard-2.1.3/starrailcard/src/generator/style_profile_phone.py
+-rw-r--r--   0        0        0    24567 2024-04-17 16:11:52.691388 starrailcard-2.1.3/starrailcard/src/generator/style_relict_score.py
+-rw-r--r--   0        0        0    30356 2024-04-17 16:11:41.400283 starrailcard-2.1.3/starrailcard/src/generator/style_ticket.py
+-rw-r--r--   0        0        0    11769 2024-04-14 20:59:53.695835 starrailcard-2.1.3/starrailcard/src/model/api_mihomo.py
+-rw-r--r--   0        0        0     4759 2024-04-13 14:26:08.588002 starrailcard-2.1.3/starrailcard/src/model/StarRailCard.py
+-rw-r--r--   0        0        0     4065 2024-03-13 13:47:58.864230 starrailcard-2.1.3/starrailcard/src/model/style.py
+-rw-r--r--   0        0        0      493 2024-03-13 13:48:02.345029 starrailcard-2.1.3/starrailcard/src/model/ukrainization_model.py
+-rw-r--r--   0        0        0      845 2024-03-13 13:48:07.469416 starrailcard-2.1.3/starrailcard/src/model/utils_model.py
+-rw-r--r--   0        0        0      373 2024-04-06 18:51:59.632223 starrailcard-2.1.3/starrailcard/src/tools/calculator/src/assets/max.json
+-rw-r--r--   0        0        0       49 2024-04-06 18:52:00.222443 starrailcard-2.1.3/starrailcard/src/tools/calculator/src/assets/relic_id.json
+-rw-r--r--   0        0        0     3434 2024-04-06 18:52:00.479448 starrailcard-2.1.3/starrailcard/src/tools/calculator/src/assets/rolls.json
+-rw-r--r--   0        0        0    92881 2024-04-06 18:52:01.246844 starrailcard-2.1.3/starrailcard/src/tools/calculator/src/assets/score.json
+-rw-r--r--   0        0        0     1959 2024-03-13 13:47:21.923389 starrailcard-2.1.3/starrailcard/src/tools/calculator/src/utils.py
+-rw-r--r--   0        0        0     5747 2024-04-01 14:16:17.689304 starrailcard-2.1.3/starrailcard/src/tools/calculator/stats.py
+-rw-r--r--   0        0        0     2526 2024-02-22 12:56:12.220916 starrailcard-2.1.3/starrailcard/src/tools/cashe.py
+-rw-r--r--   0        0        0      709 2024-04-09 17:29:46.754642 starrailcard-2.1.3/starrailcard/src/tools/enums.py
+-rw-r--r--   0        0        0    10136 2024-02-23 21:20:24.125982 starrailcard-2.1.3/starrailcard/src/tools/git.py
+-rw-r--r--   0        0        0    10025 2024-04-14 05:20:03.169865 starrailcard-2.1.3/starrailcard/src/tools/http.py
+-rw-r--r--   0        0        0      938 2024-04-09 16:56:51.818599 starrailcard-2.1.3/starrailcard/src/tools/json_data.py
+-rw-r--r--   0        0        0     6341 2024-04-14 04:42:09.584031 starrailcard-2.1.3/starrailcard/src/tools/options.py
+-rw-r--r--   0        0        0      199 2024-02-18 13:46:16.566296 starrailcard-2.1.3/starrailcard/src/tools/pill/__init__.py
+-rw-r--r--   0        0        0     3854 2024-02-22 12:55:07.451038 starrailcard-2.1.3/starrailcard/src/tools/pill/color.py
+-rw-r--r--   0        0        0     2330 2024-02-22 13:03:49.291296 starrailcard-2.1.3/starrailcard/src/tools/pill/color_controle.py
+-rw-r--r--   0        0        0     5518 2024-02-25 12:31:53.901150 starrailcard-2.1.3/starrailcard/src/tools/pill/grandiend_v2.py
+-rw-r--r--   0        0        0     3284 2024-02-22 12:55:28.873148 starrailcard-2.1.3/starrailcard/src/tools/pill/grandient_v1.py
+-rw-r--r--   0        0        0     3952 2024-04-14 22:23:43.804859 starrailcard-2.1.3/starrailcard/src/tools/pill/image_controle.py
+-rw-r--r--   0        0        0     5106 2024-02-22 12:55:59.845148 starrailcard-2.1.3/starrailcard/src/tools/pill/style_editor.py
+-rw-r--r--   0        0        0     2116 2024-02-22 13:01:14.697378 starrailcard-2.1.3/starrailcard/src/tools/pill/text_controle.py
+-rw-r--r--   0        0        0     2360 2024-03-13 13:31:40.291343 starrailcard-2.1.3/starrailcard/src/tools/translator.py
+-rw-r--r--   0        0        0     6585 2024-02-22 12:57:06.983609 starrailcard-2.1.3/starrailcard/src/tools/treePaths.py
+-rw-r--r--   0        0        0     1748 2024-03-28 18:26:54.868269 starrailcard-2.1.3/starrailcard/src/tools/ukrainization.py
+-rw-r--r--   0        0        0     6884 2024-03-18 20:19:11.991157 starrailcard-2.1.3/starrailcard/utils.py
+-rw-r--r--   0        0        0     5037 1970-01-01 00:00:00.000000 starrailcard-2.1.3/PKG-INFO
```

### Comparing `starrailcard-2.1.2/LICENSE` & `starrailcard-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/pyproject.toml` & `starrailcard-2.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starrailcard"
-version = "2.1.2"
+version = "2.1.3"
 description = "This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players."
 authors = ["DEViantUA <deviantapi@gmail.com>"]
 license = "MIT License with Additional Restrictions"
 
 readme = 'README.md'  # Markdown files are supported
 
 repository = "https://github.com/DEViantUA/StarRailCard"
@@ -20,11 +20,12 @@
 cachetools = "^5.3.1"
 imageio = "^2.14.0"
 moviepy = "^1.0.3"
 more-itertools = "^8.9.0"
 numpy = "^1.21.2"
 pydantic = "^1.9.0"
 beautifulsoup4 = "^4.12.3"
+anyio = "^4.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `starrailcard-2.1.2/README.md` & `starrailcard-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/client.py` & `starrailcard-2.1.3/starrailcard/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 # Copyright 2024 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
 
-import asyncio
+import anyio
+#import asyncio
 
 from .src.tools import http, ukrainization, options, translator, cashe, git
 from .src.generator import style_relict_score, style_ticket, style_profile_phone
-from .src.api import api
+from .src.api import api, enka
 from .src.model import StarRailCard
 
 
 class Card:
     def __init__(self, lang = "en", character_art = None, character_id = None, seeleland = False,
                  user_font = None, save = False, asset_save = False, remove_logo = False,
-                 cashe = {"maxsize": 150, "ttl": 300}):
+                 cashe = {"maxsize": 150, "ttl": 300}, enka = False):
         """Main class for generating cards
 
         Args:
             lang (str, optional): Language in which generation will take place, supported languages: cht, cn, de, en, es, fr, id, jp, kr, pt, ru, th, vi, ua . Defaults to "en".
             character_art (dict, optional): A dictionary that contains a key - character id and link value (If you want to pass several images for 1 character, you can use list in the values). Defaults to None.
             character_id (str, optional): List character ids separated by commas. Defaults to None.
             seeleland (bool, optional): Enable Seeleland statistics. Defaults to False.
             user_font (srt, optional): Font path or font name. Defaults to None.
             save (bool, optional): Whether to save images or not (Does not work for animated cards). Defaults to False.
             asset_save (bool, optional): Save assets to the device so that in subsequent calls you do not have to download them, but open them from the device. Defaults to False.
             remove_logo (bool, optional): Remove GItHub logo. Defaults to False.
             cashe (dict, optional): Set your cache settings. Defaults to {"maxsize": 150, "ttl": 300}.
         """
-        self.session = None
         self.lang = lang
         self.character_art  = character_art
         self.character_id  = character_id
         self.seeleland = seeleland
         self.user_font = user_font
         self.save = save
         self.asset_save = asset_save
         self.remove_logo = remove_logo
         self.cashe = cashe
+        self.enka = enka
         
     async def __aenter__(self):
         cashe.Cache.get_cache(maxsize = self.cashe.get("maxsize", 150), ttl = self.cashe.get("ttl", 300))
-        self.session = await http.AioSession.creat_session()
+        await http.AioSession.enter()
         
         await git.ImageCache.set_assets_dowload(self.asset_save)
         
         if self.character_id:
             self.character_id = await options.get_charter_id(self.character_id)
         
         if self.character_art:
             if not isinstance(self.character_art, dict):
                 raise TypeError(4,"The character_art parameter must be a dictionary, where the key is the name of the character, and the parameter is an image.\nExample: character_art = {'1235': 'img.png', '1235': ['img.png','http.../img2.png']} or {'123596': 'img.png', '123854': 'http.../img2.png', ...}")
             else:
                 self.character_art = await options.get_character_art(self.character_art)
         
+        
         if not self.lang in translator.SUPPORTED_LANGUAGES:
             self.lang = "en"
         
         if self.lang == "ua":
             await ukrainization.TranslateDataManager().check_update()
         
         self.translateLang = translator.Translator(self.lang)
 
-            
         if self.user_font:
             await git.change_font(font_path = self.user_font)
         
         if self.remove_logo:
             print("""
                 Thank you for using our StarRailCard!
                 By removing the GitHub logo from the generated results, you acknowledge supporting the author through one of the following links:
@@ -72,15 +73,15 @@
                 - Ko-fi: https://ko-fi.com/dezzso
 
                 Failure to contribute to the project may lead to the author discontinuing updates in the future.
                 """)
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
-        await http.AioSession.close_session()
+        await http.AioSession.exit(exc_type, exc, tb)
         
     async def set_lang(self, lang):
         """Sets the language
 
         Args:
             lang (str): lang (str): Language in which generation will take place, supported languages: cht, cn, de, en, es, fr, id, jp, kr, pt, ru, th, vi, ua . Defaults to "en".
         """
@@ -112,15 +113,18 @@
             hide_uid (bool, optional): Hide UID. Defaults to False.
             background (str, optional): Link to custom card background. Defaults to None.
             force_update (bool, optional): Forced update of user data. Defaults to False.
 
         Returns:
             StarRail: A class object containing profile information and a profile card
         """
-        data = await api.ApiMiHoMo(uid, lang= self.lang, force_update = force_update).get()
+        if self.enka:
+            data = await enka.ApiEnkaNetwork(uid, lang= self.lang).get()
+        else:
+            data = await api.ApiMiHoMo(uid, lang= self.lang, force_update = force_update).get()
         
         try:
             player = data.player.model_dump()
         except:
             player = data.player
             
         response = {
@@ -163,17 +167,26 @@
             force_update (bool, optional): forced update of user data. Defaults to False.
             style_settings (dict, optional): not implemented yet. Defaults to None.
 
         Returns:
             StarRail: A class object containing profile information and a character cards
         """
         
-        data = await api.ApiMiHoMo(uid, lang= self.lang, force_update = force_update).get()
-        task = []
-                
+        if self.enka:
+            try:
+                data = await enka.ApiEnkaNetwork(uid, lang= self.lang).get()
+            except Exception as e:
+                print("To use the EnkaNetwork API you need to download/update the asset\nExample: await enka.ApiEnkaNetwork().update_assets()")
+                data = await api.ApiMiHoMo(uid, lang= self.lang, force_update = force_update).get()
+        else:
+            data = await api.ApiMiHoMo(uid, lang= self.lang, force_update = force_update).get()
+            
+        #data = await api.ApiMiHoMo(uid, lang= self.lang, force_update = force_update).get()
+        result = []
+        
         style, style_settings = await options.style_setting(style, style_settings)
         
         try:
             player = data.player.model_dump()
         except:
             player = data.player
         
@@ -188,41 +201,68 @@
             },
             "player": player,
             "card": None,
             "character_name": [],
             "character_id": [],
         }
         
-        for key in data.characters:
+        async with anyio.create_task_group() as tasks:
+            
+            for key in data.characters:
+                async def get_result(key):    
+                    try:               
+                        response["character_id"].append(key.id)
+                        response["character_name"].append(key.name)
+                        
+                        if self.character_id:
+                            if not str(key.id) in self.character_id:
+                                return  
+                        
+                        art = None
+                        if self.character_art:
+                            if str(key.id) in self.character_art:
+                                art = self.character_art[str(key.id)]
+                        if style == 1:
+                            result.append(await style_relict_score.Creat(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo).start())
+                        elif style == 2:
+                            result.append(await style_ticket.Creat(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo).start())
+                    except Exception as e:
+                        print(f"Error in get_result for character {key.id}: {e}")
+                        
+                tasks.start_soon(get_result, key)
+        
+        '''for key in data.characters:
             response["character_id"].append(key.id)
             response["character_name"].append(key.name)
             
             if self.character_id:
                 if not str(key.id) in self.character_id:
                     continue  
             
             art = None
             if self.character_art:
                 if str(key.id) in self.character_art:
                     art = self.character_art[str(key.id)]
-                    
             if style == 1:
-                task.append(style_relict_score.Creat(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo).start())
+                result.append(style_relict_score.Creat(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo).start())
             elif style == 2:
-                task.append(style_ticket.Creat(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo).start())
+                result.append(style_ticket.Creat(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo).start())
+
+        
+        result = await asyncio.gather(*result)'''
+            
         
-        response["card"] = await asyncio.gather(*task)
+        response["card"] = result
         
         if self.lang == "ua":
             StarRailCard.UA_LANG = True
         else:
             StarRailCard.UA_LANG = False
-        task_save = []
-        if self.save:
-            for key in response["card"]:
-                if key["animation"]:
-                    continue
-                task_save.append(options.save_card(uid,key["card"],key["id"]))
-        
-            await asyncio.gather(*task_save)
         
+        if self.save:
+            async with anyio.create_task_group() as tasks:
+                for key in response["card"]:
+                    if key["animation"]:
+                        continue
+                    tasks.start_soon(options.save_card,uid,key["card"],key["id"])        
+                                
         return StarRailCard.StarRail(**response)
```

### Comparing `starrailcard-2.1.2/starrailcard/src/assets/font/font_hsr.ttf` & `starrailcard-2.1.3/starrailcard/src/assets/font/font_hsr.ttf`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/data/avatar.json` & `starrailcard-2.1.3/starrailcard/src/data/avatar.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/data/relict_sets.json` & `starrailcard-2.1.3/starrailcard/src/data/relict_sets.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/data/stats.json` & `starrailcard-2.1.3/starrailcard/src/data/stats.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/data/weapons.json` & `starrailcard-2.1.3/starrailcard/src/data/weapons.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/generator/style_profile_phone.py` & `starrailcard-2.1.3/starrailcard/src/generator/style_profile_phone.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/generator/style_relict_score.py` & `starrailcard-2.1.3/starrailcard/src/generator/style_relict_score.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright 2024 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
 
-import asyncio
+import anyio
+import functools
 import io
 from PIL import ImageDraw,Image,ImageFilter,ImageChops, ImageSequence
 
 from ..tools import git, options
 from ..tools.calculator import stats
 from ..model.style import RelictScore
 
@@ -431,15 +432,15 @@
             self.background = []
             for key in self.GIFT_BG:
                 key.alpha_composite(bg)
                 self.background.append(key.convert("RGB"))
         else:
             self.background.alpha_composite(bg)
                     
-    async def start(self):   
+    async def start(self):
         _of.set_mapping(1)
         
         if self.art:
             if "gif" in self.art:
                 self.gif = True
             self.art = await pill.get_user_image(self.art)
             
@@ -461,28 +462,42 @@
                         self.GIFT_BG.append(self.background.copy())
                     frame_count += 1            
         else:
             if self.art:
                 self.element_color = await pill.get_colors(self.art, 15, common=True, radius=5, quality=800)
             
             await self.creat_bacground()
+        
+        async with anyio.create_task_group() as tasks:
+            tasks.start_soon(self.creat_light_cone)
+            tasks.start_soon(self.creat_stats)
+            tasks.start_soon(self.creat_name)
+            tasks.start_soon(self.creat_constant)
+            tasks.start_soon(self.creat_relict_sets)
+            tasks.start_soon(self.get_score)
+            tasks.start_soon(self.get_path)
+            tasks.start_soon(self.creat_seeleland)
+        
+        async def wait_all(*funcs):
+            results = [None] * len(funcs)
             
-        await asyncio.gather(
-            self.creat_light_cone(),
-            self.creat_stats(),
-            self.creat_name(),
-            self.creat_constant(),
-            self.creat_relict_sets(),
-            self.get_score(),
-            self.get_path(),
-            self.creat_seeleland()
-        )
-        relic_tasks = [self.creat_relict(key) for key in self.data.relics]
-        self.relict = await asyncio.gather(*relic_tasks)
+            async with anyio.create_task_group() as tasks:
+                async def process(func, i):
+                    results[i] = await func()
+                
+                for i, func in enumerate(funcs):
+                    tasks.start_soon(process, func, i)
+            
+            return results
         
+        self.relict = await wait_all(*[
+            functools.partial(self.creat_relict, key)
+            for key in self.data.relics
+        ])
+                
         await self.creat_score_total()
         
         await self.build_relict()
         await self.build()
         
         data = {
             "id": self.data.id,
```

### Comparing `starrailcard-2.1.2/starrailcard/src/generator/style_ticket.py` & `starrailcard-2.1.3/starrailcard/src/generator/style_ticket.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright 2024 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
 
-import asyncio
+import anyio
+
 import io
 from PIL import ImageDraw,Image,ImageChops, ImageSequence
+import functools
 
 from ..tools import git, options
 from ..tools.calculator import stats
 from ..model.style import Ticket
 
 from ..tools import pill
 
@@ -142,22 +144,16 @@
 
         self.light_cone_background = Image.new("RGBA", (447, 255), (0, 0, 0, 0))
         self.light_cone_background.alpha_composite(light_cone_holst_image.resize((183, 244)))
         self.light_cone_background.alpha_composite(stars,(0,6))
         self.light_cone_background.alpha_composite(line, (191, 19))
         self.light_cone_background.alpha_composite(name_light_cone, (200, 23))
         
-        """if line.size[1] > 50:
-            y = int(22 + line.size[1])
-        else:
-            y = -45"""
-        
         y = int(22 + line.size[1])
 
-        background_stat.save("BF.png")
         self.light_cone_background.alpha_composite(background_stat, (188, y))
     
     async def creat_relict(self,relict):
         
         font_15 = await pill.get_font(15)
         font_26 = await pill.get_font(26)
         font_14 = await pill.get_font(14)
@@ -598,25 +594,23 @@
             for key in self.GIFT_BG:
                 key.alpha_composite(bg)
                 self.background.append(key.convert("RGB"))
         else:
             self.background.alpha_composite(bg)
         
     async def start(self):
-        
         _of.set_mapping(2)
         
         if self.art:
             if "gif" in self.art:
                 self.gif = True
             self.art = await pill.get_user_image(self.art)
             if self.gif:    
                 n = 2           
                 frame_count = 0
-                color = True
                 with io.BytesIO(self.art) as f:
                     self.art = Image.open(f)
                     for frame in ImageSequence.Iterator(self.art):
                         self.element_color = await pill.get_colors(frame.convert("RGBA"), 15, common=True, radius=5, quality=800)
                         if frame_count >= 50:
                             break
                         if frame_count % n != 0:
@@ -627,29 +621,47 @@
             else:
                 self.element_color = await pill.get_colors(self.art, 15, common=True, radius=5, quality=800)
                 await self.creat_bacground()
         else:
             self.element_color = (255,213,167,255)
             await self.creat_bacground()
         
-        await asyncio.gather(
-            self.creat_light_cone(),
-            self.creat_stats(),
-            self.creat_name(),
-            self.creat_constant(),
-            self.creat_relict_sets(),
-            self.get_score(),
-            self.creat_path(),
-            self.creat_seeleland()
-        )
-        relic_tasks = [self.creat_relict(key) for key in self.data.relics]
-        self.relict = await asyncio.gather(*relic_tasks)
+        async with anyio.create_task_group() as tasks:
+            tasks.start_soon(self.creat_light_cone)
+            tasks.start_soon(self.creat_stats)
+            tasks.start_soon(self.creat_name)
+            tasks.start_soon(self.creat_constant)
+            tasks.start_soon(self.creat_relict_sets)
+            tasks.start_soon(self.get_score)
+            tasks.start_soon(self.creat_path)
+            tasks.start_soon(self.creat_seeleland)
+        
+        async def wait_all(*funcs):
+            results = [None] * len(funcs)
+            
+            async with anyio.create_task_group() as tasks:
+                async def process(func, i):
+                    results[i] = await func()
+                
+                for i, func in enumerate(funcs):
+                    tasks.start_soon(process, func, i)
+            
+            return results
         
-        await self.creat_score_total()
+        self.relict = await wait_all(*[
+            functools.partial(self.creat_relict, key)
+            for key in self.data.relics
+        ])
+
+
+            #self.relict = await asyncio.gather(*relic_tasks)
         
+        
+        
+        await self.creat_score_total()
         await self.build_relict()
         await self.build()
         
         data = {
                 "id": self.data.id,
                 "name": self.data.name,
                 "animation": self.gif,
```

### Comparing `starrailcard-2.1.2/starrailcard/src/model/StarRailCard.py` & `starrailcard-2.1.3/starrailcard/src/model/StarRailCard.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,22 +62,22 @@
     animation: bool
     size: Optional[tuple]
     color: Optional[tuple]
     class Config:
         arbitrary_types_allowed = True
     
     async def get_info(self, lang = "en"):
-        await AioSession.get_session()
+        #await AioSession.get_session()
         url = f"https://api.yatta.top/hsr/v2/{lang}/avatar/{self.id}"
         data = await AioSession.get(url, response_format = "json")
         data["data"]["icon"] = {"icon": f'https://api.yatta.top/hsr/assets/UI/avatar/medium/{data["data"]["icon"]}.png', 
                                 "splash": f'https://api.yatta.top/hsr/assets/UI/avatar/large/{data["data"]["icon"]}.png',
                                 "avatar": f'https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/icon/avatar/{data["data"]["icon"]}.png'
         }        
-        await AioSession.close_session()
+        #await AioSession.close_session()
         
         return data["data"]
     
     def show(self):
         if self.animation:
             self.card[0].show()
         else:
```

### Comparing `starrailcard-2.1.2/starrailcard/src/model/style.py` & `starrailcard-2.1.3/starrailcard/src/model/style.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/model/utils_model.py` & `starrailcard-2.1.3/starrailcard/src/model/utils_model.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/calculator/src/assets/rolls.json` & `starrailcard-2.1.3/starrailcard/src/tools/calculator/src/assets/rolls.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/calculator/src/assets/score.json` & `starrailcard-2.1.3/starrailcard/src/tools/calculator/src/assets/score.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/calculator/src/utils.py` & `starrailcard-2.1.3/starrailcard/src/tools/calculator/src/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/calculator/stats.py` & `starrailcard-2.1.3/starrailcard/src/tools/calculator/stats.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/cashe.py` & `starrailcard-2.1.3/starrailcard/src/tools/cashe.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/git.py` & `starrailcard-2.1.3/starrailcard/src/tools/git.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/json_data.py` & `starrailcard-2.1.3/starrailcard/src/tools/json_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright 2024 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
 
 import json
 import aiofiles
 
-
 class JsonManager:
     def __init__(self, file_path):
         self.file_path = file_path
 
     async def read(self):
         try:
             async with aiofiles.open(self.file_path, mode='r', encoding="utf-8") as file:
```

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/options.py` & `starrailcard-2.1.3/starrailcard/src/tools/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     data = [value for value in data if value.isdigit()]
     
     if data == []:
         return None
     return data
 
 async def style_setting(style, settings):
-    if str(style) in ["1","2","3"]:
+    if str(style) in ["1","2"]:
         return style, settings
     
     return 1, {}
 
 
 def ups(x):
     if x == 5:
```

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/pill/color.py` & `starrailcard-2.1.3/starrailcard/src/tools/pill/color.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/pill/color_controle.py` & `starrailcard-2.1.3/starrailcard/src/tools/pill/color_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/pill/grandiend_v2.py` & `starrailcard-2.1.3/starrailcard/src/tools/pill/grandiend_v2.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/pill/grandient_v1.py` & `starrailcard-2.1.3/starrailcard/src/tools/pill/grandient_v1.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/pill/image_controle.py` & `starrailcard-2.1.3/starrailcard/src/tools/pill/image_controle.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,28 +78,30 @@
     try:
         image = await http.AioSession.get(link,headers=headers_p, response_format= "bytes")
     except:
         raise
     
     if gif:
         return image
-        
-    image = Image.open(BytesIO(image)).convert("RGBA")
-    if size:
-        image = image.resize(size)
-        _caches[cache_key] = image
-        return image
-    elif thumbnail_size:
-        image.thumbnail(thumbnail_size)
-        _caches[cache_key] = image
-        return image
-    else:
-        _caches[cache_key] = image
-        return image
-
+    try:
+        image = Image.open(BytesIO(image)).convert("RGBA")
+        if size:
+            image = image.resize(size)
+            _caches[cache_key] = image
+            return image
+        elif thumbnail_size:
+            image.thumbnail(thumbnail_size)
+            _caches[cache_key] = image
+            return image
+        else:
+            _caches[cache_key] = image
+            return image
+    except:
+        raise TypeError(f"Error Open image: {link}")
+    
 async def crop_image(img):
     width, height = img.size
     target_pixel_x = 275
     target_pixel_y = height // 2
     crop_size = 8
     left = max(0, target_pixel_x - crop_size // 2)
     right = min(width, target_pixel_x + crop_size // 2 + 1)
```

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/pill/style_editor.py` & `starrailcard-2.1.3/starrailcard/src/tools/pill/style_editor.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/pill/text_controle.py` & `starrailcard-2.1.3/starrailcard/src/tools/pill/text_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/translator.py` & `starrailcard-2.1.3/starrailcard/src/tools/translator.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/treePaths.py` & `starrailcard-2.1.3/starrailcard/src/tools/treePaths.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/src/tools/ukrainization.py` & `starrailcard-2.1.3/starrailcard/src/tools/ukrainization.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/starrailcard/utils.py` & `starrailcard-2.1.3/starrailcard/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.2/PKG-INFO` & `starrailcard-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrailcard
-Version: 2.1.2
+Version: 2.1.3
 Summary: This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
 Home-page: https://github.com/DEViantUA/StarRailCard
 License: MIT License with Additional Restrictions
 Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai
 Author: DEViantUA
 Author-email: deviantapi@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=10.0.1,<11.0.0)
 Requires-Dist: aiofiles (>=0.7.0,<0.8.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
+Requires-Dist: anyio (>=4.3.0,<5.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: cachetools (>=5.3.1,<6.0.0)
 Requires-Dist: imageio (>=2.14.0,<3.0.0)
 Requires-Dist: more-itertools (>=8.9.0,<9.0.0)
 Requires-Dist: moviepy (>=1.0.3,<2.0.0)
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
```

