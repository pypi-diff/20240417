# Comparing `tmp/juery-0.2.0.tar.gz` & `tmp/juery-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juery-0.2.0.tar", max compression
+gzip compressed data, was "juery-0.2.1.tar", max compression
```

## Comparing `juery-0.2.0.tar` & `juery-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-15 07:21:43.398054 juery-0.2.0/README.md
--rw-r--r--   0        0        0       92 2024-04-15 07:24:52.880634 juery-0.2.0/juery/__init__.py
--rw-r--r--   0        0        0     2494 2024-04-17 02:16:23.316784 juery-0.2.0/juery/juery.py
--rw-r--r--   0        0        0      118 2024-04-15 07:22:20.151676 juery-0.2.0/juery/payload.py
--rw-r--r--   0        0        0      677 2024-04-17 02:08:40.419107 juery-0.2.0/juery/special.py
--rw-r--r--   0        0        0      272 2024-04-17 02:18:56.331842 juery-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 juery-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 07:21:43.398054 juery-0.2.1/README.md
+-rw-r--r--   0        0        0       92 2024-04-15 07:24:52.880634 juery-0.2.1/juery/__init__.py
+-rw-r--r--   0        0        0     2589 2024-04-17 02:29:08.021368 juery-0.2.1/juery/juery.py
+-rw-r--r--   0        0        0      118 2024-04-15 07:22:20.151676 juery-0.2.1/juery/payload.py
+-rw-r--r--   0        0        0      677 2024-04-17 02:08:40.419107 juery-0.2.1/juery/special.py
+-rw-r--r--   0        0        0      272 2024-04-17 02:29:16.229288 juery-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 juery-0.2.1/PKG-INFO
```

### Comparing `juery-0.2.0/juery/juery.py` & `juery-0.2.1/juery/juery.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,27 +51,28 @@
                 if index >= len(keys):
                     # Comparator terminated before
                     # finishing the path.
                     # Exclude this payload.
                     index = -1
                     break
 
-                a = str(keys[index])
-
-                special = Special.new(a)
-
-                b = payload.path[i]
+                special = Special.new(str(keys[index]))
+                value = payload.path[i]
 
                 ok = False
 
                 if special.regular_expression:
-                    special = re.search(special.value, b, re.I)
+                    special = re.search(
+                        special.value,
+                        value,
+                        re.I,
+                    )
                     ok = special != None
 
-                elif a.lower() == b.lower():
+                elif special.value.lower() == value.lower():
                     ok = True
 
                 if ok:
                     index += 1
 
                 elif special.direct_descendant:
                     # Not a direct descendant.
```

### Comparing `juery-0.2.0/juery/special.py` & `juery-0.2.1/juery/special.py`

 * *Files identical despite different names*

