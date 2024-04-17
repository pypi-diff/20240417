# Comparing `tmp/badbyte-0.1.4.tar.gz` & `tmp/badbyte-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badbyte-0.1.4.tar", last modified: Sun Jan 14 14:00:47 2024, max compression
+gzip compressed data, was "badbyte-0.1.5.tar", last modified: Wed Apr 17 09:52:02 2024, max compression
```

## Comparing `badbyte-0.1.4.tar` & `badbyte-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:00:47.035940 badbyte-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-14 14:00:38.000000 badbyte-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-01-14 14:00:47.031940 badbyte-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-01-14 14:00:38.000000 badbyte-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:00:47.031940 badbyte-0.1.4/badbyte/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-14 14:00:38.000000 badbyte-0.1.4/badbyte/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-01-14 14:00:38.000000 badbyte-0.1.4/badbyte/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4547 2024-01-14 14:00:38.000000 badbyte-0.1.4/badbyte/badbyte
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:00:47.031940 badbyte-0.1.4/badbyte/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 14:00:38.000000 badbyte-0.1.4/badbyte/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-14 14:00:38.000000 badbyte-0.1.4/badbyte/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-01-14 14:00:38.000000 badbyte-0.1.4/badbyte/utils/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:00:47.031940 badbyte-0.1.4/badbyte.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-01-14 14:00:47.000000 badbyte-0.1.4/badbyte.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-14 14:00:47.000000 badbyte-0.1.4/badbyte.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 14:00:47.000000 badbyte-0.1.4/badbyte.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-14 14:00:47.000000 badbyte-0.1.4/badbyte.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-14 14:00:47.000000 badbyte-0.1.4/badbyte.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-14 14:00:47.035940 badbyte-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-01-14 14:00:38.000000 badbyte-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:52:02.586988 badbyte-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-17 09:51:58.000000 badbyte-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-17 09:52:02.586988 badbyte-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-17 09:51:58.000000 badbyte-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:52:02.586988 badbyte-0.1.5/badbyte/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 09:51:58.000000 badbyte-0.1.5/badbyte/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-17 09:51:58.000000 badbyte-0.1.5/badbyte/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4667 2024-04-17 09:51:58.000000 badbyte-0.1.5/badbyte/badbyte
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:52:02.586988 badbyte-0.1.5/badbyte/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:58.000000 badbyte-0.1.5/badbyte/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-17 09:51:58.000000 badbyte-0.1.5/badbyte/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-17 09:51:58.000000 badbyte-0.1.5/badbyte/utils/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:52:02.586988 badbyte-0.1.5/badbyte.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-17 09:52:02.000000 badbyte-0.1.5/badbyte.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-17 09:52:02.000000 badbyte-0.1.5/badbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:52:02.000000 badbyte-0.1.5/badbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 09:52:02.000000 badbyte-0.1.5/badbyte.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 09:52:02.000000 badbyte-0.1.5/badbyte.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:52:02.586988 badbyte-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-17 09:51:58.000000 badbyte-0.1.5/setup.py
```

### Comparing `badbyte-0.1.4/LICENSE` & `badbyte-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `badbyte-0.1.4/PKG-INFO` & `badbyte-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badbyte
-Version: 0.1.4
+Version: 0.1.5
 Summary: Deal with bad characters easily during exploit writing with badchars.
 Home-page: https://github.com/C3l1n/badbyte
 Author: Karol Jerzy Celiński
 Author-email: karol@celin.pl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `badbyte-0.1.4/README.md` & `badbyte-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `badbyte-0.1.4/badbyte/badbyte` & `badbyte-0.1.5/badbyte/badbyte`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,18 @@
         g = cyclic.cyclic_gen(alphabet=alphabet, n=args.uniqlength)
         print(f"{GREEN}Pattern:{RST} {g.get(args.length)}")
     elif args.mode[0] == "o":
         validate_args_cyclic(search_offset=True)
         alphabet = get_cyclic_alphabet(args.bad)
         g = cyclic.cyclic_gen(alphabet=alphabet, n=args.uniqlength)
         print(f"{GREEN}Pattern:{RST} {g.get(args.length)}")
-        print(f"{GREEN}Offset:{RST} {g.find(args.pattern)[0]}")
+        if {g.find(args.pattern) == -1:
+            print(f"{GREEN}Offset:{RST} {RED}NOT FOUND{END}")
+        else:
+            print(f"{GREEN}Offset:{RST} {g.find(args.pattern)[0]}")
     elif args.mode[0] == "p":
         print(f"{GREEN}Please paste hexdump (every non whitespace is treated as hexstring). "
               f"Press CTRL+D to end.{RST}")
         try:
             hexdump = ""
             while True:
                 hexdump += input()
```

### Comparing `badbyte-0.1.4/badbyte/utils/functions.py` & `badbyte-0.1.5/badbyte/utils/functions.py`

 * *Files identical despite different names*

### Comparing `badbyte-0.1.4/badbyte.egg-info/PKG-INFO` & `badbyte-0.1.5/badbyte.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badbyte
-Version: 0.1.4
+Version: 0.1.5
 Summary: Deal with bad characters easily during exploit writing with badchars.
 Home-page: https://github.com/C3l1n/badbyte
 Author: Karol Jerzy Celiński
 Author-email: karol@celin.pl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `badbyte-0.1.4/setup.py` & `badbyte-0.1.5/setup.py`

 * *Files identical despite different names*

