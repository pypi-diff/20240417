# Comparing `tmp/chippy_ai-0.2.6.tar.gz` & `tmp/chippy_ai-0.2.7.tar.gz`

## Comparing `chippy_ai-0.2.6.tar` & `chippy_ai-0.2.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/MANIFEST.in
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/setup.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/build/lib/chip/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/build/lib/chip/config.ini
--rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/build/lib/chip/main.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/build/lib/chippy_ai/__init__.py
--rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/build/lib/chippy_ai/main.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip.egg-info/PKG-INFO
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip.egg-info/entry_points.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip.egg-info/top_level.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip_ai.egg-info/PKG-INFO
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip_ai.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip_ai.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip_ai.egg-info/entry_points.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chip_ai.egg-info/top_level.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/.gitignore
--rw-r--r--   0        0        0     9743 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/README.MD
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/config.ini
--rw-r--r--   0        0        0    13460 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/main.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/pyproject.toml
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/cheats/git.txt
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/cheats/shell.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai/env/placeholder.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai.egg-info/PKG-INFO
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai.egg-info/entry_points.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/chippy_ai.egg-info/top_level.txt
--rw-r--r--   0        0        0   340261 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/images/chip1.png
--rw-r--r--   0        0        0   376104 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/images/chip2.png
--rw-r--r--   0        0        0   798043 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/images/demo.gif
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/LICENSE
--rw-r--r--   0        0        0     9323 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/README.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     9833 2020-02-02 00:00:00.000000 chippy_ai-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/MANIFEST.in
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/setup.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/build/lib/chip/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/build/lib/chip/config.ini
+-rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/build/lib/chip/main.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/build/lib/chippy_ai/__init__.py
+-rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/build/lib/chippy_ai/main.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chip.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chip.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chip.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chip.egg-info/entry_points.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chip.egg-info/top_level.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chip_ai.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chip_ai.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chip_ai.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chip_ai.egg-info/entry_points.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chip_ai.egg-info/top_level.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chippy_ai/.gitignore
+-rw-r--r--   0        0        0     9743 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chippy_ai/README.MD
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chippy_ai/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chippy_ai/config.ini
+-rw-r--r--   0        0        0    12821 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chippy_ai/main.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chippy_ai/pyproject.toml
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chippy_ai/cheats/git.txt
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chippy_ai/cheats/shell.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chippy_ai/env/placeholder.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chippy_ai.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chippy_ai.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chippy_ai.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chippy_ai.egg-info/entry_points.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/chippy_ai.egg-info/top_level.txt
+-rw-r--r--   0        0        0   340261 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/images/chip1.png
+-rw-r--r--   0        0        0   376104 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/images/chip2.png
+-rw-r--r--   0        0        0   798043 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/images/demo.gif
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/LICENSE
+-rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 chippy_ai-0.2.7/PKG-INFO
```

### Comparing `chippy_ai-0.2.6/setup.py` & `chippy_ai-0.2.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     url='https://github.com/yourusername/chippy_ai',  # Optionally add the URL of your project
     packages=find_packages(),
     include_package_data=True,  # Uncomment this if you use MANIFEST.in for including non-code files
     package_data={
         'chippy_ai': ['config.ini', 'README.md']
     },
     install_requires=[
-        'openai',          # Ensure these are the correct package names on PyPI
+        'OpenAI',          # Ensure these are the correct package names on PyPI
         'python-dotenv'
     ],
     entry_points={
         'console_scripts': [
             'chip=chippy_ai.main:main',
         ],
     },
```

### Comparing `chippy_ai-0.2.6/.github/workflows/publish.yml` & `chippy_ai-0.2.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.6/build/lib/chip/main.py` & `chippy_ai-0.2.7/build/lib/chip/main.py`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.6/build/lib/chippy_ai/main.py` & `chippy_ai-0.2.7/build/lib/chippy_ai/main.py`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.6/chippy_ai/README.MD` & `chippy_ai-0.2.7/chippy_ai/README.MD`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.6/chippy_ai/main.py` & `chippy_ai-0.2.7/chippy_ai/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,45 +7,30 @@
 from dotenv import load_dotenv
 import os
 import configparser
 import os
 import os
 import importlib.resources as pkg_resources
 
-#old config
-# Read configuration
-#config = configparser.ConfigParser()
-#config.read('config.ini')
-
-# Configurations for ERROR and QUESTION
-#ERROR_CONFIG = config['ERROR']
-#QUESTION_CONFIG = config['QUESTION']
-#mode = ERROR_CONFIG.get('Default', 'HardcoreMode')
-#hardcore_mode = config['DEFAULT'].get('Hardcore', 'no').lower()
-
 def load_configuration():
     try:
         with pkg_resources.open_text('chippy_ai', 'config.ini') as config_file:
             config = configparser.ConfigParser()
             config.read_file(config_file)
-            # Debug: Print out sections and keys to verify
-            #print("Available sections:", config.sections())
-            #for section in config.sections():
-                #print(f"Keys in {section}: {list(config[section])}")
             return config
     except Exception as e:
         print(f"Failed to read or parse config.ini: {e}")
         raise
 
 config = load_configuration()
 # Access the specific configuration sections
 ERROR_CONFIG = config['ERROR']
 QUESTION_CONFIG = config['QUESTION']
 
-# Assuming 'Default' is a section in your config.ini, and 'HardcoreMode' is a key within that section
+# Assuming 'Default' is a section in config.ini, and 'HardcoreMode' is a key within that section
 mode = config.get('Default', 'HardcoreMode', fallback='HardcoreModeDefault')
 hardcore_mode = config.get('DEFAULT', 'Hardcore', fallback='no').lower()
 
 
 #load env
 package_dir = os.path.dirname(os.path.abspath(__file__))
 env_file_path = os.path.join(package_dir, 'env', '.env')
@@ -226,25 +211,20 @@
         print("File not found: shell.txt")
     except Exception as e:
         print(f"Error reading file: {e}")
 
 
 def create_env_file(api_key):
     try:
-
-
-
         package_dir = os.path.dirname(os.path.abspath(__file__))
         file_path = os.path.join(package_dir, 'env', '.env')
         with open(file_path, 'w+') as file:
             git_content = file.read()
             file.write(f"TOGETHER_API_KEY={api_key}")
-        print("Successfully created .env file.")
-        print(f"File path: {file_path}")
-        print(f"File content:\n{file.read()}")
+        print(format_in_rectangle("Successfully created .env file."))
     except Exception as e:
         print(f"Error creating .env file: {e}")
         #later expand function to validate the api key by running a quick call
 
 
 def main():
     red_color_code = '\033[91m'  # ANSI color code for red
```

### Comparing `chippy_ai-0.2.6/chippy_ai/pyproject.toml` & `chippy_ai-0.2.7/chippy_ai/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chippy_ai"
-version = "0.2.6"
+version = "0.2.7"
 description = "A small example package"
 readme = "README.md"
 authors = [{ name = "Alex Behrens", email = "alexanderbbehrens@gmail.com" }]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `chippy_ai-0.2.6/chippy_ai/cheats/git.txt` & `chippy_ai-0.2.7/chippy_ai/cheats/git.txt`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.6/chippy_ai/cheats/shell.txt` & `chippy_ai-0.2.7/chippy_ai/cheats/shell.txt`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.6/images/chip1.png` & `chippy_ai-0.2.7/images/chip1.png`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.6/images/chip2.png` & `chippy_ai-0.2.7/images/chip2.png`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.6/images/demo.gif` & `chippy_ai-0.2.7/images/demo.gif`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.6/LICENSE` & `chippy_ai-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.6/README.md` & `chippy_ai-0.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     ```bash
     pip install chippy-ai
     ```
 
 2. **Configuration**
 
     Set up your [together.ai](https://together.ai) key:
-    - Save API keys in your environment variables for secure access.
-    - Enter keys via command ```bash chip api "YOUR_KEY_HERE"``` 
+    - Enter API keys via command ```chip api "YOUR_KEY_HERE"``` 
     - or via the `config.ini` file
     - Configure Chippy to your liking through the `config.ini` file or via command-line options.
 
 3. **Usage**
 
 
     **Error Analysis**
```

### Comparing `chippy_ai-0.2.6/pyproject.toml` & `chippy_ai-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chippy_ai"
-version = "0.2.6"
+version = "0.2.7"
 description = "A small example package"
 readme = "README.md"
 authors = [{ name = "Alex Behrens", email = "alexanderbbehrens@gmail.com" }]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `chippy_ai-0.2.6/PKG-INFO` & `chippy_ai-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: chippy_ai
-Version: 0.2.6
+Version: 0.2.7
 Summary: A small example package
 Project-URL: Homepage, https://github.com/alexbehrens/chip
 Project-URL: Issues, https://github.com/alexbehrens/chip/issues
 Author-email: Alex Behrens <alexanderbbehrens@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -47,16 +47,15 @@
     ```bash
     pip install chippy-ai
     ```
 
 2. **Configuration**
 
     Set up your [together.ai](https://together.ai) key:
-    - Save API keys in your environment variables for secure access.
-    - Enter keys via command ```bash chip api "YOUR_KEY_HERE"``` 
+    - Enter API keys via command ```chip api "YOUR_KEY_HERE"``` 
     - or via the `config.ini` file
     - Configure Chippy to your liking through the `config.ini` file or via command-line options.
 
 3. **Usage**
 
 
     **Error Analysis**
```

