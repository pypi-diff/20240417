# Comparing `tmp/foxesscloud-2.2.3.tar.gz` & `tmp/foxesscloud-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-q84cp6_u\foxesscloud-2.2.3.tar", last modified: Tue Apr 16 08:09:37 2024, max compression
+gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-i2tqbp31\foxesscloud-2.2.4.tar", last modified: Wed Apr 17 10:07:31 2024, max compression
```

## Comparing `foxesscloud-2.2.3.tar` & `foxesscloud-2.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 08:09:37.000000 foxesscloud-2.2.3/
--rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.3/LICENCE
--rw-rw-rw-   0        0        0    39583 2024-04-16 08:09:37.000000 foxesscloud-2.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    39028 2024-04-16 08:01:34.000000 foxesscloud-2.2.3/README.md
--rw-rw-rw-   0        0        0      635 2024-04-16 08:01:43.000000 foxesscloud-2.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 08:09:37.000000 foxesscloud-2.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-16 08:09:37.000000 foxesscloud-2.2.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-16 08:09:37.000000 foxesscloud-2.2.3/src/foxesscloud/
--rw-rw-rw-   0        0        0   175907 2024-04-16 08:02:16.000000 foxesscloud-2.2.3/src/foxesscloud/foxesscloud.py
--rw-rw-rw-   0        0        0   170117 2024-04-16 08:02:16.000000 foxesscloud-2.2.3/src/foxesscloud/openapi.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:09:37.000000 foxesscloud-2.2.3/src/foxesscloud.egg-info/
--rw-rw-rw-   0        0        0    39583 2024-04-16 08:09:37.000000 foxesscloud-2.2.3/src/foxesscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-16 08:09:37.000000 foxesscloud-2.2.3/src/foxesscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 08:09:37.000000 foxesscloud-2.2.3/src/foxesscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 08:09:37.000000 foxesscloud-2.2.3/src/foxesscloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/
+-rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.4/LICENCE
+-rw-rw-rw-   0        0        0    39688 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    39133 2024-04-17 10:00:06.000000 foxesscloud-2.2.4/README.md
+-rw-rw-rw-   0        0        0      635 2024-04-17 09:50:25.000000 foxesscloud-2.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/src/foxesscloud/
+-rw-rw-rw-   0        0        0   175961 2024-04-17 10:05:41.000000 foxesscloud-2.2.4/src/foxesscloud/foxesscloud.py
+-rw-rw-rw-   0        0        0   170165 2024-04-17 10:05:34.000000 foxesscloud-2.2.4/src/foxesscloud/openapi.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/src/foxesscloud.egg-info/
+-rw-rw-rw-   0        0        0    39688 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/src/foxesscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/src/foxesscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/src/foxesscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/src/foxesscloud.egg-info/top_level.txt
```

### Comparing `foxesscloud-2.2.3/LICENCE` & `foxesscloud-2.2.4/LICENCE`

 * *Files identical despite different names*

### Comparing `foxesscloud-2.2.3/PKG-INFO` & `foxesscloud-2.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.2.3
+Version: 2.2.4
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -367,14 +367,15 @@
 special_days: ['12-25', '12-26', '01-01']
 full_charge: None             # day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue' etc
 derate_temp: 21               # battery temperature in C when derating charge current is applied
 derate_step: 5                # step size for derating e.g. 21, 16, 11
 derating: [24, 15, 10, 2]     # derated charge current for each temperature step e.g. 21C, 16C, 11C, 6C
 force: 1                      # 1 = disable strategy periods when setting charge. 0 = fail if strategy period has been set.
 data_wrap: 6                  # data items to show per line
+target_soc: None              # target soc for charging
 ```
 These values are stored / available in f.charge_config.
 
 The default battery open circuit voltage curve versus SoC from 0% to 100% is:
 ```
 lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50]
 ```
@@ -665,15 +666,16 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.3<br>
+2.2.4<br>
+Added 'target_soc' to charge_needed() settings
 Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50 where there is no battery
 Fix key error when accessing cell volts and temps using an agent / installer account.
 Ensure output is generated if get_battery() fails using battery_info().
 Update f.avg() to include calculation of averages in lists containng None values.
 Added 'data_wrap' to charge_config.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.3 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.4 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -272,41 +272,42 @@
 None special_contingency: 30 # contingency for special days when consumption
 might be higher special_days: ['12-25', '12-26', '01-01'] full_charge: None #
 day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue'
 etc derate_temp: 21 # battery temperature in C when derating charge current is
 applied derate_step: 5 # step size for derating e.g. 21, 16, 11 derating: [24,
 15, 10, 2] # derated charge current for each temperature step e.g. 21C, 16C,
 11C, 6C force: 1 # 1 = disable strategy periods when setting charge. 0 = fail
-if strategy period has been set. data_wrap: 6 # data items to show per line ```
-These values are stored / available in f.charge_config. The default battery
-open circuit voltage curve versus SoC from 0% to 100% is: ``` lifepo4_curve =
-[51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ```
-This example shows the results reported by charge needed: ![image](https://
-github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-
-20d806b1e7e8) ## Battery Info Provides detailed information on the current
-state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
-(interval, run, log, save, count) ``` battery_info() prints information on the
-battery and cells: + count: optional over-ride. The default is based on
-factorising the number of cells reported by 16 or 18 to work out the number of
-batteries. + plot: 1 plot the cell voltages for each battery, 2 plot the cell
-temperatueres, 0 don't plot. The default is 1 + log: see below. Default is 0
-battery_monitor() runs battery_info() in log mode on a schedule to provide
-information on the battery status over a period of time: + interval: the time
-in minutes between log entries. The default is 30 minutes + run: the number of
-log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
-total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
-cell temps. The default is 1 + save: name of a CSV file to write log data to +
-count: optional over-ride for the number of batteries This is an example of the
-output from battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/
-assets/63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ```
-f.date_list(s, e, limit, span, today) ``` Returns a list of dates in the format
-'YYYY-MM-DD'. This function will not return dates in the future. The last date
-will be yesterday or today (if today is True). All parameters are optional: +
-s: start date + e: end date + limit: maximum number of days. The default is 200
-+ span: the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
+if strategy period has been set. data_wrap: 6 # data items to show per line
+target_soc: None # target soc for charging ``` These values are stored /
+available in f.charge_config. The default battery open circuit voltage curve
+versus SoC from 0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30, 52.40,
+52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ``` This example shows the
+results reported by charge needed: ![image](https://github.com/TonyM1958/
+FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-20d806b1e7e8) ## Battery
+Info Provides detailed information on the current state of the batteries: ```
+f.battery_info(count, plot, log) f.battery_monitor(interval, run, log, save,
+count) ``` battery_info() prints information on the battery and cells: + count:
+optional over-ride. The default is based on factorising the number of cells
+reported by 16 or 18 to work out the number of batteries. + plot: 1 plot the
+cell voltages for each battery, 2 plot the cell temperatueres, 0 don't plot.
+The default is 1 + log: see below. Default is 0 battery_monitor() runs
+battery_info() in log mode on a schedule to provide information on the battery
+status over a period of time: + interval: the time in minutes between log
+entries. The default is 30 minutes + run: the number of log entries to create.
+The default is 48 i.e. every 30 minues for 24 hours in total + log: 0 =
+display, 1 = log battery info, 2 = add cell volts, 3 = add cell temps. The
+default is 1 + save: name of a CSV file to write log data to + count: optional
+over-ride for the number of batteries This is an example of the output from
+battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
+63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ``` f.date_list
+(s, e, limit, span, today) ``` Returns a list of dates in the format 'YYYY-MM-
+DD'. This function will not return dates in the future. The last date will be
+yesterday or today (if today is True). All parameters are optional: + s: start
+date + e: end date + limit: maximum number of days. The default is 200 + span:
+the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
 'weekday' + today: 1 allows today to be included, 2 allows future dates to be
 included. Default is 0, date list will stop at yesterday You can use 'span' as
 follows: + 'day' provides a single day + 'week' will provide the dates of 7
 consequetive days + 'month' will provide the dates of the days up to the same
 date in the preceeding (or follwing) month + '2days' will provide the dates of
 yesterday and today + 'weekday' will provide the dates of the same day of the
 week, going backwards (or forwards) up to 7 weeks ``` f.british_summer_time(d)
@@ -457,20 +458,21 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.3
-Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50
-where there is no battery Fix key error when accessing cell volts and temps
-using an agent / installer account. Ensure output is generated if get_battery()
-fails using battery_info(). Update f.avg() to include calculation of averages
-in lists containng None values. Added 'data_wrap' to charge_config. 2.1.9
+(verbose) # Version Info 2.2.4
+Added 'target_soc' to charge_needed() settings Fix bat_info() giving incorrect
+temperatures when API returns 0 instead of -50 where there is no battery Fix
+key error when accessing cell volts and temps using an agent / installer
+account. Ensure output is generated if get_battery() fails using battery_info
+(). Update f.avg() to include calculation of averages in lists containng None
+values. Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

### Comparing `foxesscloud-2.2.3/README.md` & `foxesscloud-2.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -353,14 +353,15 @@
 special_days: ['12-25', '12-26', '01-01']
 full_charge: None             # day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue' etc
 derate_temp: 21               # battery temperature in C when derating charge current is applied
 derate_step: 5                # step size for derating e.g. 21, 16, 11
 derating: [24, 15, 10, 2]     # derated charge current for each temperature step e.g. 21C, 16C, 11C, 6C
 force: 1                      # 1 = disable strategy periods when setting charge. 0 = fail if strategy period has been set.
 data_wrap: 6                  # data items to show per line
+target_soc: None              # target soc for charging
 ```
 These values are stored / available in f.charge_config.
 
 The default battery open circuit voltage curve versus SoC from 0% to 100% is:
 ```
 lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50]
 ```
@@ -651,15 +652,16 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.3<br>
+2.2.4<br>
+Added 'target_soc' to charge_needed() settings
 Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50 where there is no battery
 Fix key error when accessing cell volts and temps using an agent / installer account.
 Ensure output is generated if get_battery() fails using battery_info().
 Update f.avg() to include calculation of averages in lists containng None values.
 Added 'data_wrap' to charge_config.
```

#### html2text {}

```diff
@@ -265,41 +265,42 @@
 None special_contingency: 30 # contingency for special days when consumption
 might be higher special_days: ['12-25', '12-26', '01-01'] full_charge: None #
 day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue'
 etc derate_temp: 21 # battery temperature in C when derating charge current is
 applied derate_step: 5 # step size for derating e.g. 21, 16, 11 derating: [24,
 15, 10, 2] # derated charge current for each temperature step e.g. 21C, 16C,
 11C, 6C force: 1 # 1 = disable strategy periods when setting charge. 0 = fail
-if strategy period has been set. data_wrap: 6 # data items to show per line ```
-These values are stored / available in f.charge_config. The default battery
-open circuit voltage curve versus SoC from 0% to 100% is: ``` lifepo4_curve =
-[51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ```
-This example shows the results reported by charge needed: ![image](https://
-github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-
-20d806b1e7e8) ## Battery Info Provides detailed information on the current
-state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
-(interval, run, log, save, count) ``` battery_info() prints information on the
-battery and cells: + count: optional over-ride. The default is based on
-factorising the number of cells reported by 16 or 18 to work out the number of
-batteries. + plot: 1 plot the cell voltages for each battery, 2 plot the cell
-temperatueres, 0 don't plot. The default is 1 + log: see below. Default is 0
-battery_monitor() runs battery_info() in log mode on a schedule to provide
-information on the battery status over a period of time: + interval: the time
-in minutes between log entries. The default is 30 minutes + run: the number of
-log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
-total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
-cell temps. The default is 1 + save: name of a CSV file to write log data to +
-count: optional over-ride for the number of batteries This is an example of the
-output from battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/
-assets/63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ```
-f.date_list(s, e, limit, span, today) ``` Returns a list of dates in the format
-'YYYY-MM-DD'. This function will not return dates in the future. The last date
-will be yesterday or today (if today is True). All parameters are optional: +
-s: start date + e: end date + limit: maximum number of days. The default is 200
-+ span: the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
+if strategy period has been set. data_wrap: 6 # data items to show per line
+target_soc: None # target soc for charging ``` These values are stored /
+available in f.charge_config. The default battery open circuit voltage curve
+versus SoC from 0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30, 52.40,
+52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ``` This example shows the
+results reported by charge needed: ![image](https://github.com/TonyM1958/
+FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-20d806b1e7e8) ## Battery
+Info Provides detailed information on the current state of the batteries: ```
+f.battery_info(count, plot, log) f.battery_monitor(interval, run, log, save,
+count) ``` battery_info() prints information on the battery and cells: + count:
+optional over-ride. The default is based on factorising the number of cells
+reported by 16 or 18 to work out the number of batteries. + plot: 1 plot the
+cell voltages for each battery, 2 plot the cell temperatueres, 0 don't plot.
+The default is 1 + log: see below. Default is 0 battery_monitor() runs
+battery_info() in log mode on a schedule to provide information on the battery
+status over a period of time: + interval: the time in minutes between log
+entries. The default is 30 minutes + run: the number of log entries to create.
+The default is 48 i.e. every 30 minues for 24 hours in total + log: 0 =
+display, 1 = log battery info, 2 = add cell volts, 3 = add cell temps. The
+default is 1 + save: name of a CSV file to write log data to + count: optional
+over-ride for the number of batteries This is an example of the output from
+battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
+63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ``` f.date_list
+(s, e, limit, span, today) ``` Returns a list of dates in the format 'YYYY-MM-
+DD'. This function will not return dates in the future. The last date will be
+yesterday or today (if today is True). All parameters are optional: + s: start
+date + e: end date + limit: maximum number of days. The default is 200 + span:
+the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
 'weekday' + today: 1 allows today to be included, 2 allows future dates to be
 included. Default is 0, date list will stop at yesterday You can use 'span' as
 follows: + 'day' provides a single day + 'week' will provide the dates of 7
 consequetive days + 'month' will provide the dates of the days up to the same
 date in the preceeding (or follwing) month + '2days' will provide the dates of
 yesterday and today + 'weekday' will provide the dates of the same day of the
 week, going backwards (or forwards) up to 7 weeks ``` f.british_summer_time(d)
@@ -450,20 +451,21 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.3
-Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50
-where there is no battery Fix key error when accessing cell volts and temps
-using an agent / installer account. Ensure output is generated if get_battery()
-fails using battery_info(). Update f.avg() to include calculation of averages
-in lists containng None values. Added 'data_wrap' to charge_config. 2.1.9
+(verbose) # Version Info 2.2.4
+Added 'target_soc' to charge_needed() settings Fix bat_info() giving incorrect
+temperatures when API returns 0 instead of -50 where there is no battery Fix
+key error when accessing cell volts and temps using an agent / installer
+account. Ensure output is generated if get_battery() fails using battery_info
+(). Update f.avg() to include calculation of averages in lists containng None
+values. Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

### Comparing `foxesscloud-2.2.3/pyproject.toml` & `foxesscloud-2.2.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "foxesscloud"
-version = "2.2.3"
+version = "2.2.4"
 authors = [
   {name="Tony Matthews", email="tony@quasair.co.uk"},
 ]
 description = "library for accessing Fox ESS cloud data using Open API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `foxesscloud-2.2.3/src/foxesscloud/foxesscloud.py` & `foxesscloud-2.2.4/src/foxesscloud/foxesscloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud
-Updated:  16 April 2024
+Updated:  17 April 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud web site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2023
 ##################################################################################################
 
-version = "1.3.5"
+version = "1.3.6"
 print(f"FoxESS-Cloud version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -2363,15 +2363,16 @@
     'special_contingency': 33,        # contingency for special days when consumption might be higher
     'special_days': ['12-25', '12-26', '01-01'],
     'full_charge': None,              # day of month (1-28) to do full charge, or 'daily' or 'Mon', 'Tue' etc
     'derate_temp': 22,                # battery temperature where cold derating starts to be applied
     'derate_step': 5,                 # scale for derating factors in C
     'derating': [24, 15, 10, 2],      # max charge current e.g. 5C step = 22C, 17C, 12C, 7C
     'force': 1,                       # 0 = don't over-ride schedule, 1 = disable schedule
-    'data_wrap': 6                    # data to show per line
+    'data_wrap': 6,                   # data items to show per line
+    'target_soc': None                # set the target SoC for charging
 }
 
 # app key for charge_needed (used to send output via pushover)
 charge_needed_app_key = "awcr5gro2v13oher3v1qu6hwnovp28"
 
 # work out the charge times to set using the parameters:
 #  forecast: the kWh expected tomorrow. If none, forecast data is loaded from solcast etc
@@ -2759,33 +2760,36 @@
             kwh_current = capacity
         bat_timed.append(kwh_current)
         if kwh_current < kwh_min:       # track minimum and time
             kwh_min = kwh_current
             min_hour = h
         kwh_current += kwh_timed[i]
         h += 1
-    # work out what we need to add to stay above reserve and provide contingency
+    # work out what we need to add to stay above reserve and provide contingency or to hit target_soc
     output_spool(charge_needed_app_key)
     contingency = charge_config['special_contingency'] if tomorrow[-5:] in charge_config['special_days'] else charge_config['contingency']
     kwh_contingency = consumption * contingency / 100
     kwh_needed = reserve + kwh_contingency - kwh_min
-    day_when = 'today' if min_hour < 24 else 'tomorrow' if min_hour <= 48 else 'day after tomorrow'
     start_residual = interpolate(time_to_start, bat_timed)      # residual when charging starts
+    target_soc = charge_config['target_soc'] if charge_config.get('target_soc') is not None else 0
+    target_kwh = capacity if target_soc > 100 else target_soc / 100 * capacity
+    if target_kwh > (start_residual + kwh_needed):
+        kwh_needed = target_kwh - start_residual
+    day_when = 'today' if min_hour < 24 else 'tomorrow' if min_hour <= 48 else 'day after tomorrow'
     if kwh_min > reserve and kwh_needed < charge_config['min_kwh'] and full_charge is None and test_charge is None:
-        output(f"\nNo charging is needed, lowest forecast SoC = {kwh_min / capacity * 100:3.0f}% (Residual = {kwh_min:.2f}kWh)")
-        output(f"  Contingency of {kwh_contingency:.2f}kWh ({contingency}%) is available at {hours_time(min_hour)} {day_when}")
+        output(f"\nNo charging is needed")
         charge_message = "no charge needed"
         kwh_needed = 0.0
         hours = 0.0
         end1 = start_at
     else:
         charge_message = "with charge added"
         if test_charge is None:
             min_hour_adjust = min_hour - hour_adjustment if min_hour >= change_hour else 0
-            output(f"\nCharge of {kwh_needed:.2f} kWh is needed for a contingency of {kwh_contingency:.2f} kWh ({contingency}%) at {hours_time(min_hour_adjust)} {day_when}")
+            output(f"\nCharge of {kwh_needed:.2f}kWh is needed")
         else:
             output(f"\nTest charge of {test_charge}kWh")
             charge_message = "** test charge **"
             kwh_needed = test_charge
         # work out time to add kwh_needed to battery
         taper_time = 10/60 if (start_residual + kwh_needed) >= (capacity * 0.95) else 0
         hours = round_time(kwh_needed / (charge_limit * charge_loss + discharge_timed[time_to_next]) + taper_time)
```

### Comparing `foxesscloud-2.2.3/src/foxesscloud/openapi.py` & `foxesscloud-2.2.4/src/foxesscloud/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud using Open API
-Updated:  16 April 2024
+Updated:  17 April 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud api site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2024
 ##################################################################################################
 
-version = "2.2.3"
+version = "2.2.4"
 print(f"FoxESS-Cloud Open API version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -2233,15 +2233,16 @@
     'special_contingency': 33,        # contingency for special days when consumption might be higher
     'special_days': ['12-25', '12-26', '01-01'],
     'full_charge': None,              # day of month (1-28) to do full charge, or 'daily' or 'Mon', 'Tue' etc
     'derate_temp': 22,                # battery temperature where cold derating starts to be applied
     'derate_step': 5,                 # scale for derating factors in C
     'derating': [24, 15, 10, 2],      # max charge current e.g. 5C step = 22C, 17C, 12C, 7C
     'force': 1,                       # 0 = don't over-ride schedule, 1 = disable schedule
-    'data_wrap': 6                    # data items to show per line
+    'data_wrap': 6,                   # data items to show per line
+    'target_soc': None                # set the target SoC for charging
 }
 
 # app key for charge_needed (used to send output via pushover)
 charge_needed_app_key = "awcr5gro2v13oher3v1qu6hwnovp28"
 
 # work out the charge times to set using the parameters:
 #  forecast: the kWh expected tomorrow. If none, forecast data is loaded from solcast etc
@@ -2626,33 +2627,36 @@
             kwh_current = capacity
         bat_timed.append(kwh_current)
         if kwh_current < kwh_min:       # track minimum and time
             kwh_min = kwh_current
             min_hour = h
         kwh_current += kwh_timed[i]
         h += 1
-    # work out what we need to add to stay above reserve and provide contingency
+    # work out what we need to add to stay above reserve and provide contingency or to hit target_soc
     output_spool(charge_needed_app_key)
     contingency = charge_config['special_contingency'] if tomorrow[-5:] in charge_config['special_days'] else charge_config['contingency']
     kwh_contingency = consumption * contingency / 100
     kwh_needed = reserve + kwh_contingency - kwh_min
-    day_when = 'today' if min_hour < 24 else 'tomorrow' if min_hour <= 48 else 'day after tomorrow'
     start_residual = interpolate(time_to_start, bat_timed)      # residual when charging starts
+    target_soc = charge_config['target_soc'] if charge_config.get('target_soc') is not None else 0
+    target_kwh = capacity if target_soc > 100 else target_soc / 100 * capacity
+    if target_kwh > (start_residual + kwh_needed):
+        kwh_needed = target_kwh - start_residual
+    day_when = 'today' if min_hour < 24 else 'tomorrow' if min_hour <= 48 else 'day after tomorrow'
     if kwh_min > reserve and kwh_needed < charge_config['min_kwh'] and full_charge is None and test_charge is None:
-        output(f"\nNo charging is needed, lowest forecast SoC = {kwh_min / capacity * 100:3.0f}% (Residual = {kwh_min:.2f}kWh)")
-        output(f"  Contingency of {kwh_contingency:.2f}kWh ({contingency}%) is available at {hours_time(min_hour)} {day_when}")
+        output(f"\nNo charging is needed")
         charge_message = "no charge needed"
         kwh_needed = 0.0
         hours = 0.0
         end1 = start_at
     else:
         charge_message = "with charge added"
         if test_charge is None:
             min_hour_adjust = min_hour - hour_adjustment if min_hour >= change_hour else 0
-            output(f"\nCharge of {kwh_needed:.2f} kWh is needed for a contingency of {kwh_contingency:.2f} kWh ({contingency}%) at {hours_time(min_hour_adjust)} {day_when}")
+            output(f"\nCharge of {kwh_needed:.2f}kWh is needed")
         else:
             output(f"\nTest charge of {test_charge}kWh")
             charge_message = "** test charge **"
             kwh_needed = test_charge
         # work out time to add kwh_needed to battery
         taper_time = 10/60 if (start_residual + kwh_needed) >= (capacity * 0.95) else 0
         hours = round_time(kwh_needed / (charge_limit * charge_loss + discharge_timed[time_to_next]) + taper_time)
```

### Comparing `foxesscloud-2.2.3/src/foxesscloud.egg-info/PKG-INFO` & `foxesscloud-2.2.4/src/foxesscloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.2.3
+Version: 2.2.4
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -367,14 +367,15 @@
 special_days: ['12-25', '12-26', '01-01']
 full_charge: None             # day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue' etc
 derate_temp: 21               # battery temperature in C when derating charge current is applied
 derate_step: 5                # step size for derating e.g. 21, 16, 11
 derating: [24, 15, 10, 2]     # derated charge current for each temperature step e.g. 21C, 16C, 11C, 6C
 force: 1                      # 1 = disable strategy periods when setting charge. 0 = fail if strategy period has been set.
 data_wrap: 6                  # data items to show per line
+target_soc: None              # target soc for charging
 ```
 These values are stored / available in f.charge_config.
 
 The default battery open circuit voltage curve versus SoC from 0% to 100% is:
 ```
 lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50]
 ```
@@ -665,15 +666,16 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.3<br>
+2.2.4<br>
+Added 'target_soc' to charge_needed() settings
 Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50 where there is no battery
 Fix key error when accessing cell volts and temps using an agent / installer account.
 Ensure output is generated if get_battery() fails using battery_info().
 Update f.avg() to include calculation of averages in lists containng None values.
 Added 'data_wrap' to charge_config.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.3 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.4 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -272,41 +272,42 @@
 None special_contingency: 30 # contingency for special days when consumption
 might be higher special_days: ['12-25', '12-26', '01-01'] full_charge: None #
 day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue'
 etc derate_temp: 21 # battery temperature in C when derating charge current is
 applied derate_step: 5 # step size for derating e.g. 21, 16, 11 derating: [24,
 15, 10, 2] # derated charge current for each temperature step e.g. 21C, 16C,
 11C, 6C force: 1 # 1 = disable strategy periods when setting charge. 0 = fail
-if strategy period has been set. data_wrap: 6 # data items to show per line ```
-These values are stored / available in f.charge_config. The default battery
-open circuit voltage curve versus SoC from 0% to 100% is: ``` lifepo4_curve =
-[51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ```
-This example shows the results reported by charge needed: ![image](https://
-github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-
-20d806b1e7e8) ## Battery Info Provides detailed information on the current
-state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
-(interval, run, log, save, count) ``` battery_info() prints information on the
-battery and cells: + count: optional over-ride. The default is based on
-factorising the number of cells reported by 16 or 18 to work out the number of
-batteries. + plot: 1 plot the cell voltages for each battery, 2 plot the cell
-temperatueres, 0 don't plot. The default is 1 + log: see below. Default is 0
-battery_monitor() runs battery_info() in log mode on a schedule to provide
-information on the battery status over a period of time: + interval: the time
-in minutes between log entries. The default is 30 minutes + run: the number of
-log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
-total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
-cell temps. The default is 1 + save: name of a CSV file to write log data to +
-count: optional over-ride for the number of batteries This is an example of the
-output from battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/
-assets/63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ```
-f.date_list(s, e, limit, span, today) ``` Returns a list of dates in the format
-'YYYY-MM-DD'. This function will not return dates in the future. The last date
-will be yesterday or today (if today is True). All parameters are optional: +
-s: start date + e: end date + limit: maximum number of days. The default is 200
-+ span: the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
+if strategy period has been set. data_wrap: 6 # data items to show per line
+target_soc: None # target soc for charging ``` These values are stored /
+available in f.charge_config. The default battery open circuit voltage curve
+versus SoC from 0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30, 52.40,
+52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ``` This example shows the
+results reported by charge needed: ![image](https://github.com/TonyM1958/
+FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-20d806b1e7e8) ## Battery
+Info Provides detailed information on the current state of the batteries: ```
+f.battery_info(count, plot, log) f.battery_monitor(interval, run, log, save,
+count) ``` battery_info() prints information on the battery and cells: + count:
+optional over-ride. The default is based on factorising the number of cells
+reported by 16 or 18 to work out the number of batteries. + plot: 1 plot the
+cell voltages for each battery, 2 plot the cell temperatueres, 0 don't plot.
+The default is 1 + log: see below. Default is 0 battery_monitor() runs
+battery_info() in log mode on a schedule to provide information on the battery
+status over a period of time: + interval: the time in minutes between log
+entries. The default is 30 minutes + run: the number of log entries to create.
+The default is 48 i.e. every 30 minues for 24 hours in total + log: 0 =
+display, 1 = log battery info, 2 = add cell volts, 3 = add cell temps. The
+default is 1 + save: name of a CSV file to write log data to + count: optional
+over-ride for the number of batteries This is an example of the output from
+battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
+63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ``` f.date_list
+(s, e, limit, span, today) ``` Returns a list of dates in the format 'YYYY-MM-
+DD'. This function will not return dates in the future. The last date will be
+yesterday or today (if today is True). All parameters are optional: + s: start
+date + e: end date + limit: maximum number of days. The default is 200 + span:
+the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
 'weekday' + today: 1 allows today to be included, 2 allows future dates to be
 included. Default is 0, date list will stop at yesterday You can use 'span' as
 follows: + 'day' provides a single day + 'week' will provide the dates of 7
 consequetive days + 'month' will provide the dates of the days up to the same
 date in the preceeding (or follwing) month + '2days' will provide the dates of
 yesterday and today + 'weekday' will provide the dates of the same day of the
 week, going backwards (or forwards) up to 7 weeks ``` f.british_summer_time(d)
@@ -457,20 +458,21 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.3
-Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50
-where there is no battery Fix key error when accessing cell volts and temps
-using an agent / installer account. Ensure output is generated if get_battery()
-fails using battery_info(). Update f.avg() to include calculation of averages
-in lists containng None values. Added 'data_wrap' to charge_config. 2.1.9
+(verbose) # Version Info 2.2.4
+Added 'target_soc' to charge_needed() settings Fix bat_info() giving incorrect
+temperatures when API returns 0 instead of -50 where there is no battery Fix
+key error when accessing cell volts and temps using an agent / installer
+account. Ensure output is generated if get_battery() fails using battery_info
+(). Update f.avg() to include calculation of averages in lists containng None
+values. Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

