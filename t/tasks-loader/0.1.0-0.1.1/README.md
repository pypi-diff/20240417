# Comparing `tmp/tasks_loader-0.1.0.tar.gz` & `tmp/tasks_loader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tasks_loader-0.1.0.tar", last modified: Sat Apr  6 17:50:08 2024, max compression
+gzip compressed data, was "tasks_loader-0.1.1.tar", last modified: Tue Apr 16 22:31:54 2024, max compression
```

## Comparing `tasks_loader-0.1.0.tar` & `tasks_loader-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-04-06 17:50:08.204076 tasks_loader-0.1.0/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)    10763 2024-04-06 17:50:08.203387 tasks_loader-0.1.0/PKG-INFO
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     9953 2024-04-06 17:49:48.000000 tasks_loader-0.1.0/README.md
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       38 2024-04-06 17:50:08.204199 tasks_loader-0.1.0/setup.cfg
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1014 2024-04-06 17:33:57.000000 tasks_loader-0.1.0/setup.py
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-04-06 17:50:08.199880 tasks_loader-0.1.0/tasks_loader/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       29 2024-04-06 17:42:33.000000 tasks_loader-0.1.0/tasks_loader/__init__.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     7111 2024-04-06 17:42:10.000000 tasks_loader-0.1.0/tasks_loader/main.py
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-04-06 17:50:08.202441 tasks_loader-0.1.0/tasks_loader.egg-info/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)    10763 2024-04-06 17:50:08.000000 tasks_loader-0.1.0/tasks_loader.egg-info/PKG-INFO
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      208 2024-04-06 17:50:08.000000 tasks_loader-0.1.0/tasks_loader.egg-info/SOURCES.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)        1 2024-04-06 17:50:08.000000 tasks_loader-0.1.0/tasks_loader.egg-info/dependency_links.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       13 2024-04-06 17:50:08.000000 tasks_loader-0.1.0/tasks_loader.egg-info/top_level.txt
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-04-16 22:31:54.858677 tasks_loader-0.1.1/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)    13533 2024-04-16 22:31:54.857531 tasks_loader-0.1.1/PKG-INFO
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)    12723 2024-04-16 22:22:25.000000 tasks_loader-0.1.1/README.md
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       38 2024-04-16 22:31:54.858859 tasks_loader-0.1.1/setup.cfg
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1014 2024-04-16 22:22:38.000000 tasks_loader-0.1.1/setup.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-04-16 22:31:54.840050 tasks_loader-0.1.1/tasks_loader/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       58 2024-04-16 22:14:15.000000 tasks_loader-0.1.1/tasks_loader/__init__.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     6648 2024-04-16 22:12:40.000000 tasks_loader-0.1.1/tasks_loader/main.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     2623 2024-04-16 22:12:21.000000 tasks_loader-0.1.1/tasks_loader/models.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-04-16 22:31:54.845459 tasks_loader-0.1.1/tasks_loader.egg-info/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)    13533 2024-04-16 22:30:26.000000 tasks_loader-0.1.1/tasks_loader.egg-info/PKG-INFO
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      231 2024-04-16 22:30:30.000000 tasks_loader-0.1.1/tasks_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)        1 2024-04-16 22:30:26.000000 tasks_loader-0.1.1/tasks_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       13 2024-04-16 22:30:26.000000 tasks_loader-0.1.1/tasks_loader.egg-info/top_level.txt
```

### Comparing `tasks_loader-0.1.0/PKG-INFO` & `tasks_loader-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tasks_loader
-Version: 0.1.0
+Version: 0.1.1
 Summary: A module for dynamically creating tasks from CSV files with extensive validation features.
 Home-page: https://github.com/glizzykingdreko/tasks-loader
 Author: GlizzyKingDreko
 Author-email: glizzykingdreko@protonmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -32,15 +32,18 @@
   - [Installation](#installation)
   - [Key Features](#key-features)
   - [Task Format Dictionary](#task-format-dictionary)
   - [Examples](#examples)
     - [Example 1: Basic Task Loading](#example-1-basic-task-loading)
     - [Example 2: Advanced Validation with Regex and Lambda](#example-2-advanced-validation-with-regex-and-lambda)
     - [Example 3: Post-processing Data](#example-3-post-processing-data)
-      - [Example 4: Ticket / Sneakers Bot-like Validation](#example-4-ticket--sneakers-bot-like-validation)
+    - [Example 4: Ticket / Sneakers Bot-like Validation](#example-4-ticket--sneakers-bot-like-validation)
+    - [Example 2: Advanced Validation with Regex and Lambda](#example-2-advanced-validation-with-regex-and-lambda-1)
+    - [Example 5: Using Pre-Made Regex Checks with the Patterns Class](#example-5-using-pre-made-regex-checks-with-the-patterns-class)
+    - [Example 6: File Check and Creation Handling](#example-6-file-check-and-creation-handling)
   - [Stay in touch with me](#stay-in-touch-with-me)
 
 ## Installation
 
 To install `tasks-loader`, run the following command:
 ```bash
 pip install tasks-loader
@@ -177,15 +180,15 @@
 
 tasks = Tasks(input_file='post_processing.csv', task_format=task_format)
 
 for task in tasks:
     print(task)
 ```
 
-#### Example 4: Ticket / Sneakers Bot-like Validation
+### Example 4: Ticket / Sneakers Bot-like Validation
 
 This example demonstrates a setup tailored for automated tasks commonly used in ticket purchasing or sneaker bot scenarios. The configuration ensures all necessary information for a purchase is validated against specific criteria before proceeding with a task.
 
 **CSV (`ticket_sneakers_bot.csv`):**
 
 ```csv
 Name,Surname,Mail,URL,Min Price,Max Price,Error Delay, Monitor Delay,Credit Card Number,Credit Card Month,Credit Card Year,Credit Card CVV
@@ -257,14 +260,132 @@
 - **Credit Card Number**: Must be a 16-digit string.
 - **Credit Card Month**: Validates with a regex pattern that the month is in MM format, allowing only values from 01 to 12.
 - **Credit Card Year**: Must be a 4-digit year in YYYY format.
 - **Credit Card CVV**: A 3-digit security code validated with a regex pattern.
 
 This setup is an example of an automated module that initiates tasks based on the validated entries from a CSV file, ensuring each task has all the necessary and correctly formatted information before proceeding. This kind of validation is crucial in scenarios where precise and validated data is essential for the success of automated tasks, such as in ticket purchasing or sneaker bot operations.
 
+
+### Example 2: Advanced Validation with Regex and Lambda
+
+**CSV (`advanced_validation.csv`):**
+
+```csv
+Name,Email,Role
+John Doe,johndoe@example.com,admin
+Jane Smith,janesmith@bademail,visitor
+```
+
+**Task Format:**
+
+```python
+task_format = {
+    "name": {"type": str, "required": True},
+    "email": {
+        "type": str,
+        "required": True,
+        "validation": r"^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$"
+    },
+    "role": {
+        "type": str,
+        "required": True,
+        "choices": ["admin", "user", "guest"],
+        "validation": lambda x: x in ["admin", "user", "guest"]
+    },
+}
+```
+
+**Python Code:**
+
+```python
+from tasks_loader import Tasks
+
+tasks = Tasks(input_file='advanced_validation.csv', task_format=task_format)
+
+for task in tasks:
+    print(task)
+```
+
+### Example 5: Using Pre-Made Regex Checks with the Patterns Class
+
+**CSV (`regex_validation.csv`):**
+
+```csv
+Name,Email,Phone,Month
+John Doe,johndoe@example.com,+12345678901,January
+Jane Smith,janesmith@bademail,+12345,Smarch
+```
+
+**Task Format:**
+
+```python
+task_format = {
+    "name": {"type": str, "required": True},
+    "email": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.MAIL
+    },
+    "phone": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.PHONE
+    },
+    "month": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.MONTH
+    }
+}
+```
+
+**Python Code:**
+
+```python
+from tasks_loader import Patterns
+
+task_format = {
+    "name": {"type": str, "required": True},
+    "email": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.MAIL
+    },
+    "phone": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.PHONE
+    },
+    "month": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.MONTH
+    }
+}
+```
+
+### Example 6: File Check and Creation Handling
+
+If the specified CSV file does not exist, ty can createa new one by calling the function `create_file` with the appropriate headers based on the `task_format` to ensure data consistency.
+
+**Python Code:**
+
+```python
+from tasks_loader import Tasks
+
+# Define the CSV file and format
+tasks = Tasks(input_file='new_tasks.csv', task_format=task_format)
+
+if tasks.create_file():
+    print("File created, please fill it and then restart the script")
+    exit(0)
+print("File aready created")
+```
+
+
 ## Stay in touch with me
 
 For any inquiries or further information, please reach out:
 
 - [GitHub](https://github.com/glizzykingdreko)
 - [Twitter](https://mobile.twitter.com/glizzykingdreko)
 - [Medium](https://medium.com/@glizzykingdreko)
```

### Comparing `tasks_loader-0.1.0/README.md` & `tasks_loader-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,18 @@
   - [Installation](#installation)
   - [Key Features](#key-features)
   - [Task Format Dictionary](#task-format-dictionary)
   - [Examples](#examples)
     - [Example 1: Basic Task Loading](#example-1-basic-task-loading)
     - [Example 2: Advanced Validation with Regex and Lambda](#example-2-advanced-validation-with-regex-and-lambda)
     - [Example 3: Post-processing Data](#example-3-post-processing-data)
-      - [Example 4: Ticket / Sneakers Bot-like Validation](#example-4-ticket--sneakers-bot-like-validation)
+    - [Example 4: Ticket / Sneakers Bot-like Validation](#example-4-ticket--sneakers-bot-like-validation)
+    - [Example 2: Advanced Validation with Regex and Lambda](#example-2-advanced-validation-with-regex-and-lambda-1)
+    - [Example 5: Using Pre-Made Regex Checks with the Patterns Class](#example-5-using-pre-made-regex-checks-with-the-patterns-class)
+    - [Example 6: File Check and Creation Handling](#example-6-file-check-and-creation-handling)
   - [Stay in touch with me](#stay-in-touch-with-me)
 
 ## Installation
 
 To install `tasks-loader`, run the following command:
 ```bash
 pip install tasks-loader
@@ -158,15 +161,15 @@
 
 tasks = Tasks(input_file='post_processing.csv', task_format=task_format)
 
 for task in tasks:
     print(task)
 ```
 
-#### Example 4: Ticket / Sneakers Bot-like Validation
+### Example 4: Ticket / Sneakers Bot-like Validation
 
 This example demonstrates a setup tailored for automated tasks commonly used in ticket purchasing or sneaker bot scenarios. The configuration ensures all necessary information for a purchase is validated against specific criteria before proceeding with a task.
 
 **CSV (`ticket_sneakers_bot.csv`):**
 
 ```csv
 Name,Surname,Mail,URL,Min Price,Max Price,Error Delay, Monitor Delay,Credit Card Number,Credit Card Month,Credit Card Year,Credit Card CVV
@@ -238,14 +241,132 @@
 - **Credit Card Number**: Must be a 16-digit string.
 - **Credit Card Month**: Validates with a regex pattern that the month is in MM format, allowing only values from 01 to 12.
 - **Credit Card Year**: Must be a 4-digit year in YYYY format.
 - **Credit Card CVV**: A 3-digit security code validated with a regex pattern.
 
 This setup is an example of an automated module that initiates tasks based on the validated entries from a CSV file, ensuring each task has all the necessary and correctly formatted information before proceeding. This kind of validation is crucial in scenarios where precise and validated data is essential for the success of automated tasks, such as in ticket purchasing or sneaker bot operations.
 
+
+### Example 2: Advanced Validation with Regex and Lambda
+
+**CSV (`advanced_validation.csv`):**
+
+```csv
+Name,Email,Role
+John Doe,johndoe@example.com,admin
+Jane Smith,janesmith@bademail,visitor
+```
+
+**Task Format:**
+
+```python
+task_format = {
+    "name": {"type": str, "required": True},
+    "email": {
+        "type": str,
+        "required": True,
+        "validation": r"^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$"
+    },
+    "role": {
+        "type": str,
+        "required": True,
+        "choices": ["admin", "user", "guest"],
+        "validation": lambda x: x in ["admin", "user", "guest"]
+    },
+}
+```
+
+**Python Code:**
+
+```python
+from tasks_loader import Tasks
+
+tasks = Tasks(input_file='advanced_validation.csv', task_format=task_format)
+
+for task in tasks:
+    print(task)
+```
+
+### Example 5: Using Pre-Made Regex Checks with the Patterns Class
+
+**CSV (`regex_validation.csv`):**
+
+```csv
+Name,Email,Phone,Month
+John Doe,johndoe@example.com,+12345678901,January
+Jane Smith,janesmith@bademail,+12345,Smarch
+```
+
+**Task Format:**
+
+```python
+task_format = {
+    "name": {"type": str, "required": True},
+    "email": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.MAIL
+    },
+    "phone": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.PHONE
+    },
+    "month": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.MONTH
+    }
+}
+```
+
+**Python Code:**
+
+```python
+from tasks_loader import Patterns
+
+task_format = {
+    "name": {"type": str, "required": True},
+    "email": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.MAIL
+    },
+    "phone": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.PHONE
+    },
+    "month": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.MONTH
+    }
+}
+```
+
+### Example 6: File Check and Creation Handling
+
+If the specified CSV file does not exist, ty can createa new one by calling the function `create_file` with the appropriate headers based on the `task_format` to ensure data consistency.
+
+**Python Code:**
+
+```python
+from tasks_loader import Tasks
+
+# Define the CSV file and format
+tasks = Tasks(input_file='new_tasks.csv', task_format=task_format)
+
+if tasks.create_file():
+    print("File created, please fill it and then restart the script")
+    exit(0)
+print("File aready created")
+```
+
+
 ## Stay in touch with me
 
 For any inquiries or further information, please reach out:
 
 - [GitHub](https://github.com/glizzykingdreko)
 - [Twitter](https://mobile.twitter.com/glizzykingdreko)
 - [Medium](https://medium.com/@glizzykingdreko)
```

### Comparing `tasks_loader-0.1.0/setup.py` & `tasks_loader-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tasks_loader',
-    version='0.1.0',
+    version='0.1.1',
     author='GlizzyKingDreko',
     author_email='glizzykingdreko@protonmail.com',
     description='A module for dynamically creating tasks from CSV files with extensive validation features.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/glizzykingdreko/tasks-loader',
     packages=find_packages(),
```

### Comparing `tasks_loader-0.1.0/tasks_loader/main.py` & `tasks_loader-0.1.1/tasks_loader/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,11 @@
 import csv, re
+from os import path
 
-class Task:
-    """
-    Represents a single task, dynamically creating attributes based on input keyword arguments.
-    
-    Attributes:
-        id (str): A unique identifier for the task, formatted as a zero-padded string.
-    
-    Parameters:
-        **kwargs: Arbitrary keyword arguments representing task attributes and their values.
-    """
-    _id_counter = 1  # Class variable to keep track of the next id
-
-    def __init__(self, **kwargs):
-        self.id = str(Task._id_counter).zfill(3)  # Format the id as '001', '002',...
-        Task._id_counter += 1  # Increment for the next task
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-
-    def __str__(self):
-        """Return the task id as a string representation of the Task object."""
-        return self.id
-
-    def to_dict(self):
-        """
-        Convert the Task instance into a dictionary.
-        
-        Returns:
-            dict: A dictionary representation of the Task instance, including its id and all dynamically added attributes.
-        """
-        return {**self.__dict__}
+from .models import Task
 
 class Tasks:
     """
     Manages a collection of Task objects created from a CSV file based on a specified task format.
     
     Attributes:
         input_file (str): Path to the input CSV file containing task data.
@@ -82,14 +54,32 @@
         Provide a string representation indicating the number of valid tasks loaded.
         
         Returns:
             str: A message stating the number of loaded tasks.
         """
         return f"Loaded {len(self.tasks)} valid tasks."
 
+    def create_file(self) -> bool:
+        """
+        Create a default CSV file with headers based on the task format.
+
+        Returns:
+            bool: True if the file was successfully created, False otherwise.
+        """
+        headers = self.task_format.keys()
+        
+        # Check if file exists
+        if path.exists(self.input_file):
+            return False
+
+        with open(self.input_file, mode='w', newline='', encoding='utf-8') as file:
+            writer = csv.DictWriter(file, fieldnames=headers)
+            writer.writeheader()
+        return True
+
     def to_dict(self):
         """
         Convert all loaded tasks into a list of dictionaries.
         
         Returns:
             list: A list of dictionaries, each representing a Task instance.
         """
```

### Comparing `tasks_loader-0.1.0/tasks_loader.egg-info/PKG-INFO` & `tasks_loader-0.1.1/tasks_loader.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tasks_loader
-Version: 0.1.0
+Version: 0.1.1
 Summary: A module for dynamically creating tasks from CSV files with extensive validation features.
 Home-page: https://github.com/glizzykingdreko/tasks-loader
 Author: GlizzyKingDreko
 Author-email: glizzykingdreko@protonmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -32,15 +32,18 @@
   - [Installation](#installation)
   - [Key Features](#key-features)
   - [Task Format Dictionary](#task-format-dictionary)
   - [Examples](#examples)
     - [Example 1: Basic Task Loading](#example-1-basic-task-loading)
     - [Example 2: Advanced Validation with Regex and Lambda](#example-2-advanced-validation-with-regex-and-lambda)
     - [Example 3: Post-processing Data](#example-3-post-processing-data)
-      - [Example 4: Ticket / Sneakers Bot-like Validation](#example-4-ticket--sneakers-bot-like-validation)
+    - [Example 4: Ticket / Sneakers Bot-like Validation](#example-4-ticket--sneakers-bot-like-validation)
+    - [Example 2: Advanced Validation with Regex and Lambda](#example-2-advanced-validation-with-regex-and-lambda-1)
+    - [Example 5: Using Pre-Made Regex Checks with the Patterns Class](#example-5-using-pre-made-regex-checks-with-the-patterns-class)
+    - [Example 6: File Check and Creation Handling](#example-6-file-check-and-creation-handling)
   - [Stay in touch with me](#stay-in-touch-with-me)
 
 ## Installation
 
 To install `tasks-loader`, run the following command:
 ```bash
 pip install tasks-loader
@@ -177,15 +180,15 @@
 
 tasks = Tasks(input_file='post_processing.csv', task_format=task_format)
 
 for task in tasks:
     print(task)
 ```
 
-#### Example 4: Ticket / Sneakers Bot-like Validation
+### Example 4: Ticket / Sneakers Bot-like Validation
 
 This example demonstrates a setup tailored for automated tasks commonly used in ticket purchasing or sneaker bot scenarios. The configuration ensures all necessary information for a purchase is validated against specific criteria before proceeding with a task.
 
 **CSV (`ticket_sneakers_bot.csv`):**
 
 ```csv
 Name,Surname,Mail,URL,Min Price,Max Price,Error Delay, Monitor Delay,Credit Card Number,Credit Card Month,Credit Card Year,Credit Card CVV
@@ -257,14 +260,132 @@
 - **Credit Card Number**: Must be a 16-digit string.
 - **Credit Card Month**: Validates with a regex pattern that the month is in MM format, allowing only values from 01 to 12.
 - **Credit Card Year**: Must be a 4-digit year in YYYY format.
 - **Credit Card CVV**: A 3-digit security code validated with a regex pattern.
 
 This setup is an example of an automated module that initiates tasks based on the validated entries from a CSV file, ensuring each task has all the necessary and correctly formatted information before proceeding. This kind of validation is crucial in scenarios where precise and validated data is essential for the success of automated tasks, such as in ticket purchasing or sneaker bot operations.
 
+
+### Example 2: Advanced Validation with Regex and Lambda
+
+**CSV (`advanced_validation.csv`):**
+
+```csv
+Name,Email,Role
+John Doe,johndoe@example.com,admin
+Jane Smith,janesmith@bademail,visitor
+```
+
+**Task Format:**
+
+```python
+task_format = {
+    "name": {"type": str, "required": True},
+    "email": {
+        "type": str,
+        "required": True,
+        "validation": r"^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$"
+    },
+    "role": {
+        "type": str,
+        "required": True,
+        "choices": ["admin", "user", "guest"],
+        "validation": lambda x: x in ["admin", "user", "guest"]
+    },
+}
+```
+
+**Python Code:**
+
+```python
+from tasks_loader import Tasks
+
+tasks = Tasks(input_file='advanced_validation.csv', task_format=task_format)
+
+for task in tasks:
+    print(task)
+```
+
+### Example 5: Using Pre-Made Regex Checks with the Patterns Class
+
+**CSV (`regex_validation.csv`):**
+
+```csv
+Name,Email,Phone,Month
+John Doe,johndoe@example.com,+12345678901,January
+Jane Smith,janesmith@bademail,+12345,Smarch
+```
+
+**Task Format:**
+
+```python
+task_format = {
+    "name": {"type": str, "required": True},
+    "email": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.MAIL
+    },
+    "phone": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.PHONE
+    },
+    "month": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.MONTH
+    }
+}
+```
+
+**Python Code:**
+
+```python
+from tasks_loader import Patterns
+
+task_format = {
+    "name": {"type": str, "required": True},
+    "email": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.MAIL
+    },
+    "phone": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.PHONE
+    },
+    "month": {
+        "type": str,
+        "required": True,
+        "validation": Patterns.MONTH
+    }
+}
+```
+
+### Example 6: File Check and Creation Handling
+
+If the specified CSV file does not exist, ty can createa new one by calling the function `create_file` with the appropriate headers based on the `task_format` to ensure data consistency.
+
+**Python Code:**
+
+```python
+from tasks_loader import Tasks
+
+# Define the CSV file and format
+tasks = Tasks(input_file='new_tasks.csv', task_format=task_format)
+
+if tasks.create_file():
+    print("File created, please fill it and then restart the script")
+    exit(0)
+print("File aready created")
+```
+
+
 ## Stay in touch with me
 
 For any inquiries or further information, please reach out:
 
 - [GitHub](https://github.com/glizzykingdreko)
 - [Twitter](https://mobile.twitter.com/glizzykingdreko)
 - [Medium](https://medium.com/@glizzykingdreko)
```

