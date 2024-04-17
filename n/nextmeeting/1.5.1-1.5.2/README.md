# Comparing `tmp/nextmeeting-1.5.1.tar.gz` & `tmp/nextmeeting-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextmeeting-1.5.1.tar", max compression
+gzip compressed data, was "nextmeeting-1.5.2.tar", max compression
```

## Comparing `nextmeeting-1.5.1.tar` & `nextmeeting-1.5.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-09-29 18:26:44.726056 nextmeeting-1.5.1/LICENSE
--rw-r--r--   0        0        0     3561 2024-03-18 08:14:39.312984 nextmeeting-1.5.1/README.md
--rw-r--r--   0        0        0        0 2023-09-29 18:32:44.557415 nextmeeting-1.5.1/nextmeeting/__init__.py
--rwxr-xr-x   0        0        0    13884 2024-04-05 07:42:01.288982 nextmeeting-1.5.1/nextmeeting/cli.py
--rw-r--r--   0        0        0      829 2024-04-05 07:42:56.608385 nextmeeting-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 nextmeeting-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-09-29 18:26:44.726056 nextmeeting-1.5.2/LICENSE
+-rw-r--r--   0        0        0     3501 2024-04-17 12:02:53.549178 nextmeeting-1.5.2/README.md
+-rw-r--r--   0        0        0        0 2023-09-29 18:32:44.557415 nextmeeting-1.5.2/nextmeeting/__init__.py
+-rwxr-xr-x   0        0        0    13979 2024-04-17 12:02:53.552511 nextmeeting-1.5.2/nextmeeting/cli.py
+-rw-r--r--   0        0        0      829 2024-04-17 12:03:11.818973 nextmeeting-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4268 1970-01-01 00:00:00.000000 nextmeeting-1.5.2/PKG-INFO
```

### Comparing `nextmeeting-1.5.1/LICENSE` & `nextmeeting-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nextmeeting-1.5.1/README.md` & `nextmeeting-1.5.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -23,40 +23,42 @@
 
 You need to install [gcalcli](https://github.com/insanum/gcalcli) and [setup
 the google Oauth integration](https://github.com/insanum/gcalcli#login-information) with google calendar.
 
 By default you can start `nextmeeting` and it will show the list of meetings you
 have with "human date".
 
-There is a few options to customize things, see `nextmeeting --help` for more.
+There is a few options to customize things, see `nextmeeting --help` for more options.
 
 ### Waybar
 
-More interesting to integrate with waybar you can have something like this:
+A more interesting use of `nextmeeting` is the integration with waybar, to output nicely on your desktop,
+for example my configuration look like this:
 
 ```json
     "custom/agenda": {
         "format": "{}",
-        "exec": "size=30;swaymsg -t get_outputs -p |grep -q 'Current mode: 3440x1440' && size=80; nextmeeting --max-title-length ${size} --waybar",
+        "exec": "nextmeeting --max-title-length 30 --waybar",
         "on-click": "nextmeeting --open-meet-url",
-        "on-click-right": "kitty --class=GClock -- /bin/bash -c \"batz;echo;cal -3;echo;nextmeeting;read;\";",
+        "on-click-right": "kitty -- /bin/bash -c \"batz;echo;cal -3;echo;nextmeeting;read;\";",
         "interval": 59,
         "return-type": "json",
         "tooltip": "true"
     },
 ```
 
-This will detect if i have my external display connected for the length of the
-tile and show how long i have until the next meeting. If if i click on the item
-it will open the meet URL attached to the event. On right click it will use
+This will show how long i have until the next meeting. If I click on the item
+it will open the meet URL attached to the event. If I hit via a right click it will launch a
 `kitty` terminal to show the time zones with
 [batz](https://github.com/chmouel/batzconverter) and my next meeting. I can
 click on the title in the terminal and it will open the meet URL.
 
-You can style the waybar item with the following CSS:
+#### Styling
+
+You can style some of the waybar item with the following CSS:
 
 ```css
 #custom-agenda {
   color: #696969;
 }
 ```
```

### Comparing `nextmeeting-1.5.1/nextmeeting/cli.py` & `nextmeeting-1.5.2/nextmeeting/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,22 +224,25 @@
     t = f"{title}{start_date}{end_date}".encode("utf-8")
     uuid = hashlib.md5(t).hexdigest()
     notified = False
     cached = []
     cache_path = args.cache_dir / "cache.json"
     if cache_path.exists():
         with cache_path.open() as f:
-            cached = json.load(f)
+            try:
+                cached = json.load(f)
+            except json.JSONDecodeError:
+                cached = []
             if uuid in cached:
                 notified = True
     if notified:
         return
     cached.append(uuid)
     with cache_path.open("w") as f:
-        if cached >= MAX_CACHED_ENTRIES:
+        if len(cached) >= MAX_CACHED_ENTRIES:
             cached = cached[-MAX_CACHED_ENTRIES:]
         json.dump(cached, f)
     if NOTIFY_PROGRAM == "":
         return
     other_args = []
     if args.notify_expiry > 0:
         milliseconds = args.notify_expiry * 60 * 1000
```

### Comparing `nextmeeting-1.5.1/pyproject.toml` & `nextmeeting-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nextmeeting"
-version = "1.5.1"
+version = "1.5.2"
 description = "Show your nextmeeting in your poly/waybar with gcalcli"
 authors = ["Chmouel Boudjnah <chmouel@chmouel.com>"]
 keywords = ["calendar", "cli"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/chmouel/nextmeeting"
 repository = "https://github.com/chmouel/nextmeeting"
```

### Comparing `nextmeeting-1.5.1/PKG-INFO` & `nextmeeting-1.5.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextmeeting
-Version: 1.5.1
+Version: 1.5.2
 Summary: Show your nextmeeting in your poly/waybar with gcalcli
 Home-page: https://github.com/chmouel/nextmeeting
 License: Apache-2.0
 Keywords: calendar,cli
 Author: Chmouel Boudjnah
 Author-email: chmouel@chmouel.com
 Requires-Python: >=3.9,<4.0
@@ -43,40 +43,42 @@
 
 You need to install [gcalcli](https://github.com/insanum/gcalcli) and [setup
 the google Oauth integration](https://github.com/insanum/gcalcli#login-information) with google calendar.
 
 By default you can start `nextmeeting` and it will show the list of meetings you
 have with "human date".
 
-There is a few options to customize things, see `nextmeeting --help` for more.
+There is a few options to customize things, see `nextmeeting --help` for more options.
 
 ### Waybar
 
-More interesting to integrate with waybar you can have something like this:
+A more interesting use of `nextmeeting` is the integration with waybar, to output nicely on your desktop,
+for example my configuration look like this:
 
 ```json
     "custom/agenda": {
         "format": "{}",
-        "exec": "size=30;swaymsg -t get_outputs -p |grep -q 'Current mode: 3440x1440' && size=80; nextmeeting --max-title-length ${size} --waybar",
+        "exec": "nextmeeting --max-title-length 30 --waybar",
         "on-click": "nextmeeting --open-meet-url",
-        "on-click-right": "kitty --class=GClock -- /bin/bash -c \"batz;echo;cal -3;echo;nextmeeting;read;\";",
+        "on-click-right": "kitty -- /bin/bash -c \"batz;echo;cal -3;echo;nextmeeting;read;\";",
         "interval": 59,
         "return-type": "json",
         "tooltip": "true"
     },
 ```
 
-This will detect if i have my external display connected for the length of the
-tile and show how long i have until the next meeting. If if i click on the item
-it will open the meet URL attached to the event. On right click it will use
+This will show how long i have until the next meeting. If I click on the item
+it will open the meet URL attached to the event. If I hit via a right click it will launch a
 `kitty` terminal to show the time zones with
 [batz](https://github.com/chmouel/batzconverter) and my next meeting. I can
 click on the title in the terminal and it will open the meet URL.
 
-You can style the waybar item with the following CSS:
+#### Styling
+
+You can style some of the waybar item with the following CSS:
 
 ```css
 #custom-agenda {
   color: #696969;
 }
 ```
```

