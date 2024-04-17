# Comparing `tmp/kurumii-1.4.7.tar.gz` & `tmp/kurumii-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kurumii-1.4.7.tar", last modified: Fri Apr 12 08:50:24 2024, max compression
+gzip compressed data, was "kurumii-1.4.8.tar", last modified: Wed Apr 17 08:21:09 2024, max compression
```

## Comparing `kurumii-1.4.7.tar` & `kurumii-1.4.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 08:50:24.356714 kurumii-1.4.7/
--rw-rw-rw-   0        0        0      307 2024-04-12 08:50:24.354564 kurumii-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 kurumii-1.4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 08:50:24.302254 kurumii-1.4.7/kurumii/
--rw-rw-rw-   0        0        0     3847 2024-04-12 08:45:13.000000 kurumii-1.4.7/kurumii/__init__.py
--rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 kurumii-1.4.7/kurumii/additional_functions.py
--rw-rw-rw-   0        0        0    13965 2024-04-08 07:07:29.000000 kurumii-1.4.7/kurumii/ascii.py
--rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 kurumii-1.4.7/kurumii/data_manipulation.py
--rw-rw-rw-   0        0        0    35843 2024-04-12 08:47:35.000000 kurumii-1.4.7/kurumii/database.py
--rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 kurumii-1.4.7/kurumii/files.py
--rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 kurumii-1.4.7/kurumii/id.py
--rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 kurumii-1.4.7/kurumii/jsonify.py
--rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 kurumii-1.4.7/kurumii/keyboard.py
--rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 kurumii-1.4.7/kurumii/print_additions.py
--rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 kurumii-1.4.7/kurumii/profanities.py
--rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 kurumii-1.4.7/kurumii/youtube.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:50:24.351394 kurumii-1.4.7/kurumii.egg-info/
--rw-rw-rw-   0        0        0      307 2024-04-12 08:50:24.000000 kurumii-1.4.7/kurumii.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-04-12 08:50:24.000000 kurumii-1.4.7/kurumii.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 08:50:24.000000 kurumii-1.4.7/kurumii.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-12 08:50:24.000000 kurumii-1.4.7/kurumii.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 08:50:24.000000 kurumii-1.4.7/kurumii.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 08:50:24.356714 kurumii-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0      386 2024-04-12 08:49:43.000000 kurumii-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:21:09.860334 kurumii-1.4.8/
+-rw-rw-rw-   0        0        0      307 2024-04-17 08:21:09.857854 kurumii-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 kurumii-1.4.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 08:21:09.812775 kurumii-1.4.8/kurumii/
+-rw-rw-rw-   0        0        0     3847 2024-04-12 08:45:13.000000 kurumii-1.4.8/kurumii/__init__.py
+-rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 kurumii-1.4.8/kurumii/additional_functions.py
+-rw-rw-rw-   0        0        0    13965 2024-04-08 07:07:29.000000 kurumii-1.4.8/kurumii/ascii.py
+-rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 kurumii-1.4.8/kurumii/data_manipulation.py
+-rw-rw-rw-   0        0        0    38109 2024-04-17 08:20:32.000000 kurumii-1.4.8/kurumii/database.py
+-rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 kurumii-1.4.8/kurumii/files.py
+-rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 kurumii-1.4.8/kurumii/id.py
+-rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 kurumii-1.4.8/kurumii/jsonify.py
+-rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 kurumii-1.4.8/kurumii/keyboard.py
+-rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 kurumii-1.4.8/kurumii/print_additions.py
+-rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 kurumii-1.4.8/kurumii/profanities.py
+-rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 kurumii-1.4.8/kurumii/youtube.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:21:09.849255 kurumii-1.4.8/kurumii.egg-info/
+-rw-rw-rw-   0        0        0      307 2024-04-17 08:21:09.000000 kurumii-1.4.8/kurumii.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2024-04-17 08:21:09.000000 kurumii-1.4.8/kurumii.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 08:21:09.000000 kurumii-1.4.8/kurumii.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-17 08:21:09.000000 kurumii-1.4.8/kurumii.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 08:21:09.000000 kurumii-1.4.8/kurumii.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 08:21:09.861378 kurumii-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      386 2024-04-17 08:10:05.000000 kurumii-1.4.8/setup.py
```

### Comparing `kurumii-1.4.7/kurumii/__init__.py` & `kurumii-1.4.8/kurumii/__init__.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.7/kurumii/additional_functions.py` & `kurumii-1.4.8/kurumii/additional_functions.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.7/kurumii/ascii.py` & `kurumii-1.4.8/kurumii/ascii.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.7/kurumii/data_manipulation.py` & `kurumii-1.4.8/kurumii/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.7/kurumii/database.py` & `kurumii-1.4.8/kurumii/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import os
 import json
 import sqlite3
+import shutil
+from datetime import datetime
+
 
 class DatabaseCreationError(Exception):
     pass
 class FileExistsError(Exception):
     pass
 class FileDeletionError(Exception):
     pass
@@ -911,14 +914,80 @@
     except Exception as e:
         if logging:
             print(f"Error loading data: {str(e)}")
         return None
     finally:
         conn.close()
 
+def backup_database(source_filepath, backup_dir=".\\backup"):
+    """
+    Create a backup of an SQLite database file with a specified naming convention.
+
+    Args:
+        - source_filepath (str): The path to the source SQLite database file.
+        - backup_dir (str, optional): The directory where the backup will be saved. Defaults to ".\\backup".
+
+    Returns:
+        - str: The filepath of the created backup.
+        - bool: True if the backup was successful, False otherwise.
+
+    Example: 
+        >>> backup_database(backup_dir="./db-bu",source_filepath="./db/test.db")
+    """
+    try:
+        if not os.path.exists(backup_dir):
+            os.makedirs(backup_dir)
+
+        # Extract filename and extension from source filepath
+        filename, ext = os.path.splitext(os.path.basename(source_filepath))
+        
+        # Generate backup filename with date
+        backup_filename = f"backup-{filename}-{datetime.now().strftime('%Y-%m-%d_%H-%M-%S')}{ext}"
+        
+        # Create backup filepath
+        backup_filepath = os.path.join(backup_dir, backup_filename)
+        
+        # Perform backup
+        shutil.copyfile(source_filepath, backup_filepath)
+        
+        return backup_filepath, True
+    except Exception as e:
+        print(f"Error backing up database: {e}")
+        return None, False
+
+def check_if_table_exists(filepath, table_name):
+    """
+    Check if a table exists in an SQLite database.
+
+    Args:
+        - filepath (str): The path to the SQLite database file.
+        - table_name (str): The name of the table to check.
+
+    Returns:
+        - bool: Whether the table exists (True) or not (False).
+    
+    Example:
+        >>> ex = check_if_table_exists(filepath="./db/test.db",table_name="data3")
+    """
+    try:
+        conn = sqlite3.connect(filepath)
+        c = conn.cursor()
+
+        # Check if the table exists
+        c.execute(f"SELECT name FROM sqlite_master WHERE type='table' AND name=?", (table_name,))
+        result = c.fetchone()
+
+        conn.close()
+
+        return result is not None
+    except Exception as e:
+        print(f"Error checking if table exists: {e}")
+        return False
+
+
 
 
 
 # Example usage:
 # exists = database_exists("example.db")
 # print(exists)
 # remove_data_from_table(table_name="data2",filepath=".\\db\\test.db",key_values=5333,logging=True)
```

### Comparing `kurumii-1.4.7/kurumii/files.py` & `kurumii-1.4.8/kurumii/files.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.7/kurumii/id.py` & `kurumii-1.4.8/kurumii/id.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.7/kurumii/jsonify.py` & `kurumii-1.4.8/kurumii/jsonify.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.7/kurumii/keyboard.py` & `kurumii-1.4.8/kurumii/keyboard.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.7/kurumii/print_additions.py` & `kurumii-1.4.8/kurumii/print_additions.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.7/kurumii/profanities.py` & `kurumii-1.4.8/kurumii/profanities.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.7/kurumii/youtube.py` & `kurumii-1.4.8/kurumii/youtube.py`

 * *Files identical despite different names*

