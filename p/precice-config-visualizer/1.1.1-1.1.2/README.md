# Comparing `tmp/precice-config-visualizer-1.1.1.tar.gz` & `tmp/precice_config_visualizer-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precice-config-visualizer-1.1.1.tar", last modified: Fri Apr 12 06:58:52 2024, max compression
+gzip compressed data, was "precice_config_visualizer-1.1.2.tar", last modified: Wed Apr 17 08:25:13 2024, max compression
```

## Comparing `precice-config-visualizer-1.1.1.tar` & `precice_config_visualizer-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:58:52.591658 precice-config-visualizer-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 06:58:42.000000 precice-config-visualizer-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-12 06:58:52.591658 precice-config-visualizer-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-12 06:58:42.000000 precice-config-visualizer-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:58:52.591658 precice-config-visualizer-1.1.1/precice_config_visualizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-12 06:58:52.000000 precice-config-visualizer-1.1.1/precice_config_visualizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-12 06:58:52.000000 precice-config-visualizer-1.1.1/precice_config_visualizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:58:52.000000 precice-config-visualizer-1.1.1/precice_config_visualizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 06:58:52.000000 precice-config-visualizer-1.1.1/precice_config_visualizer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 06:58:52.000000 precice-config-visualizer-1.1.1/precice_config_visualizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 06:58:52.000000 precice-config-visualizer-1.1.1/precice_config_visualizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:58:52.591658 precice-config-visualizer-1.1.1/preciceconfigvisualizer/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2462 2024-04-12 06:58:42.000000 precice-config-visualizer-1.1.1/preciceconfigvisualizer/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15627 2024-04-12 06:58:42.000000 precice-config-visualizer-1.1.1/preciceconfigvisualizer/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-12 06:58:42.000000 precice-config-visualizer-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 06:58:52.591658 precice-config-visualizer-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 06:58:42.000000 precice-config-visualizer-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:25:13.175918 precice_config_visualizer-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 08:25:01.000000 precice_config_visualizer-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-17 08:25:13.175918 precice_config_visualizer-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-17 08:25:01.000000 precice_config_visualizer-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:25:13.175918 precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-17 08:25:13.000000 precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-17 08:25:13.000000 precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:25:13.000000 precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 08:25:13.000000 precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-17 08:25:13.000000 precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 08:25:13.000000 precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:25:13.175918 precice_config_visualizer-1.1.2/preciceconfigvisualizer/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2452 2024-04-17 08:25:01.000000 precice_config_visualizer-1.1.2/preciceconfigvisualizer/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15627 2024-04-17 08:25:01.000000 precice_config_visualizer-1.1.2/preciceconfigvisualizer/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-17 08:25:01.000000 precice_config_visualizer-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:25:13.175918 precice_config_visualizer-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:25:01.000000 precice_config_visualizer-1.1.2/setup.py
```

### Comparing `precice-config-visualizer-1.1.1/LICENSE` & `precice_config_visualizer-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-1.1.1/PKG-INFO` & `precice_config_visualizer-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precice-config-visualizer
-Version: 1.1.1
+Version: 1.1.2
 Summary: A tool for visualizing a preCICE configuration file as a dot file.
 Author-email: The preCICE Developers <info@precice.org>
 Maintainer-email: Frédéric Simonis <frederic.simonis@ipvs.uni-stuttgart.de>
 License: GPLv3
 Project-URL: Homepage, https://precice.org
 Project-URL: Documentation, https://precice.org/tooling-config-visualization.html
 Project-URL: Repository, https://github.com/precice/config-visualizer.git
```

### Comparing `precice-config-visualizer-1.1.1/README.md` & `precice_config_visualizer-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-1.1.1/precice_config_visualizer.egg-info/PKG-INFO` & `precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precice-config-visualizer
-Version: 1.1.1
+Version: 1.1.2
 Summary: A tool for visualizing a preCICE configuration file as a dot file.
 Author-email: The preCICE Developers <info@precice.org>
 Maintainer-email: Frédéric Simonis <frederic.simonis@ipvs.uni-stuttgart.de>
 License: GPLv3
 Project-URL: Homepage, https://precice.org
 Project-URL: Documentation, https://precice.org/tooling-config-visualization.html
 Project-URL: Repository, https://github.com/precice/config-visualizer.git
```

### Comparing `precice-config-visualizer-1.1.1/preciceconfigvisualizer/cli.py` & `precice_config_visualizer-1.1.2/preciceconfigvisualizer/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 def parse_args():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-o",
         "--outfile",
         nargs="?",
-        type=argparse.FileType("wb"),
+        type=argparse.FileType("w"),
         default=sys.stdout,
         help=f"The output file. Files with extensions {', '.join(SUPPORTED_FORMATS)} will be rendered using graphviz. Omit to output dot to stdout.",
     )
     displayChoices = ["full", "merged", "hide"]
     parser.add_argument(
         "--data-access",
         choices=displayChoices,
@@ -82,12 +82,12 @@
     dot = configFileToDotCode(args.infile, **vars(args))
 
     ext = os.path.splitext(args.outfile.name)[1].lower().lstrip(".")
     if ext in SUPPORTED_FORMATS:
         g = pydot.graph_from_dot_data(dot)[0]
         args.outfile.write(g.create(format=ext))
     else:
-        args.outfile.write(dot.encode())
+        args.outfile.write(dot)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `precice-config-visualizer-1.1.1/preciceconfigvisualizer/common.py` & `precice_config_visualizer-1.1.2/preciceconfigvisualizer/common.py`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-1.1.1/pyproject.toml` & `precice_config_visualizer-1.1.2/pyproject.toml`

 * *Files identical despite different names*

