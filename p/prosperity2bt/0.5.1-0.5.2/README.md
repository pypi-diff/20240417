# Comparing `tmp/prosperity2bt-0.5.1.tar.gz` & `tmp/prosperity2bt-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.5.1.tar", last modified: Tue Apr 16 13:36:55 2024, max compression
+gzip compressed data, was "prosperity2bt-0.5.2.tar", last modified: Tue Apr 16 15:57:27 2024, max compression
```

## Comparing `prosperity2bt-0.5.1.tar` & `prosperity2bt-0.5.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:55.012262 prosperity2bt-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-16 13:36:55.012262 prosperity2bt-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:54.992262 prosperity2bt-0.5.1/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:54.992262 prosperity2bt-0.5.1/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:54.996262 prosperity2bt-0.5.1/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:55.000262 prosperity2bt-0.5.1/prosperity2bt/resources/round1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:55.012262 prosperity2bt-0.5.1/prosperity2bt/resources/round3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2581061 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round3/prices_round_3_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2580446 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round3/prices_round_3_day_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2580491 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round3/prices_round_3_day_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)   148534 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   142870 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   146400 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-16 13:36:48.000000 prosperity2bt-0.5.1/prosperity2bt/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:36:55.012262 prosperity2bt-0.5.1/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-16 13:36:54.000000 prosperity2bt-0.5.1/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-16 13:36:54.000000 prosperity2bt-0.5.1/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:36:54.000000 prosperity2bt-0.5.1/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 13:36:54.000000 prosperity2bt-0.5.1/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 13:36:54.000000 prosperity2bt-0.5.1/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 13:36:54.000000 prosperity2bt-0.5.1/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-16 13:36:52.000000 prosperity2bt-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:36:55.012262 prosperity2bt-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:57:27.207334 prosperity2bt-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-16 15:57:27.207334 prosperity2bt-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:57:27.187334 prosperity2bt-0.5.2/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:57:27.187334 prosperity2bt-0.5.2/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:57:27.191334 prosperity2bt-0.5.2/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:57:27.195334 prosperity2bt-0.5.2/prosperity2bt/resources/round1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round1/prices_round_1_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:57:27.207334 prosperity2bt-0.5.2/prosperity2bt/resources/round3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2581061 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round3/prices_round_3_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580446 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round3/prices_round_3_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580491 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round3/prices_round_3_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   148534 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   142870 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   146400 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-16 15:57:22.000000 prosperity2bt-0.5.2/prosperity2bt/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:57:27.207334 prosperity2bt-0.5.2/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-16 15:57:27.000000 prosperity2bt-0.5.2/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-16 15:57:27.000000 prosperity2bt-0.5.2/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:57:27.000000 prosperity2bt-0.5.2/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 15:57:27.000000 prosperity2bt-0.5.2/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 15:57:27.000000 prosperity2bt-0.5.2/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 15:57:27.000000 prosperity2bt-0.5.2/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-16 15:57:24.000000 prosperity2bt-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:57:27.207334 prosperity2bt-0.5.2/setup.cfg
```

### Comparing `prosperity2bt-0.5.1/LICENSE` & `prosperity2bt-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/PKG-INFO` & `prosperity2bt-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.5.1
+Version: 0.5.2
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2bt-0.5.1/README.md` & `prosperity2bt-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/__main__.py` & `prosperity2bt-0.5.2/prosperity2bt/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from prosperity2bt.file_reader import FileSystemReader, PackageResourcesReader
 from prosperity2bt.models import BacktestResult
 from prosperity2bt.runner import run_backtest
 from typing import Any, Optional
 
 def parse_algorithm(algorithm: str) -> Any:
     algorithm_path = Path(algorithm).expanduser().resolve()
+    if not algorithm_path.is_file():
+        raise ModuleNotFoundError(f"{algorithm_path} is not a file")
 
     sys.path.append(str(algorithm_path.parent))
     return import_module(algorithm_path.stem)
 
 def parse_days(days: list[str], data_root: Optional[str]) -> list[BacktestData]:
     if data_root is not None:
         file_reader = FileSystemReader(Path(data_root).expanduser().resolve())
@@ -51,14 +53,18 @@
 
             if len(parsed_days_in_round) == 0:
                 print(f"Warning: no data found for round {round_num}")
                 continue
 
             parsed_days.extend(parsed_days_in_round)
 
+    if len(parsed_days) == 0:
+        print("Error: did not find data for any requested round/day")
+        sys.exit(1)
+
     return parsed_days
 
 def parse_out(out: Optional[str]) -> Path:
     if out is not None:
         return Path(out).expanduser().resolve()
     else:
         timestamp = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
@@ -184,16 +190,16 @@
     parser.add_argument("--no-trades-matching", action="store_true", help="disable matching orders against market trades")
     parser.add_argument("-v", "--version", action="version", version=f"%(prog)s {metadata.version(__package__)}")
 
     args = parser.parse_args()
 
     try:
         trader_module = parse_algorithm(args.algorithm)
-    except ModuleNotFoundError:
-        print(f"{args.algorithm} is not a valid algorithm file")
+    except ModuleNotFoundError as e:
+        print(f"{args.algorithm} is not a valid algorithm file: {e}")
         sys.exit(1)
 
     if not hasattr(trader_module, "Trader"):
         print(f"{args.algorithm} does not expose a Trader class")
         sys.exit(1)
 
     days = parse_days(args.days, args.data)
```

### Comparing `prosperity2bt-0.5.1/prosperity2bt/data.py` & `prosperity2bt-0.5.2/prosperity2bt/data.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/datamodel.py` & `prosperity2bt-0.5.2/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/file_reader.py` & `prosperity2bt-0.5.2/prosperity2bt/file_reader.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/models.py` & `prosperity2bt-0.5.2/prosperity2bt/models.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.5.2/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.5.2/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv` & `prosperity2bt-0.5.2/prosperity2bt/resources/round1/prices_round_1_day_-1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv` & `prosperity2bt-0.5.2/prosperity2bt/resources/round1/prices_round_1_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv` & `prosperity2bt-0.5.2/prosperity2bt/resources/round1/prices_round_1_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv` & `prosperity2bt-0.5.2/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv` & `prosperity2bt-0.5.2/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv` & `prosperity2bt-0.5.2/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/resources/round3/prices_round_3_day_0.csv` & `prosperity2bt-0.5.2/prosperity2bt/resources/round3/prices_round_3_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/resources/round3/prices_round_3_day_1.csv` & `prosperity2bt-0.5.2/prosperity2bt/resources/round3/prices_round_3_day_1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/resources/round3/prices_round_3_day_2.csv` & `prosperity2bt-0.5.2/prosperity2bt/resources/round3/prices_round_3_day_2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv` & `prosperity2bt-0.5.2/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv` & `prosperity2bt-0.5.2/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv` & `prosperity2bt-0.5.2/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt/runner.py` & `prosperity2bt-0.5.2/prosperity2bt/runner.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.5.2/prosperity2bt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.5.1
+Version: 0.5.2
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2bt-0.5.1/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.5.2/prosperity2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.5.1/pyproject.toml` & `prosperity2bt-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.5.1"
+version = "0.5.2"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

