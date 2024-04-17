# Comparing `tmp/dune_rivals-0.4.3.tar.gz` & `tmp/dune_rivals-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.4.3.tar", last modified: Wed Apr 17 14:53:58 2024, max compression
+gzip compressed data, was "dune_rivals-0.4.4.tar", last modified: Wed Apr 17 14:58:28 2024, max compression
```

## Comparing `dune_rivals-0.4.3.tar` & `dune_rivals-0.4.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-17 14:53:58.266237 dune_rivals-0.4.3/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-17 14:53:58.265591 dune_rivals-0.4.3/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.4.3/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-17 14:53:58.264724 dune_rivals-0.4.3/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-17 14:53:58.000000 dune_rivals-0.4.3/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-17 14:53:58.000000 dune_rivals-0.4.3/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-17 14:53:58.000000 dune_rivals-0.4.3/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-17 14:53:58.000000 dune_rivals-0.4.3/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    24219 2024-04-17 14:52:38.000000 dune_rivals-0.4.3/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-17 14:53:19.000000 dune_rivals-0.4.3/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-17 14:53:58.266364 dune_rivals-0.4.3/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-17 14:58:28.324990 dune_rivals-0.4.4/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-17 14:58:28.324573 dune_rivals-0.4.4/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.4.4/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-17 14:58:28.324149 dune_rivals-0.4.4/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-17 14:58:28.000000 dune_rivals-0.4.4/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-17 14:58:28.000000 dune_rivals-0.4.4/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-17 14:58:28.000000 dune_rivals-0.4.4/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-17 14:58:28.000000 dune_rivals-0.4.4/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    24218 2024-04-17 14:58:15.000000 dune_rivals-0.4.4/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-17 14:58:23.000000 dune_rivals-0.4.4/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-17 14:58:28.325083 dune_rivals-0.4.4/setup.cfg
```

### Comparing `dune_rivals-0.4.3/dune_rivals.py` & `dune_rivals-0.4.4/dune_rivals.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,17 +402,16 @@
         # once everyone is finished, leader will run the show
         self.gamestate.send_message.remote(leader, self.id, {"free": True}, "rival")
         if self.id == leader:
             # destroy remaining obj spice
             first_pass, skipped_lst, warrior_free_states = True, [], {id: False for id in range(1, 5)}
             warrior_free_states[self.id] = True
             while first_pass or len(skipped_lst) > 0:
-                first_pass = False
-
                 obj_arr = obj_spice_arr if first_pass else skipped_lst
+                first_pass = False
                 for loc in obj_arr:
                     i, j = loc[0], loc[1]
                     warrior_ids = self.order_map[(i,j)]
 
                     # if one of warrior_ids isn't free then skip
                     not_free = False
                     for warrior_id in warrior_ids:
```

