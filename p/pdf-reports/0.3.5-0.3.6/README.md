# Comparing `tmp/pdf_reports-0.3.5.tar.gz` & `tmp/pdf_reports-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_reports-0.3.5.tar", last modified: Fri Jul 21 22:25:37 2023, max compression
+gzip compressed data, was "pdf_reports-0.3.6.tar", last modified: Wed Apr 17 11:06:16 2024, max compression
```

## Comparing `pdf_reports-0.3.5.tar` & `pdf_reports-0.3.6.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-21 22:25:37.636816 pdf_reports-0.3.5/
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1081 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/LICENCE.txt
--rwxrwxr-x   0 peter     (1000) peter     (1000)       84 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/MANIFEST.in
--rw-rw-r--   0 peter     (1000) peter     (1000)     1888 2023-07-21 22:25:37.636816 pdf_reports-0.3.5/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     7102 2023-07-21 22:25:15.000000 pdf_reports-0.3.5/README.rst
--rwxrwxr-x   0 peter     (1000) peter     (1000)     8512 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/ez_setup.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-21 22:25:37.632816 pdf_reports-0.3.5/pdf_reports/
--rw-rw-r--   0 peter     (1000) peter     (1000)      239 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/pdf_reports/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-21 22:25:37.636816 pdf_reports-0.3.5/pdf_reports/css/
--rwxrwxr-x   0 peter     (1000) peter     (1000)    19352 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/pdf_reports/css/egf-logo.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)   618735 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/pdf_reports/css/semantic.min.css
--rw-rw-r--   0 peter     (1000) peter     (1000)     1502 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/pdf_reports/css/style.css
--rw-rw-r--   0 peter     (1000) peter     (1000)     6822 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/pdf_reports/pdf_reports.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5645 2023-07-21 22:25:15.000000 pdf_reports-0.3.5/pdf_reports/tools.py
--rw-rw-r--   0 peter     (1000) peter     (1000)       22 2023-07-21 22:25:15.000000 pdf_reports-0.3.5/pdf_reports/version.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-21 22:25:37.632816 pdf_reports-0.3.5/pdf_reports.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1888 2023-07-21 22:25:36.000000 pdf_reports-0.3.5/pdf_reports.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      428 2023-07-21 22:25:37.000000 pdf_reports-0.3.5/pdf_reports.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-21 22:25:37.000000 pdf_reports-0.3.5/pdf_reports.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       87 2023-07-21 22:25:37.000000 pdf_reports-0.3.5/pdf_reports.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       12 2023-07-21 22:25:37.000000 pdf_reports-0.3.5/pdf_reports.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)     1590 2023-07-21 22:25:15.000000 pdf_reports-0.3.5/pypi-readme.rst
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-21 22:25:37.636816 pdf_reports-0.3.5/setup.cfg
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1295 2023-07-21 22:25:15.000000 pdf_reports-0.3.5/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-17 11:06:16.018083 pdf_reports-0.3.6/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1081 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/LICENCE.txt
+-rwxrwxr-x   0 peter     (1000) peter     (1000)       84 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/MANIFEST.in
+-rw-r--r--   0 peter     (1000) peter     (1000)     2060 2024-04-17 11:06:16.014083 pdf_reports-0.3.6/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7294 2024-04-17 11:05:59.000000 pdf_reports-0.3.6/README.rst
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     8512 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/ez_setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-17 11:06:15.994084 pdf_reports-0.3.6/pdf_reports/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      239 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/pdf_reports/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-17 11:06:16.014083 pdf_reports-0.3.6/pdf_reports/css/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)    19352 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/pdf_reports/css/egf-logo.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)   618735 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/pdf_reports/css/semantic.min.css
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1502 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/pdf_reports/css/style.css
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6797 2024-04-17 11:05:59.000000 pdf_reports-0.3.6/pdf_reports/pdf_reports.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5656 2024-04-17 11:05:59.000000 pdf_reports-0.3.6/pdf_reports/tools.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)       22 2024-04-17 11:05:59.000000 pdf_reports-0.3.6/pdf_reports/version.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-17 11:06:16.014083 pdf_reports-0.3.6/pdf_reports.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2060 2024-04-17 11:06:12.000000 pdf_reports-0.3.6/pdf_reports.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      469 2024-04-17 11:06:12.000000 pdf_reports-0.3.6/pdf_reports.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2024-04-17 11:06:12.000000 pdf_reports-0.3.6/pdf_reports.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       87 2024-04-17 11:06:12.000000 pdf_reports-0.3.6/pdf_reports.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       12 2024-04-17 11:06:12.000000 pdf_reports-0.3.6/pdf_reports.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1590 2023-07-21 22:25:15.000000 pdf_reports-0.3.6/pypi-readme.rst
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2024-04-17 11:06:16.018083 pdf_reports-0.3.6/setup.cfg
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1326 2024-04-17 11:05:59.000000 pdf_reports-0.3.6/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-17 11:06:16.014083 pdf_reports-0.3.6/tests/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2272 2024-04-17 11:05:59.000000 pdf_reports-0.3.6/tests/test_basics.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1067 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/tests/test_tools.py
```

### Comparing `pdf_reports-0.3.5/LICENCE.txt` & `pdf_reports-0.3.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.5/PKG-INFO` & `pdf_reports-0.3.6/pypi-readme.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: pdf_reports
-Version: 0.3.5
-Summary: Create nice-looking PDF reports from HTML content.
-Home-page: https://github.com/Edinburgh-Genome-Foundry/pdf_reports
-Author: Zulko
-License: MIT
-Keywords: PDF report web jinja weasyprint
-Platform: UNKNOWN
-License-File: LICENCE.txt
-
 PDF Reports
 ===========
 
 *PDF Reports* (complete documentation `here <https://edinburgh-genome-foundry.github.io/pdf_reports/>`_) is a Python library to create nice-looking PDF reports from HTML or `Pug <https://pugjs.org>`_ templates. It features modern-looking components (via the `Semantic UI <https://semantic-ui.com/>`_ framework) and provides routines to embed tables or plots in the documents.
 
 
 Example of use
@@ -60,9 +49,7 @@
 `<https://github.com/Edinburgh-Genome-Foundry/pdf_reports>`_
 
 **Live demo:**
 
 `<http://cuba.genomefoundry.org/sculpt_a_sequence>`_
 
 **License:** MIT, Copyright Edinburgh Genome Foundry
-
-
```

### Comparing `pdf_reports-0.3.5/README.rst` & `pdf_reports-0.3.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,17 @@
 
     <p align="center">
     <img alt="PDF Reports Logo" title="PDF Reports" src="https://raw.githubusercontent.com/Edinburgh-Genome-Foundry/pdf_reports/master/docs/_static/images/title.png" width="350">
     <br /><br />
     </p>
 
 
-PDF_Reports
-===========
-
 .. image:: https://github.com/Edinburgh-Genome-Foundry/pdf_reports/actions/workflows/build.yml/badge.svg
    :target: https://github.com/Edinburgh-Genome-Foundry/pdf_reports/actions/workflows/build.yml
    :alt: GitHub CI build status
-
 .. image:: https://coveralls.io/repos/github/Edinburgh-Genome-Foundry/pdf_reports/badge.svg?branch=master
    :target: https://coveralls.io/github/Edinburgh-Genome-Foundry/pdf_reports?branch=master
 
 
 
 *PDF Reports* (complete documentation `here <https://edinburgh-genome-foundry.github.io/pdf_reports/>`_) is a Python library to create nice-looking PDF reports from HTML or `Pug <https://pugjs.org>`_ templates. It features modern-looking components (via the `Semantic UI <https://semantic-ui.com/>`_ framework) and provides routines to embed tables or plots in the documents.
 
@@ -173,17 +169,19 @@
 .. code::
 
     python setup.py install
 
 **Note:** the package depends on the WeasyPrint Python package. If there are any issues,
 see installation instructions in the `WeasyPrint documentation <https://doc.courtbouillon.org/weasyprint/stable/first_steps.html>`_.
 
-If you have an older GNU/Linux distribution (e.g. Ubuntu 18.04), then install an older WeasyPrint (<=52),
-as they don't have the latest Pango that is required by the latest WeasyPrint: ``pip install weasyprint==52``
+If Pango is not available in your conda environment (``which pango-view``), but otherwise it's installed, then install it with ``conda install anaconda::pango``
+
 
+PDF Reports has been tested on Ubuntu 22.04. If you have an older GNU/Linux distribution (e.g. Ubuntu 18.04) which
+doesn't have the latest Pango that is required by the latest WeasyPrint, then installing an older WeasyPrint (<=52) may help: ``pip install weasyprint==52``
 
 **Note: on some Debian systems** you may need to first install ``libffi-dev`` (``apt install libffi-dev``). The package name may be ``libffi-devel`` on some systems.
 
 **Note: on macOS,** you may need to first install pango with: ``brew install pango``
 
 
 License = MIT
```

### Comparing `pdf_reports-0.3.5/ez_setup.py` & `pdf_reports-0.3.6/ez_setup.py`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.5/pdf_reports/css/egf-logo.svg` & `pdf_reports-0.3.6/pdf_reports/css/egf-logo.svg`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.5/pdf_reports/css/semantic.min.css` & `pdf_reports-0.3.6/pdf_reports/css/semantic.min.css`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.5/pdf_reports/css/style.css` & `pdf_reports-0.3.6/pdf_reports/css/style.css`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.5/pdf_reports/pdf_reports.py` & `pdf_reports-0.3.6/pdf_reports/pdf_reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,15 @@
         "properly! You will not be able to generate PDF reports until"
         "you fix this issue.\n"
     )
 
     if "pango" in str(err):
         message += (
             "\nMaybe you haven't installed the Pango dependency? "
-            "('brew install pango' on Mac, 'apt install libpango' "
-            "on Ubuntu).\n"
+            "See PDF Reports install instructions in documentation.\n"
         )
     if "cairo" in str(err):
         message += "\nMaybe you haven't installed the Cairo dependency?\n"
 
     message += (
         "\nIn any other case the weasyprint docs may be able to help:\n\n"
         "http://weasyprint.readthedocs.io/en/stable/install.html#windows\n\n"
```

### Comparing `pdf_reports-0.3.5/pdf_reports/tools.py` & `pdf_reports-0.3.6/pdf_reports/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     bbox_inches
       Keeping this option to "tight" will ensure that your plot's delimitation
       is optimal.
 
     **kwargs
       Any other option of Matplotlib's figure.savefig() method.
     """
-    if isinstance(fig, Axes):
+    if fig.__class__.__name__ == "Axes":
         fig = fig.figure
     output = BytesIO()
     original_size = fig.get_size_inches()
     if size is not None:
         fig.set_size_inches((int(size[0]), int(size[1])))
     fig.savefig(output, format=fmt, bbox_inches=bbox_inches, **kwargs)
     fig.set_size_inches(original_size)
```

### Comparing `pdf_reports-0.3.5/pdf_reports.egg-info/PKG-INFO` & `pdf_reports-0.3.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
-Name: pdf-reports
-Version: 0.3.5
+Name: pdf_reports
+Version: 0.3.6
 Summary: Create nice-looking PDF reports from HTML content.
 Home-page: https://github.com/Edinburgh-Genome-Foundry/pdf_reports
 Author: Zulko
 License: MIT
 Keywords: PDF report web jinja weasyprint
-Platform: UNKNOWN
 License-File: LICENCE.txt
+Requires-Dist: pypugjs
+Requires-Dist: jinja2
+Requires-Dist: weasyprint
+Requires-Dist: beautifulsoup4
+Requires-Dist: pandas
+Requires-Dist: Markdown
+Requires-Dist: backports.functools-lru-cache
 
 PDF Reports
 ===========
 
 *PDF Reports* (complete documentation `here <https://edinburgh-genome-foundry.github.io/pdf_reports/>`_) is a Python library to create nice-looking PDF reports from HTML or `Pug <https://pugjs.org>`_ templates. It features modern-looking components (via the `Semantic UI <https://semantic-ui.com/>`_ framework) and provides routines to embed tables or plots in the documents.
 
 
@@ -60,9 +66,7 @@
 `<https://github.com/Edinburgh-Genome-Foundry/pdf_reports>`_
 
 **Live demo:**
 
 `<http://cuba.genomefoundry.org/sculpt_a_sequence>`_
 
 **License:** MIT, Copyright Edinburgh Genome Foundry
-
-
```

### Comparing `pdf_reports-0.3.5/pypi-readme.rst` & `pdf_reports-0.3.6/pdf_reports.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: pdf_reports
+Version: 0.3.6
+Summary: Create nice-looking PDF reports from HTML content.
+Home-page: https://github.com/Edinburgh-Genome-Foundry/pdf_reports
+Author: Zulko
+License: MIT
+Keywords: PDF report web jinja weasyprint
+License-File: LICENCE.txt
+Requires-Dist: pypugjs
+Requires-Dist: jinja2
+Requires-Dist: weasyprint
+Requires-Dist: beautifulsoup4
+Requires-Dist: pandas
+Requires-Dist: Markdown
+Requires-Dist: backports.functools-lru-cache
+
 PDF Reports
 ===========
 
 *PDF Reports* (complete documentation `here <https://edinburgh-genome-foundry.github.io/pdf_reports/>`_) is a Python library to create nice-looking PDF reports from HTML or `Pug <https://pugjs.org>`_ templates. It features modern-looking components (via the `Semantic UI <https://semantic-ui.com/>`_ framework) and provides routines to embed tables or plots in the documents.
 
 
 Example of use
```

### Comparing `pdf_reports-0.3.5/setup.py` & `pdf_reports-0.3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,21 @@
             " neither setuptools nor ez_setup are installed on"
             "this computer. \nInstall ez_setup "
             "([sudo] pip install ez_setup) and try again."
         )
 
 from setuptools import setup, find_packages
 
-exec(open("pdf_reports/version.py").read())  # loads __version__
+version = {}
+with open("pdf_reports/version.py") as fp:
+    exec(fp.read(), version)
 
 setup(
     name="pdf_reports",
-    version=__version__,
+    version=version["__version__"],
     author="Zulko",
     url="https://github.com/Edinburgh-Genome-Foundry/pdf_reports",
     description="Create nice-looking PDF reports from HTML content.",
     long_description=open("pypi-readme.rst").read(),
     license="MIT",
     keywords="PDF report web jinja weasyprint",
     packages=find_packages(exclude="docs"),
```

