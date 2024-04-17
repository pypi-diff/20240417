# Comparing `tmp/eflips_depot-3.0.2.tar.gz` & `tmp/eflips_depot-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips_depot-3.0.2.tar", max compression
+gzip compressed data, was "eflips_depot-3.0.3.tar", max compression
```

## Comparing `eflips_depot-3.0.2.tar` & `eflips_depot-3.0.3.tar`

### file list

```diff
@@ -1,59 +1,40 @@
--rw-r--r--   0        0        0    34143 2023-09-12 12:04:52.313847 eflips_depot-3.0.2/LICENSE.md
--rw-r--r--   0        0        0     4923 2024-01-30 11:53:09.584369 eflips_depot-3.0.2/README.md
--rw-r--r--   0        0        0     6148 2023-10-25 16:23:56.817889 eflips_depot-3.0.2/eflips/depot/.DS_Store
--rw-r--r--   0        0        0     1556 2023-09-18 10:32:47.648700 eflips_depot-3.0.2/eflips/depot/__init__.py
--rw-r--r--   0        0        0    48272 2024-04-08 08:44:07.631762 eflips_depot-3.0.2/eflips/depot/api/__init__.py
--rw-r--r--   0        0        0     9147 2024-01-15 12:09:04.913191 eflips_depot-3.0.2/eflips/depot/api/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    42910 2024-03-20 16:52:43.351740 eflips_depot-3.0.2/eflips/depot/api/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     5375 2024-03-19 13:55:55.791236 eflips_depot-3.0.2/eflips/depot/api/defaults/default_settings.json
--rw-r--r--   0        0        0        0 2024-03-20 16:37:13.222393 eflips_depot-3.0.2/eflips/depot/api/private/__init__.py
--rw-r--r--   0        0        0      186 2024-03-20 16:42:14.644098 eflips_depot-3.0.2/eflips/depot/api/private/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    16582 2024-03-20 16:52:43.354244 eflips_depot-3.0.2/eflips/depot/api/private/__pycache__/depot.cpython-312.pyc
--rw-r--r--   0        0        0     8963 2024-03-18 17:23:57.413115 eflips_depot-3.0.2/eflips/depot/api/private/__pycache__/depot_layout.cpython-312.pyc
--rw-r--r--   0        0        0    15908 2024-03-20 16:42:14.649900 eflips_depot-3.0.2/eflips/depot/api/private/__pycache__/util.cpython-312.pyc
--rw-r--r--   0        0        0    16594 2024-04-08 08:44:07.632141 eflips_depot-3.0.2/eflips/depot/api/private/depot.py
--rw-r--r--   0        0        0    15261 2024-03-20 16:37:13.222833 eflips_depot-3.0.2/eflips/depot/api/private/util.py
--rw-r--r--   0        0        0    35678 2024-03-19 13:55:55.792840 eflips_depot-3.0.2/eflips/depot/configuration.py
--rw-r--r--   0        0        0   105566 2024-04-08 08:44:07.632864 eflips_depot-3.0.2/eflips/depot/depot.py
--rw-r--r--   0        0        0   140842 2024-03-19 13:55:55.793916 eflips_depot-3.0.2/eflips/depot/evaluation.py
--rw-r--r--   0        0        0    15522 2023-09-18 10:44:13.224151 eflips_depot-3.0.2/eflips/depot/filters.py
--rw-r--r--   0        0        0     5569 2023-09-12 07:17:14.199982 eflips_depot-3.0.2/eflips/depot/input_epex_power_price.py
--rw-r--r--   0        0        0        0 2023-07-04 10:37:34.116338 eflips_depot-3.0.2/eflips/depot/layout_opt/__init__.py
--rw-r--r--   0        0        0      197 2023-07-04 13:45:08.435464 eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      185 2024-01-15 16:09:16.741928 eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    35672 2023-07-04 14:28:06.446062 eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/evaluation.cpython-311.pyc
--rw-r--r--   0        0        0    83908 2023-07-04 14:28:06.127266 eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/packing.cpython-311.pyc
--rw-r--r--   0        0        0     1378 2023-07-04 14:27:45.921545 eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0     5898 2023-07-04 14:28:06.443416 eflips_depot-3.0.2/eflips/depot/layout_opt/__pycache__/util.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-07-04 10:37:34.116399 eflips_depot-3.0.2/eflips/depot/layout_opt/doc/__init__.py
--rw-r--r--   0        0        0    22330 2023-07-04 10:37:34.116540 eflips_depot-3.0.2/eflips/depot/layout_opt/doc/direct_details.pdf
--rw-r--r--   0        0        0    24855 2023-11-27 13:13:21.354478 eflips_depot-3.0.2/eflips/depot/layout_opt/evaluation.py
--rw-r--r--   0        0        0      594 2023-09-12 07:17:14.200220 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__init__.py
--rw-r--r--   0        0        0     1114 2023-07-04 14:28:06.119012 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1871 2023-07-04 14:28:06.119582 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/crossover.cpython-311.pyc
--rw-r--r--   0        0        0    10041 2023-07-04 14:29:58.881420 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/fitness_c_urfd.cpython-311.pyc
--rw-r--r--   0        0        0     8052 2023-07-04 14:28:06.442624 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/fitness_util.cpython-311.pyc
--rw-r--r--   0        0        0    21433 2023-07-04 14:28:06.122179 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/init.cpython-311.pyc
--rw-r--r--   0        0        0    14402 2023-07-04 14:28:06.120785 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__pycache__/mutation.cpython-311.pyc
--rw-r--r--   0        0        0     1057 2023-07-04 10:37:34.116782 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/crossover.py
--rw-r--r--   0        0        0     8230 2024-03-19 13:55:55.794538 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py
--rw-r--r--   0        0        0     7027 2024-03-19 13:55:55.794746 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/fitness_util.py
--rw-r--r--   0        0        0    14707 2023-09-18 10:44:13.136159 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/init.py
--rw-r--r--   0        0        0    12238 2023-09-18 10:44:13.095315 eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/mutation.py
--rw-r--r--   0        0        0     9821 2023-11-27 13:13:21.355200 eflips_depot-3.0.2/eflips/depot/layout_opt/optimize_c_urfd.py
--rw-r--r--   0        0        0    56989 2023-11-27 13:13:21.355852 eflips_depot-3.0.2/eflips/depot/layout_opt/packing.py
--rw-r--r--   0        0        0      810 2023-09-12 07:17:14.201273 eflips_depot-3.0.2/eflips/depot/layout_opt/settings.py
--rw-r--r--   0        0        0     9736 2023-09-18 10:44:13.156260 eflips_depot-3.0.2/eflips/depot/layout_opt/template_creation.py
--rw-r--r--   0        0        0     3780 2023-09-18 10:44:13.048607 eflips_depot-3.0.2/eflips/depot/layout_opt/util.py
--rw-r--r--   0        0        0     2509 2023-10-26 12:56:09.063373 eflips_depot-3.0.2/eflips/depot/plots.py
--rw-r--r--   0        0        0    58757 2024-04-08 08:44:07.633396 eflips_depot-3.0.2/eflips/depot/processes.py
--rw-r--r--   0        0        0    16648 2023-09-18 10:44:12.914701 eflips_depot-3.0.2/eflips/depot/rating.py
--rw-r--r--   0        0        0    13568 2024-01-15 15:15:16.955650 eflips_depot-3.0.2/eflips/depot/resources.py
--rw-r--r--   0        0        0     2527 2023-09-24 11:00:36.366976 eflips_depot-3.0.2/eflips/depot/settings_config.py
--rw-r--r--   0        0        0     9375 2023-10-09 12:48:51.301551 eflips_depot-3.0.2/eflips/depot/simple_vehicle.py
--rw-r--r--   0        0        0    10676 2024-03-20 16:37:13.224092 eflips_depot-3.0.2/eflips/depot/simulation.py
--rw-r--r--   0        0        0    54311 2023-11-27 13:13:21.357629 eflips_depot-3.0.2/eflips/depot/smart_charging.py
--rw-r--r--   0        0        0    22338 2023-11-13 11:10:33.262925 eflips_depot-3.0.2/eflips/depot/standalone.py
--rw-r--r--   0        0        0     7097 2023-09-18 10:44:13.235715 eflips_depot-3.0.2/eflips/depot/validation.py
--rw-r--r--   0        0        0     1084 2024-04-08 08:50:00.210743 eflips_depot-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     5648 1970-01-01 00:00:00.000000 eflips_depot-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34143 2023-09-12 12:04:52.313847 eflips_depot-3.0.3/LICENSE.md
+-rw-r--r--   0        0        0     4923 2024-01-30 11:53:09.584369 eflips_depot-3.0.3/README.md
+-rw-r--r--   0        0        0     1556 2023-09-18 10:32:47.648700 eflips_depot-3.0.3/eflips/depot/__init__.py
+-rw-r--r--   0        0        0    50146 2024-04-17 15:24:47.935757 eflips_depot-3.0.3/eflips/depot/api/__init__.py
+-rw-r--r--   0        0        0     5375 2024-03-19 13:55:55.791236 eflips_depot-3.0.3/eflips/depot/api/defaults/default_settings.json
+-rw-r--r--   0        0        0        0 2024-03-20 16:37:13.222393 eflips_depot-3.0.3/eflips/depot/api/private/__init__.py
+-rw-r--r--   0        0        0    17136 2024-04-17 13:40:18.399085 eflips_depot-3.0.3/eflips/depot/api/private/depot.py
+-rw-r--r--   0        0        0    15261 2024-03-20 16:37:13.222833 eflips_depot-3.0.3/eflips/depot/api/private/util.py
+-rw-r--r--   0        0        0    35678 2024-03-19 13:55:55.792840 eflips_depot-3.0.3/eflips/depot/configuration.py
+-rw-r--r--   0        0        0   105566 2024-04-08 08:44:07.632864 eflips_depot-3.0.3/eflips/depot/depot.py
+-rw-r--r--   0        0        0   140842 2024-03-19 13:55:55.793916 eflips_depot-3.0.3/eflips/depot/evaluation.py
+-rw-r--r--   0        0        0    16131 2024-04-17 12:44:22.875673 eflips_depot-3.0.3/eflips/depot/filters.py
+-rw-r--r--   0        0        0     5569 2023-09-12 07:17:14.199982 eflips_depot-3.0.3/eflips/depot/input_epex_power_price.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:37:34.116338 eflips_depot-3.0.3/eflips/depot/layout_opt/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:37:34.116399 eflips_depot-3.0.3/eflips/depot/layout_opt/doc/__init__.py
+-rw-r--r--   0        0        0    22330 2023-07-04 10:37:34.116540 eflips_depot-3.0.3/eflips/depot/layout_opt/doc/direct_details.pdf
+-rw-r--r--   0        0        0    24855 2023-11-27 13:13:21.354478 eflips_depot-3.0.3/eflips/depot/layout_opt/evaluation.py
+-rw-r--r--   0        0        0      594 2023-09-12 07:17:14.200220 eflips_depot-3.0.3/eflips/depot/layout_opt/opt_tools/__init__.py
+-rw-r--r--   0        0        0     1057 2023-07-04 10:37:34.116782 eflips_depot-3.0.3/eflips/depot/layout_opt/opt_tools/crossover.py
+-rw-r--r--   0        0        0     8230 2024-03-19 13:55:55.794538 eflips_depot-3.0.3/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py
+-rw-r--r--   0        0        0     7027 2024-03-19 13:55:55.794746 eflips_depot-3.0.3/eflips/depot/layout_opt/opt_tools/fitness_util.py
+-rw-r--r--   0        0        0    14707 2023-09-18 10:44:13.136159 eflips_depot-3.0.3/eflips/depot/layout_opt/opt_tools/init.py
+-rw-r--r--   0        0        0    12238 2023-09-18 10:44:13.095315 eflips_depot-3.0.3/eflips/depot/layout_opt/opt_tools/mutation.py
+-rw-r--r--   0        0        0     9821 2023-11-27 13:13:21.355200 eflips_depot-3.0.3/eflips/depot/layout_opt/optimize_c_urfd.py
+-rw-r--r--   0        0        0    56989 2023-11-27 13:13:21.355852 eflips_depot-3.0.3/eflips/depot/layout_opt/packing.py
+-rw-r--r--   0        0        0      810 2023-09-12 07:17:14.201273 eflips_depot-3.0.3/eflips/depot/layout_opt/settings.py
+-rw-r--r--   0        0        0     9736 2023-09-18 10:44:13.156260 eflips_depot-3.0.3/eflips/depot/layout_opt/template_creation.py
+-rw-r--r--   0        0        0     3780 2023-09-18 10:44:13.048607 eflips_depot-3.0.3/eflips/depot/layout_opt/util.py
+-rw-r--r--   0        0        0     2509 2023-10-26 12:56:09.063373 eflips_depot-3.0.3/eflips/depot/plots.py
+-rw-r--r--   0        0        0    58757 2024-04-08 08:44:07.633396 eflips_depot-3.0.3/eflips/depot/processes.py
+-rw-r--r--   0        0        0    16648 2023-09-18 10:44:12.914701 eflips_depot-3.0.3/eflips/depot/rating.py
+-rw-r--r--   0        0        0    13568 2024-01-15 15:15:16.955650 eflips_depot-3.0.3/eflips/depot/resources.py
+-rw-r--r--   0        0        0     2527 2023-09-24 11:00:36.366976 eflips_depot-3.0.3/eflips/depot/settings_config.py
+-rw-r--r--   0        0        0     9375 2023-10-09 12:48:51.301551 eflips_depot-3.0.3/eflips/depot/simple_vehicle.py
+-rw-r--r--   0        0        0    10676 2024-03-20 16:37:13.224092 eflips_depot-3.0.3/eflips/depot/simulation.py
+-rw-r--r--   0        0        0    54311 2023-11-27 13:13:21.357629 eflips_depot-3.0.3/eflips/depot/smart_charging.py
+-rw-r--r--   0        0        0    22338 2023-11-13 11:10:33.262925 eflips_depot-3.0.3/eflips/depot/standalone.py
+-rw-r--r--   0        0        0     7097 2023-09-18 10:44:13.235715 eflips_depot-3.0.3/eflips/depot/validation.py
+-rw-r--r--   0        0        0     1084 2024-04-17 15:25:06.777804 eflips_depot-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5648 1970-01-01 00:00:00.000000 eflips_depot-3.0.3/PKG-INFO
```

### Comparing `eflips_depot-3.0.2/LICENSE.md` & `eflips_depot-3.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/README.md` & `eflips_depot-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/__init__.py` & `eflips_depot-3.0.3/eflips/depot/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/api/__init__.py` & `eflips_depot-3.0.3/eflips/depot/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     c. Use the :func:`add_evaluation_to_database` function to add the results to the database.
 4. For the results to be valid, the consumption simulation should now be run again.
     a. If you are using an external consumption model, run it again making sure it does not create new vehicles.
     b. Run the :func:`simple_consumption_simulation` function again, this time with ``initialize_vehicles=False``.
 """
 import copy
 import os
+import warnings
 from datetime import timedelta
 from math import ceil
 from typing import Any, Dict, Optional, Union
 
 import numpy as np
 import sqlalchemy.orm
 from eflips.model import (
@@ -37,14 +38,16 @@
     Depot,
     Event,
     EventType,
     Rotation,
     Scenario,
     Trip,
     Vehicle,
+    Process,
+    AssocAreaProcess,
 )
 from sqlalchemy.orm import Session
 from sqlalchemy.sql import select
 
 import eflips.depot
 from eflips.depot import DepotEvaluation, ProcessStatus, SimulationHost
 from eflips.depot.api.private.depot import (
@@ -525,21 +528,23 @@
                 raise ValueError(
                     "The vehicle count dictionary does not contain all vehicle types for depot {depot_id}."
                 )
             eflips.globalConstants["depot"]["vehicle_count"][
                 depot_id
             ] = vehicle_count_dict[depot_id]
         else:
-            # Calculate it from the size of the areas, with a 2x margin
+            # Calculate it from the size of the areas (except the area for the first standby process, which is already
+            # really large), with a 2x margin
             for vehicle_type in vehicle_types_for_depot:
                 vehicle_count = sum(
                     [
                         area.capacity
                         for area in depot.areas
                         if area.vehicle_type_id == int(vehicle_type)
+                        and depot.default_plan.processes[0] not in area.processes
                     ]
                 )
                 eflips.globalConstants["depot"]["vehicle_count"][depot_id][
                     vehicle_type
                 ] = (vehicle_count * 2)
 
     # We  need to put the vehicle type objects into the GlobalConstants
@@ -680,14 +685,15 @@
             # Flush the vehicle object to get the vehicle id
             session.add(current_vehicle_db)
             session.flush()
             list_of_vehicles.append(current_vehicle_db)
 
             dict_of_events = {}
 
+            # Generate process log for each schedule
             for finished_trip in current_vehicle.finished_trips:
                 dict_of_events[finished_trip.atd] = {
                     "type": "trip",
                     "is_copy": finished_trip.is_copy,
                     "id": finished_trip.ID,
                 }
 
@@ -706,14 +712,65 @@
             area_log = current_vehicle.logger.loggedData["dwd.current_area"]
             slot_log = current_vehicle.logger.loggedData["dwd.current_slot"]
 
             # For future uses
             waiting_log = current_vehicle.logger.loggedData["area_waiting_time"]
             battery_log = current_vehicle.battery_logs
 
+            # Create standby events according to waiting_log
+            waiting_log_timekeys = sorted(waiting_log.keys())
+
+            for idx in range(len(waiting_log_timekeys)):
+                end_time = waiting_log_timekeys[idx]
+                waiting_info = waiting_log[end_time]
+
+                if waiting_info["waiting_time"] == 0:
+                    continue
+
+                # Vehicle is waiting in the last area in waiting_log and expecting to enter the current area
+                expected_area = waiting_info["area"]
+                # Find the area for standby arrival event
+
+                waiting_area_id = (
+                    session.query(Area.id)
+                    .join(AssocAreaProcess, AssocAreaProcess.area_id == Area.id)
+                    .join(Process, Process.id == AssocAreaProcess.process_id)
+                    .filter(
+                        Process.dispatchable == False,
+                        Process.duration.is_(None),
+                        Process.electric_power.is_(None),
+                        Area.vehicle_type_id == int(current_vehicle.vehicle_type.ID),
+                        Area.scenario_id == scenario.id,
+                    )
+                    .one()[0]
+                )
+
+                # Make sure the vehicle is waiting at an area with enough capacity
+
+                current_slot = slot_log[waiting_log_timekeys[idx - 1]]
+
+                start_time = end_time - waiting_info["waiting_time"]
+
+                warnings.warn(
+                    f"Vehicle {current_vehicle.ID} is waiting at {waiting_area_id} because area {expected_area} is full."
+                )
+
+                dict_of_events[start_time] = {
+                    "type": "Standby",
+                    "end": end_time,
+                    "area": waiting_area_id,
+                    "slot": current_slot,
+                    "is_area_sink": waiting_area_id,
+                }
+
+            # Create a list of battery log in order of time asc. Convenient for looking up corresponding soc
+            battery_log_list = []
+            for log in battery_log:
+                battery_log_list.append((log.t, log.energy / log.energy_real))
+
             for start_time, process_log in current_vehicle.logger.loggedData[
                 "dwd.active_processes_copy"
             ].items():
                 if len(process_log) == 0:
                     # A departure happens
                     if last_standby_departure_start != 0:
                         # Update the last standby-departure end time
@@ -839,19 +896,19 @@
                                 )
 
                             case _:
                                 raise ValueError(
                                     f"Invalid process status {process.status} for process {process.ID}."
                                 )
 
-            time_keys = sorted(dict_of_events.keys(), reverse=True)
-            if len(time_keys) != 0:
+            reversed_time_keys = sorted(dict_of_events.keys(), reverse=True)
+            if len(reversed_time_keys) != 0:
                 # Generating valid event-list
                 is_copy = True
-                for start_time in time_keys:
+                for start_time in reversed_time_keys:
                     process_dict = dict_of_events[start_time]
                     if process_dict["type"] == "trip":
                         is_copy = process_dict["is_copy"]
                     else:
                         if is_copy is False:
                             # Generate EventType
                             match process_dict["type"]:
@@ -871,25 +928,39 @@
                                         'Invalid process type %s. Valid process types are "Serve", "Charge", '
                                         '"Standby", "Precondition"'
                                     )
 
                             # End time of 0-duration processes are start time of the next process
 
                             if "end" not in process_dict:
-                                end_time = time_keys[time_keys.index(start_time) - 1]
+                                # End time will be the one time key "later"
+                                end_time = reversed_time_keys[
+                                    reversed_time_keys.index(start_time) - 1
+                                ]
                                 process_dict["end"] = end_time
 
                             # Get soc
                             soc_start = None
                             soc_end = None
-                            for log in battery_log:
-                                if log.t == start_time:
-                                    soc_start = log.energy / log.energy_real
-                                if log.t == process_dict["end"]:
-                                    soc_end = log.energy / log.energy_real
+
+                            for i in range(len(battery_log_list)):
+                                log = battery_log_list[i]
+
+                                if log[0] == start_time:
+                                    soc_start = log[1]
+                                if log[0] == process_dict["end"]:
+                                    soc_end = log[1]
+                                if log[0] < start_time < battery_log_list[i + 1][0]:
+                                    soc_start = log[1]
+                                if (
+                                    log[0]
+                                    < process_dict["end"]
+                                    < battery_log_list[i + 1][0]
+                                ):
+                                    soc_end = log[1]
 
                             current_event = Event(
                                 scenario=scenario,
                                 vehicle_type_id=vehicle_type_id,
                                 vehicle=current_vehicle_db,
                                 station_id=None,
                                 area_id=int(process_dict["area"]),
@@ -913,20 +984,20 @@
                             session.add(current_event)
                             list_of_events_per_vehicle.append(current_event)
 
                 list_of_events.extend(list_of_events_per_vehicle)
 
                 # For non-copy schedules with no predecessor events, adding a dummy standby-departure
                 if (
-                    dict_of_events[time_keys[-1]]["type"] == "trip"
-                    and dict_of_events[time_keys[-1]]["is_copy"] is False
+                    dict_of_events[reversed_time_keys[-1]]["type"] == "trip"
+                    and dict_of_events[reversed_time_keys[-1]]["is_copy"] is False
                 ):
-                    standby_start = time_keys[-1] - 1
-                    standby_end = time_keys[-1]
-                    rotation_id = str(dict_of_events[time_keys[-1]]["id"])
+                    standby_start = reversed_time_keys[-1] - 1
+                    standby_end = reversed_time_keys[-1]
+                    rotation_id = str(dict_of_events[reversed_time_keys[-1]]["id"])
                     area = (
                         session.query(Area)
                         .filter(Area.vehicle_type_id == vehicle_type_id)
                         .first()
                     )
 
                     first_trip = (
@@ -957,67 +1028,33 @@
                         soc_start=soc,
                         soc_end=soc,
                         event_type=EventType.STANDBY_DEPARTURE,
                         description=f"DUMMY Standby event for {rotation_id}.",
                         timeseries=None,
                     )
 
+                    session.add(standby_event)
                     list_of_events.append(standby_event)
 
-        new_old_vehicle = {}
-        matched_vehicle_id = 0
-        for schedule_id, vehicle_id in list_of_assigned_schedules:
-            if vehicle_id != matched_vehicle_id:
-                matched_vehicle_id = vehicle_id
-                # Get rotation from db with id
-                rotation_q = session.query(Rotation).filter(Rotation.id == schedule_id)
-                # Match old and new vehicle id
-                old_vehicle_id = rotation_q.one().vehicle_id
-                new_old_vehicle[vehicle_id] = old_vehicle_id
-
         # New rotation assignment
-
         for schedule_id, vehicle_id in list_of_assigned_schedules:
             # Get corresponding old vehicle id
-            old_vehicle_id = new_old_vehicle[vehicle_id]
             session.query(Rotation).filter(Rotation.id == schedule_id).update(
-                {"vehicle_id": old_vehicle_id}, synchronize_session="auto"
+                {"vehicle_id": vehicle_id}, synchronize_session="auto"
             )
 
         # Delete all non-depot events
         session.query(Event).filter(
             Event.scenario == scenario,
             Event.trip_id.isnot(None) | Event.station_id.isnot(None),
-        ).delete()
-
-        session.flush()
-
-        # Update depot events with old vehicle id
-        for new_vehicle_id, old_vehicle_id in new_old_vehicle.items():
-            session.query(Event).filter(
-                Event.scenario == scenario,
-                Event.vehicle_id == new_vehicle_id,
-            ).update({"vehicle_id": old_vehicle_id}, synchronize_session="auto")
-
-            session.query(Vehicle).filter(
-                Vehicle.id == new_vehicle_id,
-            ).delete(synchronize_session="auto")
-
-            session.flush()
-
-        # Delete all non-depot events
-        session.query(Event).filter(
-            Event.scenario == scenario,
-            Event.trip_id.isnot(None) | Event.station_id.isnot(None),
         ).delete(synchronize_session="auto")
 
         session.flush()
 
         # Delete all vehicles without rotations
-
         vehicle_assigned_sq = (
             session.query(Rotation.vehicle_id)
             .filter(Rotation.scenario == scenario)
             .distinct()
             .subquery()
         )
```

### Comparing `eflips_depot-3.0.2/eflips/depot/api/defaults/default_settings.json` & `eflips_depot-3.0.3/eflips/depot/api/defaults/default_settings.json`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/api/private/depot.py` & `eflips_depot-3.0.3/eflips/depot/api/private/depot.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,18 +298,21 @@
 ) -> None:
     """
     Creates a simple depot for a given scenario.
 
     It has one area for each vehicle type and a charging process for each
     area. Also an arrival area for each vehicle type.
 
-    :param scenario:
-    :param station:
-    :param vehicle_type_dict:
-    :param session:
+    :param scenario: The scenario to be simulated
+    :param station: The station where the depot is located
+    :param charging_capacities: A dictionary of vehicle types and the number of vehicles that can be charged at the same time
+    :param cleaning_capacities: A dictionary of vehicle types and the number of vehicles that can be cleaned at the same time
+    :param charging_power: The power of the charging process
+    :param cleaning_duration: The duration of the cleaning process
+    :param session: An SQLAlchemy session object to the database
     :return: Nothing. Depots are created in the database.
     """
 
     # Create a simple depot
     depot = Depot(
         scenario=scenario,
         name=f"Depot at {station.name}",
@@ -350,54 +353,55 @@
     session.add(standby_arrival)
     session.add(clean)
     session.add(charging)
     session.add(standby_departure)
 
     for vehicle_type in charging_capacities.keys():
         charging_count = charging_capacities[vehicle_type]
-        # Add a safety margin of 20% to the parking capacity
-        charging_count = int(ceil(charging_count * 1.2))
-
-        # Create stand by arrival area
-        arrival_area = Area(
-            scenario=scenario,
-            name=f"Arrival for {vehicle_type.name_short}",
-            depot=depot,
-            area_type=AreaType.DIRECT_ONESIDE,
-            capacity=charging_count,
-        )
-        session.add(arrival_area)
-        arrival_area.vehicle_type = vehicle_type
+        # Add a safety margin of 100% to the parking capacity
+        charging_count = int(ceil(charging_count * 2))
 
         # Create charging area
         charging_area = Area(
             scenario=scenario,
             name=f"Direct Charging Area for {vehicle_type.name_short}",
             depot=depot,
             area_type=AreaType.DIRECT_ONESIDE,
             capacity=charging_count,
         )
         session.add(charging_area)
         charging_area.vehicle_type = vehicle_type
 
         # Create cleaning area
         cleaning_count = cleaning_capacities[vehicle_type]
-        # Add a safety margin of 20% to the parking capacity
-        cleaning_count = int(ceil(cleaning_count * 1.2))
+        # Add a safety margin of 100% to the parking capacity
+        cleaning_count = int(ceil(cleaning_count * 2))
 
         cleaning_area = Area(
             scenario=scenario,
             name=f"Cleaning Area for {vehicle_type.name_short}",
             depot=depot,
             area_type=AreaType.DIRECT_ONESIDE,
             capacity=cleaning_count,
         )
         session.add(cleaning_area)
         cleaning_area.vehicle_type = vehicle_type
 
+        # Create stand by arrival area
+        arrival_area = Area(
+            scenario=scenario,
+            name=f"Arrival for {vehicle_type.name_short}",
+            depot=depot,
+            area_type=AreaType.DIRECT_ONESIDE,
+            capacity=(charging_count + cleaning_count)
+            * 2,  # SHould be huge, not all of it will be used
+        )
+        session.add(arrival_area)
+        arrival_area.vehicle_type = vehicle_type
+
         arrival_area.processes.append(standby_arrival)
         cleaning_area.processes.append(clean)
         charging_area.processes.append(charging)
         charging_area.processes.append(standby_departure)
 
         assocs = [
             AssocPlanProcess(
```

### Comparing `eflips_depot-3.0.2/eflips/depot/api/private/util.py` & `eflips_depot-3.0.3/eflips/depot/api/private/util.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/configuration.py` & `eflips_depot-3.0.3/eflips/depot/configuration.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/depot.py` & `eflips_depot-3.0.3/eflips/depot/depot.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/evaluation.py` & `eflips_depot-3.0.3/eflips/depot/evaluation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/filters.py` & `eflips_depot-3.0.3/eflips/depot/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+import warnings
+
 import eflips
 from eflips.settings import globalConstants
 from eflips.helperFunctions import flexprint
 
 
 class VehicleFilter:
     """Class to build and apply filters for vehicles. Designed to work with
@@ -244,14 +246,26 @@
         elif globalConstants["depot"]["consumption_calc_mode"] == "soc_given":
             if self.trip.charge_on_track:
                 result = round(vehicle.battery.soc, 5) >= self.trip.start_soc
             else:
                 required_energy = (
                     self.trip.start_soc - self.trip.end_soc
                 ) * vehicle.battery.energy_real
+
+                # If the vehicle is fully charged and its fully charged energy is still lower than the required energy,
+                # dispatch anyway and warn the user
+                if (
+                    abs(vehicle.battery.soc - 1) < 1e-6
+                    and vehicle.battery.energy_real < required_energy
+                ):
+                    warnings.warn(
+                        f"Vehicle {vehicle.ID} is fully charged but the required energy for the trip is higher than the fully charged energy. Dispatching anyway."
+                    )
+                    return True
+
                 result = required_energy <= vehicle.battery.energy_remaining
 
         else:
             raise ValueError(
                 "Invalid value %s for 'consumption_calc_mode' in globalConstants."
                 % globalConstants["depot"]["consumption_calc_mode"]
             )
```

### Comparing `eflips_depot-3.0.2/eflips/depot/input_epex_power_price.py` & `eflips_depot-3.0.3/eflips/depot/input_epex_power_price.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/layout_opt/doc/direct_details.pdf` & `eflips_depot-3.0.3/eflips/depot/layout_opt/doc/direct_details.pdf`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/layout_opt/evaluation.py` & `eflips_depot-3.0.3/eflips/depot/layout_opt/evaluation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/__init__.py` & `eflips_depot-3.0.3/eflips/depot/layout_opt/opt_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/crossover.py` & `eflips_depot-3.0.3/eflips/depot/layout_opt/opt_tools/crossover.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py` & `eflips_depot-3.0.3/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/fitness_util.py` & `eflips_depot-3.0.3/eflips/depot/layout_opt/opt_tools/fitness_util.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/init.py` & `eflips_depot-3.0.3/eflips/depot/layout_opt/opt_tools/init.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/layout_opt/opt_tools/mutation.py` & `eflips_depot-3.0.3/eflips/depot/layout_opt/opt_tools/mutation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/layout_opt/optimize_c_urfd.py` & `eflips_depot-3.0.3/eflips/depot/layout_opt/optimize_c_urfd.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/layout_opt/packing.py` & `eflips_depot-3.0.3/eflips/depot/layout_opt/packing.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/layout_opt/settings.py` & `eflips_depot-3.0.3/eflips/depot/layout_opt/settings.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/layout_opt/template_creation.py` & `eflips_depot-3.0.3/eflips/depot/layout_opt/template_creation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/layout_opt/util.py` & `eflips_depot-3.0.3/eflips/depot/layout_opt/util.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/plots.py` & `eflips_depot-3.0.3/eflips/depot/plots.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/processes.py` & `eflips_depot-3.0.3/eflips/depot/processes.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/rating.py` & `eflips_depot-3.0.3/eflips/depot/rating.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/resources.py` & `eflips_depot-3.0.3/eflips/depot/resources.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/settings_config.py` & `eflips_depot-3.0.3/eflips/depot/settings_config.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/simple_vehicle.py` & `eflips_depot-3.0.3/eflips/depot/simple_vehicle.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/simulation.py` & `eflips_depot-3.0.3/eflips/depot/simulation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/smart_charging.py` & `eflips_depot-3.0.3/eflips/depot/smart_charging.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/standalone.py` & `eflips_depot-3.0.3/eflips/depot/standalone.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/eflips/depot/validation.py` & `eflips_depot-3.0.3/eflips/depot/validation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.2/pyproject.toml` & `eflips_depot-3.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "eflips-depot"
-version = "3.0.2"
+version = "3.0.3"
 description = "Depot Simulation for eFLIPS"
 authors = ["Enrico Lauth <enrico.lauth@tu-berlin.de>",
     "Ludger Heide <ludger.heide@tu-berlin.de",
     "Shuyao Guo <shuyao.guo@tu-berlin.de"]
 license = "AGPLv3"
 readme = "README.md"
 packages = [{ include = "eflips/depot" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 simpy = "^4.0.1"
-eflips-model = "^3.1.0"
+eflips-model = "^3.2.0"
 # Legacy dependencies, which are still needed until we refactor the code
-eflips = "^0.1.1"
+eflips = "^0.1.3"
 xlsxwriter = "^3.1.9"
 pandas = "^2.1.4"
 xlrd = "<=1.2.0"
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
```

### Comparing `eflips_depot-3.0.2/PKG-INFO` & `eflips_depot-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: eflips-depot
-Version: 3.0.2
+Version: 3.0.3
 Summary: Depot Simulation for eFLIPS
 License: AGPLv3
 Author: Enrico Lauth
 Author-email: enrico.lauth@tu-berlin.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: eflips (>=0.1.1,<0.2.0)
-Requires-Dist: eflips-model (>=3.1.0,<4.0.0)
+Requires-Dist: eflips (>=0.1.3,<0.2.0)
+Requires-Dist: eflips-model (>=3.2.0,<4.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: simpy (>=4.0.1,<5.0.0)
 Requires-Dist: xlrd (<=1.2.0)
 Requires-Dist: xlsxwriter (>=3.1.9,<4.0.0)
 Description-Content-Type: text/markdown
 
 [![Tests](https://github.com/mpm-tu-berlin/eflips-depot/actions/workflows/postgres_eflips_depot.yml/badge.svg)](https://github.com/mpm-tu-berlin/eflips-depot/actions/workflows/postgres_eflips_depot.yml)
```

