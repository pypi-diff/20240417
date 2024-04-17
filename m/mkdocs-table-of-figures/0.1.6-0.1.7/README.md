# Comparing `tmp/mkdocs-table-of-figures-0.1.6.tar.gz` & `tmp/mkdocs-table-of-figures-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-table-of-figures-0.1.6.tar", last modified: Mon Apr 15 21:08:39 2024, max compression
+gzip compressed data, was "mkdocs-table-of-figures-0.1.7.tar", last modified: Wed Apr 17 13:55:40 2024, max compression
```

## Comparing `mkdocs-table-of-figures-0.1.6.tar` & `mkdocs-table-of-figures-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-15 21:09:13.074839 mkdocs-table-of-figures-0.1.6/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2023-05-09 09:20:19.000000 mkdocs-table-of-figures-0.1.6/MANIFEST.in
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     5439 2024-04-15 21:09:13.071839 mkdocs-table-of-figures-0.1.6/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1163 2024-04-15 20:50:29.000000 mkdocs-table-of-figures-0.1.6/changelog.md
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2023-04-28 08:21:37.000000 mkdocs-table-of-figures-0.1.6/license
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-15 21:09:12.972846 mkdocs-table-of-figures-0.1.6/mkdocs_table_of_figures/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-02 06:14:09.000000 mkdocs-table-of-figures-0.1.6/mkdocs_table_of_figures/__init__.py
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     6832 2024-04-15 20:48:24.000000 mkdocs-table-of-figures-0.1.6/mkdocs_table_of_figures/plugin.py
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-15 21:09:13.056208 mkdocs-table-of-figures-0.1.6/mkdocs_table_of_figures.egg-info/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     5439 2024-04-15 21:09:12.000000 mkdocs-table-of-figures-0.1.6/mkdocs_table_of_figures.egg-info/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      417 2024-04-15 21:09:12.000000 mkdocs-table-of-figures-0.1.6/mkdocs_table_of_figures.egg-info/SOURCES.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2024-04-15 21:09:12.000000 mkdocs-table-of-figures-0.1.6/mkdocs_table_of_figures.egg-info/dependency_links.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       83 2024-04-15 21:09:12.000000 mkdocs-table-of-figures-0.1.6/mkdocs_table_of_figures.egg-info/entry_points.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       14 2024-04-15 21:09:12.000000 mkdocs-table-of-figures-0.1.6/mkdocs_table_of_figures.egg-info/requires.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       24 2024-04-15 21:09:12.000000 mkdocs-table-of-figures-0.1.6/mkdocs_table_of_figures.egg-info/top_level.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     4117 2023-06-09 15:39:23.000000 mkdocs-table-of-figures-0.1.6/readme.md
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2024-04-15 21:09:13.075797 mkdocs-table-of-figures-0.1.6/setup.cfg
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1135 2024-04-15 20:48:46.000000 mkdocs-table-of-figures-0.1.6/setup.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-17 13:55:40.715542 mkdocs-table-of-figures-0.1.7/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2023-05-09 09:20:19.000000 mkdocs-table-of-figures-0.1.7/MANIFEST.in
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     5832 2024-04-17 13:55:40.714506 mkdocs-table-of-figures-0.1.7/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1288 2024-04-17 13:51:56.000000 mkdocs-table-of-figures-0.1.7/changelog.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2023-04-28 08:21:37.000000 mkdocs-table-of-figures-0.1.7/license
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-17 13:55:40.607178 mkdocs-table-of-figures-0.1.7/mkdocs_table_of_figures/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-02 06:14:09.000000 mkdocs-table-of-figures-0.1.7/mkdocs_table_of_figures/__init__.py
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     6830 2024-04-17 13:42:18.000000 mkdocs-table-of-figures-0.1.7/mkdocs_table_of_figures/plugin.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-17 13:55:40.700188 mkdocs-table-of-figures-0.1.7/mkdocs_table_of_figures.egg-info/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     5832 2024-04-17 13:55:40.000000 mkdocs-table-of-figures-0.1.7/mkdocs_table_of_figures.egg-info/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      417 2024-04-17 13:55:40.000000 mkdocs-table-of-figures-0.1.7/mkdocs_table_of_figures.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2024-04-17 13:55:40.000000 mkdocs-table-of-figures-0.1.7/mkdocs_table_of_figures.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       83 2024-04-17 13:55:40.000000 mkdocs-table-of-figures-0.1.7/mkdocs_table_of_figures.egg-info/entry_points.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       14 2024-04-17 13:55:40.000000 mkdocs-table-of-figures-0.1.7/mkdocs_table_of_figures.egg-info/requires.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       24 2024-04-17 13:55:40.000000 mkdocs-table-of-figures-0.1.7/mkdocs_table_of_figures.egg-info/top_level.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     4412 2024-04-17 13:55:29.000000 mkdocs-table-of-figures-0.1.7/readme.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2024-04-17 13:55:40.717757 mkdocs-table-of-figures-0.1.7/setup.cfg
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1135 2024-04-17 13:52:11.000000 mkdocs-table-of-figures-0.1.7/setup.py
```

### Comparing `mkdocs-table-of-figures-0.1.6/PKG-INFO` & `mkdocs-table-of-figures-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.1.6
+Version: 0.1.7
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Description: # mkdocs-table-of-figures
         
@@ -84,14 +84,28 @@
             The title of the mermaid diagram go here
         ```
         
         It will not work if there is a line between the diagram and the title.
         
         I highly recommend using `mkdocs-material` to use `mermaid` diagrams. For more info about `mermaid` diagrams, I invite you to check `mkdocs-material` and `mermaid`'s official documentation.
         
+        I also recommend to add this stylesheet to prevent mermaid size from being reduced by mkdocs-material stylesheet in your `mkdocs.yml` at extra-css option
+        
+        ``` css
+        figure.figure-mermaid {
+            margin: 0 1em;
+            width: 100%;
+        }
+        ```
+        
+        ``` yml
+        extra_css:
+          - fix-mermaid-figure.css
+        ```
+        
         ## License
         
         This project is under MIT license. See the `license` file for more details.
         
         ## See Also
         
         - [GitLab Repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-annexes-integration/)
```

### Comparing `mkdocs-table-of-figures-0.1.6/changelog.md` & `mkdocs-table-of-figures-0.1.7/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on Keep a Changelog, and this project adheres to Semantic Versioning.
 
+## [0.1.7] - 2024-04-17
+
+### Added
+
+- specific class to mermaid figure to let user fix width if needed in `plugin.py`
+
 ## [0.1.6] - 2024-04-15
 
 ### Fixed
 
 - print of figure in console in `plugin.py`
 
 ## [0.1.5] - 2024-04-15
```

### Comparing `mkdocs-table-of-figures-0.1.6/license` & `mkdocs-table-of-figures-0.1.7/license`

 * *Files identical despite different names*

### Comparing `mkdocs-table-of-figures-0.1.6/mkdocs_table_of_figures/plugin.py` & `mkdocs-table-of-figures-0.1.7/mkdocs_table_of_figures/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                             if match.re.pattern == pattern_img and match.group(1):
                                 self.figures.append({"number": self.counter, "description": match.group(1), "link": link})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n  <img src="{config.site_url + match.group(2) if match.group(2).startswith("/") else match.group(2)}" alt="{match.group(1)}">\n  <figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
                                 if self.keep_md_format:
                                     replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n  ![{match.group(1)}]({match.group(2)})\n  <figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
                             elif match.re.pattern == pattern_mermaid and match.group(2):
                                 self.figures.append({"number": self.counter, "description": match.group(2), "link": link})
-                                replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n  {match.group(1)}\n  <figcaption>{self.config.figure_label} {self.counter} — {match.group(2)}</figcaption>\n</figure>'
+                                replacement = f'<figure id="figure-{self.counter}" class="figure-mermaid" markdown="span">\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(2)}</figcaption>\n</figure>'
                             
                             if replacement == match.group(0):
                                 self._logger.debug(f'Ignoring image/diagram at {self.file_relative_path}{page.file.src_uri}')
                             else:
                                 self._logger.debug(f'Formating image/diagram as figure at {self.file_relative_path}{page.file.src_uri}')
                                 self.counter += 1
                                 markdown = markdown[:match.start() + position_offset] + replacement + markdown[match.end() + position_offset:]
```

### Comparing `mkdocs-table-of-figures-0.1.6/mkdocs_table_of_figures.egg-info/PKG-INFO` & `mkdocs-table-of-figures-0.1.7/mkdocs_table_of_figures.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.1.6
+Version: 0.1.7
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Description: # mkdocs-table-of-figures
         
@@ -84,14 +84,28 @@
             The title of the mermaid diagram go here
         ```
         
         It will not work if there is a line between the diagram and the title.
         
         I highly recommend using `mkdocs-material` to use `mermaid` diagrams. For more info about `mermaid` diagrams, I invite you to check `mkdocs-material` and `mermaid`'s official documentation.
         
+        I also recommend to add this stylesheet to prevent mermaid size from being reduced by mkdocs-material stylesheet in your `mkdocs.yml` at extra-css option
+        
+        ``` css
+        figure.figure-mermaid {
+            margin: 0 1em;
+            width: 100%;
+        }
+        ```
+        
+        ``` yml
+        extra_css:
+          - fix-mermaid-figure.css
+        ```
+        
         ## License
         
         This project is under MIT license. See the `license` file for more details.
         
         ## See Also
         
         - [GitLab Repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-annexes-integration/)
```

### Comparing `mkdocs-table-of-figures-0.1.6/readme.md` & `mkdocs-table-of-figures-0.1.7/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,28 @@
     The title of the mermaid diagram go here
 ```
 
 It will not work if there is a line between the diagram and the title.
 
 I highly recommend using `mkdocs-material` to use `mermaid` diagrams. For more info about `mermaid` diagrams, I invite you to check `mkdocs-material` and `mermaid`'s official documentation.
 
+I also recommend to add this stylesheet to prevent mermaid size from being reduced by mkdocs-material stylesheet in your `mkdocs.yml` at extra-css option
+
+``` css
+figure.figure-mermaid {
+    margin: 0 1em;
+    width: 100%;
+}
+```
+
+``` yml
+extra_css:
+  - fix-mermaid-figure.css
+```
+
 ## License
 
 This project is under MIT license. See the `license` file for more details.
 
 ## See Also
 
 - [GitLab Repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-annexes-integration/)
```

### Comparing `mkdocs-table-of-figures-0.1.6/setup.py` & `mkdocs-table-of-figures-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-table-of-figures',
-    version='0.1.6',
+    version='0.1.7',
     description='A MkDocs plugin listing all figures to create a table of figures page',
     long_description=io.open('readme.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs',
     url='https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures',
     author='Thibaud Briard',
     author_email='thibaud.brrd@eduge.ch',
```

