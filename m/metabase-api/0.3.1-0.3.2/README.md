# Comparing `tmp/metabase-api-0.3.1.tar.gz` & `tmp/metabase-api-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabase-api-0.3.1.tar", last modified: Wed Sep 13 16:01:32 2023, max compression
+gzip compressed data, was "metabase-api-0.3.2.tar", last modified: Wed Apr 17 05:34:16 2024, max compression
```

## Comparing `metabase-api-0.3.1.tar` & `metabase-api-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-09-13 16:01:32.694534 metabase-api-0.3.1/
--rw-rw-rw-   0        0        0     1080 2023-09-13 16:01:04.000000 metabase-api-0.3.1/LICENSE
--rw-rw-rw-   0        0        0    13118 2023-09-13 16:01:32.690519 metabase-api-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    12508 2023-09-13 16:01:04.000000 metabase-api-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-09-13 16:01:32.678282 metabase-api-0.3.1/metabase_api/
--rw-rw-rw-   0        0        0       39 2023-09-13 16:01:04.000000 metabase-api-0.3.1/metabase_api/__init__.py
--rw-rw-rw-   0        0        0    12728 2023-09-13 16:01:04.000000 metabase-api-0.3.1/metabase_api/_helper_methods.py
--rw-rw-rw-   0        0        0     1108 2023-09-13 16:01:04.000000 metabase-api-0.3.1/metabase_api/_rest_methods.py
--rw-rw-rw-   0        0        0    17182 2023-09-13 16:01:04.000000 metabase-api-0.3.1/metabase_api/copy_methods.py
--rw-rw-rw-   0        0        0    11866 2023-09-13 16:01:04.000000 metabase-api-0.3.1/metabase_api/create_methods.py
--rw-rw-rw-   0        0        0    15125 2023-09-13 16:01:04.000000 metabase-api-0.3.1/metabase_api/metabase_api.py
-drwxrwxrwx   0        0        0        0 2023-09-13 16:01:32.686281 metabase-api-0.3.1/metabase_api.egg-info/
--rw-rw-rw-   0        0        0    13118 2023-09-13 16:01:32.000000 metabase-api-0.3.1/metabase_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2023-09-13 16:01:32.000000 metabase-api-0.3.1/metabase_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-13 16:01:32.000000 metabase-api-0.3.1/metabase_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-09-13 16:01:32.000000 metabase-api-0.3.1/metabase_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-09-13 16:01:32.000000 metabase-api-0.3.1/metabase_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-13 16:01:32.694534 metabase-api-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-09-13 16:01:04.000000 metabase-api-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-13 16:01:32.690519 metabase-api-0.3.1/tests/
--rw-rw-rw-   0        0        0        1 2023-09-13 16:01:04.000000 metabase-api-0.3.1/tests/__init__.py
--rw-rw-rw-   0        0        0    10420 2023-09-13 16:01:04.000000 metabase-api-0.3.1/tests/test_metabase_api.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:34:16.108412 metabase-api-0.3.2/
+-rw-rw-rw-   0        0        0     1080 2024-04-17 05:25:08.000000 metabase-api-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0    13118 2024-04-17 05:34:16.108412 metabase-api-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    12508 2024-04-17 05:25:08.000000 metabase-api-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 05:34:16.093900 metabase-api-0.3.2/metabase_api/
+-rw-rw-rw-   0        0        0       39 2024-04-17 05:25:08.000000 metabase-api-0.3.2/metabase_api/__init__.py
+-rw-rw-rw-   0        0        0    12728 2024-04-17 05:25:08.000000 metabase-api-0.3.2/metabase_api/_helper_methods.py
+-rw-rw-rw-   0        0        0     1108 2024-04-17 05:25:08.000000 metabase-api-0.3.2/metabase_api/_rest_methods.py
+-rw-rw-rw-   0        0        0    17174 2024-04-17 05:32:06.000000 metabase-api-0.3.2/metabase_api/copy_methods.py
+-rw-rw-rw-   0        0        0    11866 2024-04-17 05:25:08.000000 metabase-api-0.3.2/metabase_api/create_methods.py
+-rw-rw-rw-   0        0        0    15125 2024-04-17 05:25:08.000000 metabase-api-0.3.2/metabase_api/metabase_api.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:34:16.100917 metabase-api-0.3.2/metabase_api.egg-info/
+-rw-rw-rw-   0        0        0    13118 2024-04-17 05:34:15.000000 metabase-api-0.3.2/metabase_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2024-04-17 05:34:15.000000 metabase-api-0.3.2/metabase_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 05:34:15.000000 metabase-api-0.3.2/metabase_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-17 05:34:15.000000 metabase-api-0.3.2/metabase_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-17 05:34:15.000000 metabase-api-0.3.2/metabase_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 05:34:16.108412 metabase-api-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      687 2024-04-17 05:25:24.000000 metabase-api-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:34:16.103390 metabase-api-0.3.2/tests/
+-rw-rw-rw-   0        0        0        1 2024-04-17 05:25:08.000000 metabase-api-0.3.2/tests/__init__.py
+-rw-rw-rw-   0        0        0    11222 2024-04-17 05:25:08.000000 metabase-api-0.3.2/tests/test_metabase_api.py
```

### Comparing `metabase-api-0.3.1/LICENSE` & `metabase-api-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.1/PKG-INFO` & `metabase-api-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python Wrapper for Metabase API
 Home-page: https://github.com/vvaezian/metabase_api_python
 Author: Vahid Vaezian
 Author-email: vahid.vaezian@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `metabase-api-0.3.1/README.md` & `metabase-api-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.1/metabase_api/_helper_methods.py` & `metabase-api-0.3.2/metabase_api/_helper_methods.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.1/metabase_api/_rest_methods.py` & `metabase-api-0.3.2/metabase_api/_rest_methods.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.1/metabase_api/copy_methods.py` & `metabase-api-0.3.2/metabase_api/copy_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,23 +169,23 @@
         res = self.post('/api/collection/', 
                         json={'name':destination_dashboard_name + "'s cards", 
                                 'color':'#509EE3', 
                                 'parent_id':destination_collection_id})
         cards_collection_id = res['id']
 
         # duplicate cards and put them in the created collection and make a card_id mapping
-        source_dashboard_card_IDs = [ i['card_id'] for i in source_dashboard['ordered_cards'] if i['card_id'] is not None ]
+        source_dashboard_card_IDs = [ i['card_id'] for i in source_dashboard['dashcards'] if i['card_id'] is not None ]
         card_id_mapping = {}
         for card_id in source_dashboard_card_IDs:
             dup_card_id = self.copy_card(source_card_id=card_id, destination_collection_id=cards_collection_id)
             card_id_mapping[card_id] = dup_card_id
 
         # replace cards in the duplicated dashboard with duplicated cards
         dup_dashboard = self.get('/api/dashboard/{}'.format(dup_dashboard_id))
-        for card in dup_dashboard['ordered_cards']:
+        for card in dup_dashboard['dashcards']:
 
             # ignore text boxes. These get copied in the shallow-copy stage.
             if card['card_id'] is None:
                 continue
 
             # prepare a json to be used for replacing the cards in the duplicated dashboard
             new_card_id = card_id_mapping[card['card_id']]
```

### Comparing `metabase-api-0.3.1/metabase_api/create_methods.py` & `metabase-api-0.3.2/metabase_api/create_methods.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.1/metabase_api/metabase_api.py` & `metabase-api-0.3.2/metabase_api/metabase_api.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.1/metabase_api.egg-info/PKG-INFO` & `metabase-api-0.3.2/metabase_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python Wrapper for Metabase API
 Home-page: https://github.com/vvaezian/metabase_api_python
 Author: Vahid Vaezian
 Author-email: vahid.vaezian@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `metabase-api-0.3.1/setup.py` & `metabase-api-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="metabase-api",
-    version="0.3.1",
+    version="0.3.2",
     author="Vahid Vaezian",
     author_email="vahid.vaezian@gmail.com",
     description="A Python Wrapper for Metabase API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vvaezian/metabase_api_python",
     packages=setuptools.find_packages(),
```

### Comparing `metabase-api-0.3.1/tests/test_metabase_api.py` & `metabase-api-0.3.2/tests/test_metabase_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,19 +121,19 @@
   def test_get_table_metadata(self):
     table_info = mb.get_table_metadata(table_id=9)
     self.assertEqual(table_info['fields'][0]['name'], 'col1')
 
 
 
   def test_get_columns_name_id(self):
-    name_id_mapping = mb.get_columns_name_id(table_id=9)
-    self.assertEqual(name_id_mapping['col1'], 72)
+    name_id_mapping = mb.get_columns_name_id(table_id=1)  # table with id 1 is the products table from sample dataset
+    self.assertEqual(name_id_mapping['CATEGORY'], 1)
 
-    id_name_mapping = mb.get_columns_name_id(table_id=9, column_id_name=True)
-    self.assertEqual(id_name_mapping[72], 'col1')
+    id_name_mapping = mb.get_columns_name_id(table_id=1, column_id_name=True)
+    self.assertEqual(id_name_mapping[1], 'CATEGORY')
 
 
 
   ### Testing the Custom Functions
 
   def test_create_card(self):
     t = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
@@ -274,23 +274,37 @@
 
   def test_clone_card(self):
     # native question
     res = mb.clone_card(2, 9, 10, new_card_name='test_clone_native', new_card_collection_id=1, return_card=True)
     # simple/custom question
     res2 = mb.clone_card(3, 9, 10, new_card_name='test_clone_simple1', new_card_collection_id=1, return_card=True)
     res3 = mb.clone_card(4, 9, 10, new_card_name='test_clone_simple2', new_card_collection_id=1, return_card=True)
-    expected_res3_query = { 'database': 2,
+    
+    # rewriting a value because it's not reliable
+    res3['dataset_query']['query']['order-by'] = ''
+    
+    expected_res3_query_version1 = { 'database': 2,
                             'query': {'source-table': 10,
                                       'aggregation': [['avg', ['field', 75, None]]],
                                       'breakout': [['field', 74, None]],
-                                      'order-by': [['desc', ['aggregation', 0, None]]]
+                                      'order-by': ''
                                     },
                             'type': 'query'
                           }
-    self.assertEqual(res3['dataset_query'], expected_res3_query)
+    # we have two versions because the assigned field id is not necessarily in the order of columns as they appear in db
+    expected_res3_query_version2 = { 'database': 2,
+                            'query': {'source-table': 10,
+                                      'aggregation': [['avg', ['field', 74, None]]],
+                                      'breakout': [['field', 75, None]],
+                                      'order-by': ''
+                                    },
+                            'type': 'query'
+                          }
+    
+    self.assertTrue(res3['dataset_query'] == expected_res3_query_version1 or res3['dataset_query'] == expected_res3_query_version2, res3['dataset_query'])
 
     # add to cleanup list
     Metabase_API_Test.cleanup_objects['card'].extend([res['id'], res2['id'], res3['id']])
 
 
 
   def test_update_column(self):
```

