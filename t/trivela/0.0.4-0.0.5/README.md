# Comparing `tmp/trivela-0.0.4.tar.gz` & `tmp/trivela-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trivela-0.0.4.tar", last modified: Wed Apr  3 16:00:18 2024, max compression
+gzip compressed data, was "trivela-0.0.5.tar", last modified: Wed Apr 17 08:56:09 2024, max compression
```

## Comparing `trivela-0.0.4.tar` & `trivela-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-03 16:00:17.994573 trivela-0.0.4/
--rw-r--r--   0 sanjayarai  (1000) sanjayarai  (1000)     3999 2024-04-03 16:00:17.994573 trivela-0.0.4/PKG-INFO
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     3502 2024-04-03 15:59:30.000000 trivela-0.0.4/README.md
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)       38 2024-04-03 16:00:17.994573 trivela-0.0.4/setup.cfg
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     1657 2024-04-03 15:59:41.000000 trivela-0.0.4/setup.py
-drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-03 16:00:17.994573 trivela-0.0.4/trivela/
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        1 2024-03-27 16:31:23.000000 trivela-0.0.4/trivela/__init__.py
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     5301 2024-04-03 14:39:41.000000 trivela-0.0.4/trivela/api.py
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      673 2024-03-27 01:46:38.000000 trivela-0.0.4/trivela/middleware.py
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      953 2024-01-03 14:20:30.000000 trivela-0.0.4/trivela/response.py
-drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-03 16:00:17.994573 trivela-0.0.4/trivela.egg-info/
--rw-r--r--   0 sanjayarai  (1000) sanjayarai  (1000)     3999 2024-04-03 16:00:17.000000 trivela-0.0.4/trivela.egg-info/PKG-INFO
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      249 2024-04-03 16:00:17.000000 trivela-0.0.4/trivela.egg-info/SOURCES.txt
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        1 2024-04-03 16:00:17.000000 trivela-0.0.4/trivela.egg-info/dependency_links.txt
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      104 2024-04-03 16:00:17.000000 trivela-0.0.4/trivela.egg-info/requires.txt
--rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        8 2024-04-03 16:00:17.000000 trivela-0.0.4/trivela.egg-info/top_level.txt
+drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-17 08:56:09.472007 trivela-0.0.5/
+-rw-r--r--   0 sanjayarai  (1000) sanjayarai  (1000)     5176 2024-04-17 08:56:09.472007 trivela-0.0.5/PKG-INFO
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     4679 2024-04-17 08:55:42.000000 trivela-0.0.5/README.md
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)       38 2024-04-17 08:56:09.472007 trivela-0.0.5/setup.cfg
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     1657 2024-04-17 08:30:28.000000 trivela-0.0.5/setup.py
+drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-17 08:56:09.468006 trivela-0.0.5/trivela/
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        1 2024-03-27 16:31:23.000000 trivela-0.0.5/trivela/__init__.py
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     5301 2024-04-03 14:39:41.000000 trivela-0.0.5/trivela/api.py
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      673 2024-03-27 01:46:38.000000 trivela-0.0.5/trivela/middleware.py
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)     6424 2024-04-17 08:16:32.000000 trivela-0.0.5/trivela/orm.py
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      953 2024-01-03 14:20:30.000000 trivela-0.0.5/trivela/response.py
+drwxrwxr-x   0 sanjayarai  (1000) sanjayarai  (1000)        0 2024-04-17 08:56:09.472007 trivela-0.0.5/trivela.egg-info/
+-rw-r--r--   0 sanjayarai  (1000) sanjayarai  (1000)     5176 2024-04-17 08:56:09.000000 trivela-0.0.5/trivela.egg-info/PKG-INFO
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      264 2024-04-17 08:56:09.000000 trivela-0.0.5/trivela.egg-info/SOURCES.txt
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        1 2024-04-17 08:56:09.000000 trivela-0.0.5/trivela.egg-info/dependency_links.txt
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)      104 2024-04-17 08:56:09.000000 trivela-0.0.5/trivela.egg-info/requires.txt
+-rw-rw-r--   0 sanjayarai  (1000) sanjayarai  (1000)        8 2024-04-17 08:56:09.000000 trivela-0.0.5/trivela.egg-info/top_level.txt
```

### Comparing `trivela-0.0.4/PKG-INFO` & `trivela-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trivela
-Version: 0.0.4
+Version: 0.0.5
 Summary: Trivela Python Web Framework build for learning purpose.
 Author: Sanjaya Rai
 Author-email: rainamite@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12.0
 Description-Content-Type: text/markdown
@@ -159,7 +159,77 @@
 
     def process_response(self, req, res):
         print("After dispatch", req.url)
 
 
 app.add_middleware(SimpleCustomMiddleware)
 ```
+### ORM
+You can use `Trivela ORM` to interact with database and perform some basic operations mentioned below:
+
+Connect to the database:
+```python
+from trivela.orm import Database
+db = Database("./demo.db")
+```
+
+Defining tables:
+```python
+from trivela.orm import Table, Column, ForeignKey
+
+class Author(Table):
+    name = Column(str)
+    age = Column(int)
+
+class Book(Table):
+    title = Column(str)
+    published = Column(bool)
+    author = ForeignKey(Author)
+```
+
+Creating tables:
+```python
+db.create(Author)
+db.create(Book)
+```
+
+Creating an instance and inserting a row in database:
+```python
+david = Author(name='David', age=23)
+db.save(david)
+```
+
+Fetching all rows from database:
+```python
+authors = db.all(Author)
+```
+
+Fetching a specific row by `Id`:
+```python
+author = db.get(Author, 100)
+
+```
+
+Saving an object with a foreign key reference:
+```python
+book = Book(title="Hello world", published=True, author=david)
+db.save(book)
+
+```
+
+Fetching an object with a foreign key:
+```python
+print(db.get(Book, 100).author.name)
+```
+
+Updating an object:
+```python
+book.title = "World Hello"
+db.update(book)
+```
+
+Deleting an object:
+```python
+db.delete(Book, id=book.id)
+```
+
+
```

### Comparing `trivela-0.0.4/README.md` & `trivela-0.0.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -141,7 +141,77 @@
 
     def process_response(self, req, res):
         print("After dispatch", req.url)
 
 
 app.add_middleware(SimpleCustomMiddleware)
 ```
+### ORM
+You can use `Trivela ORM` to interact with database and perform some basic operations mentioned below:
+
+Connect to the database:
+```python
+from trivela.orm import Database
+db = Database("./demo.db")
+```
+
+Defining tables:
+```python
+from trivela.orm import Table, Column, ForeignKey
+
+class Author(Table):
+    name = Column(str)
+    age = Column(int)
+
+class Book(Table):
+    title = Column(str)
+    published = Column(bool)
+    author = ForeignKey(Author)
+```
+
+Creating tables:
+```python
+db.create(Author)
+db.create(Book)
+```
+
+Creating an instance and inserting a row in database:
+```python
+david = Author(name='David', age=23)
+db.save(david)
+```
+
+Fetching all rows from database:
+```python
+authors = db.all(Author)
+```
+
+Fetching a specific row by `Id`:
+```python
+author = db.get(Author, 100)
+
+```
+
+Saving an object with a foreign key reference:
+```python
+book = Book(title="Hello world", published=True, author=david)
+db.save(book)
+
+```
+
+Fetching an object with a foreign key:
+```python
+print(db.get(Book, 100).author.name)
+```
+
+Updating an object:
+```python
+book.title = "World Hello"
+db.update(book)
+```
+
+Deleting an object:
+```python
+db.delete(Book, id=book.id)
+```
+
+
```

### Comparing `trivela-0.0.4/setup.py` & `trivela-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # package meta-data
 NAME = "trivela"
 DESCRIPTION = "Trivela Python Web Framework build for learning purpose."
 EMAIL = "rainamite@gmail.com"
 AUTHOR = "Sanjaya Rai"
 REQUIRES_PYTHON = ">=3.12.0"
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 
 # which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja==3.1.2",
     "parse==1.20.0",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

### Comparing `trivela-0.0.4/trivela/api.py` & `trivela-0.0.5/trivela/api.py`

 * *Files identical despite different names*

### Comparing `trivela-0.0.4/trivela/middleware.py` & `trivela-0.0.5/trivela/middleware.py`

 * *Files identical despite different names*

### Comparing `trivela-0.0.4/trivela/response.py` & `trivela-0.0.5/trivela/response.py`

 * *Files identical despite different names*

### Comparing `trivela-0.0.4/trivela.egg-info/PKG-INFO` & `trivela-0.0.5/trivela.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trivela
-Version: 0.0.4
+Version: 0.0.5
 Summary: Trivela Python Web Framework build for learning purpose.
 Author: Sanjaya Rai
 Author-email: rainamite@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12.0
 Description-Content-Type: text/markdown
@@ -159,7 +159,77 @@
 
     def process_response(self, req, res):
         print("After dispatch", req.url)
 
 
 app.add_middleware(SimpleCustomMiddleware)
 ```
+### ORM
+You can use `Trivela ORM` to interact with database and perform some basic operations mentioned below:
+
+Connect to the database:
+```python
+from trivela.orm import Database
+db = Database("./demo.db")
+```
+
+Defining tables:
+```python
+from trivela.orm import Table, Column, ForeignKey
+
+class Author(Table):
+    name = Column(str)
+    age = Column(int)
+
+class Book(Table):
+    title = Column(str)
+    published = Column(bool)
+    author = ForeignKey(Author)
+```
+
+Creating tables:
+```python
+db.create(Author)
+db.create(Book)
+```
+
+Creating an instance and inserting a row in database:
+```python
+david = Author(name='David', age=23)
+db.save(david)
+```
+
+Fetching all rows from database:
+```python
+authors = db.all(Author)
+```
+
+Fetching a specific row by `Id`:
+```python
+author = db.get(Author, 100)
+
+```
+
+Saving an object with a foreign key reference:
+```python
+book = Book(title="Hello world", published=True, author=david)
+db.save(book)
+
+```
+
+Fetching an object with a foreign key:
+```python
+print(db.get(Book, 100).author.name)
+```
+
+Updating an object:
+```python
+book.title = "World Hello"
+db.update(book)
+```
+
+Deleting an object:
+```python
+db.delete(Book, id=book.id)
+```
+
+
```

