# Comparing `tmp/pydcogenerator-0.0.5.tar.gz` & `tmp/pydcogenerator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydcogenerator-0.0.5.tar", last modified: Wed Apr 17 05:07:56 2024, max compression
+gzip compressed data, was "pydcogenerator-0.1.0.tar", last modified: Wed Apr 17 10:51:18 2024, max compression
```

## Comparing `pydcogenerator-0.0.5.tar` & `pydcogenerator-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 05:07:56.006252 pydcogenerator-0.0.5/
--rw-rw-rw-   0        0        0     1088 2024-03-20 14:29:16.000000 pydcogenerator-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1768 2024-04-17 05:07:56.004250 pydcogenerator-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1157 2024-04-11 08:00:44.000000 pydcogenerator-0.0.5/README.md
--rw-rw-rw-   0        0        0      726 2024-04-11 15:24:49.000000 pydcogenerator-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 05:07:56.007195 pydcogenerator-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 05:07:55.917476 pydcogenerator-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 05:07:56.003222 pydcogenerator-0.0.5/src/pydcogenerator.egg-info/
--rw-rw-rw-   0        0        0     1768 2024-04-17 05:07:55.000000 pydcogenerator-0.0.5/src/pydcogenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-04-17 05:07:55.000000 pydcogenerator-0.0.5/src/pydcogenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 05:07:55.000000 pydcogenerator-0.0.5/src/pydcogenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-17 05:07:55.000000 pydcogenerator-0.0.5/src/pydcogenerator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 05:07:55.998786 pydcogenerator-0.0.5/src/pydocgenerator/
--rw-rw-rw-   0        0        0      368 2024-04-11 09:27:58.000000 pydcogenerator-0.0.5/src/pydocgenerator/__init__.py
--rw-rw-rw-   0        0        0     2796 2024-04-17 05:01:29.000000 pydcogenerator-0.0.5/src/pydocgenerator/pydoc.py
--rw-rw-rw-   0        0        0       78 2024-04-17 04:34:17.000000 pydcogenerator-0.0.5/src/pydocgenerator/test1.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:51:18.265339 pydcogenerator-0.1.0/
+-rw-rw-rw-   0        0        0     1088 2024-03-20 14:29:16.000000 pydcogenerator-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2116 2024-04-17 10:51:18.260013 pydcogenerator-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1495 2024-04-17 07:07:41.000000 pydcogenerator-0.1.0/README.md
+-rw-rw-rw-   0        0        0      736 2024-04-17 10:50:56.000000 pydcogenerator-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 10:51:18.266341 pydcogenerator-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 10:51:18.200423 pydcogenerator-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 10:51:18.258016 pydcogenerator-0.1.0/src/pydcogenerator.egg-info/
+-rw-rw-rw-   0        0        0     2116 2024-04-17 10:51:18.000000 pydcogenerator-0.1.0/src/pydcogenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-04-17 10:51:18.000000 pydcogenerator-0.1.0/src/pydcogenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 10:51:18.000000 pydcogenerator-0.1.0/src/pydcogenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-17 10:51:18.000000 pydcogenerator-0.1.0/src/pydcogenerator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 10:51:18.256012 pydcogenerator-0.1.0/src/pydocgenerator/
+-rw-rw-rw-   0        0        0      368 2024-04-17 07:07:41.000000 pydcogenerator-0.1.0/src/pydocgenerator/__init__.py
+-rw-rw-rw-   0        0        0     2790 2024-04-17 10:50:24.000000 pydcogenerator-0.1.0/src/pydocgenerator/pydoc.py
```

### Comparing `pydcogenerator-0.0.5/LICENSE` & `pydcogenerator-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydcogenerator-0.0.5/PKG-INFO` & `pydcogenerator-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 Metadata-Version: 2.1
 Name: pydcogenerator
-Version: 0.0.5
+Version: 0.1.0
 Summary: A library for generating docstring for python programms.
 Author-email: Rijin <rijinraj856@example.com>, Amal <amal76735@example.com>, Yadhu <yadhu2309856@example.com>
-Project-URL: Homepage, https://github.com/RijinRaju/DocGen-AI
-Project-URL: Issues, https://github.com/RijinRaju/DocGen-AI/issues
+Project-URL: Homepage, https://github.com/RijinRaju/PyDocGenerator
+Project-URL: Issues, https://github.com/RijinRaju/PyDocGenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# DocGen-AI
-DocGen-AI is a Python library that automatically generates docstrings for Python functions. It takes a Python file as input, generates docstrings for each function in the file, and outputs a new Python file with the generated docstrings.
+# PyDocGenerator
+PyDocGenerator is a Python library that automatically generates docstrings for Python functions. It takes a Python file as input, generates docstrings for each function in the file, and outputs a new Python file with the generated docstrings.
 # Features
  * Automatically generate docstrings for Python functions
  * Easy to use: just pass the file name to the DocGen instance and call the write_to_file() method
 # Installation
-You can install DocGen-AI by cloning the repository or using pip:
-      git clone [<repository-url>](https://github.com/RijinRaju/DocGen-AI/) 
-      cd DocGen-AI/src
-      pip install DocGen-AI
+You can install PyDocGenerator by cloning the repository or using pip:
+      git clone [<repository-url>](https://github.com/RijinRaju/PyDocGenerator/) 
+
+## Dependencies
+- **transformers**: A library for natural language processing using pre-trained models.
+    pip install transformers
+
+- **torch**: The PyTorch library for deep learning and neural networks.
+    pip install torch
+
+- **astunparse**: A Python library for parsing and un-parsing abstract syntax trees (ASTs).
+    pip install astunparse
+  
 
 
 # Usage
 Here’s a simple example of how to use DocGen-AI:
 ```python 
-  from docgen_ai import DocGen
-  
-  doc_gen = DocGen('./test.py')
-  doc_gen.write_to_file()
+  from pydocgenerator.pydoc import PyDOC
+
+  py_doc = PyDOC('./filename.py')
+  py_doc.write_to_file()
 ```
-In this example, DocGen is instantiated with the path to a Python file ('./test.py'). The write_to_file() method is then called to generate docstrings for each function in the file and output a new Python file with the generated docstrings.
+In this example, DocGen is instantiated with the path to a Python file ('./filename.py'). The write_to_file() method is then called to generate docstrings for each function in the file and output a new Python file with docstrings attached.
 
 # License
 DocGen-AI is licensed under the MIT License. See the LICENSE file for more information.
```

### Comparing `pydcogenerator-0.0.5/README.md` & `pydcogenerator-0.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,33 @@
-# DocGen-AI
-DocGen-AI is a Python library that automatically generates docstrings for Python functions. It takes a Python file as input, generates docstrings for each function in the file, and outputs a new Python file with the generated docstrings.
+# PyDocGenerator
+PyDocGenerator is a Python library that automatically generates docstrings for Python functions. It takes a Python file as input, generates docstrings for each function in the file, and outputs a new Python file with the generated docstrings.
 # Features
  * Automatically generate docstrings for Python functions
  * Easy to use: just pass the file name to the DocGen instance and call the write_to_file() method
 # Installation
-You can install DocGen-AI by cloning the repository or using pip:
-      git clone [<repository-url>](https://github.com/RijinRaju/DocGen-AI/) 
-      cd DocGen-AI/src
-      pip install DocGen-AI
+You can install PyDocGenerator by cloning the repository or using pip:
+      git clone [<repository-url>](https://github.com/RijinRaju/PyDocGenerator/) 
+
+## Dependencies
+- **transformers**: A library for natural language processing using pre-trained models.
+    pip install transformers
+
+- **torch**: The PyTorch library for deep learning and neural networks.
+    pip install torch
+
+- **astunparse**: A Python library for parsing and un-parsing abstract syntax trees (ASTs).
+    pip install astunparse
+  
 
 
 # Usage
 Here’s a simple example of how to use DocGen-AI:
 ```python 
-  from docgen_ai import DocGen
-  
-  doc_gen = DocGen('./test.py')
-  doc_gen.write_to_file()
+  from pydocgenerator.pydoc import PyDOC
+
+  py_doc = PyDOC('./filename.py')
+  py_doc.write_to_file()
 ```
-In this example, DocGen is instantiated with the path to a Python file ('./test.py'). The write_to_file() method is then called to generate docstrings for each function in the file and output a new Python file with the generated docstrings.
+In this example, DocGen is instantiated with the path to a Python file ('./filename.py'). The write_to_file() method is then called to generate docstrings for each function in the file and output a new Python file with docstrings attached.
 
 # License
 DocGen-AI is licensed under the MIT License. See the LICENSE file for more information.
```

### Comparing `pydcogenerator-0.0.5/pyproject.toml` & `pydcogenerator-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pydcogenerator"
-version = "0.0.5"
+version = "0.1.0"
 authors = [
   { name="Rijin", email="rijinraj856@example.com" },
   { name="Amal", email="amal76735@example.com" },
   { name="Yadhu", email="yadhu2309856@example.com" }
 ]
 description = "A library for generating docstring for python programms."
 readme = "README.md"
@@ -16,9 +16,9 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/RijinRaju/DocGen-AI"
-Issues = "https://github.com/RijinRaju/DocGen-AI/issues"
+Homepage = "https://github.com/RijinRaju/PyDocGenerator"
+Issues = "https://github.com/RijinRaju/PyDocGenerator/issues"
```

### Comparing `pydcogenerator-0.0.5/src/pydcogenerator.egg-info/PKG-INFO` & `pydcogenerator-0.1.0/src/pydcogenerator.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 Metadata-Version: 2.1
 Name: pydcogenerator
-Version: 0.0.5
+Version: 0.1.0
 Summary: A library for generating docstring for python programms.
 Author-email: Rijin <rijinraj856@example.com>, Amal <amal76735@example.com>, Yadhu <yadhu2309856@example.com>
-Project-URL: Homepage, https://github.com/RijinRaju/DocGen-AI
-Project-URL: Issues, https://github.com/RijinRaju/DocGen-AI/issues
+Project-URL: Homepage, https://github.com/RijinRaju/PyDocGenerator
+Project-URL: Issues, https://github.com/RijinRaju/PyDocGenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# DocGen-AI
-DocGen-AI is a Python library that automatically generates docstrings for Python functions. It takes a Python file as input, generates docstrings for each function in the file, and outputs a new Python file with the generated docstrings.
+# PyDocGenerator
+PyDocGenerator is a Python library that automatically generates docstrings for Python functions. It takes a Python file as input, generates docstrings for each function in the file, and outputs a new Python file with the generated docstrings.
 # Features
  * Automatically generate docstrings for Python functions
  * Easy to use: just pass the file name to the DocGen instance and call the write_to_file() method
 # Installation
-You can install DocGen-AI by cloning the repository or using pip:
-      git clone [<repository-url>](https://github.com/RijinRaju/DocGen-AI/) 
-      cd DocGen-AI/src
-      pip install DocGen-AI
+You can install PyDocGenerator by cloning the repository or using pip:
+      git clone [<repository-url>](https://github.com/RijinRaju/PyDocGenerator/) 
+
+## Dependencies
+- **transformers**: A library for natural language processing using pre-trained models.
+    pip install transformers
+
+- **torch**: The PyTorch library for deep learning and neural networks.
+    pip install torch
+
+- **astunparse**: A Python library for parsing and un-parsing abstract syntax trees (ASTs).
+    pip install astunparse
+  
 
 
 # Usage
 Here’s a simple example of how to use DocGen-AI:
 ```python 
-  from docgen_ai import DocGen
-  
-  doc_gen = DocGen('./test.py')
-  doc_gen.write_to_file()
+  from pydocgenerator.pydoc import PyDOC
+
+  py_doc = PyDOC('./filename.py')
+  py_doc.write_to_file()
 ```
-In this example, DocGen is instantiated with the path to a Python file ('./test.py'). The write_to_file() method is then called to generate docstrings for each function in the file and output a new Python file with the generated docstrings.
+In this example, DocGen is instantiated with the path to a Python file ('./filename.py'). The write_to_file() method is then called to generate docstrings for each function in the file and output a new Python file with docstrings attached.
 
 # License
 DocGen-AI is licensed under the MIT License. See the LICENSE file for more information.
```

### Comparing `pydcogenerator-0.0.5/src/pydocgenerator/pydoc.py` & `pydcogenerator-0.1.0/src/pydocgenerator/pydoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,46 +37,39 @@
             return docstring_match.group(1).strip()
         else:
             return None
 
     def process_python_file(self):
         # Parse the source code
         module = ast.parse(self.source_code)
-
         # Find all function definitions
         functions = [node for node in module.body if isinstance(
             node, ast.FunctionDef)]
-
+        
         # Generate docstrings for each function
         for function in functions:
            # Convert the function AST back into source code
             function_source = astunparse.unparse(function)
-
-
             # Generate the docstring
             docstring = self.generate_docstring(
                 function_source)  # pass the function object
-
             # Insert the docstring into the function AST
             function.body.insert(0, ast.Expr(value=ast.Str(s=docstring)))
-
             # Unparse the modified AST back into source code
             self.source_code = astunparse.unparse(module)
 
         return self.source_code
 
 
     @staticmethod
     def insert_docstring(function_source, docstring):
         # Split the function source code into lines
         lines = function_source.split('\n')
-
         # Insert the docstring after the function definition
         lines.insert(1, f'    """{docstring}"""')
-
         # Join the lines back together
         return '\n'.join(lines)
 
 
     def write_to_file(self):
         with open(self.input_file_path, 'w') as file:
             file.write(self.process_python_file())
```

