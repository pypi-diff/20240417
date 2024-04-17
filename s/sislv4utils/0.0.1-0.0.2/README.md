# Comparing `tmp/sislv4utils-0.0.1.tar.gz` & `tmp/sislv4utils-0.0.2.tar.gz`

## Comparing `sislv4utils-0.0.1.tar` & `sislv4utils-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sislv4utils-0.0.1/src/sislv4utils/__init__.py
--rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 sislv4utils-0.0.1/src/sislv4utils/config.py
--rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 sislv4utils-0.0.1/src/sislv4utils/elastic.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 sislv4utils-0.0.1/src/sislv4utils/message.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 sislv4utils-0.0.1/src/sislv4utils/objectstore.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 sislv4utils-0.0.1/src/sislv4utils/service.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sislv4utils-0.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sislv4utils-0.0.1/LICENSE
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 sislv4utils-0.0.1/README.md
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 sislv4utils-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 sislv4utils-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sislv4utils-0.0.2/src/sislv4utils/__init__.py
+-rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 sislv4utils-0.0.2/src/sislv4utils/config.py
+-rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 sislv4utils-0.0.2/src/sislv4utils/elastic.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 sislv4utils-0.0.2/src/sislv4utils/message.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 sislv4utils-0.0.2/src/sislv4utils/mqtt.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 sislv4utils-0.0.2/src/sislv4utils/objectstore.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 sislv4utils-0.0.2/src/sislv4utils/service.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sislv4utils-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sislv4utils-0.0.2/LICENSE
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 sislv4utils-0.0.2/README.md
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 sislv4utils-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sislv4utils-0.0.2/PKG-INFO
```

### Comparing `sislv4utils-0.0.1/src/sislv4utils/config.py` & `sislv4utils-0.0.2/src/sislv4utils/config.py`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.1/src/sislv4utils/elastic.py` & `sislv4utils-0.0.2/src/sislv4utils/elastic.py`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.1/src/sislv4utils/message.py` & `sislv4utils-0.0.2/src/sislv4utils/message.py`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.1/src/sislv4utils/objectstore.py` & `sislv4utils-0.0.2/src/sislv4utils/objectstore.py`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.1/src/sislv4utils/service.py` & `sislv4utils-0.0.2/src/sislv4utils/service.py`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.1/.gitignore` & `sislv4utils-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.1/LICENSE` & `sislv4utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.1/pyproject.toml` & `sislv4utils-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sislv4utils"
-version = "0.0.1"
+version = "0.0.2"
 
 authors = [
   { name="Bibhas Das", email="bibhas.das@somnetics.in" },
 ]
 
 description = "Seamless v4 utilities"
 
@@ -20,26 +20,28 @@
 
 install_requires = [
 	"pika>=1.3.2",
 	"falcon>=3.1.3",
 	"requests>=2.25.1",
 	"minio>=7.2.5",
 	"etcd3>=0.12.0",
-        "elasticsearch>=8.13.0",
-	"protobuf>=3.20.3"
+    "elasticsearch>=8.13.0",
+	"paho-mqtt>=2.0.0",
+	"protobuf==3.20.3"
 ]
 
 dependencies = [
 	"pika>=1.3.2",
 	"falcon>=3.1.3",
 	"requests>=2.25.1",
 	"minio>=7.2.5",
 	"etcd3>=0.12.0",
-        "elasticsearch>=8.13.0",
-	"protobuf>=3.20.3"
+    "elasticsearch>=8.13.0",
+	"paho-mqtt>=2.0.0",
+	"protobuf==3.20.3"
 ]
 
 test_requires = []
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

