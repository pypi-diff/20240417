# Comparing `tmp/mkdocs-juvix-plugin-0.1.4.tar.gz` & `tmp/mkdocs-juvix-plugin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-juvix-plugin-0.1.4.tar", last modified: Thu Nov 30 16:26:36 2023, max compression
+gzip compressed data, was "mkdocs-juvix-plugin-0.2.1.tar", last modified: Wed Apr 17 10:16:16 2024, max compression
```

## Comparing `mkdocs-juvix-plugin-0.1.4.tar` & `mkdocs-juvix-plugin-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2023-11-30 16:26:36.310899 mkdocs-juvix-plugin-0.1.4/
--rw-r--r--   0 jonaprieto   (501) staff       (20)      437 2023-11-30 16:26:36.310686 mkdocs-juvix-plugin-0.1.4/PKG-INFO
--rw-r--r--   0 jonaprieto   (501) staff       (20)     2462 2023-11-24 22:41:59.000000 mkdocs-juvix-plugin-0.1.4/README.md
-drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2023-11-30 16:26:36.309106 mkdocs-juvix-plugin-0.1.4/mkdocs_juvix/
--rw-r--r--   0 jonaprieto   (501) staff       (20)        0 2023-10-30 14:15:49.000000 mkdocs-juvix-plugin-0.1.4/mkdocs_juvix/__init__.py
--rw-r--r--   0 jonaprieto   (501) staff       (20)     3658 2023-11-30 16:26:02.000000 mkdocs-juvix-plugin-0.1.4/mkdocs_juvix/plugin.py
--rw-r--r--   0 jonaprieto   (501) staff       (20)     3241 2023-10-30 16:25:40.000000 mkdocs-juvix-plugin-0.1.4/mkdocs_juvix/standalone.py
-drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2023-11-30 16:26:36.310418 mkdocs-juvix-plugin-0.1.4/mkdocs_juvix_plugin.egg-info/
--rw-r--r--   0 jonaprieto   (501) staff       (20)      437 2023-11-30 16:26:36.000000 mkdocs-juvix-plugin-0.1.4/mkdocs_juvix_plugin.egg-info/PKG-INFO
--rw-r--r--   0 jonaprieto   (501) staff       (20)      353 2023-11-30 16:26:36.000000 mkdocs-juvix-plugin-0.1.4/mkdocs_juvix_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)        1 2023-11-30 16:26:36.000000 mkdocs-juvix-plugin-0.1.4/mkdocs_juvix_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)      107 2023-11-30 16:26:36.000000 mkdocs-juvix-plugin-0.1.4/mkdocs_juvix_plugin.egg-info/entry_points.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)       14 2023-11-30 16:26:36.000000 mkdocs-juvix-plugin-0.1.4/mkdocs_juvix_plugin.egg-info/requires.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)       13 2023-11-30 16:26:36.000000 mkdocs-juvix-plugin-0.1.4/mkdocs_juvix_plugin.egg-info/top_level.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)       38 2023-11-30 16:26:36.310940 mkdocs-juvix-plugin-0.1.4/setup.cfg
--rw-r--r--   0 jonaprieto   (501) staff       (20)      860 2023-11-30 16:26:02.000000 mkdocs-juvix-plugin-0.1.4/setup.py
+drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-04-17 10:16:16.525608 mkdocs-juvix-plugin-0.2.1/
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      493 2024-04-17 10:16:16.525337 mkdocs-juvix-plugin-0.2.1/PKG-INFO
+-rw-r--r--   0 jonaprieto   (501) staff       (20)     2459 2024-04-17 09:44:23.000000 mkdocs-juvix-plugin-0.2.1/README.md
+drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-04-17 10:16:16.523895 mkdocs-juvix-plugin-0.2.1/mkdocs_juvix/
+-rw-r--r--   0 jonaprieto   (501) staff       (20)        0 2023-10-30 14:15:49.000000 mkdocs-juvix-plugin-0.2.1/mkdocs_juvix/__init__.py
+-rw-r--r--   0 jonaprieto   (501) staff       (20)    18473 2024-04-17 10:14:39.000000 mkdocs-juvix-plugin-0.2.1/mkdocs_juvix/plugin.py
+-rw-r--r--   0 jonaprieto   (501) staff       (20)     3364 2024-04-17 09:42:21.000000 mkdocs-juvix-plugin-0.2.1/mkdocs_juvix/standalone.py
+-rw-r--r--   0 jonaprieto   (501) staff       (20)     2438 2024-04-17 09:46:29.000000 mkdocs-juvix-plugin-0.2.1/mkdocs_juvix/utils.py
+drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-04-17 10:16:16.525043 mkdocs-juvix-plugin-0.2.1/mkdocs_juvix_plugin.egg-info/
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      493 2024-04-17 10:16:16.000000 mkdocs-juvix-plugin-0.2.1/mkdocs_juvix_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      375 2024-04-17 10:16:16.000000 mkdocs-juvix-plugin-0.2.1/mkdocs_juvix_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)        1 2024-04-17 10:16:16.000000 mkdocs-juvix-plugin-0.2.1/mkdocs_juvix_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      107 2024-04-17 10:16:16.000000 mkdocs-juvix-plugin-0.2.1/mkdocs_juvix_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)       40 2024-04-17 10:16:16.000000 mkdocs-juvix-plugin-0.2.1/mkdocs_juvix_plugin.egg-info/requires.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)       13 2024-04-17 10:16:16.000000 mkdocs-juvix-plugin-0.2.1/mkdocs_juvix_plugin.egg-info/top_level.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)       38 2024-04-17 10:16:16.525655 mkdocs-juvix-plugin-0.2.1/setup.cfg
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      827 2024-04-17 10:16:14.000000 mkdocs-juvix-plugin-0.2.1/setup.py
```

### Comparing `mkdocs-juvix-plugin-0.1.4/README.md` & `mkdocs-juvix-plugin-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # Juvix MkDocs
 
 This is a plugin to be used with Mkdocs to build static websites and highlight
 Juvix codeblocks using [the Juvix Compiler](https://docs.juvix.org).
 
 To utilize this feature provided by the compiler, the file should have the
 `.juvix.md` extension. Within this file, any Markdown is valid; the compiler
-would only concern itself with *juvix code blocks*. 
+would only concern itself with *juvix code blocks*.
 
-A Juvix code block in Markdown appears as follows: 
+A Juvix code block in Markdown appears as follows:
 
 <pre><code>
 ```juvix
 module Test;
 import Stdlib.Prelude open;
 
 main : IO := printStringLn "Hello!";
 ```
 </code></pre>
 
 Juvix code blocks can be hidden from the final build if you use <pre>```juvix
-hide```</pre> as the code block header. 
+hide```</pre> as the code block header.
 
 
 A special addition, exclusive for MkDocs, is the *juvix-standalone files*. These
 are modules which are compiled as standalone modules/programs. One key advantage
 of these is that they can contain all the definitions which the module depends
 on within a HTML *details* environment. To define such blocks, use the
 `juvix-standalone` header.
```

### Comparing `mkdocs-juvix-plugin-0.1.4/mkdocs_juvix/standalone.py` & `mkdocs-juvix-plugin-0.2.1/mkdocs_juvix/standalone.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import hashlib
-import markdown as mk
-from pathlib import *
 import logging
 import subprocess
+from pathlib import *
 
-log = logging.getLogger('mkdocs')
+import markdown as mk
+
+log = logging.getLogger("mkdocs")
 
 try:
     subprocess.check_output(["juvix", "--numeric-version"])
 except Exception:
     log.error("Juvix is not installed and it's required for this plugin.")
     raise
 
 docsPath = Path("./docs")
 snippetsPath = docsPath.joinpath("juvix-snippets")
 snippetsPath.mkdir(parents=True, exist_ok=True)
 
 
-def render(src: str, language: str, class_name: str, options: dict, md: mk.Markdown, **kwargs):
+def render(
+    src: str, language: str, class_name: str, options: dict, md: mk.Markdown, **kwargs
+):
     try:
-        modname = "M" + hashlib.md5(src.encode('utf-8')).hexdigest()[:5]
+        modname = "M" + hashlib.md5(src.encode("utf-8")).hexdigest()[:5]
         moduleFolder = snippetsPath.joinpath(modname)
         moduleFolder.mkdir(parents=True, exist_ok=True)
 
         fname = modname + ".juvix"
         fpath = moduleFolder.joinpath(fname)
 
         log.info("> Juvix-plugin: juvix-snippet: %s", fpath)
@@ -39,49 +42,58 @@
             f.write("end;\n")
 
         check = ["juvix", "typecheck", fname]
         runCheck = subprocess.run(check, cwd=moduleFolder, capture_output=True)
 
         if runCheck.returncode != 0:
             log.error("> Error: %s", runCheck.stderr)
-            return """<code><div class="juvix-error">%s</div></code>""" % str(runCheck.stderr.decode("utf-8"))
-
-        htmlCmd = ["juvix",
-                   "html",
-                   "--only-source",
-                   "--only-code",
-                   "--no-path",
-                   "--prefix-url=",
-                   ("--prefix-id=%s" % modname),
-                   fname]
+            return """<code><div class="juvix-error">%s</div></code>""" % str(
+                runCheck.stderr.decode("utf-8")
+            )
+
+        htmlCmd = [
+            "juvix",
+            "html",
+            "--only-source",
+            "--only-code",
+            "--no-path",
+            "--prefix-url=",
+            ("--prefix-id=%s" % modname),
+            fname,
+        ]
         cd = subprocess.run(htmlCmd, cwd=moduleFolder, capture_output=True)
 
         if cd.returncode != 0:
             log.error("> Juvix-plugin Error: %s", cd.stderr.decode("utf-8"))
             raise Exception(cd.stderr.decode("utf-8"))
 
         htmlFolder = moduleFolder.joinpath("html")
         htmlFile = modname + ".html"
         moduleHtmlPath = htmlFolder.joinpath(htmlFile)
 
         with open(moduleHtmlPath, "r") as f:
-            moduleHtml = ''.join(f.readlines()[2:])
+            moduleHtml = "".join(f.readlines()[2:])
             mainOutput = "<pre><code><div>%s</div></code></pre>" % moduleHtml
             extraOutput = []
             if len(list(htmlFolder.iterdir())) > 2:
                 extraOutput += [
-                    "<details class='quote'><summary>Auxiliary definitions</summary>"]
+                    "<details class='quote'><summary>Auxiliary definitions</summary>"
+                ]
                 for f in htmlFolder.iterdir():
                     if f.is_file() and f.name + ".html" != htmlFile:
                         with open(f, "r") as m:
-                            fOut = ''.join(m.readlines())
-                            extraOutput += ["""
+                            fOut = "".join(m.readlines())
+                            extraOutput += [
+                                """
                                             <details class='quote'><summary>%s </summary>
                                             <pre><code><div>%s</div></code></pre>
-                                            </details>""" % (f.name, fOut)]
+                                            </details>"""
+                                % (f.name, fOut)
+                            ]
                 extraOutput += ["</details>"]
             return mainOutput + "\n".join(extraOutput)
 
     except Exception:
         import traceback
+
         print(traceback.format_exc())
         raise
```

### Comparing `mkdocs-juvix-plugin-0.1.4/setup.py` & `mkdocs-juvix-plugin-0.2.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-from setuptools import setup, find_packages
-
+from setuptools import find_packages, setup
 
 setup(
-    name='mkdocs-juvix-plugin',
-    version='0.1.4',
-    description='A plugin to render Juvix code blocks in MkDocs.',
-    long_description='',
-    keywords='mkdocs',
-    # url='https//github.com/anoma/juvix-mkdocs/',
-    author='Jonathan Prieto-Cubides, and GitHub contributors',
-    author_email='jonathan@heliax.dev',
-    license='MIT',
-    python_requires='>=3.11',
-    install_requires=[
-        'mkdocs >= 1.5.0',
-    ],
+    name="mkdocs-juvix-plugin",
+    version="0.2.1",
+    description="A plugin to render Juvix code blocks in MkDocs.",
+    long_description="",
+    keywords="mkdocs",
+    author="Jonathan Prieto-Cubides, and GitHub contributors",
+    author_email="jonathan@heliax.dev",
+    license="MIT",
+    python_requires=">=3.11",
+    install_requires=["mkdocs >= 1.5.0", "pyYaml", "pymdown-extensions"],
     classifiers=[
-        'Intended Audience :: Developers',
-        'Intended Audience :: Information Technology',
-        'Programming Language :: Python',
+        "Intended Audience :: Developers",
+        "Intended Audience :: Information Technology",
+        "Programming Language :: Python",
     ],
     packages=find_packages(),
     entry_points={
-        'mkdocs.plugins': [
-            'juvix = mkdocs_juvix.plugin:JuvixPlugin',
-            'juvix-standalone = mkdocs_juvix.standalone:render'
+        "mkdocs.plugins": [
+            "juvix = mkdocs_juvix.plugin:JuvixPlugin",
+            "juvix-standalone = mkdocs_juvix.standalone:render",
         ]
-    }
+    },
 )
```

