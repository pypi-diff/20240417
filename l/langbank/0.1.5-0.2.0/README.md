# Comparing `tmp/langbank-0.1.5.tar.gz` & `tmp/langbank-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langbank-0.1.5.tar", last modified: Mon Apr 15 23:23:56 2024, max compression
+gzip compressed data, was "langbank-0.2.0.tar", last modified: Wed Apr 17 01:45:08 2024, max compression
```

## Comparing `langbank-0.1.5.tar` & `langbank-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 23:23:56.869405 langbank-0.1.5/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      894 2024-04-15 23:23:56.869143 langbank-0.1.5/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)      622 2024-04-15 10:40:40.000000 langbank-0.1.5/README.md
--rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-04-15 23:23:56.869451 langbank-0.1.5/setup.cfg
--rw-r--r--   0 teddygonyea   (501) staff       (20)      492 2024-04-15 23:23:42.000000 langbank-0.1.5/setup.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 23:23:56.867674 langbank-0.1.5/src/
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 23:23:56.868226 langbank-0.1.5/src/langbank/
--rw-r--r--   0 teddygonyea   (501) staff       (20)       27 2024-04-14 12:25:24.000000 langbank-0.1.5/src/langbank/__init__.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     4400 2024-04-15 23:19:32.000000 langbank-0.1.5/src/langbank/main.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 23:23:56.868949 langbank-0.1.5/src/langbank.egg-info/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      894 2024-04-15 23:23:56.000000 langbank-0.1.5/src/langbank.egg-info/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)      222 2024-04-15 23:23:56.000000 langbank-0.1.5/src/langbank.egg-info/SOURCES.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-04-15 23:23:56.000000 langbank-0.1.5/src/langbank.egg-info/dependency_links.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)        9 2024-04-15 23:23:56.000000 langbank-0.1.5/src/langbank.egg-info/top_level.txt
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 23:23:56.868795 langbank-0.1.5/tests/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      430 2024-04-15 23:22:11.000000 langbank-0.1.5/tests/test.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-17 01:45:08.430269 langbank-0.2.0/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      894 2024-04-17 01:45:08.430023 langbank-0.2.0/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      622 2024-04-15 10:40:40.000000 langbank-0.2.0/README.md
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-04-17 01:45:08.430312 langbank-0.2.0/setup.cfg
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      492 2024-04-17 01:44:57.000000 langbank-0.2.0/setup.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-17 01:45:08.428317 langbank-0.2.0/src/
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-17 01:45:08.429014 langbank-0.2.0/src/langbank/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       67 2024-04-17 01:39:05.000000 langbank-0.2.0/src/langbank/__init__.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     4935 2024-04-17 01:20:50.000000 langbank-0.2.0/src/langbank/langbank.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     2754 2024-04-17 01:35:59.000000 langbank-0.2.0/src/langbank/review_list.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-17 01:45:08.429835 langbank-0.2.0/src/langbank.egg-info/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      894 2024-04-17 01:45:08.000000 langbank-0.2.0/src/langbank.egg-info/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      254 2024-04-17 01:45:08.000000 langbank-0.2.0/src/langbank.egg-info/SOURCES.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-04-17 01:45:08.000000 langbank-0.2.0/src/langbank.egg-info/dependency_links.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)        9 2024-04-17 01:45:08.000000 langbank-0.2.0/src/langbank.egg-info/top_level.txt
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-17 01:45:08.429669 langbank-0.2.0/tests/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      904 2024-04-17 01:43:16.000000 langbank-0.2.0/tests/test.py
```

### Comparing `langbank-0.1.5/PKG-INFO` & `langbank-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langbank
-Version: 0.1.5
+Version: 0.2.0
 Summary: A simple word bank for language learning
 Home-page: https://github.com/tebby24/langbank
 Author: Teddy Gonyea
 Author-email: enterted@gmail.com
 Keywords: language learning
 Description-Content-Type: text/markdown
```

### Comparing `langbank-0.1.5/README.md` & `langbank-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `langbank-0.1.5/src/langbank/main.py` & `langbank-0.2.0/src/langbank/langbank.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import json
 import os
 from datetime import datetime
 
 DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
+DEFAULT_FILE_PATH = os.path.expanduser("~/langbank/bank.json")
 
 
 class LangBank:
     """
     A class for managing a word bank for language learning.
     """
 
     def __init__(self, file_path=None):
         """
         Initialize LangBank with an optional file path.
         If no file path is provided, a default one will be used.
         """
         if file_path is None:
             # Default file path: ~/langbank/bank.json
-            self.file_path = os.path.expanduser("~/langbank/bank.json")
+            self.file_path = DEFAULT_FILE_PATH
         else:
             self.file_path = file_path
-
         self.setup_bank()
 
     def set_file_path(self, file_path):
         """
         Set the file path for the word bank.
         """
         self.file_path = file_path
@@ -33,15 +33,14 @@
         """
         Create the word bank file and parent directories if they do not exist.
         """
         # Create parent directories if they do not exist
         parent_dir = os.path.dirname(self.file_path)
         if not os.path.exists(parent_dir):
             os.makedirs(parent_dir)
-
         # Create the word bank file if it does not exist
         if not os.path.exists(self.file_path):
             with open(self.file_path, "w") as f:
                 f.write("[]")
 
     def get_bank(self):
         """
@@ -70,46 +69,62 @@
         Args:
             bank: The word bank (list) to write.
         """
         # Convert datetime objects to strings
         for item in bank:
             if "datetime" in item:
                 item["datetime"] = item["datetime"].strftime(DATETIME_FORMAT)
-
         # Write bank to JSON file
         with open(self.file_path, "w") as f:
             json.dump(bank, f, indent=4)
 
     def add_word(self, word, tags=None):
         """
         Add a new word to the wordbank
         Args:
             word: the word to add
             tags: a list of string tags
         """
         if tags is None:
             tags = []
-
         dt = datetime.now()
         entry = {"word": word, "datetime": dt, "tags": tags}
         bank = self.get_bank()
         bank.append(entry)
         self.write_bank(bank)
 
+    def get_all_words(self):
+        """
+        Get a list of all the words in the bank
+        """
+        bank = self.get_bank()
+        words = [entry["word"] for entry in bank]
+        return words
+
+    def get_all_unique_words(self):
+        """
+        Get a list of all the unique words in the bank
+        """
+        bank = self.get_bank()
+        words = []
+        for entry in bank:
+            if entry["word"] not in words:
+                words.append(entry["word"])
+        return words
+
     def get_words_from_past_n_days(self, n=0):
         """
         Get a list of all the words added in the past n days, where n=0 will return the words added today
         """
         bank = self.get_bank()
         today = datetime.now().date()
         words = []
         for entry in bank:
             if (today - entry["datetime"].date()).days <= n:
                 words.append(entry["word"])
-
         return words
 
     def get_todays_words(self):
         """
         Get the list of words added today
         """
         return self.get_words_from_past_n_days(0)
@@ -119,33 +134,30 @@
         Get a list of all the words with a specific tag
         """
         bank = self.get_bank()
         words = []
         for entry in bank:
             if tag in entry["tags"]:
                 words.append(entry["word"])
-
         return words
 
     def get_words_by_date(self, date):
         """
         Get a list of all the words added on a specific date
         """
         bank = self.get_bank()
         words = []
         for entry in bank:
             if entry["datetime"].date() == date:
                 words.append(entry["word"])
-
         return words
 
     def occurences(self, word):
         """
         Get the number of times a word has been added to the bank
         """
         bank = self.get_bank()
         count = 0
         for entry in bank:
             if entry["word"] == word:
                 count += 1
-
         return count
```

### Comparing `langbank-0.1.5/src/langbank.egg-info/PKG-INFO` & `langbank-0.2.0/src/langbank.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langbank
-Version: 0.1.5
+Version: 0.2.0
 Summary: A simple word bank for language learning
 Home-page: https://github.com/tebby24/langbank
 Author: Teddy Gonyea
 Author-email: enterted@gmail.com
 Keywords: language learning
 Description-Content-Type: text/markdown
```

