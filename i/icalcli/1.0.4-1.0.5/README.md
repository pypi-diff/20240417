# Comparing `tmp/icalcli-1.0.4.tar.gz` & `tmp/icalcli-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icalcli-1.0.4.tar", last modified: Tue Oct 11 15:44:24 2022, max compression
+gzip compressed data, was "icalcli-1.0.5.tar", last modified: Wed Apr 17 13:41:05 2024, max compression
```

## Comparing `icalcli-1.0.4.tar` & `icalcli-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2022-10-11 15:44:24.498568 icalcli-1.0.4/
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     1137 2019-12-19 12:54:20.000000 icalcli-1.0.4/LICENSE
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     5588 2022-10-11 15:44:24.498568 icalcli-1.0.4/PKG-INFO
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     5030 2022-07-12 08:00:39.000000 icalcli-1.0.4/README.md
-drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2022-10-11 15:44:24.495235 icalcli-1.0.4/icalcli/
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)      450 2022-10-11 15:38:57.000000 icalcli-1.0.4/icalcli/__init__.py
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)    11403 2022-08-16 08:36:07.000000 icalcli-1.0.4/icalcli/argparsers.py
-drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2022-10-11 15:44:24.498568 icalcli-1.0.4/icalcli/etesync_backend/
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       29 2022-07-12 07:50:56.000000 icalcli-1.0.4/icalcli/etesync_backend/__init__.py
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     3908 2022-07-25 08:52:55.000000 icalcli-1.0.4/icalcli/etesync_backend/etesync_crud.py
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     3325 2020-01-08 14:23:24.000000 icalcli-1.0.4/icalcli/etesync_backend/etesync_interface.py
-drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2022-10-11 15:44:24.498568 icalcli-1.0.4/icalcli/file_backend/
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       29 2022-07-12 07:48:59.000000 icalcli-1.0.4/icalcli/file_backend/__init__.py
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     2193 2022-08-16 11:36:43.000000 icalcli-1.0.4/icalcli/file_backend/ics_interface.py
--rwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)    66022 2022-10-11 15:37:59.000000 icalcli-1.0.4/icalcli/icalcli.py
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     4037 2019-02-28 12:11:14.000000 icalcli-1.0.4/icalcli/printer.py
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     4193 2022-08-10 09:40:48.000000 icalcli-1.0.4/icalcli/utils.py
-drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2022-10-11 15:44:24.498568 icalcli-1.0.4/icalcli.egg-info/
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     5588 2022-10-11 15:44:24.000000 icalcli-1.0.4/icalcli.egg-info/PKG-INFO
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)      503 2022-10-11 15:44:24.000000 icalcli-1.0.4/icalcli.egg-info/SOURCES.txt
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)        1 2022-10-11 15:44:24.000000 icalcli-1.0.4/icalcli.egg-info/dependency_links.txt
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       49 2022-10-11 15:44:24.000000 icalcli-1.0.4/icalcli.egg-info/entry_points.txt
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       93 2022-10-11 15:44:24.000000 icalcli-1.0.4/icalcli.egg-info/requires.txt
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)        8 2022-10-11 15:44:24.000000 icalcli-1.0.4/icalcli.egg-info/top_level.txt
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       38 2022-10-11 15:44:24.498568 icalcli-1.0.4/setup.cfg
--rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     1173 2022-10-11 15:39:21.000000 icalcli-1.0.4/setup.py
+drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2024-04-17 13:41:05.252852 icalcli-1.0.5/
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     2634 2024-04-17 13:16:33.000000 icalcli-1.0.5/CHANGELOG.md
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     1137 2019-12-19 12:54:20.000000 icalcli-1.0.5/LICENSE
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     6814 2024-04-17 13:41:05.252852 icalcli-1.0.5/PKG-INFO
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     6256 2024-04-17 13:10:57.000000 icalcli-1.0.5/README.md
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)      104 2020-01-08 05:10:41.000000 icalcli-1.0.5/exclude
+drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2024-04-17 13:41:05.252852 icalcli-1.0.5/icalcli/
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)      450 2022-10-11 15:38:57.000000 icalcli-1.0.5/icalcli/__init__.py
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)    11604 2024-04-17 09:15:43.000000 icalcli-1.0.5/icalcli/argparsers.py
+drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2024-04-17 13:41:05.252852 icalcli-1.0.5/icalcli/etesync_backend/
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       29 2022-07-12 07:50:56.000000 icalcli-1.0.5/icalcli/etesync_backend/__init__.py
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     3908 2022-07-25 08:52:55.000000 icalcli-1.0.5/icalcli/etesync_backend/etesync_crud.py
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     3325 2020-01-08 14:23:24.000000 icalcli-1.0.5/icalcli/etesync_backend/etesync_interface.py
+drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2024-04-17 13:41:05.252852 icalcli-1.0.5/icalcli/file_backend/
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       29 2022-07-12 07:48:59.000000 icalcli-1.0.5/icalcli/file_backend/__init__.py
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     2627 2024-04-17 12:29:26.000000 icalcli-1.0.5/icalcli/file_backend/ics_interface.py
+-rwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)    68901 2024-04-17 12:28:55.000000 icalcli-1.0.5/icalcli/icalcli.py
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     4037 2019-02-28 12:11:14.000000 icalcli-1.0.5/icalcli/printer.py
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     4193 2022-08-10 09:40:48.000000 icalcli-1.0.5/icalcli/utils.py
+drwxr-xr-x   0 jrvarma   (1000) jrvarma   (1000)        0 2024-04-17 13:41:05.252852 icalcli-1.0.5/icalcli.egg-info/
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     6814 2024-04-17 13:41:05.000000 icalcli-1.0.5/icalcli.egg-info/PKG-INFO
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)      541 2024-04-17 13:41:05.000000 icalcli-1.0.5/icalcli.egg-info/SOURCES.txt
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)        1 2024-04-17 13:41:05.000000 icalcli-1.0.5/icalcli.egg-info/dependency_links.txt
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       49 2024-04-17 13:41:05.000000 icalcli-1.0.5/icalcli.egg-info/entry_points.txt
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       93 2024-04-17 13:41:05.000000 icalcli-1.0.5/icalcli.egg-info/requires.txt
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)        8 2024-04-17 13:41:05.000000 icalcli-1.0.5/icalcli.egg-info/top_level.txt
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)       38 2024-04-17 13:41:05.252852 icalcli-1.0.5/setup.cfg
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)     1173 2024-04-17 13:16:47.000000 icalcli-1.0.5/setup.py
+-rw-r--r--   0 jrvarma   (1000) jrvarma   (1000)      890 2020-09-10 14:15:34.000000 icalcli-1.0.5/update-github.md
```

### Comparing `icalcli-1.0.4/LICENSE` & `icalcli-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `icalcli-1.0.4/PKG-INFO` & `icalcli-1.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: icalcli
-Version: 1.0.4
-Summary: Icalendar Calendar Command Line Interface
-Home-page: https://github.com/jrvarma/icalcli
-Maintainer: Jayanth R. Varma
-Maintainer-email: jrvarma@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: parsedatetime
-License-File: LICENSE
-
 # icalcli
 
 ### An iCalendar Command Line Interface
 
 `icalcli` - a modification of [gcalcli](https://github.com/insanum/gcalcli) - is a Python command line front-end to your Calendar. It allows you to get your agenda, view weekly and monthly calendars (ascii text graphical calendar), search for events, add new events, delete events, and edit events. 
 
 Unlike [gcalcli](https://github.com/insanum/gcalcli) which is tied to Google Calendar, `icalcli` is agnostic to (abstracts away from) the actual backend calendar service. It relies on a backend interface which interacts with the backend calendar to perform all the CRUD (Create, Retrieve, Update and Delete) operations on the actual calendar. The package includes two backends:
@@ -62,14 +45,15 @@
 ### Command line arguments
 
 `icalcli` provides a series of subcommands with the following functionality:
 
     edit (e)               edit calendar events
     agenda (g)             get an agenda for a time period
     calw (w)               get a week-based agenda in calendar format
+    cal5w (5w)             get this week / 2 past / 2 future weeks agenda in calendar format
     calm (m)               get a month agenda in calendar format
     add (a)                add a detailed event to the calendar
     search (s)             (regex) search for events 
     sync (y)               sync the backend calendar
     quit (q)               quit icalcli
 
 By default, `icalcli` runs interactively as an REPL (Read Evaluate Print Loop). Run `icalcli --help` for more details. `icalcli <subcommand> --help` gives help on each subcommand.
@@ -83,14 +67,23 @@
 ```
 from icalcli import ICSInterface
 
 backend_interface = ICSInterface("/path/to/ics-file")
 
 ```
 
+#### Example configuration for multiple readonly file_backend
+
+```
+from icalcli import ICSInterface
+
+backend_interface = ICSInterface(["/path/to/ics-file-1", "/path/to/ics-file-2"])
+
+```
+
 #### Example configuration for etesync_backend
 
 This configuration assumes that all the credentials are stored in a plain text (`json`) file. In practice, you would use a more secure storage (perhaps, the `Gnome keyring`) or just read it from the terminal.
 
 ```
 from icalcli import EtesyncInterface
 import base64
@@ -102,14 +95,24 @@
 backend_interface = EtesyncInterface(
     c['email'], c['userPassword'], c['remoteUrl'],
     c['uid'], c['authToken'],
     base64.decodebytes(c['cipher_key'].encode('ascii')))
 ```
 See the [Example code](https://github.com/jrvarma/icalcli/issues/1#issuecomment-979851222) for getting the  `uid` and `authToken` for the `etesync` calendar.
 
+## Recurring events and default search period
+
+`icalcli` understands the `RRULE`, `RDATE`, `EXRULE`, `EXDATE` elements of the `icalendar` specification. These elements can be added while creating or editing events using `--rrule`, `--rdate`, `--exrule` and `--exdate` options.
+
+In most views, the instances of the recurring event are displayed. Since a recurring event can have an unlimited number of instances, searches with no start or end date can produce an unending series of events. By default therefore searches with no start or end date are limited to the previous five years and following five years. These defaults can be changed using the options ` --default_past_years` and `--default_future_years`
+
+## Raw ICS
+
+The `icalendar` specification is quite large and complex, and `icalcli` implements only the most common parts of this specification. It is possible to use the `--raw_ics` option to create/edit event using raw ICS text. 
+
 ## Screenshots
 
 Some screenshots are available at Github:
 
 #### Agenda and Week Views
 
 ![Agenda and Week Views]( https://github.com/jrvarma/icalcli/raw/master/screenshots/icalci-0-agenda-week-views.png)
```

### Comparing `icalcli-1.0.4/icalcli/argparsers.py` & `icalcli-1.0.5/icalcli/argparsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -259,14 +259,19 @@
     agenda.add_argument('-n', "--days", type=int, default=5, nargs="?")
 
     calw = sub.add_parser(
         "calw", aliases=['w'],
         parents=[outputs_parser, output_parser, cal_query_parser])
     calw.add_argument('-n', "--weeks", type=int, default=2, nargs="?")
 
+    cal5w = sub.add_parser(
+        "cal5w", aliases=['5w'],
+        parents=[outputs_parser, output_parser, cal_query_parser])
+    cal5w.add_argument('-n', "--weeks", type=int, default=2, nargs="?")
+
     sub.add_parser(
         "calm", aliases=['m'],
         parents=[outputs_parser, output_parser, cal_query_parser])
 
     # sub.add_parser("interactive", aliases=['i'])
 
     add = sub.add_parser("add", aliases=['a'],
```

### Comparing `icalcli-1.0.4/icalcli/etesync_backend/etesync_crud.py` & `icalcli-1.0.5/icalcli/etesync_backend/etesync_crud.py`

 * *Files identical despite different names*

### Comparing `icalcli-1.0.4/icalcli/etesync_backend/etesync_interface.py` & `icalcli-1.0.5/icalcli/etesync_backend/etesync_interface.py`

 * *Files identical despite different names*

### Comparing `icalcli-1.0.4/icalcli/file_backend/ics_interface.py` & `icalcli-1.0.5/icalcli/file_backend/ics_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,48 +8,61 @@
         r"""Initialize ICSInterface
 
         Parameters
         ----------
         filename : path to ics file
         backup: boolean whether to back up old file before overwriting
         """
-        self.filepath = Path(filename).resolve()
+        if isinstance(filename, list):
+            self.filepaths = [Path(f).resolve() for f in filename]
+            self.readonly = True
+        else:
+            self.filepaths = [Path(filename).resolve()]
+            self.readonly = False
         self.backup = backup
-        with open(self.filepath, 'r') as fp:
-            self.ics = fp.read()
+        self.ics = []
         self.all_events()
 
     def all_events(self):
         def check_event(event):
             if event.errors:
                 print("iCalendar error:\n{:} while parsing\n{:}".format(
                     event.errors, event.to_ical().decode()))
                 return False
             else:
                 return True
-        self.calendar = Calendar.from_ical(self.ics)
-        self.events = [ev for ev in self.calendar.walk('VEVENT')
-                       if check_event(ev)]
+        self.events = []
         self.cache_events = {}
-        for ev in self.events:
-            uid = ev.decoded('uid').decode()
-            self.cache_events[uid] = ev
+        filecount = 0
+        for path in self.filepaths:
+            with open(path, 'r') as fp:
+                cal = Calendar.from_ical(fp.read())
+            events = [ev for ev in cal.walk('VEVENT') if check_event(ev)]
+            self.events += events
+            for ev in events:
+                uid = ev.decoded('uid').decode()
+                if len(self.filepaths) > 1:
+                    uid = f"File{filecount}:{uid}"
+                self.cache_events[uid] = ev
+            filecount += 1
 
     def create_event(self, event, vtimezone=None):
         uid = event.decoded('uid').decode()
         self.cache_events[uid] = event
 
     def update_event(self, event, vtimezone=None):
         uid = event.decoded('uid').decode()
         self.cache_events[uid] = event
 
     def delete_event(self, uid):
         del self.cache_events[uid]
 
     def sync(self, vtimezone=None):
+        if self.readonly:
+            return
         if self.backup:
             with NamedTemporaryFile(mode='w',
                                     suffix=self.filepath.suffix,
                                     prefix=self.filepath.name,
                                     dir=self.filepath.parent,
                                     delete=False) as fp:
                 fp.write(self.ics)
```

### Comparing `icalcli-1.0.4/icalcli/icalcli.py` & `icalcli-1.0.5/icalcli/icalcli.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,23 +91,25 @@
     cache = {}
     allCals = []
     allEvents = []
 
     UNIWIDTH = {'W': 2, 'F': 2, 'N': 1, 'Na': 1, 'H': 1, 'A': 1}
     backend_cache_dirty = False
     default_outputs = ['end', 'alarms', 'freebusy', 'location']
+    default_graphical_outputs = ['end', 'alarms']
     no_past_events = 5
     no_future_events = 10
 
     def __init__(self, add_parser, backend_interface, printer,
                  **options):
 
         self.cals = []
         self.printer = printer
         self.initial_options = options
+        self.initial_options['stack_trace'] = True
         self.set_options(options)
         self.add_parser = add_parser
         self.backend_interface = backend_interface
         self.events = self.backend_interface.events.copy()
         self.check_duplicate_uids()
         self.setup_recurring_events()
         # stored as detail, but provided as option: TODO: fix that
@@ -124,14 +126,18 @@
         """
         self.options = options
         self.set_now()  # set self.now
         self.outputs = options.get('outputs', {})
         for key in self.default_outputs:
             if key not in self.outputs:
                 self.outputs[key] = True
+        self.graphical_outputs = options.get('outputs', {})
+        for key in self.default_graphical_outputs:
+            if key not in self.outputs:
+                self.graphical_outputs[key] = True
 
     def set_now(self):
         # This command is run at initiaization, but it should also be
         # run frequently to prevent self.now from becoming stale
         self.now = datetime.now(tzlocal())
 
         def offset(now, years):
@@ -153,14 +159,20 @@
         if len(set(self.uid(e) for e in self.events)) < len(self.events):
             # list to dict to list is a one-liner dedup
             self.events = list(
                 {self.uid(e): e for e in self.events}.values())
             self.readonly = True
             self.printer.err_msg('Duplicate UIDs found. '
                                  'Calendar deduplicated and set to readonly\n')
+        elif (
+                    hasattr(self.backend_interface, 'readonly')
+                    and self.backend_interface.readonly
+        ):
+            self.readonly = True
+            self.printer.err_msg('Calendar backend interface is readonly\n')
         else:
             self.readonly = False
 
     def setup_recurring_events(self):
         self.recur_uids = set(self.uid(e) for e in self.events
                               if 'RRULE' in e or 'RDATE' in e)
         if self.recur_uids:
@@ -319,39 +331,72 @@
 
         Returns
         -------
         boolean
         """
         return e_start < time_point and e_end >= time_point
 
-    def format_title(self, event, allday=False):
+    def event_summary(self, event, allday=False):
         r"""Return event title (summary and start time)
 
         Parameters
         ----------
         event : icalendar event
         allday : boolean
 
         Returns
         -------
         string
         """
+        def fmt_time(field):
+            if self.options['military']:
+                return self.decode_dtm(event, field).strftime("%H:%M")
+            else:
+                return (
+                    self.decode_dtm(event, field).strftime("%I:%M")
+                    .lstrip('0') +
+                    self.decode_dtm(event, field).strftime('%p') .lower())
         titlestr = self.valid_title(event)
         if allday:
-            return titlestr
-        elif self.options['military']:
-            return ' '.join(
-                [self.decode_dtm(event, 'dtstart').strftime("%H:%M"),
-                 titlestr])
-        else:
-            return ' '.join([
-                self.decode_dtm(event, 'dtstart').strftime("%I:%M")
-                .lstrip('0') +
-                self.decode_dtm(event, 'dtstart').strftime('%p')
-                .lower(), titlestr])
+            summary = titlestr
+        else:
+            tm = fmt_time('dtstart')
+            if self.graphical_outputs.get('end'):
+                tm += " - " + fmt_time('dtend')
+            summary = tm + " " + titlestr
+        if self.graphical_outputs.get('alarms'):
+            alarms = event.walk('valarm')
+            if alarms:
+                if isinstance(alarms[0].Decoded('trigger'), timedelta):
+                    minutes = -(alarms[0].Decoded('trigger')
+                                .total_seconds()/60)
+                    summary += ' AL:%.0fm' % minutes
+                else:
+                    summary += ' AL: ??'
+        if self.graphical_outputs.get('freebusy'):
+            free = ('transp' in event and
+                    event.Decoded('transp').decode() == 'TRANSPARENT')
+            summary += (' free ' if free else ' busy ')
+        if (
+                self.graphical_outputs.get('location')
+                and 'location' in event
+                and event.Decoded('location').decode().strip()
+        ):
+            summary += " [%s]" % (event.Decoded('location').
+                                  decode().strip())
+        if self.graphical_outputs.get('uid'):
+            summary += " <%s>" % (event.Decoded('uid').decode().strip())
+        # if (
+        #         self.graphical_outputs.get('description')
+        #         and 'description' in event
+        #         and event.Decoded('description').decode().strip()
+        #         and self.outputs.get('description')
+        # ):
+        #     summary += event.Decoded('description'). decode().strip()
+        return summary
 
     def get_week_events(self, start_dt, end_dt, event_list):
         r"""Returns all events during a week (start_dt to end_dt)
 
         Parameters
         ----------
         start_dt : datetime
@@ -397,17 +442,19 @@
             # which was started before current period of time and are
             # still continue in current period of time
             if event_is_today or (event_allday
                                   and event_continues_today):
                 force_now_marker = False
 
                 if to_show_now:
-                    if(self.now >= event_start_date
-                       and self.now <= event_end_date
-                       and not event_allday):
+                    if (
+                            self.now >= event_start_date
+                            and self.now <= event_end_date
+                            and not event_allday
+                    ):
                         # line marker is during event (recolor event)
                         force_now_marker = True
                         to_show_now = False
                     # elif (int(days_since_epoch(self.now)) <
                     #       int(days_since_epoch(event_start_date))):
                     #     force_now_marker = False
                     #     week_events[event_daynum - 1].append(
@@ -425,35 +472,35 @@
                         to_show_now = False
                 if force_now_marker:
                     event_color = self.options['color_now_marker']
                 else:
                     event_color = 'default'
                 # NOTE(slawqo): for all day events it's necessary to
                 # add event to more than one day in week_events
-                titlestr = self.format_title(event, allday=event_allday)
+                summary = self.event_summary(event, allday=event_allday)
                 if event_allday and event_start_date < event_end_date:
                     if event_end_date >= end_dt:
                         end_daynum = 6
                     else:
                         end_daynum = self.cal_monday(int(
                             event_end_date.strftime("%w")))
                     if event_start_date < start_dt:
                         start_daynum = 0
                     else:
                         start_daynum = event_daynum
                     # if event_daynum > end_daynum:
                     #     event_daynum = 0
                     for day in range(start_daynum, end_daynum + 1):
                         week_events[day].append(
-                            EventTitle('\n' + titlestr, event_color))
+                            EventTitle('\n' + summary, event_color))
                 else:
                     # newline and empty string are the keys to turn off
                     # coloring
                     week_events[event_daynum].append(
-                            EventTitle('\n' + titlestr, event_color))
+                            EventTitle('\n' + summary, event_color))
         return week_events
 
     def printed_len(self, string):
         r"""Find printed length of a string
 
         We need to treat everything as unicode for this to give
         us the info we want.  Data string comes in as `str` type
@@ -505,16 +552,18 @@
         int: where to cut the word
         """
         print_len = 0
 
         words = _u(string).split()
         for i, word in enumerate(words):
             word_len = self.printed_len(word)
-            if ((cur_print_len + word_len + print_len
-                 ) >= self.options['cal_width']):
+            if (
+                    (cur_print_len + word_len + print_len
+                     ) >= self.options['cal_width']
+            ):
                 cut_idx = len(' '.join(words[:i]))
                 # if the  word is too long,
                 # we cannot cut between words
                 if cut_idx == 0:
                     return self.word_cut(word)
                 return (print_len, cut_idx)
             print_len += word_len + i  # +i for the space between words
@@ -549,15 +598,15 @@
 
     def GraphEvents(self, cmd, startDateTime, count, eventList):
         r"""Constructs graphical display with weeks in rows,
         days of week in columns, and event strings in cells
 
         Parameters
         ----------
-        cmd : Command ('calw' or 'calm' for week and month)
+        cmd : Command ('calw', 'cal5w'  or 'calm' for week, 5weeks and month)
         startDateTime : datetime (start date)
         count : int (number of weeks or months)
         eventList : list of icalendar events
         """
 
         color_border = self.options['color_border']
 
@@ -633,28 +682,30 @@
             startDateTime = (startDateTime - timedelta(days=day_num))
         startWeekDateTime = startDateTime
         endWeekDateTime = (startWeekDateTime + timedelta(days=7))
 
         for i in range(count):
             # create and print the date line for a week
             for j in range(days):
-                if cmd == 'calw':
+                if cmd in ('calw', 'cal5w'):
                     d = (startWeekDateTime +
                          timedelta(days=j)).strftime("%d %b")
                 else:  # (cmd == 'calm'):
                     d = (startWeekDateTime +
                          timedelta(days=j)).strftime("%d")
                     if cur_month != (startWeekDateTime +
                                      timedelta(days=j)).strftime("%b"):
                         d = ''
                 tmpDateColor = self.options['color_date']
 
-                if (self.now.strftime("%d%b%Y") == (
-                        (startWeekDateTime + timedelta(days=j))
-                        .strftime("%d%b%Y"))):
+                if (
+                        self.now.strftime("%d%b%Y") == (
+                            (startWeekDateTime + timedelta(days=j))
+                            .strftime("%d%b%Y"))
+                ):
                     tmpDateColor = self.options['color_now_marker']
                     d += " **"
 
                 d += ' ' * (self.options['cal_width']
                             - self.printed_len(d))
 
                 # print dates
@@ -830,29 +881,33 @@
                     event.Decoded('transp').decode() == 'TRANSPARENT')
             self.printer.msg(' free ' if free else ' busy ',
                              eventColor)
 
         self.printer.msg('  %s' % self.valid_title(event).strip(),
                          eventColor)
 
-        if(self.outputs.get('location')
-           and 'location' in event
-           and event.Decoded('location').decode().strip()):
+        if (
+                self.outputs.get('location')
+                and 'location' in event
+                and event.Decoded('location').decode().strip()
+        ):
             xstr = " [%s]" % (event.Decoded('location').
                               decode().strip())
             self.printer.msg(xstr, 'default')
 
         if self.outputs.get('uid'):
             xstr = " <%s>" % (event.Decoded('uid').decode().strip())
             self.printer.msg(xstr, 'default')
 
         self.printer.msg('\n')
 
-        if(self.outputs.get('description') and 'description' in event
-           and event.Decoded('description').decode().strip()):
+        if (
+                self.outputs.get('description') and 'description' in event
+                and event.Decoded('description').decode().strip()
+        ):
             descrIndent = outputsIndent + '  '
             box = True  # leave old non-box code for option later
             if box:
                 topMarker = (descrIndent +
                              self.printer.art['ulc'] +
                              (self.printer.art['hrz'] *
                               ((self.outputs.get('width')
@@ -911,16 +966,18 @@
                                  'yellow')
 
         # 12 chars for day & length must match 'indent' in PrintEvent
         dayFormat = '\n%a %d-%b-%y' if yearDate else '\n%a %b %d  '
         day = ''
 
         for event in eventList:
-            if(self.options['ignore_started'] and
-               (self.decode_dtm(event, 'dtstart') < self.now)):
+            if (
+                    self.options['ignore_started'] and
+                    (self.decode_dtm(event, 'dtstart') < self.now)
+            ):
                 continue
             if self.options['ignore_declined'] and self._DeclinedEvent(
                     event):
                 continue
 
             selected += 1
             tmpDayStr = self.decode_dtm(event, 'dtstart').strftime(
@@ -1154,16 +1211,22 @@
                 if self.initial_options['stack_trace']:
                     print_exc()
                 return
 
         # convert start date to the beginning of the week or month
         if cmd == 'calw':
             dayNum = self.cal_monday(int(start.strftime("%w")))
-            start = (start - timedelta(days=dayNum))
-            end = (start + timedelta(days=(count * 7)))
+            start -= timedelta(days=dayNum)
+            weeks = count
+            end = (start + timedelta(days=(weeks * 7)))
+        elif cmd == 'cal5w':
+            dayNum = self.cal_monday(int(start.strftime("%w")))
+            start -= timedelta(days=(dayNum + count * 7))
+            weeks = 2 * count + 1
+            end = (start + timedelta(days=(weeks * 7)))
         else:  # cmd == 'calm':
             start = (start - timedelta(days=(start.day - 1)))
             endMonth = (start.month + 1)
             endYear = start.year
             if endMonth == 13:
                 endMonth = 1
                 endYear += 1
@@ -1171,21 +1234,21 @@
             daysInMonth = (end - start).days
             offsetDays = int(start.strftime('%w'))
             if self.options['cal_monday']:
                 offsetDays -= 1
                 if offsetDays < 0:
                     offsetDays = 6
             totalDays = (daysInMonth + offsetDays)
-            count = int(totalDays / 7)
+            weeks = int(totalDays / 7)
             if totalDays % 7:
-                count += 1
+                weeks += 1
 
         eventList = self.search_for_events(start, end, None)
 
-        self.GraphEvents(cmd, start, count, eventList)
+        self.GraphEvents(cmd, start, weeks, eventList)
 
     def sync(self):
         r"""Sync calendar
         """
         self.printer.msg("Syncing in progress\n")
         self.backend_interface.sync(self.vtimezone)
         self.events = self.backend_interface.events.copy()
@@ -1397,16 +1460,18 @@
             uid = old.Decoded('uid').decode()
             old_start = self.display_timezone(old.Decoded('dtstart'))
             old_duration = (
                 ('duration' in old and old.Decoded('duration')) or
                 (old.Decoded('dtend') - old.Decoded('dtstart')))
             if not args.summary:
                 args.summary = old.Decoded('summary').decode()
-            if(not args.time and not (args.start and 'T' in args.start)
-               and self.isallday(old)):
+            if (
+                    not args.time and not (args.start and 'T' in args.start)
+                    and self.isallday(old)
+            ):
                 args.allday = True
             day = args.day or old_start.day
             month = args.month or old_start.month
             year = args.year or old_start.year
         else:
             uid = "%s (%s)" % (datetime.now().isoformat(),
                                gethostname())
@@ -1686,14 +1751,18 @@
             ecal.AgendaQuery(start=FLAGS.start, end=FLAGS.end,
                              days=FLAGS.days)
 
         elif FLAGS.command in ['w', 'calw']:
             ecal.CalQuery(
                     'calw', count=FLAGS.weeks, startText=FLAGS.start)
 
+        elif FLAGS.command in ['5w', 'cal5w']:
+            ecal.CalQuery(
+                    'cal5w', count=FLAGS.weeks, startText=FLAGS.start)
+
         elif FLAGS.command in ['m', 'calm']:
             ecal.CalQuery('calm', startText=FLAGS.start)
 
         elif FLAGS.command in ['s', 'search']:
             ecal.TextQuery(FLAGS.text[0], start=FLAGS.start,
                            end=FLAGS.end,
                            # field='uid' if FLAGS.uid else 'summary')
@@ -1712,17 +1781,19 @@
 
         elif FLAGS.command in ['d', 'delete']:
             ecal.delete(FLAGS.text[0], start=FLAGS.start, end=FLAGS.end,
                         # field='uid' if FLAGS.uid else 'summary')
                         field=FLAGS.property)
 
         elif FLAGS.command in ['q', 'quit']:
-            if(ecal.backend_cache_dirty and ecal.no_auto_sync
-               and not IcalendarInterface.confirm(
-                   "Changes made in calendar not yet synced. Quit y/n? ")):
+            if (
+                    ecal.backend_cache_dirty and ecal.no_auto_sync
+                    and not IcalendarInterface.confirm(
+                        "Changes made in calendar not yet synced. Quit y/n? ")
+            ):
                 pass
             else:
                 ecal.interactive = False
 
     except Exception as exc:
         ecal.printer.err_msg(str(exc)+'\n')
         if ecal.initial_options['stack_trace']:
```

### Comparing `icalcli-1.0.4/icalcli/printer.py` & `icalcli-1.0.5/icalcli/printer.py`

 * *Files identical despite different names*

### Comparing `icalcli-1.0.4/icalcli/utils.py` & `icalcli-1.0.5/icalcli/utils.py`

 * *Files identical despite different names*

### Comparing `icalcli-1.0.4/icalcli.egg-info/PKG-INFO` & `icalcli-1.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icalcli
-Version: 1.0.4
+Version: 1.0.5
 Summary: Icalendar Calendar Command Line Interface
 Home-page: https://github.com/jrvarma/icalcli
 Maintainer: Jayanth R. Varma
 Maintainer-email: jrvarma@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -62,14 +62,15 @@
 ### Command line arguments
 
 `icalcli` provides a series of subcommands with the following functionality:
 
     edit (e)               edit calendar events
     agenda (g)             get an agenda for a time period
     calw (w)               get a week-based agenda in calendar format
+    cal5w (5w)             get this week / 2 past / 2 future weeks agenda in calendar format
     calm (m)               get a month agenda in calendar format
     add (a)                add a detailed event to the calendar
     search (s)             (regex) search for events 
     sync (y)               sync the backend calendar
     quit (q)               quit icalcli
 
 By default, `icalcli` runs interactively as an REPL (Read Evaluate Print Loop). Run `icalcli --help` for more details. `icalcli <subcommand> --help` gives help on each subcommand.
@@ -83,14 +84,23 @@
 ```
 from icalcli import ICSInterface
 
 backend_interface = ICSInterface("/path/to/ics-file")
 
 ```
 
+#### Example configuration for multiple readonly file_backend
+
+```
+from icalcli import ICSInterface
+
+backend_interface = ICSInterface(["/path/to/ics-file-1", "/path/to/ics-file-2"])
+
+```
+
 #### Example configuration for etesync_backend
 
 This configuration assumes that all the credentials are stored in a plain text (`json`) file. In practice, you would use a more secure storage (perhaps, the `Gnome keyring`) or just read it from the terminal.
 
 ```
 from icalcli import EtesyncInterface
 import base64
@@ -102,14 +112,24 @@
 backend_interface = EtesyncInterface(
     c['email'], c['userPassword'], c['remoteUrl'],
     c['uid'], c['authToken'],
     base64.decodebytes(c['cipher_key'].encode('ascii')))
 ```
 See the [Example code](https://github.com/jrvarma/icalcli/issues/1#issuecomment-979851222) for getting the  `uid` and `authToken` for the `etesync` calendar.
 
+## Recurring events and default search period
+
+`icalcli` understands the `RRULE`, `RDATE`, `EXRULE`, `EXDATE` elements of the `icalendar` specification. These elements can be added while creating or editing events using `--rrule`, `--rdate`, `--exrule` and `--exdate` options.
+
+In most views, the instances of the recurring event are displayed. Since a recurring event can have an unlimited number of instances, searches with no start or end date can produce an unending series of events. By default therefore searches with no start or end date are limited to the previous five years and following five years. These defaults can be changed using the options ` --default_past_years` and `--default_future_years`
+
+## Raw ICS
+
+The `icalendar` specification is quite large and complex, and `icalcli` implements only the most common parts of this specification. It is possible to use the `--raw_ics` option to create/edit event using raw ICS text. 
+
 ## Screenshots
 
 Some screenshots are available at Github:
 
 #### Agenda and Week Views
 
 ![Agenda and Week Views]( https://github.com/jrvarma/icalcli/raw/master/screenshots/icalci-0-agenda-week-views.png)
```

### Comparing `icalcli-1.0.4/setup.py` & `icalcli-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='icalcli',
-      version='1.0.4',
+      version='1.0.5',
       maintainer='Jayanth R. Varma',
       maintainer_email='jrvarma@gmail.com',
       description='Icalendar Calendar Command Line Interface',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/jrvarma/icalcli",
       packages=['icalcli', 'icalcli.etesync_backend', 'icalcli.file_backend'],
```

