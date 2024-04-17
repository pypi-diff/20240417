# Comparing `tmp/pywis-topics-0.3.0.tar.gz` & `tmp/pywis-topics-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywis-topics-0.3.0.tar", last modified: Mon Feb 19 00:34:26 2024, max compression
+gzip compressed data, was "pywis-topics-0.3.1.tar", last modified: Wed Apr 17 15:07:32 2024, max compression
```

## Comparing `pywis-topics-0.3.0.tar` & `pywis-topics-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2024-02-19 00:34:26.000000 pywis-topics-0.3.0/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)    11357 2022-10-11 15:29:10.000000 pywis-topics-0.3.0/LICENSE
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       43 2023-11-21 01:19:27.000000 pywis-topics-0.3.0/MANIFEST.in
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     4789 2024-02-19 00:34:26.000000 pywis-topics-0.3.0/PKG-INFO
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     2958 2023-11-27 11:50:28.000000 pywis-topics-0.3.0/README.md
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2024-02-19 00:34:26.000000 pywis-topics-0.3.0/pywis_topics/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     1305 2024-02-19 00:33:48.000000 pywis-topics-0.3.0/pywis_topics/__init__.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     2643 2023-11-27 11:50:28.000000 pywis-topics-0.3.0/pywis_topics/bundle.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     3524 2023-11-27 11:50:28.000000 pywis-topics-0.3.0/pywis_topics/centre_id.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     6660 2023-11-21 11:48:36.000000 pywis-topics-0.3.0/pywis_topics/pygeoapi_plugin.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     6756 2024-02-19 00:32:52.000000 pywis-topics-0.3.0/pywis_topics/topics.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     3917 2023-11-24 02:05:42.000000 pywis-topics-0.3.0/pywis_topics/util.py
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2024-02-19 00:34:26.000000 pywis-topics-0.3.0/pywis_topics.egg-info/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     4789 2024-02-19 00:34:26.000000 pywis-topics-0.3.0/pywis_topics.egg-info/PKG-INFO
--rw-rw-r--   0 tomkralidis   (501) staff       (20)      423 2024-02-19 00:34:26.000000 pywis-topics-0.3.0/pywis_topics.egg-info/SOURCES.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)        1 2024-02-19 00:34:26.000000 pywis-topics-0.3.0/pywis_topics.egg-info/dependency_links.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       51 2024-02-19 00:34:26.000000 pywis-topics-0.3.0/pywis_topics.egg-info/entry_points.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)        6 2024-02-19 00:34:26.000000 pywis-topics-0.3.0/pywis_topics.egg-info/requires.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       13 2024-02-19 00:34:26.000000 pywis-topics-0.3.0/pywis_topics.egg-info/top_level.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)        6 2023-11-21 11:50:44.000000 pywis-topics-0.3.0/requirements.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       38 2024-02-19 00:34:26.000000 pywis-topics-0.3.0/setup.cfg
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     3254 2023-11-21 13:44:41.000000 pywis-topics-0.3.0/setup.py
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2024-04-17 15:07:32.351873 pywis-topics-0.3.1/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)    11357 2024-04-17 15:06:15.000000 pywis-topics-0.3.1/LICENSE
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       43 2024-04-17 15:06:15.000000 pywis-topics-0.3.1/MANIFEST.in
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3955 2024-04-17 15:07:32.351480 pywis-topics-0.3.1/PKG-INFO
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3194 2024-04-17 15:06:15.000000 pywis-topics-0.3.1/README.md
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2024-04-17 15:07:32.347580 pywis-topics-0.3.1/pywis_topics/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     1305 2024-04-17 15:06:52.000000 pywis-topics-0.3.1/pywis_topics/__init__.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     2772 2024-04-17 15:06:15.000000 pywis-topics-0.3.1/pywis_topics/bundle.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3524 2024-04-17 15:06:15.000000 pywis-topics-0.3.1/pywis_topics/centre_id.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     6660 2024-04-17 15:06:15.000000 pywis-topics-0.3.1/pywis_topics/pygeoapi_plugin.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     6884 2024-04-17 15:06:15.000000 pywis-topics-0.3.1/pywis_topics/topics.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3917 2024-04-17 15:06:15.000000 pywis-topics-0.3.1/pywis_topics/util.py
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2024-04-17 15:07:32.350721 pywis-topics-0.3.1/pywis_topics.egg-info/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3955 2024-04-17 15:07:32.000000 pywis-topics-0.3.1/pywis_topics.egg-info/PKG-INFO
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)      423 2024-04-17 15:07:32.000000 pywis-topics-0.3.1/pywis_topics.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)        1 2024-04-17 15:07:32.000000 pywis-topics-0.3.1/pywis_topics.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       50 2024-04-17 15:07:32.000000 pywis-topics-0.3.1/pywis_topics.egg-info/entry_points.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)        6 2024-04-17 15:07:32.000000 pywis-topics-0.3.1/pywis_topics.egg-info/requires.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       13 2024-04-17 15:07:32.000000 pywis-topics-0.3.1/pywis_topics.egg-info/top_level.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)        6 2024-04-17 15:06:15.000000 pywis-topics-0.3.1/requirements.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       38 2024-04-17 15:07:32.352058 pywis-topics-0.3.1/setup.cfg
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3254 2024-04-17 15:06:15.000000 pywis-topics-0.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pywis-topics-0.3.0/LICENSE` & `pywis-topics-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywis-topics-0.3.0/README.md` & `pywis-topics-0.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -40,27 +40,33 @@
 
 ## Running
 
 First check pywis-topics was correctly installed
 
 ```bash
 pywis-topics --version
+
+# sync WTH bundle
+pywis-topics bundle sync
 ```
 
 ### Listing and validation
 
 ```bash
 # validate a WIS2 topic hierarchy
 pywis-topics topic validate origin/a/wis2/ca-eccc-msc
 
 # validate a WIS2 topic hierarchy in no-strict mode
 pywis-topics topic validate --no-strict origin/a/wis2/fake-centre-id/data/core
 
 # list children of a given WIS2 topic hierarchy level
 pywis-topics topic list wis2/a
+
+# validate a WIS2 topic hierarchy with wildcards (needs no-strict mode)
+pywis-topics topic validate origin/a/wis2/+/data/core --no-strict
 ```
 
 ### Centre identification validation
 
 ```bash
 # validate a centre-id
 pywis-topics centre-id 123
@@ -77,14 +83,16 @@
 th = TopicHierarchy()
 
 th.validate('origin/a/wis2/ca-eccc-msc/data/core')
 th.list_children('origin/a/wis2')
 
 th.validate('origin/a/wis2/fake-centre-id/data/core', strict=False)
 
+th.validate('origin/a/wis2/+/data/#', strict=False)
+
 cid = CentreId('ca-centre123')
 cid.validate()
 ```
 
 ## Development
 
 ### Running Tests
```

### Comparing `pywis-topics-0.3.0/pywis_topics/__init__.py` & `pywis-topics-0.3.1/pywis_topics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 ###############################################################################
 
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 
 import click
 
 from pywis_topics.bundle import bundle
 from pywis_topics.centre_id import centre_id
 from pywis_topics.topics import topic
```

### Comparing `pywis-topics-0.3.0/pywis_topics/bundle.py` & `pywis-topics-0.3.1/pywis_topics/bundle.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,21 +39,21 @@
 
 @click.group()
 def bundle():
     """Configuration bundle management"""
     pass
 
 
-@click.command()
-@get_cli_common_options
-@click.pass_context
-def sync(ctx, logfile, verbosity):
-    "Sync configuration bundle"""
+def sync_bundle() -> None:
+    """
+    Sync bundle locally to ~/.pywis-topics
+
+    :returns: `None`
+    """
 
-    setup_logger(verbosity, logfile)
     LOGGER.debug('Caching topic hierarchy')
 
     if USERDIR.exists():
         shutil.rmtree(USERDIR)
 
     LOGGER.debug('Downloading WIS2 topic hierarchy')
     WIS2_TOPIC_HIERARCHY_DIR.mkdir(parents=True, exist_ok=True)
@@ -74,8 +74,18 @@
     LOGGER.debug('Downloading IANA TLDs')
     IANA_URL = 'https://data.iana.org/TLD/tlds-alpha-by-domain.txt'
     iana_file = WIS2_TOPIC_HIERARCHY_DIR / 'tlds-alpha-by-domain.txt'
     with iana_file.open('wb') as fh:
         fh.write(urlopen_(f'{IANA_URL}').read())
 
 
+@click.command()
+@get_cli_common_options
+@click.pass_context
+def sync(ctx, logfile, verbosity):
+    "Sync configuration bundle"""
+
+    setup_logger(verbosity, logfile)
+    sync_bundle()
+
+
 bundle.add_command(sync)
```

### Comparing `pywis-topics-0.3.0/pywis_topics/centre_id.py` & `pywis-topics-0.3.1/pywis_topics/centre_id.py`

 * *Files identical despite different names*

### Comparing `pywis-topics-0.3.0/pywis_topics/pygeoapi_plugin.py` & `pywis-topics-0.3.1/pywis_topics/pygeoapi_plugin.py`

 * *Files identical despite different names*

### Comparing `pywis-topics-0.3.0/pywis_topics/topics.py` & `pywis-topics-0.3.1/pywis_topics/topics.py`

 * *Files 8% similar despite different names*

```diff
@@ -146,14 +146,17 @@
 
         th_tokens = topic_hierarchy.split('/', 6)
 
         for count, value in enumerate(th_tokens):
             if not strict and count == 3:
                 LOGGER.debug('Skipping centre-id validation')
                 continue
+            elif not strict and value in ['+', '#']:
+                LOGGER.debug('Skipping wildcard')
+                continue
             if value not in self.topics[count]:
                 return False
 
         return True
 
 
 def validate_baseline(topic_hierarchy: str = None) -> bool:
```

### Comparing `pywis-topics-0.3.0/pywis_topics/util.py` & `pywis-topics-0.3.1/pywis_topics/util.py`

 * *Files identical despite different names*

### Comparing `pywis-topics-0.3.0/setup.py` & `pywis-topics-0.3.1/setup.py`

 * *Files identical despite different names*

