# Comparing `tmp/chippy_ai-0.2.4.tar.gz` & `tmp/chippy_ai-0.2.5.tar.gz`

## Comparing `chippy_ai-0.2.4.tar` & `chippy_ai-0.2.5.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/.env
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/MANIFEST.in
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/setup.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/build/lib/chip/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/build/lib/chip/config.ini
--rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/build/lib/chip/main.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/build/lib/chippy_ai/__init__.py
--rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/build/lib/chippy_ai/main.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip.egg-info/PKG-INFO
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip.egg-info/entry_points.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip.egg-info/top_level.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip_ai.egg-info/PKG-INFO
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip_ai.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip_ai.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip_ai.egg-info/entry_points.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip_ai.egg-info/top_level.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/.gitignore
--rw-r--r--   0        0        0     9743 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/README.MD
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/config.ini
--rw-r--r--   0        0        0    13075 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/main.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/pyproject.toml
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/cheats/git.txt
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/cheats/shell.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai.egg-info/PKG-INFO
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai.egg-info/entry_points.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai.egg-info/top_level.txt
--rw-r--r--   0        0        0   340261 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/images/chip1.png
--rw-r--r--   0        0        0   376104 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/images/chip2.png
--rw-r--r--   0        0        0   798043 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/images/demo.gif
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/LICENSE
--rw-r--r--   0        0        0     9323 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/README.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     9833 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/MANIFEST.in
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/setup.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/build/lib/chip/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/build/lib/chip/config.ini
+-rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/build/lib/chip/main.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/build/lib/chippy_ai/__init__.py
+-rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/build/lib/chippy_ai/main.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip.egg-info/entry_points.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip.egg-info/top_level.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip_ai.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip_ai.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip_ai.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip_ai.egg-info/entry_points.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chip_ai.egg-info/top_level.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/.gitignore
+-rw-r--r--   0        0        0     9743 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/README.MD
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/config.ini
+-rw-r--r--   0        0        0    13460 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/main.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/pyproject.toml
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/cheats/git.txt
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai/cheats/shell.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai.egg-info/entry_points.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/chippy_ai.egg-info/top_level.txt
+-rw-r--r--   0        0        0   340261 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/images/chip1.png
+-rw-r--r--   0        0        0   376104 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/images/chip2.png
+-rw-r--r--   0        0        0   798043 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/images/demo.gif
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/LICENSE
+-rw-r--r--   0        0        0     9323 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     9833 2020-02-02 00:00:00.000000 chippy_ai-0.2.5/PKG-INFO
```

### Comparing `chippy_ai-0.2.4/.github/workflows/publish.yml` & `chippy_ai-0.2.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.4/build/lib/chip/main.py` & `chippy_ai-0.2.5/build/lib/chip/main.py`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.4/build/lib/chippy_ai/main.py` & `chippy_ai-0.2.5/build/lib/chippy_ai/main.py`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.4/chippy_ai/README.MD` & `chippy_ai-0.2.5/chippy_ai/README.MD`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.4/chippy_ai/main.py` & `chippy_ai-0.2.5/chippy_ai/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,16 +43,18 @@
 
 # Assuming 'Default' is a section in your config.ini, and 'HardcoreMode' is a key within that section
 mode = config.get('Default', 'HardcoreMode', fallback='HardcoreModeDefault')
 hardcore_mode = config.get('DEFAULT', 'Hardcore', fallback='no').lower()
 
 
 #load env
+package_dir = os.path.dirname(os.path.abspath(__file__))
+env_file_path = os.path.join(package_dir, 'env', '.env')
+load_dotenv(env_file_path)
 load_dotenv()  # load all the environment variables from a .env file
-
 api_key = os.getenv("TOGETHER_API_KEY")
 
 
 
 
 
 def format_in_rectangle(text, width=65, color_code='\033[94m'):
@@ -211,31 +213,38 @@
     except FileNotFoundError:
         print("File not found: shell.txt")
     except Exception as e:
         print(f"Error reading file: {e}")
 
 def read_git_file():
     try:
-        with open('/cheats/git.txt', 'r') as file:
+        package_dir = os.path.dirname(os.path.abspath(__file__))
+        file_path = os.path.join(package_dir, 'cheats', 'git.txt')
+        with open(file_path, 'r') as file:
             git_content = file.read()
             return git_content
-            #formatted_content = format_in_rectangle(content)
-            #print(formatted_content)
     except FileNotFoundError:
         print("File not found: shell.txt")
     except Exception as e:
         print(f"Error reading file: {e}")
 
 
 def create_env_file(api_key):
     try:
-        env_file_path = ".env"
-        with open(env_file_path, 'w') as file:
+
+
+
+        package_dir = os.path.dirname(os.path.abspath(__file__))
+        file_path = os.path.join(package_dir, 'env', '.env')
+        with open(file_path, 'w+') as file:
+            git_content = file.read()
             file.write(f"TOGETHER_API_KEY={api_key}")
         print("Successfully created .env file.")
+        print(f"File path: {file_path}")
+        print(f"File content:\n{file.read()}")
     except Exception as e:
         print(f"Error creating .env file: {e}")
         #later expand function to validate the api key by running a quick call
 
 
 def main():
     red_color_code = '\033[91m'  # ANSI color code for red
```

### Comparing `chippy_ai-0.2.4/chippy_ai/pyproject.toml` & `chippy_ai-0.2.5/chippy_ai/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chippy_ai"
-version = "0.2.4"
+version = "0.2.5"
 description = "A small example package"
 readme = "README.md"
 authors = [{ name = "Alex Behrens", email = "alexanderbbehrens@gmail.com" }]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `chippy_ai-0.2.4/chippy_ai/cheats/git.txt` & `chippy_ai-0.2.5/chippy_ai/cheats/git.txt`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.4/chippy_ai/cheats/shell.txt` & `chippy_ai-0.2.5/chippy_ai/cheats/shell.txt`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.4/images/chip1.png` & `chippy_ai-0.2.5/images/chip1.png`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.4/images/chip2.png` & `chippy_ai-0.2.5/images/chip2.png`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.4/images/demo.gif` & `chippy_ai-0.2.5/images/demo.gif`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.4/LICENSE` & `chippy_ai-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.4/README.md` & `chippy_ai-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.4/pyproject.toml` & `chippy_ai-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chippy_ai"
-version = "0.2.4"
+version = "0.2.5"
 description = "A small example package"
 readme = "README.md"
 authors = [{ name = "Alex Behrens", email = "alexanderbbehrens@gmail.com" }]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `chippy_ai-0.2.4/PKG-INFO` & `chippy_ai-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: chippy_ai
-Version: 0.2.4
+Version: 0.2.5
 Summary: A small example package
 Project-URL: Homepage, https://github.com/alexbehrens/chip
 Project-URL: Issues, https://github.com/alexbehrens/chip/issues
 Author-email: Alex Behrens <alexanderbbehrens@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

