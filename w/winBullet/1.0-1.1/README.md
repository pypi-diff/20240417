# Comparing `tmp/winBullet-1.0.tar.gz` & `tmp/winbullet-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winBullet-1.0.tar", last modified: Thu Apr 11 10:47:12 2024, max compression
+gzip compressed data, was "winbullet-1.1.tar", last modified: Wed Apr 17 07:13:36 2024, max compression
```

## Comparing `winBullet-1.0.tar` & `winbullet-1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 10:47:12.874758 winBullet-1.0/
--rw-rw-rw-   0        0        0     1088 2024-04-11 09:50:44.000000 winBullet-1.0/LICENSE
--rw-rw-rw-   0        0        0      355 2024-04-11 10:47:12.873741 winBullet-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2024-04-11 09:50:44.000000 winBullet-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 10:47:12.860677 winBullet-1.0/bullet/
--rw-rw-rw-   0        0        0      266 2024-04-11 09:50:44.000000 winBullet-1.0/bullet/__init__.py
--rw-rw-rw-   0        0        0     2017 2024-04-11 09:50:44.000000 winBullet-1.0/bullet/charDef.py
--rw-rw-rw-   0        0        0    32165 2024-04-11 09:50:44.000000 winBullet-1.0/bullet/client.py
--rw-rw-rw-   0        0        0      723 2024-04-11 09:50:44.000000 winBullet-1.0/bullet/colors.py
--rw-rw-rw-   0        0        0     1242 2024-04-11 09:50:44.000000 winBullet-1.0/bullet/cursor.py
--rw-rw-rw-   0        0        0      378 2024-04-11 09:50:44.000000 winBullet-1.0/bullet/emojis.py
--rw-rw-rw-   0        0        0     1427 2024-04-11 09:50:44.000000 winBullet-1.0/bullet/keyhandler.py
--rw-rw-rw-   0        0        0     1772 2024-04-11 09:50:44.000000 winBullet-1.0/bullet/styles.py
--rw-rw-rw-   0        0        0     4747 2024-04-11 09:50:44.000000 winBullet-1.0/bullet/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-11 10:47:12.876271 winBullet-1.0/setup.cfg
--rw-rw-rw-   0        0        0      488 2024-04-11 09:50:44.000000 winBullet-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:47:12.871443 winBullet-1.0/winBullet.egg-info/
--rw-rw-rw-   0        0        0      355 2024-04-11 10:47:12.000000 winBullet-1.0/winBullet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-04-11 10:47:12.000000 winBullet-1.0/winBullet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 10:47:12.000000 winBullet-1.0/winBullet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-11 10:47:12.000000 winBullet-1.0/winBullet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 07:13:36.808272 winbullet-1.1/
+-rw-rw-rw-   0        0        0     1088 2024-04-11 09:50:44.000000 winbullet-1.1/LICENSE
+-rw-rw-rw-   0        0        0      355 2024-04-17 07:13:36.804672 winbullet-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2024-04-11 09:50:44.000000 winbullet-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 07:13:36.783445 winbullet-1.1/bullet/
+-rw-rw-rw-   0        0        0      266 2024-04-11 09:50:44.000000 winbullet-1.1/bullet/__init__.py
+-rw-rw-rw-   0        0        0     2017 2024-04-11 09:50:44.000000 winbullet-1.1/bullet/charDef.py
+-rw-rw-rw-   0        0        0    31993 2024-04-17 07:11:16.000000 winbullet-1.1/bullet/client.py
+-rw-rw-rw-   0        0        0      723 2024-04-11 09:50:44.000000 winbullet-1.1/bullet/colors.py
+-rw-rw-rw-   0        0        0     1242 2024-04-11 09:50:44.000000 winbullet-1.1/bullet/cursor.py
+-rw-rw-rw-   0        0        0      378 2024-04-11 09:50:44.000000 winbullet-1.1/bullet/emojis.py
+-rw-rw-rw-   0        0        0     1427 2024-04-11 09:50:44.000000 winbullet-1.1/bullet/keyhandler.py
+-rw-rw-rw-   0        0        0     1772 2024-04-11 09:50:44.000000 winbullet-1.1/bullet/styles.py
+-rw-rw-rw-   0        0        0     4747 2024-04-11 09:50:44.000000 winbullet-1.1/bullet/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-17 07:13:36.809271 winbullet-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      490 2024-04-17 07:12:55.000000 winbullet-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:13:36.800666 winbullet-1.1/winBullet.egg-info/
+-rw-rw-rw-   0        0        0      355 2024-04-17 07:13:36.000000 winbullet-1.1/winBullet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-04-17 07:13:36.000000 winbullet-1.1/winBullet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 07:13:36.000000 winbullet-1.1/winBullet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-17 07:13:36.000000 winbullet-1.1/winBullet.egg-info/top_level.txt
```

### Comparing `winBullet-1.0/LICENSE` & `winbullet-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `winBullet-1.0/README.md` & `winbullet-1.1/README.md`

 * *Files identical despite different names*

### Comparing `winBullet-1.0/bullet/charDef.py` & `winbullet-1.1/bullet/charDef.py`

 * *Files identical despite different names*

### Comparing `winBullet-1.0/bullet/client.py` & `winbullet-1.1/bullet/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,18 +78,14 @@
             if i == NEWLINE_KEY:
                 utils.forceWrite('\n')
                 return self.getInput()
             elif i == LINE_BEGIN_KEY or \
                  i == HOME_KEY       or \
                  i == LINE_END_KEY   or \
                  i == END_KEY        or \
-                 i == ARROW_UP_KEY   or \
-                 i == ARROW_DOWN_KEY or \
-                 i == PG_UP_KEY      or \
-                 i == PG_DOWN_KEY    or \
                  i == TAB_KEY        or \
                  i == UNDEFINED_KEY:
                 return
             elif i == BACK_SPACE_KEY or i == BACK_SPACE_CHAR:
                 if self.moveCursor(self.pos - 1):
                     self.deleteChar()
             elif i == DELETE_KEY:
```

### Comparing `winBullet-1.0/bullet/colors.py` & `winbullet-1.1/bullet/colors.py`

 * *Files identical despite different names*

### Comparing `winBullet-1.0/bullet/cursor.py` & `winbullet-1.1/bullet/cursor.py`

 * *Files identical despite different names*

### Comparing `winBullet-1.0/bullet/keyhandler.py` & `winbullet-1.1/bullet/keyhandler.py`

 * *Files identical despite different names*

### Comparing `winBullet-1.0/bullet/styles.py` & `winbullet-1.1/bullet/styles.py`

 * *Files identical despite different names*

### Comparing `winBullet-1.0/bullet/utils.py` & `winbullet-1.1/bullet/utils.py`

 * *Files identical despite different names*

