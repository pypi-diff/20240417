# Comparing `tmp/salure_helpers_datev-1.0.7.tar.gz` & `tmp/salure_helpers_datev-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_datev-1.0.7.tar", last modified: Tue Apr  9 09:24:55 2024, max compression
+gzip compressed data, was "dist/salure_helpers_datev-1.0.9.tar", last modified: Wed Apr 17 09:07:36 2024, max compression
```

## Comparing `salure_helpers_datev-1.0.7.tar` & `salure_helpers_datev-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:24:55.000000 salure_helpers_datev-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      259 2024-04-09 09:24:55.000000 salure_helpers_datev-1.0.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:24:55.000000 salure_helpers_datev-1.0.7/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:24:55.000000 salure_helpers_datev-1.0.7/salure_helpers/datev/
--rw-rw-rw-   0 root         (0) root         (0)      231 2024-04-09 09:24:39.000000 salure_helpers_datev-1.0.7/salure_helpers/datev/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30522 2024-04-09 09:24:39.000000 salure_helpers_datev-1.0.7/salure_helpers/datev/datev.py
--rw-rw-rw-   0 root         (0) root         (0)    83638 2024-04-09 09:24:39.000000 salure_helpers_datev-1.0.7/salure_helpers/datev/datev_lodas.py
--rw-rw-rw-   0 root         (0) root         (0)    32802 2024-04-09 09:24:39.000000 salure_helpers_datev-1.0.7/salure_helpers/datev/datev_lodas_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)     5621 2024-04-09 09:24:39.000000 salure_helpers_datev-1.0.7/salure_helpers/datev/datev_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:24:55.000000 salure_helpers_datev-1.0.7/salure_helpers_datev.egg-info/
--rw-r--r--   0 root         (0) root         (0)      259 2024-04-09 09:24:55.000000 salure_helpers_datev-1.0.7/salure_helpers_datev.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-09 09:24:55.000000 salure_helpers_datev-1.0.7/salure_helpers_datev.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 09:24:55.000000 salure_helpers_datev-1.0.7/salure_helpers_datev.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 09:24:55.000000 salure_helpers_datev-1.0.7/salure_helpers_datev.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-09 09:24:55.000000 salure_helpers_datev-1.0.7/salure_helpers_datev.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-09 09:24:55.000000 salure_helpers_datev-1.0.7/salure_helpers_datev.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 09:24:55.000000 salure_helpers_datev-1.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-09 09:24:39.000000 salure_helpers_datev-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:07:36.000000 salure_helpers_datev-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      259 2024-04-17 09:07:36.000000 salure_helpers_datev-1.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:07:36.000000 salure_helpers_datev-1.0.9/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:07:36.000000 salure_helpers_datev-1.0.9/salure_helpers/datev/
+-rw-rw-rw-   0 root         (0) root         (0)      231 2024-04-17 09:07:17.000000 salure_helpers_datev-1.0.9/salure_helpers/datev/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30522 2024-04-17 09:07:17.000000 salure_helpers_datev-1.0.9/salure_helpers/datev/datev.py
+-rw-rw-rw-   0 root         (0) root         (0)    83638 2024-04-17 09:07:17.000000 salure_helpers_datev-1.0.9/salure_helpers/datev/datev_lodas.py
+-rw-rw-rw-   0 root         (0) root         (0)    32802 2024-04-17 09:07:17.000000 salure_helpers_datev-1.0.9/salure_helpers/datev/datev_lodas_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)     5621 2024-04-17 09:07:17.000000 salure_helpers_datev-1.0.9/salure_helpers/datev/datev_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:07:36.000000 salure_helpers_datev-1.0.9/salure_helpers_datev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      259 2024-04-17 09:07:35.000000 salure_helpers_datev-1.0.9/salure_helpers_datev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      451 2024-04-17 09:07:35.000000 salure_helpers_datev-1.0.9/salure_helpers_datev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 09:07:35.000000 salure_helpers_datev-1.0.9/salure_helpers_datev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 09:07:35.000000 salure_helpers_datev-1.0.9/salure_helpers_datev.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-17 09:07:35.000000 salure_helpers_datev-1.0.9/salure_helpers_datev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-17 09:07:35.000000 salure_helpers_datev-1.0.9/salure_helpers_datev.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 09:07:36.000000 salure_helpers_datev-1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-17 09:07:17.000000 salure_helpers_datev-1.0.9/setup.py
```

### Comparing `salure_helpers_datev-1.0.7/salure_helpers/datev/datev.py` & `salure_helpers_datev-1.0.9/salure_helpers/datev/datev.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_datev-1.0.7/salure_helpers/datev/datev_lodas.py` & `salure_helpers_datev-1.0.9/salure_helpers/datev/datev_lodas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1200,15 +1200,15 @@
         """
 
         required_fields = ['employee_id', 'booking_date', 'value', 'declaration_type', 'wage_component']
         for field in required_fields:
             if field not in df.columns:
                 raise KeyError(f'Column {field} is required. Required columns are: {tuple(required_fields)}')
 
-        template_description = [f"309;u_lod_bwd_buchung_standard;{'pnr_betriebliche#bwd' if use_alternative_employee_number else 'pnr#bwd'};abrechnung_zeitraum#bwd;bs_wert_butab#bwd;bs_nr#bwd;kostenstelle#bwd;la_eigene#bwd;abw_lohnfaktor#bwd;\n"]
+        template_description = [f"309;u_lod_bwd_buchung_standard;{'pnr_betriebliche#psd' if use_alternative_employee_number else 'pnr#bwd'};abrechnung_zeitraum#bwd;bs_wert_butab#bwd;bs_nr#bwd;kostenstelle#bwd;la_eigene#bwd;abw_lohnfaktor#bwd;\n"]
 
         body = []
         for _, row in df.iterrows():
             formatted_string = (
                 f"309;"
                 f"{row['employee_id']};"
                 f"{row['booking_date'] if 'booking_date' in row.keys() else ''};"
```

### Comparing `salure_helpers_datev-1.0.7/salure_helpers/datev/datev_lodas_mapping.py` & `salure_helpers_datev-1.0.9/salure_helpers/datev/datev_lodas_mapping.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_datev-1.0.7/salure_helpers/datev/datev_mapping.py` & `salure_helpers_datev-1.0.9/salure_helpers/datev/datev_mapping.py`

 * *Files identical despite different names*

