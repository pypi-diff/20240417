# Comparing `tmp/moobius-1.1.7.tar.gz` & `tmp/moobius-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moobius-1.1.7.tar", last modified: Tue Apr  9 05:35:07 2024, max compression
+gzip compressed data, was "moobius-1.1.8.tar", last modified: Tue Apr 16 23:48:10 2024, max compression
```

## Comparing `moobius-1.1.7.tar` & `moobius-1.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 05:35:07.293119 moobius-1.1.7/
--rw-rw-rw-   0        0        0     8910 2024-04-09 05:35:07.292117 moobius-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2024-03-24 16:36:44.000000 moobius-1.1.7/license.md
--rw-rw-rw-   0        0        0      647 2024-04-09 04:35:53.000000 moobius-1.1.7/pyproject.toml
--rw-rw-rw-   0        0        0     8055 2024-03-17 18:58:55.000000 moobius-1.1.7/readme.md
--rw-rw-rw-   0        0        0       42 2024-04-09 05:35:07.293119 moobius-1.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 05:35:07.275178 moobius-1.1.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 05:35:07.277172 moobius-1.1.7/src/moobius/
--rw-rw-rw-   0        0        0      184 2024-03-05 05:12:19.000000 moobius-1.1.7/src/moobius/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 05:35:07.283149 moobius-1.1.7/src/moobius/core/
--rw-rw-rw-   0        0        0    57346 2024-04-09 05:09:27.000000 moobius-1.1.7/src/moobius/core/sdk.py
--rw-rw-rw-   0        0        0     4170 2024-04-01 21:02:47.000000 moobius-1.1.7/src/moobius/core/wand.py
-drwxrwxrwx   0        0        0        0 2024-04-09 05:35:07.288132 moobius-1.1.7/src/moobius/database/
--rw-rw-rw-   0        0        0     2655 2024-03-13 15:36:04.000000 moobius-1.1.7/src/moobius/database/database_interface.py
--rw-rw-rw-   0        0        0     4062 2024-03-25 06:01:03.000000 moobius-1.1.7/src/moobius/database/json_database.py
--rw-rw-rw-   0        0        0      902 2024-02-16 02:53:33.000000 moobius-1.1.7/src/moobius/database/null_database.py
--rw-rw-rw-   0        0        0     1517 2024-03-25 06:01:03.000000 moobius-1.1.7/src/moobius/database/redis_database.py
--rw-rw-rw-   0        0        0     9559 2024-03-26 23:06:54.000000 moobius-1.1.7/src/moobius/database/storage.py
-drwxrwxrwx   0        0        0        0 2024-04-09 05:35:07.291121 moobius-1.1.7/src/moobius/network/
--rw-rw-rw-   0        0        0    14222 2024-04-01 23:40:33.000000 moobius-1.1.7/src/moobius/network/asserts.py
--rw-rw-rw-   0        0        0    43927 2024-04-02 20:28:42.000000 moobius-1.1.7/src/moobius/network/http_api_wrapper.py
--rw-rw-rw-   0        0        0    25652 2024-04-03 05:51:15.000000 moobius-1.1.7/src/moobius/network/ws_client.py
--rw-rw-rw-   0        0        0     7154 2024-04-08 21:51:19.000000 moobius-1.1.7/src/moobius/types.py
--rw-rw-rw-   0        0        0     7399 2024-03-29 15:46:12.000000 moobius-1.1.7/src/moobius/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-09 05:35:07.292117 moobius-1.1.7/src/moobius.egg-info/
--rw-rw-rw-   0        0        0     8910 2024-04-09 05:35:07.000000 moobius-1.1.7/src/moobius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2024-04-09 05:35:07.000000 moobius-1.1.7/src/moobius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 05:35:07.000000 moobius-1.1.7/src/moobius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2024-04-09 05:35:07.000000 moobius-1.1.7/src/moobius.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-09 05:35:07.000000 moobius-1.1.7/src/moobius.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      329 2024-04-08 18:24:26.000000 moobius-1.1.7/src/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:48:10.332909 moobius-1.1.8/
+-rw-rw-rw-   0        0        0     8910 2024-04-16 23:48:10.331911 moobius-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2024-03-24 16:36:44.000000 moobius-1.1.8/license.md
+-rw-rw-rw-   0        0        0      647 2024-04-16 23:28:47.000000 moobius-1.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0     8055 2024-03-17 18:58:55.000000 moobius-1.1.8/readme.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 23:48:10.332909 moobius-1.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 23:48:10.312366 moobius-1.1.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 23:48:10.314358 moobius-1.1.8/src/moobius/
+-rw-rw-rw-   0        0        0      184 2024-03-05 05:12:19.000000 moobius-1.1.8/src/moobius/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:48:10.323938 moobius-1.1.8/src/moobius/core/
+-rw-rw-rw-   0        0        0    57439 2024-04-16 23:42:53.000000 moobius-1.1.8/src/moobius/core/sdk.py
+-rw-rw-rw-   0        0        0     4170 2024-04-01 21:02:47.000000 moobius-1.1.8/src/moobius/core/wand.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:48:10.327926 moobius-1.1.8/src/moobius/database/
+-rw-rw-rw-   0        0        0     2655 2024-03-13 15:36:04.000000 moobius-1.1.8/src/moobius/database/database_interface.py
+-rw-rw-rw-   0        0        0     4098 2024-04-16 23:43:03.000000 moobius-1.1.8/src/moobius/database/json_database.py
+-rw-rw-rw-   0        0        0      902 2024-02-16 02:53:33.000000 moobius-1.1.8/src/moobius/database/null_database.py
+-rw-rw-rw-   0        0        0     1517 2024-03-25 06:01:03.000000 moobius-1.1.8/src/moobius/database/redis_database.py
+-rw-rw-rw-   0        0        0     9559 2024-03-26 23:06:54.000000 moobius-1.1.8/src/moobius/database/storage.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:48:10.329919 moobius-1.1.8/src/moobius/network/
+-rw-rw-rw-   0        0        0    14222 2024-04-01 23:40:33.000000 moobius-1.1.8/src/moobius/network/asserts.py
+-rw-rw-rw-   0        0        0    44002 2024-04-16 23:40:27.000000 moobius-1.1.8/src/moobius/network/http_api_wrapper.py
+-rw-rw-rw-   0        0        0    25652 2024-04-10 03:05:43.000000 moobius-1.1.8/src/moobius/network/ws_client.py
+-rw-rw-rw-   0        0        0     7154 2024-04-08 21:51:19.000000 moobius-1.1.8/src/moobius/types.py
+-rw-rw-rw-   0        0        0     7399 2024-03-29 15:46:12.000000 moobius-1.1.8/src/moobius/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:48:10.330915 moobius-1.1.8/src/moobius.egg-info/
+-rw-rw-rw-   0        0        0     8910 2024-04-16 23:48:10.000000 moobius-1.1.8/src/moobius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2024-04-16 23:48:10.000000 moobius-1.1.8/src/moobius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 23:48:10.000000 moobius-1.1.8/src/moobius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2024-04-16 23:48:10.000000 moobius-1.1.8/src/moobius.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-16 23:48:10.000000 moobius-1.1.8/src/moobius.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      329 2024-04-08 18:24:26.000000 moobius-1.1.8/src/setup.py
```

### Comparing `moobius-1.1.7/PKG-INFO` & `moobius-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moobius
-Version: 1.1.7
+Version: 1.1.8
 Summary: Moobius Platform SDK
 Author-email: Kevin Kostlan <sdk@moobius.app>
 Project-URL: Homepage, https://github.com/groupultra/sdk-public
 Project-URL: Issues, https://github.com/groupultra/sdk-public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moobius-1.1.7/license.md` & `moobius-1.1.8/license.md`

 * *Files identical despite different names*

### Comparing `moobius-1.1.7/pyproject.toml` & `moobius-1.1.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "moobius"
-version = "1.1.7"
+version = "1.1.8"
 authors = [
   { name="Kevin Kostlan", email="sdk@moobius.app"},
 ]
 description = "Moobius Platform SDK"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `moobius-1.1.7/readme.md` & `moobius-1.1.8/readme.md`

 * *Files identical despite different names*

### Comparing `moobius-1.1.7/src/moobius/core/sdk.py` & `moobius-1.1.8/src/moobius/core/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,24 +101,24 @@
         self.config_path = config_path
         self.is_agent = is_agent
 
         if type(config_path) is dict:
             logger.info('Be careful to keep the secrets in your service config safe!')
             the_config = config_path
         elif type(config_path) is str:
-            with open(config_path, "r") as f:
+            with open(config_path, "r", encoding='utf-8') as f:
                 the_config = json.load(f)
         else:
             raise Exception('config_path not understood')
         self.config = the_config
 
         if type(db_config_path) is dict:
             self.db_config = db_config_path
         elif type(db_config_path) is str and db_config_path != "":
-            with open(db_config_path, "r") as f:
+            with open(db_config_path, "r", encoding='utf-8') as f:
                 self.db_config = json.load(f)
         else:
             raise Exception('db_config_path not understood')
 
         http_server_uri = self.config["http_server_uri"]
         ws_server_uri = self.config["ws_server_uri"]
         email = self.config["email"]
@@ -188,20 +188,20 @@
                 logger.info(f"Please wait for 5 seconds...")
                 self.config["service_id"] = self.client_id
                 await asyncio.sleep(5) # TODO: Sleeps "long enough" should be replaced with polling.
             if not self.client_id:
                 raise Exception("Error creating a new service and getting its id.")
 
             if type(self.config_path) is str: # Save the newly created service if any.
-                with open(self.config_path, "r") as f:
+                with open(self.config_path, "r", encoding='utf-8') as f:
                     old_config = json.load(f)
                 s_id = self.config['service_id']
                 if s_id != old_config.get('service_id'):
                     old_config['service_id'] = s_id
-                    with open(self.config_path, "w") as f:
+                    with open(self.config_path, "w", encoding='utf-8') as f:
                         json.dump(old_config, f, indent=4, ensure_ascii=False)
                         logger.info(f"Config file 'service_id' updated to {s_id}: {self.config_path}")
 
             if len(self.config["channels"]) == 0:
                 logger.error('No channels specified in self.config')
                 return
 
@@ -277,15 +277,15 @@
     async def agent_join_service_channels(self, service_config_fname):
         """Joins service channels given by service config filename."""
         if not self.is_agent:
             logger.warning('Called agent_join_service_channels when not an agent.')
         if type(service_config_fname) is dict:
             s_config = service_config_fname
         else:
-            with open(service_config_fname, 'r') as f_obj:
+            with open(service_config_fname, 'r', encoding='utf-8') as f_obj:
                 s_config = json.load(f_obj)
             channels = s_config.get('channels', [])
         if len(channels)==0:
             logger.warning('No channels for Agent to join.')
         else:
             logger.info(f'Agent joining Service default channels (if not already joined). Will not join to any extra channels: {channels}')
 
@@ -598,15 +598,15 @@
     async def sign_out(self): """Calls self.http_api.sign_out."""; return await self.http_api.sign_out()
     async def update_current_user(self, avatar, description, name): """Calls self.http_api.update_current_user."""; return await self.http_api.update_current_user(avatar, description, name)
     async def update_character(self, character_id, avatar, description, name): """Calls self.http_api.update_character using self.client_id."""; return await self.http_api.update_character(self.client_id, character_id, avatar, description, name)
     async def update_channel(self, channel_id, channel_name, channel_desc): """Calls self.http_api.update_channel."""; return await self.http_api.update_channel(channel_id, channel_name, channel_desc)
     async def bind_service_to_channel(self, channel_id): """Calls self.http_api.bind_service_to_channel"""; return await self.http_api.bind_service_to_channel(self.client_id, channel_id)
     async def unbind_service_from_channel(self, channel_id): """Calls self.http_api.unbind_service_from_channel"""; return await self.http_api.unbind_service_from_channel(self.client_id, channel_id)
     async def create_character(self, name, avatar, description): """Calls self.http_api.create_character using self.create_character."""; return await self.http_api.create_character(self.client_id, name, avatar, description)
-    async def fetch_popular_channels(self): """Calls self.http_api.fetch_popular_channels."""; return await self.http_api.fetch_popular_chanels()
+    async def fetch_popular_channels(self): """Calls self.http_api.fetch_popular_channels."""; return await self.http_api.fetch_popular_channels()
     async def fetch_channel_list(self): """Calls self.http_api.fetch_channel_list."""; return await self.http_api.fetch_channel_list()
     async def fetch_real_character_ids(self, channel_id, raise_empty_list_err=True): """Calls self.http_api.fetch_real_character_ids using self.client_id."""; return await self.http_api.fetch_real_character_ids(channel_id, self.client_id, raise_empty_list_err=raise_empty_list_err)
     async def fetch_character_profile(self, character_id): """Calls self.http_api.fetch_character_profile"""; return await self.http_api.fetch_character_profile(character_id)
     async def fetch_service_id_list(self): """Calls self.http_api.fetch_service_id_list"""; return await self.http_api.fetch_service_id_list()
     async def fetch_service_characters(self): """Calls self.http_api.fetch_service_characters using self.client_id."""; return await self.http_api.fetch_service_characters(self.client_id)
     async def upload_file(self, filepath): """Calls self.http_api.upload_file."""; return await self.http_api.upload_file(filepath)
     async def fetch_message_history(self, channel_id, limit=1024, before="null"): """Calls self.http_api.fetch_message_history."""; return await self.http_api.fetch_message_history(channel_id, limit, before)
@@ -619,15 +619,15 @@
     async def fetch_channel_temp_group(self, channel_id): """Calls self.http_api.fetch_channel_temp_group."""; return await self.http_api.fetch_channel_temp_group(channel_id, self.client_id)
     async def fetch_channel_group_list(self, channel_id): """Calls self.http_api.fetch_target_group."""; return await self.http_api.fetch_channel_group_list(channel_id, self.client_id)
     async def fetch_user_from_group(self, user_id, channel_id, group_id): """Calls self.http_api.fetch_user_from_group."""; return await self.http_api.fetch_user_from_group(user_id, channel_id, group_id)
     async def fetch_target_group(self, user_id, channel_id, group_id): """Calls self.http_api.fetch_target_group."""; return await self.http_api.fetch_target_group(user_id, channel_id, group_id)
 
     async def send_agent_login(self): """Calls self.ws_client.agent_login using self.http_api.access_token; one of the agent vs service differences."""; return await self.ws_client.agent_login(self.http_api.access_token)
     async def send_service_login(self): """Calls self.ws_client.service_login using self.client_id and self.http_api.access_token; one of the agent vs service differences."""; return await self.ws_client.service_login(self.client_id, self.http_api.access_token)
-    async def send_update(self, target_client_id, data): """Calls self.ws_client.TODO"""; return await self.ws_client.update(self.client_id, target_client_id, data)
+    async def send_update(self, target_client_id, data): """Calls self.ws_client.update"""; return await self.ws_client.update(self.client_id, target_client_id, data)
     async def send_update_character_list(self, channel_id, character_list, recipients): """Calls self.ws_client.update_character_list using self.client_id. Converts recipients to a group_id if a list."""; return await self.ws_client.update_character_list(self.client_id, channel_id, await self._update_rec(character_list, True), await self._update_rec(recipients, True))
     async def send_update_channel_info(self, channel_id, channel_info): """Calls self.ws_client.update_channel_info using self.client_id."""; return await self.ws_client.update_channel_info(self.client_id, channel_id, channel_info)
     async def send_update_canvas(self, channel_id, canvas_elements, recipients): """Calls self.ws_client.update_canvas using self.client_id. Converts recipients to a group_id if a list."""; return await self.ws_client.update_canvas(self.client_id, channel_id, canvas_elements, await self._update_rec(recipients, True))
     async def send_update_buttons(self, channel_id, buttons, recipients): """Calls self.ws_client.update_buttons using self.client_id. Converts recipients to a group_id if a list."""; return await self.ws_client.update_buttons(self.client_id, channel_id, buttons, await self._update_rec(recipients, True))
     async def send_update_context_menu(self, channel_id, menu_elements, recipients): """Calls self.ws_client.update_context_menu using self.client_id. Converts recipients to a group_id if a list."""; return await self.ws_client.update_context_menu(self.client_id, channel_id, menu_elements, await self._update_rec(recipients, True))
     async def send_update_style(self, channel_id, style_content, recipients): """Calls self.ws_client.update_style using self.client_id. Converts recipients to a group_id if a list."""; return await self.ws_client.update_style(self.client_id, channel_id, style_content, await self._update_rec(recipients, True))
     async def send_fetch_characters(self, channel_id): """Calls self.ws_client.fetch_characters using self.client_id."""; return await self.ws_client.fetch_characters(self.client_id, channel_id)
```

### Comparing `moobius-1.1.7/src/moobius/core/wand.py` & `moobius-1.1.8/src/moobius/core/wand.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.7/src/moobius/database/database_interface.py` & `moobius-1.1.8/src/moobius/database/database_interface.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.7/src/moobius/database/json_database.py` & `moobius-1.1.8/src/moobius/database/json_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         Raises:
           TypeError: If the type of the value is unknown, so we can't construct the object.
         """
         filename = os.path.join(self.path, key + '.json')
 
         if not os.path.exists(filename):
             return False, f'No json file found for {key}.'
-        with open(filename, 'r') as f:
+        with open(filename, 'r', encoding='utf-8') as f:
             data = json.load(f)
 
             if data['_type'] == 'NoneType':
                 return True, None   # You can't use NoneType(None) to construct a NoneType object, so we have to return None directly
             else:
                 class_name = data['_type']
                 data_type = locate(f'{self.ref_module.__name__}.{class_name}')
@@ -79,15 +79,15 @@
                         raise TypeError(f'Unknown type: {class_name}')
 
     def set_value(self, key, value):
         """Set the value (a dict) of a key (a string). Returns (is_success, the_key).
            Note: This function should not be called directly."""
         filename = os.path.join(self.path, key + '.json')
 
-        with open(filename, 'w') as f:
+        with open(filename, 'w', encoding='utf-8') as f:
             data = {key: value, '_type': type(value).__name__}
             json.dump(data, f, indent=4, cls=EnhancedJSONEncoder, ensure_ascii=False)
             return True, key
 
     def delete_key(self, key):
         """Delete a (string-valued) key. Returns (is_success, key)
            Note: This function should not be called directly."""
```

### Comparing `moobius-1.1.7/src/moobius/database/null_database.py` & `moobius-1.1.8/src/moobius/database/null_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.7/src/moobius/database/redis_database.py` & `moobius-1.1.8/src/moobius/database/redis_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.7/src/moobius/database/storage.py` & `moobius-1.1.8/src/moobius/database/storage.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.7/src/moobius/network/asserts.py` & `moobius-1.1.8/src/moobius/network/asserts.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.7/src/moobius/network/http_api_wrapper.py` & `moobius-1.1.8/src/moobius/network/http_api_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,16 +295,17 @@
         charlist = response_dict["data"]
         return [self._xtract_character(d) for d in charlist]
 
     async def fetch_user_info(self):
         """Used by the Agent to get their info as a UserInfo object."""
         response_dict = await self.checked_get(url=self.http_server_uri + f"/user/info", the_request=None, requests_kwargs={'headers':self.headers}, good_message="Successfully fetched user info", bad_message="Error getting user info", raise_errors=True)
         idict = response_dict.get('data')
+        email_verified = idict.get('email_verified') # Sometimes this is unfilled.
         return UserInfo(avatar=idict['context']['avatar'], description=idict['context']['description'], name=idict['context']['name'],
-                        email=idict['email'], email_verified=idict['email_verified'], user_id=idict['user_id'], system_context=idict['system_context'])
+                        email=idict['email'], email_verified=email_verified, user_id=idict['user_id'], system_context=idict['system_context'])
 
     async def update_current_user(self, avatar, description, name):
         """Updates the user info. Will only be an Agent function in the .net version.
 
            Parameters:
              avatar: Link to image.
              description: Of the user.
@@ -410,15 +411,15 @@
 
         No return value.
         """
         asserts.types_assert(str, channel_name=channel_name, channel_id=channel_id, channel_desc=channel_desc)
         jsonr = {"channel_id": channel_id, "channel_name": channel_name, "context":{"channel_description":channel_desc}}
         await self.checked_post(url=self.http_server_uri + "/channel/update", the_request=jsonr, requests_kwargs={'headers':self.headers}, good_message=f"Successfully updated channel {channel_id}", bad_message=f"Error updating channel {channel_id}", raise_errors=True)
 
-    async def fetch_popular_chanels(self):
+    async def fetch_popular_channels(self):
         """Fetches the popular channels, returning a list of channel_id strings."""
         response_dict = await self.checked_get(url=self.http_server_uri + "/channel/popular", the_request=None, requests_kwargs={'headers':self.headers}, good_message=f"Successfully fetched popular channels", bad_message=f"Error fetching popular channels", raise_errors=True)
         out = []
         for ch in response_dict['data']:
             if type(ch) is not str:
                 ch = ch['channel_id']
             out.append(ch)
```

### Comparing `moobius-1.1.7/src/moobius/network/ws_client.py` & `moobius-1.1.8/src/moobius/network/ws_client.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.7/src/moobius/types.py` & `moobius-1.1.8/src/moobius/types.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.7/src/moobius/utils.py` & `moobius-1.1.8/src/moobius/utils.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.7/src/moobius.egg-info/PKG-INFO` & `moobius-1.1.8/src/moobius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moobius
-Version: 1.1.7
+Version: 1.1.8
 Summary: Moobius Platform SDK
 Author-email: Kevin Kostlan <sdk@moobius.app>
 Project-URL: Homepage, https://github.com/groupultra/sdk-public
 Project-URL: Issues, https://github.com/groupultra/sdk-public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moobius-1.1.7/src/moobius.egg-info/SOURCES.txt` & `moobius-1.1.8/src/moobius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

