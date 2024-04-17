# Comparing `tmp/ms2rescore-3.1.0.dev2.tar.gz` & `tmp/ms2rescore-3.1.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms2rescore-3.1.0.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ms2rescore-3.1.0.dev3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ms2rescore-3.1.0.dev2.tar` & `ms2rescore-3.1.0.dev3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    11357 2024-04-10 13:42:16.821182 ms2rescore-3.1.0.dev2/LICENSE
--rw-r--r--   0        0        0     6477 2024-04-10 13:42:16.821182 ms2rescore-3.1.0.dev2/README.md
--rw-r--r--   0        0        0      458 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/__init__.py
--rw-r--r--   0        0        0     5876 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/__main__.py
--rw-r--r--   0        0        0     5957 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/config_parser.py
--rw-r--r--   0        0        0     9229 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/core.py
--rw-r--r--   0        0        0      633 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/exceptions.py
--rw-r--r--   0        0        0      803 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/__init__.py
--rw-r--r--   0        0        0      522 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/base.py
--rw-r--r--   0        0        0     3436 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/basic.py
--rw-r--r--   0        0        0    10496 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/deeplc.py
--rw-r--r--   0        0        0     6261 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/im2deep.py
--rw-r--r--   0        0        0    10740 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/ionmob.py
--rw-r--r--   0        0        0     7069 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/maxquant.py
--rw-r--r--   0        0        0    17272 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/ms2pip.py
--rw-r--r--   0        0        0        0 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/gui/__init__.py
--rw-r--r--   0        0        0      419 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/gui/__main__.py
--rw-r--r--   0        0        0    25980 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/gui/app.py
--rw-r--r--   0        0        0    11797 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/gui/function2ctk.py
--rw-r--r--   0        0        0    14890 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/gui/widgets.py
--rw-r--r--   0        0        0        0 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/package_data/__init__.py
--rw-r--r--   0        0        0     1154 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/package_data/config_default.json
--rw-r--r--   0        0        0      601 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/package_data/config_default_tims.json
--rw-r--r--   0        0        0    12404 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/package_data/config_schema.json
--rw-r--r--   0        0        0        0 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/__init__.py
--rw-r--r--   0        0        0 44669194 2024-04-10 13:42:17.029183 ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/config_icon.png
--rw-r--r--   0        0        0     4837 2024-04-10 13:42:17.029183 ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/github-mark-white.png
--rw-r--r--   0        0        0     5557 2024-04-10 13:42:17.029183 ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/github-mark.png
--rw-r--r--   0        0        0    52066 2024-04-10 13:42:17.029183 ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/ms2rescore_logo.png
--rw-r--r--   0        0        0    43034 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/program_icon.ico
--rw-r--r--   0        0        0     5068 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/package_data/ms2rescore-gui-theme.json
--rw-r--r--   0        0        0     7974 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/parse_psms.py
--rw-r--r--   0        0        0     1935 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/parse_spectra.py
--rw-r--r--   0        0        0      138 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/__init__.py
--rw-r--r--   0        0        0      614 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/__main__.py
--rw-r--r--   0        0        0    18673 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/charts.py
--rw-r--r--   0        0        0    14787 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/generate.py
--rw-r--r--   0        0        0        0 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/__init__.py
--rw-r--r--   0        0        0     1677 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/about.html
--rw-r--r--   0        0        0     3182 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/base.html
--rw-r--r--   0        0        0      107 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/config.html
--rw-r--r--   0        0        0      138 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/features.html
--rw-r--r--   0        0        0       22 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/log.html
--rw-r--r--   0        0        0      559 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/metadata.html
--rw-r--r--   0        0        0      341 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/overview.html
--rw-r--r--   0        0        0      831 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/stats-card.html
--rw-r--r--   0        0        0     1904 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/style.html
--rw-r--r--   0        0        0      138 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/target-decoy.html
--rw-r--r--   0        0        0     5189 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/texts.toml
--rw-r--r--   0        0        0     2804 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/utils.py
--rw-r--r--   0        0        0      302 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/rescoring_engines/__init__.py
--rw-r--r--   0        0        0     8809 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/rescoring_engines/mokapot.py
--rw-r--r--   0        0        0     8207 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/rescoring_engines/percolator.py
--rw-r--r--   0        0        0     3717 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/utils.py
--rw-r--r--   0        0        0     2680 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     9028 1970-01-01 00:00:00.000000 ms2rescore-3.1.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-17 15:17:02.421019 ms2rescore-3.1.0.dev3/LICENSE
+-rw-r--r--   0        0        0     6477 2024-04-17 15:17:02.421019 ms2rescore-3.1.0.dev3/README.md
+-rw-r--r--   0        0        0      458 2024-04-17 15:17:02.473019 ms2rescore-3.1.0.dev3/ms2rescore/__init__.py
+-rw-r--r--   0        0        0     6608 2024-04-17 15:17:02.473019 ms2rescore-3.1.0.dev3/ms2rescore/__main__.py
+-rw-r--r--   0        0        0     5957 2024-04-17 15:17:02.473019 ms2rescore-3.1.0.dev3/ms2rescore/config_parser.py
+-rw-r--r--   0        0        0     9229 2024-04-17 15:17:02.473019 ms2rescore-3.1.0.dev3/ms2rescore/core.py
+-rw-r--r--   0        0        0      633 2024-04-17 15:17:02.473019 ms2rescore-3.1.0.dev3/ms2rescore/exceptions.py
+-rw-r--r--   0        0        0      803 2024-04-17 15:17:02.473019 ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/__init__.py
+-rw-r--r--   0        0        0      522 2024-04-17 15:17:02.473019 ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/base.py
+-rw-r--r--   0        0        0     3436 2024-04-17 15:17:02.473019 ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/basic.py
+-rw-r--r--   0        0        0    10496 2024-04-17 15:17:02.477019 ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/deeplc.py
+-rw-r--r--   0        0        0     6261 2024-04-17 15:17:02.477019 ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/im2deep.py
+-rw-r--r--   0        0        0    10740 2024-04-17 15:17:02.477019 ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/ionmob.py
+-rw-r--r--   0        0        0     7069 2024-04-17 15:17:02.477019 ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/maxquant.py
+-rw-r--r--   0        0        0    17272 2024-04-17 15:17:02.477019 ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/ms2pip.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:17:02.477019 ms2rescore-3.1.0.dev3/ms2rescore/gui/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-17 15:17:02.477019 ms2rescore-3.1.0.dev3/ms2rescore/gui/__main__.py
+-rw-r--r--   0        0        0    25980 2024-04-17 15:17:02.477019 ms2rescore-3.1.0.dev3/ms2rescore/gui/app.py
+-rw-r--r--   0        0        0    11797 2024-04-17 15:17:02.477019 ms2rescore-3.1.0.dev3/ms2rescore/gui/function2ctk.py
+-rw-r--r--   0        0        0    14890 2024-04-17 15:17:02.477019 ms2rescore-3.1.0.dev3/ms2rescore/gui/widgets.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:17:02.477019 ms2rescore-3.1.0.dev3/ms2rescore/package_data/__init__.py
+-rw-r--r--   0        0        0     1154 2024-04-17 15:17:02.477019 ms2rescore-3.1.0.dev3/ms2rescore/package_data/config_default.json
+-rw-r--r--   0        0        0      601 2024-04-17 15:17:02.477019 ms2rescore-3.1.0.dev3/ms2rescore/package_data/config_default_tims.json
+-rw-r--r--   0        0        0    12615 2024-04-17 15:17:02.477019 ms2rescore-3.1.0.dev3/ms2rescore/package_data/config_schema.json
+-rw-r--r--   0        0        0        0 2024-04-17 15:17:02.477019 ms2rescore-3.1.0.dev3/ms2rescore/package_data/img/__init__.py
+-rw-r--r--   0        0        0 44669194 2024-04-17 15:17:02.629019 ms2rescore-3.1.0.dev3/ms2rescore/package_data/img/config_icon.png
+-rw-r--r--   0        0        0     4837 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/package_data/img/github-mark-white.png
+-rw-r--r--   0        0        0     5557 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/package_data/img/github-mark.png
+-rw-r--r--   0        0        0    52066 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/package_data/img/ms2rescore_logo.png
+-rw-r--r--   0        0        0    43034 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/package_data/img/program_icon.ico
+-rw-r--r--   0        0        0     5068 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/package_data/ms2rescore-gui-theme.json
+-rw-r--r--   0        0        0     7974 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/parse_psms.py
+-rw-r--r--   0        0        0     1935 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/parse_spectra.py
+-rw-r--r--   0        0        0      138 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/__init__.py
+-rw-r--r--   0        0        0      614 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/__main__.py
+-rw-r--r--   0        0        0    18673 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/charts.py
+-rw-r--r--   0        0        0    14787 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/generate.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/templates/__init__.py
+-rw-r--r--   0        0        0     1677 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/templates/about.html
+-rw-r--r--   0        0        0     3182 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/templates/base.html
+-rw-r--r--   0        0        0      107 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/templates/config.html
+-rw-r--r--   0        0        0      138 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/templates/features.html
+-rw-r--r--   0        0        0       22 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/templates/log.html
+-rw-r--r--   0        0        0      559 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/templates/metadata.html
+-rw-r--r--   0        0        0      341 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/templates/overview.html
+-rw-r--r--   0        0        0      831 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/templates/stats-card.html
+-rw-r--r--   0        0        0     1904 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/templates/style.html
+-rw-r--r--   0        0        0      138 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/templates/target-decoy.html
+-rw-r--r--   0        0        0     5189 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/templates/texts.toml
+-rw-r--r--   0        0        0     2804 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/report/utils.py
+-rw-r--r--   0        0        0      302 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/rescoring_engines/__init__.py
+-rw-r--r--   0        0        0     9524 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/rescoring_engines/mokapot.py
+-rw-r--r--   0        0        0     8207 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/rescoring_engines/percolator.py
+-rw-r--r--   0        0        0     3717 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/ms2rescore/utils.py
+-rw-r--r--   0        0        0     2680 2024-04-17 15:17:02.633019 ms2rescore-3.1.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     9028 1970-01-01 00:00:00.000000 ms2rescore-3.1.0.dev3/PKG-INFO
```

### Comparing `ms2rescore-3.1.0.dev2/LICENSE` & `ms2rescore-3.1.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/README.md` & `ms2rescore-3.1.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/__main__.py` & `ms2rescore-3.1.0.dev3/ms2rescore/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """MS²Rescore: Sensitive PSM rescoring with predicted MS² peak intensities and RTs."""
 
 import argparse
+import cProfile
 import importlib.resources
 import json
 import logging
 import sys
 from pathlib import Path
 from typing import Union
 
@@ -135,14 +136,22 @@
         "--fasta-file",
         metavar="FILE",
         action="store",
         type=str,
         dest="fasta_file",
         help="path to FASTA file",
     )
+    parser.add_argument(
+        "--profile",
+        # metavar="BOOL",
+        action="store_true",
+        # type=bool,
+        # dest="profile",
+        help="boolean to enable profiling with cProfile",
+    )
 
     return parser
 
 
 def _setup_logging(passed_level: str, log_file: Union[str, Path]):
     """Setup logging for writing to log file and Rich Console."""
     if passed_level not in LOG_MAPPING:
@@ -157,14 +166,26 @@
         handlers=[
             logging.FileHandler(log_file, mode="w", encoding="utf-8"),
             RichHandler(rich_tracebacks=True, console=CONSOLE, show_path=False),
         ],
     )
 
 
+def profile(fnc, filepath):
+    """A decorator that uses cProfile to profile a function"""
+
+    def inner(*args, **kwargs):
+        with cProfile.Profile() as profiler:
+            return_value = fnc(*args, **kwargs)
+        profiler.dump_stats(filepath + ".profile.prof")
+        return return_value
+
+    return inner
+
+
 def main_tims():
     """Run MS²Rescore command-line interface in TIMS²Rescore mode."""
     main(tims=True)
 
 
 def main(tims=False):
     """Run MS²Rescore command-line interface."""
@@ -192,15 +213,19 @@
     # Setup logging
     _setup_logging(
         config["ms2rescore"]["log_level"], config["ms2rescore"]["output_path"] + ".log.txt"
     )
 
     # Run MS²Rescore
     try:
-        rescore(configuration=config)
+        if cli_args.profile:
+            profiled_rescore = profile(rescore, config["ms2rescore"]["output_path"])
+            profiled_rescore(configuration=config)
+        else:
+            rescore(configuration=config)
     except Exception as e:
         LOGGER.exception(e)
         sys.exit(1)
     finally:
         CONSOLE.save_html(config["ms2rescore"]["output_path"] + ".log.html")
```

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/config_parser.py` & `ms2rescore-3.1.0.dev3/ms2rescore/config_parser.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/core.py` & `ms2rescore-3.1.0.dev3/ms2rescore/core.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/exceptions.py` & `ms2rescore-3.1.0.dev3/ms2rescore/exceptions.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/__init__.py` & `ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/base.py` & `ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/base.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/basic.py` & `ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/basic.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/deeplc.py` & `ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/deeplc.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/im2deep.py` & `ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/im2deep.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/ionmob.py` & `ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/ionmob.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/maxquant.py` & `ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/maxquant.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/ms2pip.py` & `ms2rescore-3.1.0.dev3/ms2rescore/feature_generators/ms2pip.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/gui/app.py` & `ms2rescore-3.1.0.dev3/ms2rescore/gui/app.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/gui/function2ctk.py` & `ms2rescore-3.1.0.dev3/ms2rescore/gui/function2ctk.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/gui/widgets.py` & `ms2rescore-3.1.0.dev3/ms2rescore/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/package_data/config_default.json` & `ms2rescore-3.1.0.dev3/ms2rescore/package_data/config_default.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/package_data/config_default_tims.json` & `ms2rescore-3.1.0.dev3/ms2rescore/package_data/config_default_tims.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/package_data/config_schema.json` & `ms2rescore-3.1.0.dev3/ms2rescore/package_data/config_schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998106060606061%*

 * *Differences: {"'properties'": "{'ms2rescore': {'properties': {'profile': OrderedDict([('description', 'Write an "*

 * *                 "txt report using cProfile for profiling'), ('type', 'boolean'), ('default', "*

 * *                 'False)])}}}'}*

```diff
@@ -258,14 +258,19 @@
                 "processes": {
                     "default": -1,
                     "description": "Number of parallel processes to use; -1 for all available",
                     "minimum": -1,
                     "multipleOf": 1,
                     "type": "number"
                 },
+                "profile": {
+                    "default": false,
+                    "description": "Write an txt report using cProfile for profiling",
+                    "type": "boolean"
+                },
                 "psm_file": {
                     "description": "Path to file with peptide-spectrum matches.",
                     "oneOf": [
                         {
                             "type": "string"
                         },
                         {
```

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/config_icon.png` & `ms2rescore-3.1.0.dev3/ms2rescore/package_data/img/config_icon.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/github-mark-white.png` & `ms2rescore-3.1.0.dev3/ms2rescore/package_data/img/github-mark-white.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/github-mark.png` & `ms2rescore-3.1.0.dev3/ms2rescore/package_data/img/github-mark.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/ms2rescore_logo.png` & `ms2rescore-3.1.0.dev3/ms2rescore/package_data/img/ms2rescore_logo.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/program_icon.ico` & `ms2rescore-3.1.0.dev3/ms2rescore/package_data/img/program_icon.ico`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/package_data/ms2rescore-gui-theme.json` & `ms2rescore-3.1.0.dev3/ms2rescore/package_data/ms2rescore-gui-theme.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/parse_psms.py` & `ms2rescore-3.1.0.dev3/ms2rescore/parse_psms.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/parse_spectra.py` & `ms2rescore-3.1.0.dev3/ms2rescore/parse_spectra.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/report/__main__.py` & `ms2rescore-3.1.0.dev3/ms2rescore/report/__main__.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/report/charts.py` & `ms2rescore-3.1.0.dev3/ms2rescore/report/charts.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/report/generate.py` & `ms2rescore-3.1.0.dev3/ms2rescore/report/generate.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/report/templates/about.html` & `ms2rescore-3.1.0.dev3/ms2rescore/report/templates/about.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/report/templates/base.html` & `ms2rescore-3.1.0.dev3/ms2rescore/report/templates/base.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/report/templates/metadata.html` & `ms2rescore-3.1.0.dev3/ms2rescore/report/templates/metadata.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/report/templates/stats-card.html` & `ms2rescore-3.1.0.dev3/ms2rescore/report/templates/stats-card.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/report/templates/style.html` & `ms2rescore-3.1.0.dev3/ms2rescore/report/templates/style.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/report/templates/texts.toml` & `ms2rescore-3.1.0.dev3/ms2rescore/report/templates/texts.toml`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/report/utils.py` & `ms2rescore-3.1.0.dev3/ms2rescore/report/utils.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/rescoring_engines/mokapot.py` & `ms2rescore-3.1.0.dev3/ms2rescore/rescoring_engines/mokapot.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,16 @@
    Fondrie W. E. & Noble W. S. mokapot: Fast and Flexible Semisupervised
    Learning for Peptide Detection. *J Proteome Res* (2021).
    `doi:10.1021/acs.jproteome.0c01010 <https://doi.org/10.1021/acs.jproteome.0c01010>`_
 
 """
 
 import logging
-from typing import Any, List, Optional, Tuple, Dict
+import re
+from typing import Any, Dict, List, Optional, Tuple
 
 import mokapot
 import numpy as np
 import pandas as pd
 import psm_utils
 from mokapot.brew import brew
 from mokapot.dataset import LinearPsmDataset
@@ -89,33 +90,50 @@
         lin_psm_data.add_proteins(fasta_file, **protein_kwargs)
 
     # Rescore
     logger.debug(f"Mokapot brew options: `{kwargs}`")
     confidence_results, models = brew(lin_psm_data, rng=8, **kwargs)
 
     # Reshape confidence estimates to match PSMList
+    keys = ["mokapot score", "mokapot q-value", "mokapot PEP"]
     mokapot_values_targets = (
-        confidence_results.confidence_estimates["psms"]
-        .set_index("index")
-        .sort_index()[["mokapot score", "mokapot q-value", "mokapot PEP"]]
+        confidence_results.confidence_estimates["psms"].set_index("index").sort_index()[keys]
     )
     mokapot_values_decoys = (
-        confidence_results.decoy_confidence_estimates["psms"]
-        .set_index("index")
-        .sort_index()[["mokapot score", "mokapot q-value", "mokapot PEP"]]
+        confidence_results.decoy_confidence_estimates["psms"].set_index("index").sort_index()[keys]
     )
     q = np.full((len(psm_list), 3), np.nan)
     q[mokapot_values_targets.index] = mokapot_values_targets.values
     q[mokapot_values_decoys.index] = mokapot_values_decoys.values
 
     # Add Mokapot results to PSMList
     psm_list["score"] = q[:, 0]
     psm_list["qvalue"] = q[:, 1]
     psm_list["pep"] = q[:, 2]
 
+    # Repeat for peptide-level scores
+    peptide_info = pd.concat(
+        [
+            confidence_results.confidence_estimates["peptides"].set_index(["peptide"])[keys],
+            confidence_results.decoy_confidence_estimates["peptides"].set_index(["peptide"])[keys],
+        ],
+        axis=0,
+    ).to_dict(orient="index")
+
+    peptidoform_without_charge = re.compile(r"(/\d+$)")
+    for psm in psm_list:
+        peptide_scores = peptide_info[peptidoform_without_charge.sub("", str(psm.peptidoform), 1)]
+        psm.metadata.update(
+            {
+                "peptide_score": peptide_scores["mokapot score"],
+                "peptide_qvalue": peptide_scores["mokapot q-value"],
+                "peptide_pep": peptide_scores["mokapot PEP"],
+            }
+        )
+
     # Write results
     if write_weights:
         try:
             save_model_weights(models, feature_names, output_file_root)
         except AttributeError:
             logger.warning(
                 "Could not extract Mokapot model weights with the `coef_` attribute. Most likely, "
@@ -170,15 +188,15 @@
     ]
     feature_df = pd.DataFrame(list(psm_df["rescoring_features"])).astype(float).fillna(0.0)
     feature_df.columns = [f"feature:{f}" for f in feature_df.columns]
     combined_df = pd.concat([psm_df[required_columns], feature_df], axis=1)
 
     # Ensure filename for FlashLFQ txt output
     if not combined_df["run"].notnull().all():
-        combined_df["run"] = "ms_run"
+        combined_df["run"] = "nan"
 
     feature_names = [f"feature:{f}" for f in feature_names] if feature_names else None
 
     lin_psm_data = LinearPsmDataset(
         psms=combined_df,
         target_column="is_target",
         spectrum_columns="index",  # Use artificial index to allow multi-rank rescoring
```

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/rescoring_engines/percolator.py` & `ms2rescore-3.1.0.dev3/ms2rescore/rescoring_engines/percolator.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/ms2rescore/utils.py` & `ms2rescore-3.1.0.dev3/ms2rescore/utils.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/pyproject.toml` & `ms2rescore-3.1.0.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev2/PKG-INFO` & `ms2rescore-3.1.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2rescore
-Version: 3.1.0.dev2
+Version: 3.1.0.dev3
 Summary: MS²Rescore: Sensitive PSM rescoring with predicted MS² peak intensities and retention times.
 Keywords: MS2Rescore,MS2PIP,DeepLC,Percolator,proteomics,mass spectrometry,peptide identification,rescoring,machine learning
 Author: Ana Sílvia C. Silva, Robbin Bouwmeester, Louise Buur
 Author-email: Ralf Gabriels <ralf@gabriels.dev>, Arthur Declercq <arthur.declercq@ugent.be>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
```

