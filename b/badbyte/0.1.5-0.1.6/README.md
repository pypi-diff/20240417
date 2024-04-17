# Comparing `tmp/badbyte-0.1.5.tar.gz` & `tmp/badbyte-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badbyte-0.1.5.tar", last modified: Wed Apr 17 09:52:02 2024, max compression
+gzip compressed data, was "badbyte-0.1.6.tar", last modified: Wed Apr 17 09:56:51 2024, max compression
```

## Comparing `badbyte-0.1.5.tar` & `badbyte-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:52:02.586988 badbyte-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-17 09:51:58.000000 badbyte-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-17 09:52:02.586988 badbyte-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-17 09:51:58.000000 badbyte-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:52:02.586988 badbyte-0.1.5/badbyte/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 09:51:58.000000 badbyte-0.1.5/badbyte/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-17 09:51:58.000000 badbyte-0.1.5/badbyte/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4667 2024-04-17 09:51:58.000000 badbyte-0.1.5/badbyte/badbyte
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:52:02.586988 badbyte-0.1.5/badbyte/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:51:58.000000 badbyte-0.1.5/badbyte/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-17 09:51:58.000000 badbyte-0.1.5/badbyte/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-17 09:51:58.000000 badbyte-0.1.5/badbyte/utils/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:52:02.586988 badbyte-0.1.5/badbyte.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-17 09:52:02.000000 badbyte-0.1.5/badbyte.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-17 09:52:02.000000 badbyte-0.1.5/badbyte.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:52:02.000000 badbyte-0.1.5/badbyte.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 09:52:02.000000 badbyte-0.1.5/badbyte.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 09:52:02.000000 badbyte-0.1.5/badbyte.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:52:02.586988 badbyte-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-17 09:51:58.000000 badbyte-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:56:51.662838 badbyte-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-17 09:56:47.000000 badbyte-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-17 09:56:51.662838 badbyte-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-17 09:56:47.000000 badbyte-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:56:51.662838 badbyte-0.1.6/badbyte/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 09:56:47.000000 badbyte-0.1.6/badbyte/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-17 09:56:47.000000 badbyte-0.1.6/badbyte/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4808 2024-04-17 09:56:47.000000 badbyte-0.1.6/badbyte/badbyte
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:56:51.662838 badbyte-0.1.6/badbyte/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:56:47.000000 badbyte-0.1.6/badbyte/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-17 09:56:47.000000 badbyte-0.1.6/badbyte/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-17 09:56:47.000000 badbyte-0.1.6/badbyte/utils/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:56:51.662838 badbyte-0.1.6/badbyte.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-17 09:56:51.000000 badbyte-0.1.6/badbyte.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-17 09:56:51.000000 badbyte-0.1.6/badbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:56:51.000000 badbyte-0.1.6/badbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 09:56:51.000000 badbyte-0.1.6/badbyte.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 09:56:51.000000 badbyte-0.1.6/badbyte.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:56:51.662838 badbyte-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-17 09:56:47.000000 badbyte-0.1.6/setup.py
```

### Comparing `badbyte-0.1.5/LICENSE` & `badbyte-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `badbyte-0.1.5/PKG-INFO` & `badbyte-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badbyte
-Version: 0.1.5
+Version: 0.1.6
 Summary: Deal with bad characters easily during exploit writing with badchars.
 Home-page: https://github.com/C3l1n/badbyte
 Author: Karol Jerzy Celiński
 Author-email: karol@celin.pl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `badbyte-0.1.5/README.md` & `badbyte-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `badbyte-0.1.5/badbyte/badbyte` & `badbyte-0.1.6/badbyte/badbyte`

 * *Files 5% similar despite different names*

```diff
@@ -37,17 +37,22 @@
                     help="use custom payload in parse (usefull when you try to search for subsequent bad cahrs).")
 parser.add_argument("--pre", type=str, default="BAD_START", help="payload prefix - default BAD_START")
 parser.add_argument("--post", type=str, default="BAD_STOP", help="payload postfix - default BAD_STOP")
 parser.add_argument("--bad", type=str, default="", help="Banned characters as hexstring i.e. '3D 0D 0A'")
 parser.add_argument("--length", "-l", type=int, help="Cyclic pattern length.")
 parser.add_argument("--pattern", "-p", type=str, help="Part of pattern to search offset for.")
 parser.add_argument("--uniqlength", "-u", default=4, type=int, help="Minimal length of character from cyclic pattern minimal needed to determine offset.")
+parser.add_argument("-v", "--version", action='store_true',
+                    help="Just print version.")
 
 args = parser.parse_args()
 
+if args.version:
+    sys.exit(0)
+
 def validate_args_cyclic(search_offset=False):
     if args.length is None or args.uniqlength is None or (search_offset and args.pattern is None and search_offset):
         parser.print_help(sys.stdout)
         print("\n\nError - you must provide -u and -l to generate pattern or search offset" +
               (" and -p to search of offset" if search_offset else ""))
         sys.exit(0)
 
@@ -69,15 +74,15 @@
         g = cyclic.cyclic_gen(alphabet=alphabet, n=args.uniqlength)
         print(f"{GREEN}Pattern:{RST} {g.get(args.length)}")
     elif args.mode[0] == "o":
         validate_args_cyclic(search_offset=True)
         alphabet = get_cyclic_alphabet(args.bad)
         g = cyclic.cyclic_gen(alphabet=alphabet, n=args.uniqlength)
         print(f"{GREEN}Pattern:{RST} {g.get(args.length)}")
-        if {g.find(args.pattern) == -1:
+        if g.find(args.pattern) == -1:
             print(f"{GREEN}Offset:{RST} {RED}NOT FOUND{END}")
         else:
             print(f"{GREEN}Offset:{RST} {g.find(args.pattern)[0]}")
     elif args.mode[0] == "p":
         print(f"{GREEN}Please paste hexdump (every non whitespace is treated as hexstring). "
               f"Press CTRL+D to end.{RST}")
         try:
```

### Comparing `badbyte-0.1.5/badbyte/utils/functions.py` & `badbyte-0.1.6/badbyte/utils/functions.py`

 * *Files identical despite different names*

### Comparing `badbyte-0.1.5/badbyte.egg-info/PKG-INFO` & `badbyte-0.1.6/badbyte.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badbyte
-Version: 0.1.5
+Version: 0.1.6
 Summary: Deal with bad characters easily during exploit writing with badchars.
 Home-page: https://github.com/C3l1n/badbyte
 Author: Karol Jerzy Celiński
 Author-email: karol@celin.pl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `badbyte-0.1.5/setup.py` & `badbyte-0.1.6/setup.py`

 * *Files identical despite different names*

