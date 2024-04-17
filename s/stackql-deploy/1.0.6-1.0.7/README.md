# Comparing `tmp/stackql_deploy-1.0.6.tar.gz` & `tmp/stackql_deploy-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackql_deploy-1.0.6.tar", last modified: Tue Apr 16 23:36:38 2024, max compression
+gzip compressed data, was "stackql_deploy-1.0.7.tar", last modified: Wed Apr 17 00:28:47 2024, max compression
```

## Comparing `stackql_deploy-1.0.6.tar` & `stackql_deploy-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:36:38.461588 stackql_deploy-1.0.6/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.0.6/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-16 23:36:38.448344 stackql_deploy-1.0.6/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8214 2024-04-16 23:03:24.000000 stackql_deploy-1.0.6/README.rst
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-16 23:36:38.463303 stackql_deploy-1.0.6/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1300 2024-04-16 23:36:28.000000 stackql_deploy-1.0.6/setup.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:36:37.827758 stackql_deploy-1.0.6/stackql_deploy/
--rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-16 23:36:28.000000 stackql_deploy-1.0.6/stackql_deploy/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3687 2024-04-16 23:18:07.000000 stackql_deploy-1.0.6/stackql_deploy/cli.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:36:38.192966 stackql_deploy-1.0.6/stackql_deploy/cmd/
--rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.0.6/stackql_deploy/cmd/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     6291 2024-04-16 23:16:19.000000 stackql_deploy-1.0.6/stackql_deploy/cmd/build.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3433 2024-04-16 23:17:44.000000 stackql_deploy-1.0.6/stackql_deploy/cmd/teardown.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     2542 2024-04-16 23:17:44.000000 stackql_deploy-1.0.6/stackql_deploy/cmd/test.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:36:38.382306 stackql_deploy-1.0.6/stackql_deploy/lib/
--rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.0.6/stackql_deploy/lib/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)      333 2024-04-12 03:18:07.000000 stackql_deploy-1.0.6/stackql_deploy/lib/bootstrap.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3647 2024-04-16 02:40:32.000000 stackql_deploy-1.0.6/stackql_deploy/lib/config.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     2782 2024-04-16 03:47:18.000000 stackql_deploy-1.0.6/stackql_deploy/lib/templating.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5279 2024-04-16 03:46:51.000000 stackql_deploy-1.0.6/stackql_deploy/lib/utils.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:36:38.432724 stackql_deploy-1.0.6/stackql_deploy.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-16 23:36:37.000000 stackql_deploy-1.0.6/stackql_deploy.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      576 2024-04-16 23:36:37.000000 stackql_deploy-1.0.6/stackql_deploy.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-16 23:36:37.000000 stackql_deploy-1.0.6/stackql_deploy.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-16 23:36:37.000000 stackql_deploy-1.0.6/stackql_deploy.egg-info/entry_points.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       37 2024-04-16 23:36:37.000000 stackql_deploy-1.0.6/stackql_deploy.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-16 23:36:37.000000 stackql_deploy-1.0.6/stackql_deploy.egg-info/top_level.txt
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 00:28:47.254779 stackql_deploy-1.0.7/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.0.7/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-17 00:28:47.240223 stackql_deploy-1.0.7/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8214 2024-04-16 23:03:24.000000 stackql_deploy-1.0.7/README.rst
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-17 00:28:47.256777 stackql_deploy-1.0.7/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1300 2024-04-17 00:28:15.000000 stackql_deploy-1.0.7/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 00:28:46.644814 stackql_deploy-1.0.7/stackql_deploy/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-17 00:28:15.000000 stackql_deploy-1.0.7/stackql_deploy/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5491 2024-04-17 00:20:23.000000 stackql_deploy-1.0.7/stackql_deploy/cli.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 00:28:46.996621 stackql_deploy-1.0.7/stackql_deploy/cmd/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.0.7/stackql_deploy/cmd/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     6291 2024-04-16 23:16:19.000000 stackql_deploy-1.0.7/stackql_deploy/cmd/build.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3433 2024-04-16 23:17:44.000000 stackql_deploy-1.0.7/stackql_deploy/cmd/teardown.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     2542 2024-04-16 23:17:44.000000 stackql_deploy-1.0.7/stackql_deploy/cmd/test.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 00:28:47.182161 stackql_deploy-1.0.7/stackql_deploy/lib/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.0.7/stackql_deploy/lib/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      333 2024-04-12 03:18:07.000000 stackql_deploy-1.0.7/stackql_deploy/lib/bootstrap.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3647 2024-04-16 02:40:32.000000 stackql_deploy-1.0.7/stackql_deploy/lib/config.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     2782 2024-04-16 03:47:18.000000 stackql_deploy-1.0.7/stackql_deploy/lib/templating.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5279 2024-04-16 03:46:51.000000 stackql_deploy-1.0.7/stackql_deploy/lib/utils.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 00:28:47.221164 stackql_deploy-1.0.7/stackql_deploy.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-17 00:28:46.000000 stackql_deploy-1.0.7/stackql_deploy.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      576 2024-04-17 00:28:46.000000 stackql_deploy-1.0.7/stackql_deploy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-17 00:28:46.000000 stackql_deploy-1.0.7/stackql_deploy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-17 00:28:46.000000 stackql_deploy-1.0.7/stackql_deploy.egg-info/entry_points.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       37 2024-04-17 00:28:46.000000 stackql_deploy-1.0.7/stackql_deploy.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-17 00:28:46.000000 stackql_deploy-1.0.7/stackql_deploy.egg-info/top_level.txt
```

### Comparing `stackql_deploy-1.0.6/LICENSE` & `stackql_deploy-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.6/PKG-INFO` & `stackql_deploy-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.0.6
+Version: 1.0.7
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
```

### Comparing `stackql_deploy-1.0.6/README.rst` & `stackql_deploy-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.6/setup.py` & `stackql_deploy-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='stackql-deploy',
-    version='1.0.6',
+    version='1.0.7',
     description='Model driven resource provisioning and deployment framework using StackQL.',
     long_description=readme,
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/stackql-deploy',
     license='MIT',
     packages=find_packages(),
```

### Comparing `stackql_deploy-1.0.6/stackql_deploy/cli.py` & `stackql_deploy-1.0.7/stackql_deploy/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import click, os
 from . import __version__ as deploy_version
 from dotenv import load_dotenv, dotenv_values
 from .lib.bootstrap import logger, stackql
 from .cmd.build import StackQLProvisioner
 from .cmd.test import StackQLTestRunner
 from .cmd.teardown import StackQLDeProvisioner
+from jinja2 import Environment, FileSystemLoader
 
 def common_args(f):
     f = click.argument('stack_dir', type=str)(f)
     f = click.argument('stack_env', type=str)(f)
     return f
 
 def common_options(f):
@@ -81,18 +82,62 @@
         ("stackql version", stackql.version),
         ("stackql binary path", stackql.bin_path),
         ("platform", stackql.platform)
     ]
     for label, value in info_items:
         click.echo(f"{label.ljust(max_label_length)}: {value}")
 
+def create_project_structure(stack_name):
+    base_path = os.path.join(os.getcwd(), stack_name)
+    if os.path.exists(base_path):
+        raise click.ClickException(f"Directory '{stack_name}' already exists.")
+    
+    # Define subdirectories to create
+    directories = [
+        'stackql_docs',
+        'stackql_resources',
+        'stackql_tests'
+    ]
+
+    # Create base and subdirectories
+    for directory in directories:
+        os.makedirs(os.path.join(base_path, directory), exist_ok=True)
+
+    # Set up Jinja2 environment
+    template_base_path = os.path.join(os.path.dirname(__file__), 'templates')
+    env = Environment(loader=FileSystemLoader(template_base_path))
+    
+    # Template files and their output locations
+    template_files = {
+        'stackql_manifest.yml.template': 'stackql_manifest.yml',
+        'stackql_docs/resource1.md.template': os.path.join('stackql_docs', 'resource1.md'),
+        'stackql_resources/resource1.iql.template': os.path.join('stackql_resources', 'resource1.iql'),
+        'stackql_tests/resource1.iql.template': os.path.join('stackql_tests', 'resource1.iql')
+    }
+    
+    # Render and write files from templates
+    for template_name, output_name in template_files.items():
+        template = env.get_template(template_name)
+        rendered_content = template.render(stack_name=stack_name)
+        with open(os.path.join(base_path, output_name), 'w') as f:
+            f.write(rendered_content)
+
+@click.command()
+@click.argument('stack_name')
+def init(stack_name):
+    """Initialize a new stackql-deploy project structure."""
+    create_project_structure(stack_name)
+    click.echo(f"Project {stack_name} initialized successfully.")
+
+
 @click.group()
 def cli():
     pass
 
 cli.add_command(build)
 cli.add_command(test)
 cli.add_command(teardown)
 cli.add_command(info)
+cli.add_command(init)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `stackql_deploy-1.0.6/stackql_deploy/cmd/build.py` & `stackql_deploy-1.0.7/stackql_deploy/cmd/build.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.6/stackql_deploy/cmd/teardown.py` & `stackql_deploy-1.0.7/stackql_deploy/cmd/teardown.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.6/stackql_deploy/cmd/test.py` & `stackql_deploy-1.0.7/stackql_deploy/cmd/test.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.6/stackql_deploy/lib/config.py` & `stackql_deploy-1.0.7/stackql_deploy/lib/config.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.6/stackql_deploy/lib/templating.py` & `stackql_deploy-1.0.7/stackql_deploy/lib/templating.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.6/stackql_deploy/lib/utils.py` & `stackql_deploy-1.0.7/stackql_deploy/lib/utils.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.6/stackql_deploy.egg-info/PKG-INFO` & `stackql_deploy-1.0.7/stackql_deploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.0.6
+Version: 1.0.7
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
```

### Comparing `stackql_deploy-1.0.6/stackql_deploy.egg-info/SOURCES.txt` & `stackql_deploy-1.0.7/stackql_deploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

