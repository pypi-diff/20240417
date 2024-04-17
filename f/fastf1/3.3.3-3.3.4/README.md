# Comparing `tmp/fastf1-3.3.3.tar.gz` & `tmp/fastf1-3.3.4.tar.gz`

## Comparing `fastf1-3.3.3.tar` & `fastf1-3.3.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/README.rst
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/example_fastf1_signalrclient.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_annotate_corners.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_annotate_speed_trace.py
--rwxr-xr-x   0        0        0     2014 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_driver_laptimes.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_gear_shifts_on_track.py
--rwxr-xr-x   0        0        0     3163 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_laptimes_distribution.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_position_changes.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_qualifying_results.py
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_results_tracker.py
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_speed_on_track.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_speed_traces.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_strategy.py
--rwxr-xr-x   0        0        0     2053 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_team_pace_ranking.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_who_can_still_win_wdc.py
--rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/__init__.py
--rw-r--r--   0        0        0    74642 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/_api.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/_version.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/api.py
--rw-r--r--   0        0        0   153144 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/core.py
--rw-r--r--   0        0        0    38660 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/events.py
--rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/legacy.py
--rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/logger.py
--rw-r--r--   0        0        0    16355 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/plotting.py
--rw-r--r--   0        0        0    26173 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/req.py
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/utils.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/ergast/__init__.py
--rw-r--r--   0        0        0    61561 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/ergast/interface.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/ergast/legacy.py
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/ergast/sphinx.py
--rw-r--r--   0        0        0    18692 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/ergast/structure.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/internals/__init__.py
--rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/internals/pandas_base.py
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/internals/pandas_extensions.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/livetiming/__init__.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/livetiming/__main__.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/livetiming/client.py
--rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/livetiming/data.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/mvapi/__init__.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/mvapi/api.py
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/mvapi/data.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/mvapi/internals.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/LICENSE
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/README.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/__init__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/_connection.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/events/__init__.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/events/_events.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/hubs/__init__.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/hubs/_hub.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/transports/__init__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/transports/_exceptions.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/transports/_parameters.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/transports/_queue_events.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/transports/_transport.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 fastf1-3.3.3/requirements/dev.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fastf1-3.3.3/requirements/minver.txt
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastf1-3.3.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastf1-3.3.3/LICENSE
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 fastf1-3.3.3/README.md
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 fastf1-3.3.3/pyproject.toml
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fastf1-3.3.3/PKG-INFO
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/README.rst
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/example_fastf1_signalrclient.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_annotate_corners.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_annotate_speed_trace.py
+-rwxr-xr-x   0        0        0     2014 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_driver_laptimes.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_gear_shifts_on_track.py
+-rwxr-xr-x   0        0        0     3163 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_laptimes_distribution.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_position_changes.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_qualifying_results.py
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_results_tracker.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_speed_on_track.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_speed_traces.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_strategy.py
+-rwxr-xr-x   0        0        0     2053 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_team_pace_ranking.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_who_can_still_win_wdc.py
+-rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/__init__.py
+-rw-r--r--   0        0        0    74642 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/_api.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/_version.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/api.py
+-rw-r--r--   0        0        0   153144 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/core.py
+-rw-r--r--   0        0        0    41549 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/events.py
+-rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/legacy.py
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/logger.py
+-rw-r--r--   0        0        0    16355 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/plotting.py
+-rw-r--r--   0        0        0    26173 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/req.py
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/utils.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/ergast/__init__.py
+-rw-r--r--   0        0        0    61561 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/ergast/interface.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/ergast/legacy.py
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/ergast/sphinx.py
+-rw-r--r--   0        0        0    18692 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/ergast/structure.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/internals/__init__.py
+-rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/internals/pandas_base.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/internals/pandas_extensions.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/livetiming/__init__.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/livetiming/__main__.py
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/livetiming/client.py
+-rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/livetiming/data.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/mvapi/__init__.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/mvapi/api.py
+-rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/mvapi/data.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/mvapi/internals.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/LICENSE
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/README.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/__init__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/_connection.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/events/__init__.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/events/_events.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/hubs/__init__.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/hubs/_hub.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/transports/__init__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/transports/_exceptions.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/transports/_parameters.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/transports/_queue_events.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/transports/_transport.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 fastf1-3.3.4/requirements/dev.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fastf1-3.3.4/requirements/minver.txt
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastf1-3.3.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastf1-3.3.4/LICENSE
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 fastf1-3.3.4/README.md
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 fastf1-3.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fastf1-3.3.4/PKG-INFO
```

### Comparing `fastf1-3.3.3/examples/plot_annotate_corners.py` & `fastf1-3.3.4/examples/plot_annotate_corners.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/examples/plot_annotate_speed_trace.py` & `fastf1-3.3.4/examples/plot_annotate_speed_trace.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/examples/plot_driver_laptimes.py` & `fastf1-3.3.4/examples/plot_driver_laptimes.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/examples/plot_gear_shifts_on_track.py` & `fastf1-3.3.4/examples/plot_gear_shifts_on_track.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/examples/plot_laptimes_distribution.py` & `fastf1-3.3.4/examples/plot_laptimes_distribution.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/examples/plot_position_changes.py` & `fastf1-3.3.4/examples/plot_position_changes.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/examples/plot_qualifying_results.py` & `fastf1-3.3.4/examples/plot_qualifying_results.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/examples/plot_results_tracker.py` & `fastf1-3.3.4/examples/plot_results_tracker.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/examples/plot_speed_on_track.py` & `fastf1-3.3.4/examples/plot_speed_on_track.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/examples/plot_speed_traces.py` & `fastf1-3.3.4/examples/plot_speed_traces.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/examples/plot_strategy.py` & `fastf1-3.3.4/examples/plot_strategy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/examples/plot_team_pace_ranking.py` & `fastf1-3.3.4/examples/plot_team_pace_ranking.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/examples/plot_who_can_still_win_wdc.py` & `fastf1-3.3.4/examples/plot_who_can_still_win_wdc.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/__init__.py` & `fastf1-3.3.4/fastf1/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/_api.py` & `fastf1-3.3.4/fastf1/_api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/api.py` & `fastf1-3.3.4/fastf1/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/core.py` & `fastf1-3.3.4/fastf1/core.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/events.py` & `fastf1-3.3.4/fastf1/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
   - ``EventDate`` | :class:`pd.Timestamp` |
     The events reference date and time. This is used mainly internally.
     Usually, this is the same as the date of the last session.
 
   - ``EventFormat`` | :class:`str` |
     The format of the event. One of 'conventional', 'sprint',
-    'sprint_shootout', 'testing'.
+    'sprint_shootout', 'sprint_qualifying', 'testing'. See :ref:`event-formats`
 
   - ``Session*`` | :class:`str` |
     The name of the session. One of 'Practice 1', 'Practice 2', 'Practice 3',
     'Qualifying', 'Sprint', 'Sprint Shootout' or 'Race'.
     Testing sessions are considered practice.
     ``*`` denotes the number of
     the session (1, 2, 3, 4, 5).
@@ -68,15 +68,15 @@
     Lap timing data and telemetry data can only be loaded if this is true.
 
 
 Supported Seasons
 .................
 
 FastF1 provides its own event schedule for the 2018 season and all later
-seasons. The schedule for the all seasons before 2018 is built using data from
+seasons. The schedule for all seasons before 2018 is built using data from
 the Ergast API. Only limited data is available for these seasons. Usage of the
 Ergast API can be enforced for all seasons by setting ``backend='ergast'``,
 in which case the same limitations apply for the more recent seasons too.
 
 **Exact scheduled starting times for all sessions**:
 Supported starting with the 2018 season.
 Starting dates for sessions before 2018 (or when enforcing usage of the Ergast
@@ -86,43 +86,74 @@
 All other sessions are calculated from this and no starting times can be
 provided for these. These assumptions will be incorrect for certain events!
 
 **Testing events**: Supported for the 2020 season and later seasons. Not
 supported if usage of the Ergast API is enforced.
 
 
-Event Schedule
-..............
+.. _event-formats:
 
-- 'conventional': Practice 1, Practice 2, Practice 3, Qualifying, Race
-- 'sprint': Practice 1, Qualifying, Practice 2, Sprint, Race
-- 'sprint_shootout': Practice 1, Qualifying, Sprint Shootout, Sprint, Race
-- 'testing': no fixed session order; usually three practice sessions on
-  three separate days
+Event Formats
+.............
+
+- **'conventional': Practice 1, Practice 2, Practice 3, Qualifying, Race**
+
+- **'sprint': Practice 1, Qualifying, Practice 2, Sprint, Race**
+
+  This is the original sprint format that was used in some races in 2021 and
+  2022. The Qualifying on friday set the grid for the Sprint on saturday.
+  The results from the Sprint set the grid for the Race on sunday.
+
+- **'sprint_shootout': Practice 1, Qualifying, Sprint Shootout, Sprint, Race**
+
+  This format was used in 2023. The Qualifying on friday sets the grid for the
+  main Race on sunday. The Sprint Shootout on saturday is held in similar
+  fashion to a normal Qualifying session and sets the grid for the Sprint that
+  takes place on saturday as well.
+
+- **'sprint_qualifying': Practice 1, Sprint Qualifying, Sprint, Qualifying,
+  Race**
+
+  This format is used starting from 2024. In general, it is similar to the
+  previous 'sprint_shootout' format, but the order of the sessions was changed
+  and 'Sprint Shootout' is renamed to 'Sprint Qualifying'. This means that
+  the Sprint Qualifying on friday is held in similar fashion to a normal
+  Qualifying and sets the grid for the Sprint on saturday. The Qualifying later
+  on saturday then sets the grid for the race on Sunday.
+
+- **'testing': no fixed session order**
+
+  usually three practice sessions on three separate days
 
 
 .. _SessionIdentifier:
 
 Session identifiers
 -------------------
 
 Multiple event (schedule) related functions and methods make use of a session
 identifier to differentiate between the various sessions of one event.
 This identifier can currently be one of the following:
 
-    - session name abbreviation: ``'FP1', 'FP2', 'FP3', 'Q', 'S', 'SS', 'R'``
+    - session name abbreviation: ``'FP1', 'FP2', 'FP3', 'Q', 'S', 'SS', 'SQ',
+      'R'``
     - full session name: ``'Practice 1', 'Practice 2',
-      'Practice 3', 'Sprint', 'Sprint Shootout', 'Qualifying', 'Race'``;
+      'Practice 3', 'Sprint', 'Sprint Shootout', 'Sprint Qualifying',
+      'Qualifying', 'Race'``;
       provided names will be normalized, so that the name is
       case-insensitive
     - number of the session: ``1, 2, 3, 4, 5``
 
-Note that 'Sprint Qualifying' is now always called 'Sprint'.
-The event name will silently be corrected if you use 'Sprint Qualifying'/'SQ'
-instead of 'Sprint'/'S'.
+Note that the old ``'sprint'`` event format from 2021 and 2022 originally used
+the name 'Sprint Qualifying' before renaming these sessions to just 'Sprint'.
+The official schedule for 2021 now lists all these sessions as 'Sprint' and
+FastF1 will therefore return all these session as 'Sprint'. When querying for a
+specific session, FastF1 will also accept the 'Sprint Qualifying'/'SQ'
+identifier instead of only 'Sprint'/'S' for backwards compatibility.
+
 
 Functions for accessing schedule data
 -------------------------------------
 
 The functions for accessing event schedule data are documented in
 :ref:`GeneralFunctions`.
 
@@ -608,15 +639,15 @@
     schedule = EventSchedule(df, year=year, force_default_cols=True)
     return schedule
 
 
 @soft_exceptions("F1 API schedule",
                  "Failed to load schedule from F1 API backend!",
                  _logger)
-def _get_schedule_from_f1_timing(year):
+def _get_schedule_from_f1_timing(year: int):
     # create an event schedule using data from the F1 API
     response = fastf1._api.season_schedule(f'/static/{year}/')
     data = collections.defaultdict(list)
 
     for event in response:
         data['Country'].append(event['Country']['Name'])
         data['Location'].append(event['Location'])
@@ -629,28 +660,45 @@
             if (ses.get('Key') != -1) and ses.get('Name'):
                 sessions.append(ses)
 
         n_events = min(len(sessions), 5)
         # number of events, usually 3 for testing, 5 for race weekends
         # in special cases there are additional unrelated events
 
-        if (n_events >= 4) and ('Sprint' in sessions[3]['Name']):
+        if 'test' in event['Name'].lower():
+            data['EventFormat'].append('testing')
+            data['RoundNumber'].append(0)
+
+        elif year <= 2020:
+            data['EventFormat'].append('conventional')
+            data['RoundNumber'].append(event['Number'])
+
+        elif year in (2021, 2022):
             if sessions[3]['Name'] == 'Sprint Qualifying':
                 # fix for 2021 where Sprint was called Sprint Qualifying
                 sessions[3]['Name'] = 'Sprint'
+
+            if sessions[3]['Name'] == 'Sprint':
+                data['EventFormat'].append('sprint')
+            else:
+                data['EventFormat'].append('conventional')
+            data['RoundNumber'].append(event['Number'])
+
+        elif year == 2023:
             if sessions[2]['Name'] == 'Sprint Shootout':
                 data['EventFormat'].append('sprint_shootout')
             else:
-                data['EventFormat'].append('sprint')
+                data['EventFormat'].append('conventional')
             data['RoundNumber'].append(event['Number'])
-        elif 'test' in event['Name'].lower():
-            data['EventFormat'].append('testing')
-            data['RoundNumber'].append(0)
-        else:
-            data['EventFormat'].append('conventional')
+
+        elif year >= 2024:
+            if sessions[1]['Name'] == 'Sprint Qualifying':
+                data['EventFormat'].append('sprint_qualifying')
+            else:
+                data['EventFormat'].append('conventional')
             data['RoundNumber'].append(event['Number'])
 
         data['F1ApiSupport'].append(True)
 
         for i in range(0, 5):
             # parse the up to five sessions for each event
             try:
@@ -703,45 +751,67 @@
             ).tz_localize(None)
         except dateutil.parser.ParserError:
             date = pd.NaT
         data['EventDate'].append(date)
 
         if 'Sprint' in rnd:
             # Ergast doesn't support sprint shootout format yet
-            data['EventFormat'].append(
-                "sprint_shootout" if year == 2023 else "sprint")
-            data['Session1'].append('Practice 1')
+            if year in (2021, 2022):
+                _format = 'sprint'
+                session_names = ['Practice 1', 'Qualifying', 'Practice 2',
+                                 'Sprint', 'Race']
+            elif year == 2023:
+                _format = 'sprint_shootout'
+                session_names = ['Practice 1', 'Qualifying', 'Sprint Shootout',
+                                 'Sprint', 'Race']
+            else:
+                _format = 'sprint_qualifying'
+                session_names = ['Practice 1', 'Sprint Qualifying', 'Sprint',
+                                 'Qualifying', 'Race']
+
+            data['EventFormat'].append(_format)
+
+            data['Session1'].append(session_names[0])
             data['Session1DateUtc'].append(
                 date.floor('D') - pd.Timedelta(days=2))
-            data['Session2'].append('Qualifying')
+
+            data['Session2'].append(session_names[1])
             data['Session2DateUtc'].append(
                 date.floor('D') - pd.Timedelta(days=2))
-            data['Session3'].append(
-                'Sprint Shootout' if year == 2023 else 'Practice 2')
+
+            data['Session3'].append(session_names[2])
             data['Session3DateUtc'].append(
                 date.floor('D') - pd.Timedelta(days=1))
-            data['Session4'].append('Sprint')
+
+            data['Session4'].append(session_names[3])
             data['Session4DateUtc'].append(
                 date.floor('D') - pd.Timedelta(days=1))
-            data['Session5'].append('Race')
+
+            data['Session5'].append(session_names[4])
             data['Session5DateUtc'].append(date)
+
         else:
             data['EventFormat'].append("conventional")
+
             data['Session1'].append('Practice 1')
             data['Session1DateUtc'].append(
                 date.floor('D') - pd.Timedelta(days=2))
+
             data['Session2'].append('Practice 2')
             data['Session2DateUtc'].append(
                 date.floor('D') - pd.Timedelta(days=2))
+
             data['Session3'].append('Practice 3')
             data['Session3DateUtc'].append(
                 date.floor('D') - pd.Timedelta(days=1))
+
             data['Session4'].append('Qualifying')
             data['Session4DateUtc'].append(
                 date.floor('D') - pd.Timedelta(days=1))
+
             data['Session5'].append('Race')
             data['Session5DateUtc'].append(date)
 
         data['F1ApiSupport'].append(True if year >= 2018 else False)
         # simplified; this is only true most of the time
 
     df = pd.DataFrame(data)
@@ -983,16 +1053,20 @@
             else:
                 try:
                     session_name = \
                         _SESSION_TYPE_ABBREVIATIONS[identifier.upper()]
                 except KeyError:
                     raise ValueError(f"Invalid session type '{identifier}'")
 
-            # 'Sprint' is called 'Sprint Qualifying' only in 2021
-            if session_name == 'Sprint Qualifying':
+            # 'Sprint' was originally called 'Sprint Qualifying' only in the
+            # old 'sprint' event format and renamed later; support the old
+            # name for backwards compatibility by silently correcting to the
+            # new name
+            if ((session_name == 'Sprint Qualifying')
+                    and (self.year in (2021, 2022))):
                 session_name = 'Sprint'
 
             if session_name not in self.values:
                 raise ValueError(f"Session type '{identifier}' does not "
                                  f"exist for this event")
         else:
             # by number
@@ -1079,13 +1153,17 @@
         """Return the sprint session."""
         return self.get_session('Sprint')
 
     def get_sprint_shootout(self) -> "Session":
         """Return the sprint shootout session."""
         return self.get_session('Sprint Shootout')
 
+    def get_sprint_qualifying(self) -> "Session":
+        """Return the sprint qualifying session."""
+        return self.get_session('Sprint Qualifying')
+
     def get_practice(self, number: int) -> "Session":
         """Return the specified practice session.
         Args:
             number: 1, 2 or 3 - Free practice session number
         """
         return self.get_session(f'Practice {number}')
```

### Comparing `fastf1-3.3.3/fastf1/legacy.py` & `fastf1-3.3.4/fastf1/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/logger.py` & `fastf1-3.3.4/fastf1/logger.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/plotting.py` & `fastf1-3.3.4/fastf1/plotting.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/req.py` & `fastf1-3.3.4/fastf1/req.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/utils.py` & `fastf1-3.3.4/fastf1/utils.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/ergast/interface.py` & `fastf1-3.3.4/fastf1/ergast/interface.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/ergast/legacy.py` & `fastf1-3.3.4/fastf1/ergast/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/ergast/sphinx.py` & `fastf1-3.3.4/fastf1/ergast/sphinx.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/ergast/structure.py` & `fastf1-3.3.4/fastf1/ergast/structure.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/internals/pandas_base.py` & `fastf1-3.3.4/fastf1/internals/pandas_base.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/internals/pandas_extensions.py` & `fastf1-3.3.4/fastf1/internals/pandas_extensions.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/livetiming/__init__.py` & `fastf1-3.3.4/fastf1/livetiming/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/livetiming/__main__.py` & `fastf1-3.3.4/fastf1/livetiming/__main__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/livetiming/client.py` & `fastf1-3.3.4/fastf1/livetiming/client.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/livetiming/data.py` & `fastf1-3.3.4/fastf1/livetiming/data.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/mvapi/api.py` & `fastf1-3.3.4/fastf1/mvapi/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/mvapi/data.py` & `fastf1-3.3.4/fastf1/mvapi/data.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/signalr_aio/LICENSE` & `fastf1-3.3.4/fastf1/signalr_aio/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/signalr_aio/_connection.py` & `fastf1-3.3.4/fastf1/signalr_aio/_connection.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/signalr_aio/hubs/_hub.py` & `fastf1-3.3.4/fastf1/signalr_aio/hubs/_hub.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/signalr_aio/transports/_parameters.py` & `fastf1-3.3.4/fastf1/signalr_aio/transports/_parameters.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/fastf1/signalr_aio/transports/_transport.py` & `fastf1-3.3.4/fastf1/signalr_aio/transports/_transport.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/.gitignore` & `fastf1-3.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/LICENSE` & `fastf1-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/README.md` & `fastf1-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/pyproject.toml` & `fastf1-3.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.3/PKG-INFO` & `fastf1-3.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fastf1
-Version: 3.3.3
+Version: 3.3.4
 Summary: Python package for accessing and analyzing Formula 1 results, schedules, timing data and telemetry.
 Project-URL: Source Code, https://github.com/theOehrly/Fast-F1
 Project-URL: Documentation, https://docs.fastf1.dev
 Author: Philipp Schaefer
 Author-email: oehrly@mailbox.org
 License: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: fastf1 Version: 3.3.3 Summary: Python package for
+Metadata-Version: 2.3 Name: fastf1 Version: 3.3.4 Summary: Python package for
 accessing and analyzing Formula 1 results, schedules, timing data and
 telemetry. Project-URL: Source Code, https://github.com/theOehrly/Fast-F1
 Project-URL: Documentation, https://docs.fastf1.dev Author: Philipp Schaefer
 Author-email: oehrly@mailbox.org License: MIT License Copyright (c) 2024
 Philipp SchÃ¤fer Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
```

