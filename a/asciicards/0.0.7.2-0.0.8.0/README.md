# Comparing `tmp/asciicards-0.0.7.2.tar.gz` & `tmp/asciicards-0.0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asciicards-0.0.7.2.tar", last modified: Thu May 11 19:19:08 2023, max compression
+gzip compressed data, was "asciicards-0.0.8.0.tar", last modified: Wed Apr 17 01:26:47 2024, max compression
```

## Comparing `asciicards-0.0.7.2.tar` & `asciicards-0.0.8.0.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 19:19:08.280303 asciicards-0.0.7.2/
--rw-rw-rw-   0        0        0    35149 2023-05-06 18:11:30.000000 asciicards-0.0.7.2/LICENSE
--rw-rw-rw-   0        0        0      544 2023-05-11 19:19:08.280303 asciicards-0.0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-05-06 18:11:30.000000 asciicards-0.0.7.2/README.md
--rw-rw-rw-   0        0        0      437 2023-05-11 19:14:03.000000 asciicards-0.0.7.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 19:19:08.280303 asciicards-0.0.7.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 19:19:08.237424 asciicards-0.0.7.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 19:19:08.265891 asciicards-0.0.7.2/src/asciicards/
--rw-rw-rw-   0        0        0        0 2023-05-07 00:04:42.000000 asciicards-0.0.7.2/src/asciicards/__init__.py
--rw-rw-rw-   0        0        0     1456 2023-05-11 19:16:00.000000 asciicards-0.0.7.2/src/asciicards/asciicards.py
-drwxrwxrwx   0        0        0        0 2023-05-11 19:19:08.278307 asciicards-0.0.7.2/src/asciicards.egg-info/
--rw-rw-rw-   0        0        0      544 2023-05-11 19:19:08.000000 asciicards-0.0.7.2/src/asciicards.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-05-11 19:19:08.000000 asciicards-0.0.7.2/src/asciicards.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 19:19:08.000000 asciicards-0.0.7.2/src/asciicards.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-11 19:19:08.000000 asciicards-0.0.7.2/src/asciicards.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 01:26:47.293310 asciicards-0.0.8.0/
+-rw-rw-rw-   0        0        0    35149 2023-05-06 18:11:30.000000 asciicards-0.0.8.0/LICENSE
+-rw-rw-rw-   0        0        0    41777 2024-04-17 01:26:47.292310 asciicards-0.0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-05-06 18:11:30.000000 asciicards-0.0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 01:26:47.290311 asciicards-0.0.8.0/asciicards.egg-info/
+-rw-rw-rw-   0        0        0    41777 2024-04-17 01:26:47.000000 asciicards-0.0.8.0/asciicards.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2024-04-17 01:26:47.000000 asciicards-0.0.8.0/asciicards.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 01:26:47.000000 asciicards-0.0.8.0/asciicards.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-17 01:26:47.000000 asciicards-0.0.8.0/asciicards.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1696 2024-04-17 00:49:07.000000 asciicards-0.0.8.0/asciicards.py
+-rw-rw-rw-   0        0        0      538 2024-04-17 01:26:41.000000 asciicards-0.0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 01:26:47.293310 asciicards-0.0.8.0/setup.cfg
```

### Comparing `asciicards-0.0.7.2/LICENSE` & `asciicards-0.0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asciicards-0.0.7.2/src/asciicards/asciicards.py` & `asciicards-0.0.8.0/asciicards.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,27 +26,32 @@
 │         │
 │    {card_value:<2}   │
 │         │
 │    {suit}    │
 │         │
 │    {card_value:>2}   │
 │         │
-└─────────┘"""
+└─────────┘
+"""
     if len(card_value) > 2:
         ascii_card = f"""
 ┌─────────┐
 │         │
 │    {card_value:<2}  │
 │         │
 │    {suit}    │
 │         │
 │    {card_value:>2}  │
 │         │
-└─────────┘"""
+└─────────┘
+"""
     return ascii_card
 
 def show_hand(hand):
-    """Return the ascii art for a given hand"""
-    ascii_hand = ""
+    """Return the ascii art for a given hand with cards displayed horizontally"""
+    hand_lines = [""] * 10  # Number of lines in each card representation
     for card in hand:
-        ascii_hand += show_card(card)
-    return ascii_hand
+        card_lines = show_card(card).split('\n')
+        for i in range(len(hand_lines)):
+            hand_lines[i] += card_lines[i] + "  "  # Add spacing between cards
+    return '\n'.join(hand_lines)
+
```

