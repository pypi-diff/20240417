# Comparing `tmp/prelude-cli-1.7.3.tar.gz` & `tmp/prelude_cli-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.7.3.tar", last modified: Fri Apr 12 14:35:45 2024, max compression
+gzip compressed data, was "prelude_cli-1.7.4.tar", last modified: Wed Apr 17 18:50:45 2024, max compression
```

## Comparing `prelude-cli-1.7.3.tar` & `prelude_cli-1.7.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-12 14:35:45.207879 prelude-cli-1.7.3/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.7.3/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.7.3/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      940 2024-04-12 14:35:45.207792 prelude-cli-1.7.3/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.7.3/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-12 14:35:45.202139 prelude-cli-1.7.3/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.7.3/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1014 2024-04-03 22:19:39.000000 prelude-cli-1.7.3/prelude_cli/cli.py
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-12-08 16:31:30.000000 prelude-cli-1.7.3/prelude_cli/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-12 14:35:45.203919 prelude-cli-1.7.3/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)     1120 2024-01-05 14:14:44.000000 prelude-cli-1.7.3/prelude_cli/templates/README.md
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.7.3/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      261 2024-01-05 14:14:44.000000 prelude-cli-1.7.3/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-12 14:35:45.206852 prelude-cli-1.7.3/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.7.3/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)    10043 2024-04-03 22:19:39.000000 prelude-cli-1.7.3/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.7.3/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)    10050 2024-04-11 16:14:14.000000 prelude-cli-1.7.3/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     2543 2024-04-11 19:46:08.000000 prelude-cli-1.7.3/prelude_cli/views/generate.py
--rw-r--r--   0 pack       (501) staff       (20)     8143 2024-01-05 14:14:44.000000 prelude-cli-1.7.3/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)     4674 2024-03-21 18:38:20.000000 prelude-cli-1.7.3/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)      662 2024-04-03 22:19:39.000000 prelude-cli-1.7.3/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-12 14:35:45.207519 prelude-cli-1.7.3/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      940 2024-04-12 14:35:45.000000 prelude-cli-1.7.3/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      660 2024-04-12 14:35:45.000000 prelude-cli-1.7.3/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2024-04-12 14:35:45.000000 prelude-cli-1.7.3/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2024-04-12 14:35:45.000000 prelude-cli-1.7.3/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2024-04-12 14:35:45.000000 prelude-cli-1.7.3/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2024-04-12 14:35:45.000000 prelude-cli-1.7.3/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.7.3/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      680 2024-04-12 14:35:45.208154 prelude-cli-1.7.3/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:45.430266 prelude_cli-1.7.4/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude_cli-1.7.4/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude_cli-1.7.4/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      940 2024-04-17 18:50:45.430079 prelude_cli-1.7.4/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude_cli-1.7.4/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:45.423944 prelude_cli-1.7.4/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_cli-1.7.4/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1014 2024-04-03 22:19:39.000000 prelude_cli-1.7.4/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-12-08 16:31:30.000000 prelude_cli-1.7.4/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:45.426344 prelude_cli-1.7.4/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)     1120 2024-01-05 14:14:44.000000 prelude_cli-1.7.4/prelude_cli/templates/README.md
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_cli-1.7.4/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      261 2024-01-05 14:14:44.000000 prelude_cli-1.7.4/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:45.429006 prelude_cli-1.7.4/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_cli-1.7.4/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)    10043 2024-04-03 22:19:39.000000 prelude_cli-1.7.4/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude_cli-1.7.4/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)    10255 2024-04-17 18:29:22.000000 prelude_cli-1.7.4/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     2543 2024-04-11 19:46:08.000000 prelude_cli-1.7.4/prelude_cli/views/generate.py
+-rw-r--r--   0 pack       (501) staff       (20)     8568 2024-04-17 18:29:22.000000 prelude_cli-1.7.4/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     4771 2024-04-17 18:29:22.000000 prelude_cli-1.7.4/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)      662 2024-04-03 22:19:39.000000 prelude_cli-1.7.4/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:45.429602 prelude_cli-1.7.4/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      940 2024-04-17 18:50:45.000000 prelude_cli-1.7.4/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      660 2024-04-17 18:50:45.000000 prelude_cli-1.7.4/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2024-04-17 18:50:45.000000 prelude_cli-1.7.4/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2024-04-17 18:50:45.000000 prelude_cli-1.7.4/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2024-04-17 18:50:45.000000 prelude_cli-1.7.4/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2024-04-17 18:50:45.000000 prelude_cli-1.7.4/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude_cli-1.7.4/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      680 2024-04-17 18:50:45.430658 prelude_cli-1.7.4/setup.cfg
```

### Comparing `prelude-cli-1.7.3/LICENSE` & `prelude_cli-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.3/PKG-INFO` & `prelude_cli-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.7.3
+Version: 1.7.4
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prelude-sdk==1.7.1
+Requires-Dist: prelude-sdk==1.7.2
 Requires-Dist: click>8
 Requires-Dist: rich
 Requires-Dist: python-dateutil
 
 # Prelude CLI
 
 Interact with the full range of features in Prelude Detect, organized by:
```

### Comparing `prelude-cli-1.7.3/prelude_cli/cli.py` & `prelude_cli-1.7.4/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.3/prelude_cli/templates/README.md` & `prelude_cli-1.7.4/prelude_cli/templates/README.md`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.3/prelude_cli/views/build.py` & `prelude_cli-1.7.4/prelude_cli/views/build.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.3/prelude_cli/views/configure.py` & `prelude_cli-1.7.4/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.3/prelude_cli/views/detect.py` & `prelude_cli-1.7.4/prelude_cli/views/detect.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,20 +45,24 @@
     """ Update an existing endpoint """
     with Spinner(description='Updating endpoint'):
         data = controller.update_endpoint(endpoint_id=endpoint_id, tags=tags)
     print_json(data=data)
 
 
 @detect.command('tests')
+@click.option('--techniques', help='comma-separated list of techniques', type=str)
 @click.pass_obj
 @handle_api_error
-def list_tests(controller):
+def list_tests(controller, techniques):
     """ List all security tests """
     with Spinner(description='Fetching all security tests'):
-        data = controller.list_tests()
+        filters = dict()
+        if techniques:
+            filters['techniques'] = techniques
+        data = controller.list_tests(filters=filters)
     print_json(data=data)
 
 
 @detect.command('test')
 @click.argument('test_id')
 @click.pass_obj
 @handle_api_error
```

### Comparing `prelude-cli-1.7.3/prelude_cli/views/generate.py` & `prelude_cli-1.7.4/prelude_cli/views/generate.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.3/prelude_cli/views/iam.py` & `prelude_cli-1.7.4/prelude_cli/views/iam.py`

 * *Files 6% similar despite different names*

```diff
@@ -197,14 +197,24 @@
 @handle_api_error
 def unsubscribe(controller, event):
     """ Unsubscribe to email notifications for an event """
     with Spinner(description='Unsubscribing'):
         data = controller.unsubscribe(event=AuditEvent[event])
     print_json(data=data)
 
+@iam.command('accept-terms', hidden=True)
+@click.argument('name', type=str, required=True)
+@click.option('-v', '--version', type=int, required=True)
+@click.pass_obj
+@handle_api_error
+def accept_terms(controller, name, version):
+    """ Accept terms and conditions """
+    with Spinner(description='Accepting terms and conditions'):
+        data = controller.accept_terms(name=name, version=version)
+    print_json(data=data)
 
 @iam.command('purge')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
 def purge(controller):
     """ Delete your account """
```

### Comparing `prelude-cli-1.7.3/prelude_cli/views/partner.py` & `prelude_cli-1.7.4/prelude_cli/views/partner.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,20 +56,21 @@
 
 @partner.command('endpoints')
 @click.argument('partner',
                 type=click.Choice([c.name for c in Control if c != Control.INVALID], case_sensitive=False))
 @click.option('--platform', required=True, help='platform name (e.g. "windows")', type=click.Choice(['windows', 'linux', 'darwin'], case_sensitive=False))
 @click.option('--hostname', default='', help='hostname pattern (e.g. "mycompany-c24oi444")')
 @click.option('--offset', default=0, help='API pagination offset', type=int)
+@click.option('--limit', default=100, help='API pagination limit', type=int)
 @click.pass_obj
 @handle_api_error
-def partner_endpoints(controller, partner, platform, hostname, offset):
+def partner_endpoints(controller, partner, platform, hostname, offset, limit):
     """ Get a list of endpoints from a partner """
     with Spinner(description='Fetching endpoints from partner'):
-        data = controller.endpoints(partner=Control[partner], platform=platform, hostname=hostname, offset=offset)
+        data = controller.endpoints(partner=Control[partner], platform=platform, hostname=hostname, offset=offset, count=limit)
     print_json(data=data)
 
 
 @partner.command('deploy')
 @click.confirmation_option(prompt='Are you sure?')
 @click.argument('partner', type=click.Choice([Control.CROWDSTRIKE.name], case_sensitive=False))
 @click.option('--host_ids', required=True, help='a list of host IDs to deploy to', multiple=True, default=[])
```

### Comparing `prelude-cli-1.7.3/prelude_cli/views/shared.py` & `prelude_cli-1.7.4/prelude_cli/views/shared.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.3/prelude_cli.egg-info/PKG-INFO` & `prelude_cli-1.7.4/prelude_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.7.3
+Version: 1.7.4
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prelude-sdk==1.7.1
+Requires-Dist: prelude-sdk==1.7.2
 Requires-Dist: click>8
 Requires-Dist: rich
 Requires-Dist: python-dateutil
 
 # Prelude CLI
 
 Interact with the full range of features in Prelude Detect, organized by:
```

### Comparing `prelude-cli-1.7.3/prelude_cli.egg-info/SOURCES.txt` & `prelude_cli-1.7.4/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.3/setup.cfg` & `prelude_cli-1.7.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.7.3
+version = 1.7.4
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 1.7.1
+	prelude-sdk == 1.7.2
 	click > 8
 	rich
 	python-dateutil
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
```

