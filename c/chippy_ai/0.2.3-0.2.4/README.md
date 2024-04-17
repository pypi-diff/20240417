# Comparing `tmp/chippy_ai-0.2.3.tar.gz` & `tmp/chippy_ai-0.2.4.tar.gz`

## Comparing `chippy_ai-0.2.3.tar` & `chippy_ai-0.2.4.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/MANIFEST.in
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/git.txt
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/setup.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/shell.txt
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/build/lib/chip/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/build/lib/chip/config.ini
--rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/build/lib/chip/main.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/build/lib/chippy_ai/__init__.py
--rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/build/lib/chippy_ai/main.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chip.egg-info/PKG-INFO
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chip.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chip.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chip.egg-info/entry_points.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chip.egg-info/top_level.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chip_ai.egg-info/PKG-INFO
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chip_ai.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chip_ai.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chip_ai.egg-info/entry_points.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chip_ai.egg-info/top_level.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chippy_ai/.gitignore
--rw-r--r--   0        0        0     9743 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chippy_ai/README.MD
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chippy_ai/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chippy_ai/config.ini
--rw-r--r--   0        0        0    12398 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chippy_ai/main.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chippy_ai/pyproject.toml
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chippy_ai.egg-info/PKG-INFO
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chippy_ai.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chippy_ai.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chippy_ai.egg-info/entry_points.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/chippy_ai.egg-info/top_level.txt
--rw-r--r--   0        0        0   340261 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/images/chip1.png
--rw-r--r--   0        0        0   376104 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/images/chip2.png
--rw-r--r--   0        0        0   798043 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/images/demo.gif
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/LICENSE
--rw-r--r--   0        0        0     9323 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/README.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     9833 2020-02-02 00:00:00.000000 chippy_ai-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/.env
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/MANIFEST.in
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/setup.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/build/lib/chip/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/build/lib/chip/config.ini
+-rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/build/lib/chip/main.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/build/lib/chippy_ai/__init__.py
+-rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/build/lib/chippy_ai/main.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip.egg-info/entry_points.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip.egg-info/top_level.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip_ai.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip_ai.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip_ai.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip_ai.egg-info/entry_points.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chip_ai.egg-info/top_level.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/.gitignore
+-rw-r--r--   0        0        0     9743 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/README.MD
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/config.ini
+-rw-r--r--   0        0        0    13075 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/main.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/pyproject.toml
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/cheats/git.txt
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai/cheats/shell.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai.egg-info/entry_points.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/chippy_ai.egg-info/top_level.txt
+-rw-r--r--   0        0        0   340261 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/images/chip1.png
+-rw-r--r--   0        0        0   376104 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/images/chip2.png
+-rw-r--r--   0        0        0   798043 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/images/demo.gif
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/LICENSE
+-rw-r--r--   0        0        0     9323 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     9833 2020-02-02 00:00:00.000000 chippy_ai-0.2.4/PKG-INFO
```

### Comparing `chippy_ai-0.2.3/git.txt` & `chippy_ai-0.2.4/chippy_ai/cheats/git.txt`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.3/shell.txt` & `chippy_ai-0.2.4/chippy_ai/cheats/shell.txt`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.3/.github/workflows/publish.yml` & `chippy_ai-0.2.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.3/build/lib/chip/main.py` & `chippy_ai-0.2.4/build/lib/chip/main.py`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.3/build/lib/chippy_ai/main.py` & `chippy_ai-0.2.4/build/lib/chippy_ai/main.py`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.3/chippy_ai/README.MD` & `chippy_ai-0.2.4/chippy_ai/README.MD`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.3/chippy_ai/main.py` & `chippy_ai-0.2.4/chippy_ai/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import textwrap
 import subprocess
 import configparser
 from openai import OpenAI
 from dotenv import load_dotenv
 import os
 import configparser
+import os
+import os
 import importlib.resources as pkg_resources
 
 #old config
 # Read configuration
 #config = configparser.ConfigParser()
 #config.read('config.ini')
 
@@ -197,34 +199,48 @@
     )
     return chat_completion.choices[0].message.content
 
 
 
 def read_shell_file():
     try:
-        with open('shell.txt', 'r') as file:
+        package_dir = os.path.dirname(os.path.abspath(__file__))
+        file_path = os.path.join(package_dir, 'cheats', 'shell.txt')
+        with open(file_path, 'r') as file:
             shell_content = file.read()
             return shell_content
     except FileNotFoundError:
         print("File not found: shell.txt")
     except Exception as e:
         print(f"Error reading file: {e}")
 
 def read_git_file():
     try:
-        with open('git.txt', 'r') as file:
+        with open('/cheats/git.txt', 'r') as file:
             git_content = file.read()
             return git_content
             #formatted_content = format_in_rectangle(content)
             #print(formatted_content)
     except FileNotFoundError:
         print("File not found: shell.txt")
     except Exception as e:
         print(f"Error reading file: {e}")
 
+
+def create_env_file(api_key):
+    try:
+        env_file_path = ".env"
+        with open(env_file_path, 'w') as file:
+            file.write(f"TOGETHER_API_KEY={api_key}")
+        print("Successfully created .env file.")
+    except Exception as e:
+        print(f"Error creating .env file: {e}")
+        #later expand function to validate the api key by running a quick call
+
+
 def main():
     red_color_code = '\033[91m'  # ANSI color code for red
     green_color_code = '\033[92m'  # ANSI color code for green
     reset_color = '\033[0m'  # Resets the color to default
     if hardcore_mode.lower() != 'yes':
         if len(sys.argv) > 1:
             if sys.argv[1] == "error":
@@ -255,14 +271,17 @@
                     print(format_in_rectangle(detailed_analysis))
             elif sys.argv[1] == "shell":
                 text = read_shell_file()
                 print(format_in_rectangle(text))
             elif sys.argv[1] == "git":
                 text = read_git_file()
                 print(format_in_rectangle(text))
+            elif sys.argv[1] == "api" and len(sys.argv) > 2:
+                api_key = sys.argv[2]
+                create_env_file(api_key)
             elif sys.argv[1] == "-q" and len(sys.argv) > 2:
                 question = " ".join(sys.argv[2:])
                 answer = ask_gpt(question)
                 print(format_in_rectangle("△ Chippy Q&A △"))
                 print(format_in_rectangle(f"Q: {question}\n\nA: {answer}"))
             else:
                 print(format_in_rectangle("Usage: chip error"))
```

### Comparing `chippy_ai-0.2.3/chippy_ai/pyproject.toml` & `chippy_ai-0.2.4/chippy_ai/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chippy_ai"
-version = "0.2.3"
+version = "0.2.4"
 description = "A small example package"
 readme = "README.md"
 authors = [{ name = "Alex Behrens", email = "alexanderbbehrens@gmail.com" }]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `chippy_ai-0.2.3/images/chip1.png` & `chippy_ai-0.2.4/images/chip1.png`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.3/images/chip2.png` & `chippy_ai-0.2.4/images/chip2.png`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.3/images/demo.gif` & `chippy_ai-0.2.4/images/demo.gif`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.3/LICENSE` & `chippy_ai-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.3/README.md` & `chippy_ai-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `chippy_ai-0.2.3/pyproject.toml` & `chippy_ai-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chippy_ai"
-version = "0.2.3"
+version = "0.2.4"
 description = "A small example package"
 readme = "README.md"
 authors = [{ name = "Alex Behrens", email = "alexanderbbehrens@gmail.com" }]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `chippy_ai-0.2.3/PKG-INFO` & `chippy_ai-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: chippy_ai
-Version: 0.2.3
+Version: 0.2.4
 Summary: A small example package
 Project-URL: Homepage, https://github.com/alexbehrens/chip
 Project-URL: Issues, https://github.com/alexbehrens/chip/issues
 Author-email: Alex Behrens <alexanderbbehrens@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

