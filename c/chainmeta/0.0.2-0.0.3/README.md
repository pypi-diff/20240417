# Comparing `tmp/chainmeta-0.0.2.tar.gz` & `tmp/chainmeta-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainmeta-0.0.2.tar", last modified: Fri Mar 29 00:18:46 2024, max compression
+gzip compressed data, was "chainmeta-0.0.3.tar", last modified: Wed Apr 17 20:55:56 2024, max compression
```

## Comparing `chainmeta-0.0.2.tar` & `chainmeta-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 zhanwu    (1000) zhanwu    (1000)        0 2024-03-29 00:18:46.304119 chainmeta-0.0.2/
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)    11357 2024-03-26 22:46:41.000000 chainmeta-0.0.2/LICENSE
--rw-r--r--   0 zhanwu    (1000) zhanwu    (1000)     1581 2024-03-29 00:18:46.304119 chainmeta-0.0.2/PKG-INFO
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)      988 2024-03-29 00:16:58.000000 chainmeta-0.0.2/README.md
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)      784 2024-03-29 00:01:54.000000 chainmeta-0.0.2/pyproject.toml
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)       38 2024-03-29 00:18:46.304119 chainmeta-0.0.2/setup.cfg
-drwxrwxr-x   0 zhanwu    (1000) zhanwu    (1000)        0 2024-03-29 00:18:46.300119 chainmeta-0.0.2/src/
-drwxrwxr-x   0 zhanwu    (1000) zhanwu    (1000)        0 2024-03-29 00:18:46.300119 chainmeta-0.0.2/src/chainmeta/
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)     4143 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/__init__.py
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)     2381 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/artifact.py
-drwxrwxr-x   0 zhanwu    (1000) zhanwu    (1000)        0 2024-03-29 00:18:46.300119 chainmeta-0.0.2/src/chainmeta/config/
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)     3510 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/config/__init__.py
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)    20519 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/config/categories.json
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)     2679 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/config/chains.json
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)    43396 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/config/entities.json
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)      404 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/config/sources.json
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)      979 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/constants.py
-drwxrwxr-x   0 zhanwu    (1000) zhanwu    (1000)        0 2024-03-29 00:18:46.300119 chainmeta-0.0.2/src/chainmeta/contrib/
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)     4529 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/contrib/chaintool.py
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)     1342 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/contrib/chaintool_schema.json
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)     1293 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/contrib/messari.py
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)      423 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/contrib/messari_schema.json
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)    15395 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/db.py
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)      664 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/logger.py
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)     1979 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/metadata.py
-drwxrwxr-x   0 zhanwu    (1000) zhanwu    (1000)        0 2024-03-29 00:18:46.304119 chainmeta-0.0.2/src/chainmeta/schema/
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)     2743 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/schema/__init__.py
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)     3320 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/schema/artifact_schema.json
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)     4124 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/schema/meta_schema.json
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)     2332 2024-03-28 22:07:27.000000 chainmeta-0.0.2/src/chainmeta/validator.py
-drwxrwxr-x   0 zhanwu    (1000) zhanwu    (1000)        0 2024-03-29 00:18:46.304119 chainmeta-0.0.2/src/chainmeta.egg-info/
--rw-r--r--   0 zhanwu    (1000) zhanwu    (1000)     1581 2024-03-29 00:18:46.000000 chainmeta-0.0.2/src/chainmeta.egg-info/PKG-INFO
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)      901 2024-03-29 00:18:46.000000 chainmeta-0.0.2/src/chainmeta.egg-info/SOURCES.txt
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)        1 2024-03-29 00:18:46.000000 chainmeta-0.0.2/src/chainmeta.egg-info/dependency_links.txt
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)       45 2024-03-29 00:18:46.000000 chainmeta-0.0.2/src/chainmeta.egg-info/requires.txt
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)       10 2024-03-29 00:18:46.000000 chainmeta-0.0.2/src/chainmeta.egg-info/top_level.txt
-drwxrwxr-x   0 zhanwu    (1000) zhanwu    (1000)        0 2024-03-29 00:18:46.304119 chainmeta-0.0.2/tests/
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)      715 2024-03-28 02:52:00.000000 chainmeta-0.0.2/tests/test_config.py
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)     1738 2024-03-28 21:44:37.000000 chainmeta-0.0.2/tests/test_translator.py
--rw-rw-r--   0 zhanwu    (1000) zhanwu    (1000)     1600 2024-03-27 21:12:50.000000 chainmeta-0.0.2/tests/test_validator.py
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.807409 chainmeta-0.0.3/
+-rw-r--r--   0 zhanwu     (501) staff       (20)    11357 2024-04-10 07:26:37.000000 chainmeta-0.0.3/LICENSE
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1581 2024-04-17 20:55:56.807243 chainmeta-0.0.3/PKG-INFO
+-rw-r--r--   0 zhanwu     (501) staff       (20)      988 2024-04-10 07:26:37.000000 chainmeta-0.0.3/README.md
+-rw-r--r--   0 zhanwu     (501) staff       (20)      784 2024-04-17 20:55:04.000000 chainmeta-0.0.3/pyproject.toml
+-rw-r--r--   0 zhanwu     (501) staff       (20)       38 2024-04-17 20:55:56.807447 chainmeta-0.0.3/setup.cfg
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.802389 chainmeta-0.0.3/src/
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.804174 chainmeta-0.0.3/src/chainmeta/
+-rw-r--r--   0 zhanwu     (501) staff       (20)     4925 2024-04-17 20:55:04.000000 chainmeta-0.0.3/src/chainmeta/__init__.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     2746 2024-04-17 20:02:26.000000 chainmeta-0.0.3/src/chainmeta/artifact.py
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.805557 chainmeta-0.0.3/src/chainmeta/config/
+-rw-r--r--   0 zhanwu     (501) staff       (20)     3510 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/config/__init__.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)    20519 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/config/categories.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)     2679 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/config/chains.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)    43396 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/config/entities.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)      404 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/config/sources.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)      979 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/constants.py
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.806090 chainmeta-0.0.3/src/chainmeta/contrib/
+-rw-r--r--   0 zhanwu     (501) staff       (20)     4529 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/contrib/chaintool.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1342 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/contrib/chaintool_schema.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1293 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/contrib/messari.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)      423 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/contrib/messari_schema.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)    15395 2024-04-17 20:11:06.000000 chainmeta-0.0.3/src/chainmeta/db.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)      664 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/logger.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1979 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/metadata.py
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.806476 chainmeta-0.0.3/src/chainmeta/schema/
+-rw-r--r--   0 zhanwu     (501) staff       (20)     2743 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/schema/__init__.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     3320 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/schema/artifact_schema.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)     4124 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/schema/meta_schema.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)     2332 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/validator.py
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.807064 chainmeta-0.0.3/src/chainmeta.egg-info/
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1581 2024-04-17 20:55:56.000000 chainmeta-0.0.3/src/chainmeta.egg-info/PKG-INFO
+-rw-r--r--   0 zhanwu     (501) staff       (20)      901 2024-04-17 20:55:56.000000 chainmeta-0.0.3/src/chainmeta.egg-info/SOURCES.txt
+-rw-r--r--   0 zhanwu     (501) staff       (20)        1 2024-04-17 20:55:56.000000 chainmeta-0.0.3/src/chainmeta.egg-info/dependency_links.txt
+-rw-r--r--   0 zhanwu     (501) staff       (20)       45 2024-04-17 20:55:56.000000 chainmeta-0.0.3/src/chainmeta.egg-info/requires.txt
+-rw-r--r--   0 zhanwu     (501) staff       (20)       10 2024-04-17 20:55:56.000000 chainmeta-0.0.3/src/chainmeta.egg-info/top_level.txt
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.806884 chainmeta-0.0.3/tests/
+-rw-r--r--   0 zhanwu     (501) staff       (20)      715 2024-04-10 07:26:37.000000 chainmeta-0.0.3/tests/test_config.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1738 2024-04-10 07:26:37.000000 chainmeta-0.0.3/tests/test_translator.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1600 2024-04-10 07:26:37.000000 chainmeta-0.0.3/tests/test_validator.py
```

### Comparing `chainmeta-0.0.2/LICENSE` & `chainmeta-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/PKG-INFO` & `chainmeta-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainmeta
-Version: 0.0.2
+Version: 0.0.3
 Summary: Onchain metadata exchange protocol
 Project-URL: Homepage, https://github.com/microscopexyz/chainmeta-core
 Project-URL: Issues, https://github.com/microscopexyz/chainmeta-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `chainmeta-0.0.2/README.md` & `chainmeta-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/pyproject.toml` & `chainmeta-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chainmeta"
-version = "0.0.2"
+version = "0.0.3"
 authors = []
 description = "Onchain metadata exchange protocol"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `chainmeta-0.0.2/src/chainmeta/__init__.py` & `chainmeta-0.0.3/src/chainmeta/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pathlib import Path
 from typing import Optional, Union
 
 from chainmeta.artifact import load as artifact_load
 from chainmeta.db import init_db
 from chainmeta.db import search_chainmeta as search_chainmeta
 from chainmeta.db import upload_chainmeta
+from chainmeta.schema import Schema, common_schema
 from chainmeta.schema import resolve as schema_resolve
 from chainmeta.validator import common_artifact_validator, common_metadata_validator
 
 
 def set_connection_string(connection_string: Optional[str] = None):
     if not connection_string:
         connection_string = os.environ.get("CHAINMETA_DB_CONN")
@@ -120,18 +121,40 @@
         s,
         ignore_unrecognized=ignore_unrecognized,
         artifact_base_path=artifact_base_path,
         **kw,
     )
 
 
+def load_artifact(
+    uri: str,
+    *,
+    schema: Schema = common_schema,
+    artifact_base_path: Union[str, Path, None] = None,
+    **kw,
+):
+    fileformat = uri.split(".")[-1].lower()
+    if artifact_base_path:
+        artifact_base_path = Path(artifact_base_path)
+    loaded_artifact = artifact_load(
+        uri, fileformat=fileformat, base_path=artifact_base_path
+    )
+    if not isinstance(loaded_artifact, list):
+        raise ValueError("artifact must be a list")
+    schema.validator.validate(loaded_artifact)
+    common_schema = [schema.translator.to_common_schema(a) for a in loaded_artifact]
+    common_artifact_validator.validate([c.__dict__ for c in common_schema])
+    return common_schema
+
+
 set_connection_string()
 
 __all__ = [
     "validate",
     "validates",
     "load",
     "loads",
+    "load_artifact",
     "upload_chainmeta",
     "search_chainmeta",
     "set_connection_string",
 ]
```

### Comparing `chainmeta-0.0.2/src/chainmeta/artifact.py` & `chainmeta-0.0.3/src/chainmeta/artifact.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,31 +9,40 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 from pathlib import Path
-from typing import Dict, Optional, no_type_check
+from typing import Dict, Optional, Union, no_type_check
+
+import boto3
 
 file_prefix = "file:///"
+s3_prefix = "s3://"
 
 
-def local_loader(uri: str, *, base_path: Optional[Path] = None) -> str:
+def local_loader(uri: str, *, base_path: Union[str, Path, None] = None) -> str:
     if not base_path:
         raise ValueError("missing artifact base path for local artifact file")
+
+    base_path = Path(base_path)
     relative_path = uri[len(file_prefix) :]
     resolved_path = base_path.joinpath(relative_path)
     with open(resolved_path) as f:
         return f.read()
 
 
 @no_type_check
 def s3_loader(uri: str, **kw) -> str:
-    pass
+    s3_client = boto3.client("s3")
+    bucket, key = uri[5:].split("/", 1)
+    response = s3_client.get_object(Bucket=bucket, Key=key)
+    content = response["Body"].read().decode("utf-8")
+    return content
 
 
 @no_type_check
 def http_loader(uri: str, **kw) -> str:
     pass
 
 
@@ -68,13 +77,19 @@
     "json": json_parser,
     "JSON": json_parser,
     "csv": csv_parser,
     "CSV": csv_parser,
 }
 
 
-def load(uri: str, fileformat: str, *, base_path: Optional[Path] = None) -> object:
-    loader = local_loader if uri.lower().startswith(file_prefix) else None
+def load(
+    uri: str, fileformat: str, *, base_path: Union[str, Path, None] = None
+) -> object:
+    loader = None
+    if uri.startswith(file_prefix):
+        loader = local_loader
+    if uri.startswith(s3_prefix):
+        loader = s3_loader
     parser = parsers.get(fileformat)
     if loader and parser:
         return parser(loader(uri, base_path=base_path))
     raise ValueError("unsupported artifact type")
```

### Comparing `chainmeta-0.0.2/src/chainmeta/config/__init__.py` & `chainmeta-0.0.3/src/chainmeta/config/__init__.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/src/chainmeta/config/categories.json` & `chainmeta-0.0.3/src/chainmeta/config/categories.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/src/chainmeta/config/chains.json` & `chainmeta-0.0.3/src/chainmeta/config/chains.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/src/chainmeta/config/entities.json` & `chainmeta-0.0.3/src/chainmeta/config/entities.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/src/chainmeta/constants.py` & `chainmeta-0.0.3/src/chainmeta/constants.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/src/chainmeta/contrib/chaintool.py` & `chainmeta-0.0.3/src/chainmeta/contrib/chaintool.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/src/chainmeta/contrib/chaintool_schema.json` & `chainmeta-0.0.3/src/chainmeta/contrib/chaintool_schema.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/src/chainmeta/contrib/messari.py` & `chainmeta-0.0.3/src/chainmeta/contrib/messari.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/src/chainmeta/db.py` & `chainmeta-0.0.3/src/chainmeta/db.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/src/chainmeta/logger.py` & `chainmeta-0.0.3/src/chainmeta/logger.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/src/chainmeta/metadata.py` & `chainmeta-0.0.3/src/chainmeta/metadata.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/src/chainmeta/schema/__init__.py` & `chainmeta-0.0.3/src/chainmeta/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/src/chainmeta/schema/artifact_schema.json` & `chainmeta-0.0.3/src/chainmeta/schema/artifact_schema.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/src/chainmeta/schema/meta_schema.json` & `chainmeta-0.0.3/src/chainmeta/schema/meta_schema.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/src/chainmeta/validator.py` & `chainmeta-0.0.3/src/chainmeta/validator.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/src/chainmeta.egg-info/PKG-INFO` & `chainmeta-0.0.3/src/chainmeta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainmeta
-Version: 0.0.2
+Version: 0.0.3
 Summary: Onchain metadata exchange protocol
 Project-URL: Homepage, https://github.com/microscopexyz/chainmeta-core
 Project-URL: Issues, https://github.com/microscopexyz/chainmeta-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `chainmeta-0.0.2/src/chainmeta.egg-info/SOURCES.txt` & `chainmeta-0.0.3/src/chainmeta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/tests/test_config.py` & `chainmeta-0.0.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/tests/test_translator.py` & `chainmeta-0.0.3/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.2/tests/test_validator.py` & `chainmeta-0.0.3/tests/test_validator.py`

 * *Files identical despite different names*

