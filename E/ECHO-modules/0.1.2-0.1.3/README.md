# Comparing `tmp/echo_modules-0.1.2.tar.gz` & `tmp/echo_modules-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echo_modules-0.1.2.tar", last modified: Mon Feb  5 23:51:55 2024, max compression
+gzip compressed data, was "echo_modules-0.1.3.tar", last modified: Wed Apr 17 20:21:31 2024, max compression
```

## Comparing `echo_modules-0.1.2.tar` & `echo_modules-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     6148 2024-02-05 23:51:55.000000 echo_modules-0.1.2/ECHO_modules/.DS_Store
--rw-r--r--   0        0        0    14324 2024-02-05 23:51:55.000000 echo_modules-0.1.2/ECHO_modules/DataSet.py
--rw-r--r--   0        0        0     5289 2024-02-05 23:51:55.000000 echo_modules-0.1.2/ECHO_modules/DataSetResults.py
--rw-r--r--   0        0        0       22 2024-02-05 23:51:55.000000 echo_modules-0.1.2/ECHO_modules/__init__.py
--rw-r--r--   0        0        0      908 2024-02-05 23:51:55.000000 echo_modules-0.1.2/ECHO_modules/correct_counties.py
--rw-r--r--   0        0        0     9204 2024-02-05 23:51:55.000000 echo_modules-0.1.2/ECHO_modules/data_set_presets.py
--rw-r--r--   0        0        0     3849 2024-02-05 23:51:55.000000 echo_modules-0.1.2/ECHO_modules/geographies.py
--rw-r--r--   0        0        0     6353 2024-02-05 23:51:55.000000 echo_modules-0.1.2/ECHO_modules/get_data.py
--rw-r--r--   0        0        0     2663 2024-02-05 23:51:55.000000 echo_modules-0.1.2/ECHO_modules/make_data_sets.py
--rw-r--r--   0        0        0    33024 2024-02-05 23:51:55.000000 echo_modules-0.1.2/ECHO_modules/utilities.py
--rw-r--r--   0        0        0    35149 2024-02-05 23:51:55.000000 echo_modules-0.1.2/LICENSE
--rw-r--r--   0        0        0    13701 2024-02-05 23:51:55.000000 echo_modules-0.1.2/README.md
--rw-r--r--   0        0        0     1105 2024-02-05 23:51:55.000000 echo_modules-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    14711 1970-01-01 00:00:00.000000 echo_modules-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-04-17 20:21:31.000000 echo_modules-0.1.3/ECHO_modules/.DS_Store
+-rw-r--r--   0        0        0    14324 2024-04-17 20:21:31.000000 echo_modules-0.1.3/ECHO_modules/DataSet.py
+-rw-r--r--   0        0        0     5289 2024-04-17 20:21:31.000000 echo_modules-0.1.3/ECHO_modules/DataSetResults.py
+-rw-r--r--   0        0        0       22 2024-04-17 20:21:31.000000 echo_modules-0.1.3/ECHO_modules/__init__.py
+-rw-r--r--   0        0        0      908 2024-04-17 20:21:31.000000 echo_modules-0.1.3/ECHO_modules/correct_counties.py
+-rw-r--r--   0        0        0     9204 2024-04-17 20:21:31.000000 echo_modules-0.1.3/ECHO_modules/data_set_presets.py
+-rw-r--r--   0        0        0     3849 2024-04-17 20:21:31.000000 echo_modules-0.1.3/ECHO_modules/geographies.py
+-rw-r--r--   0        0        0     6353 2024-04-17 20:21:31.000000 echo_modules-0.1.3/ECHO_modules/get_data.py
+-rw-r--r--   0        0        0     2663 2024-04-17 20:21:31.000000 echo_modules-0.1.3/ECHO_modules/make_data_sets.py
+-rw-r--r--   0        0        0    34355 2024-04-17 20:21:31.000000 echo_modules-0.1.3/ECHO_modules/utilities.py
+-rw-r--r--   0        0        0    35149 2024-04-17 20:21:31.000000 echo_modules-0.1.3/LICENSE
+-rw-r--r--   0        0        0    13690 2024-04-17 20:21:31.000000 echo_modules-0.1.3/README.md
+-rw-r--r--   0        0        0     1105 2024-04-17 20:21:31.000000 echo_modules-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    14700 1970-01-01 00:00:00.000000 echo_modules-0.1.3/PKG-INFO
```

### Comparing `echo_modules-0.1.2/ECHO_modules/.DS_Store` & `echo_modules-0.1.3/ECHO_modules/.DS_Store`

 * *Files identical despite different names*

### Comparing `echo_modules-0.1.2/ECHO_modules/DataSet.py` & `echo_modules-0.1.3/ECHO_modules/DataSet.py`

 * *Files identical despite different names*

### Comparing `echo_modules-0.1.2/ECHO_modules/DataSetResults.py` & `echo_modules-0.1.3/ECHO_modules/DataSetResults.py`

 * *Files identical despite different names*

### Comparing `echo_modules-0.1.2/ECHO_modules/correct_counties.py` & `echo_modules-0.1.3/ECHO_modules/correct_counties.py`

 * *Files identical despite different names*

### Comparing `echo_modules-0.1.2/ECHO_modules/data_set_presets.py` & `echo_modules-0.1.3/ECHO_modules/data_set_presets.py`

 * *Files identical despite different names*

### Comparing `echo_modules-0.1.2/ECHO_modules/geographies.py` & `echo_modules-0.1.3/ECHO_modules/geographies.py`

 * *Files identical despite different names*

### Comparing `echo_modules-0.1.2/ECHO_modules/get_data.py` & `echo_modules-0.1.3/ECHO_modules/get_data.py`

 * *Files identical despite different names*

### Comparing `echo_modules-0.1.2/ECHO_modules/make_data_sets.py` & `echo_modules-0.1.3/ECHO_modules/make_data_sets.py`

 * *Files identical despite different names*

### Comparing `echo_modules-0.1.2/ECHO_modules/utilities.py` & `echo_modules-0.1.3/ECHO_modules/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -264,35 +264,40 @@
         description='Data sets:',
         disabled=False,
     ) 
     display(data_set_widget)
     return data_set_widget
 
 
-def show_fac_widget( fac_series ):
+def show_fac_widget( fac_series, top_violators ):
     '''
     Create and return a dropdown list of facilities from the 
-    input Series
+    input Series. Pre-select the facilities identified in
+    top_violators.
 
     Parameters
     ----------
     fac_series : Series
         The facilities to be shown.  It may have duplicates.
 
+    top_violators : Dataframe
+        The top violators in the region.
+
     Returns
     -------
     widget
         The widget with facility names
     '''
-
+    selected = list(set(fac_series) & set(top_violators))
     fac_list = fac_series.dropna().unique()
     fac_list.sort()
     style = {'description_width': 'initial'}
     widget=widgets.SelectMultiple(
         options=fac_list,
+        value=selected,
         style=style,
         layout=Layout(width='70%'),
         description='Facility Name:',
         disabled=False,
     )
     display(widget)
     return widget
@@ -363,15 +368,15 @@
             zc_str = ",".join( map( lambda x: "\'"+str(x)+"\'", regions_selected.split(',') ))
             sql = 'select * from "ECHO_EXPORTER" where "FAC_ZIP" in ({})'
             sql += ' and "FAC_ACTIVE_FLAG" = \'Y\''
             sql = sql.format( zc_str )
             df_active = get_echo_data( sql, 'REGISTRY_ID' )
         elif ( region_type == 'Watershed' ):
             regions_selected = ''.join(regions_selected.split())
-            ws_str = ",".join( map( lambda x: "\'"+str(x)+"\'", regions_selected.split(',') ))
+            zc_str = ",".join( map( lambda x: "\'"+str(x)+"\'", regions_selected.split(',') ))
             sql = 'select * from "ECHO_EXPORTER" where "FAC_DERIVED_HUC" in ({})'
             sql += ' and "FAC_ACTIVE_FLAG" = \'Y\''
             sql = sql.format( ws_str )
             df_active = get_echo_data( sql, 'REGISTRY_ID' )
         else:
             df_active = None
         if ( region_type == 'County' ):
@@ -791,27 +796,29 @@
         The data to write.
     base: str
         A base string of the file to write
     type: str
         The region type of the data
     state: str
         The state, or None
-    regions: list
+    regions: tuple
         The region identifiers, e.g. CD number, County, State, Zip code
     '''
     if ( df is not None and len( df ) > 0 ):
         if ( not os.path.exists( 'CSVs' )):
             os.makedirs( 'CSVs' )
         filename = 'CSVs/' + base[:50]
         if ( type != 'Zip Code' and type != 'Watershed' ):
             filename += '-' + state
         filename += '-' + type
+
         if ( regions is not None ):
             for region in regions:
                 filename += '-' + str(region)
+        filename = filename.replace('\'', '').replace(',', '-')
         filename = urllib.parse.quote_plus(filename, safe='/')
         filename += '.csv'
         df.to_csv( filename ) 
         print( "Wrote " + filename )
     else:
         print( "There is no data to write." )
 
@@ -903,14 +910,42 @@
             'DFR_URL', 'FAC_LAT', 'FAC_LONG']]
     df_active = df_active[df_active['noncomp_count'] > 0]
     df_active = df_active.sort_values( by=['noncomp_count', action_field], 
             ascending=False )
     df_active = df_active.head( num_fac )
     return df_active   
 
+
+def get_tri_ghg_violators(df_active, field, num_violators):
+    df = df_active.loc[df_active[field]  > 0]
+    df_a = df.copy()
+    df_a = df_a[['FAC_NAME', field, 'DFR_URL', 'FAC_LAT', 'FAC_LONG']]
+    df_a = df_a.sort_values(by=[field], ascending=False)
+    df_a = df_a.head(num_violators)
+    return df_a
+
+# def get_sdwa_violators(df_active, num_violators):
+# use SDWA_FORMAL_ACTION_COUNT ?
+    
+
+def chart_tri_ghg_violators(df, field, title, xlabel):
+    unit = df.index
+    values = df[field]
+    sns.set(style='whitegrid')
+    fig, ax = plt.subplots(figsize=(10,10))
+    try:
+      g = sns.barplot(x=values, y=unit, order=list(unit), orient='h', color=colour)
+      g.set_title(title)
+      ax.set_xlabel(xlabel)
+      ax.set_ylabel('Facility')
+      ax.set_yticklabels(df['FAC_NAME'])
+    except TypeError as te:
+      print("TypeError: {}".format(str(te)))
+
+
 def chart_top_violators( ranked, state, selections, epa_pgm ):
     '''
     Draw a horizontal bar chart of the top non-compliant facilities.
 
     Parameters
     ----------
     ranked : Dataframe
@@ -929,16 +964,20 @@
     '''
     if ranked is None:
         print( 'There is no {} data to graph.'.format( epa_pgm ))
         return None
     unit = ranked.index 
     values = ranked['noncomp_count'] 
     if ( len(values) == 0 ):
-        return "No {} facilities with non-compliant quarters in {} - {}".format(
-            epa_pgm, state, str( selections ))
+        if state == None:
+            return "No {} facilities with non-compliant quarters in {}".format(
+                epa_pgm, str(selections))
+        else:
+            return "No {} facilities with non-compliant quarters in {} - {}".format(
+                epa_pgm, state, str( selections ))
     sns.set(style='whitegrid')
     fig, ax = plt.subplots(figsize=(10,10))
     try:
         g = sns.barplot(x=values, y=unit, order=list(unit), orient="h", color = colour) 
         g.set_title('{} facilities with the most non-compliant quarters in {} - {}'.format( 
                 epa_pgm, state, str( selections )))
         ax.set_xlabel("Non-compliant quarters")
```

### Comparing `echo_modules-0.1.2/LICENSE` & `echo_modules-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `echo_modules-0.1.2/README.md` & `echo_modules-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ECHO_modules 
 ===============================
 [![Download Latest Version from PyPI](https://img.shields.io/pypi/v/echo-modules.svg)](https://pypi.python.org/pypi/echo-modules)
 [![Code of Conduct](https://img.shields.io/badge/%E2%9D%A4-code%20of%20conduct-blue.svg?style=flat)](https://github.com/edgi-govdata-archiving/overview/blob/main/CONDUCT.md)
 
-*ECHO_modules* is a Python package repository for analyzing a copy of the US Environmental Protection Agency's (EPA) Enforcement and Compliance History Online (ECHO) database.
+*ECHO_modules* is a Python package for analyzing a copy of the US Environmental Protection Agency's (EPA) Enforcement and Compliance History Online (ECHO) database.
 
 Background
 --------------------------
 The US EPA collects a wide variety of data concerning environmental pollution and makes this available through several portals. The ECHO database collates information on industrial facilities' compliance with environmental protection laws like the Clean Water Act and regulatory agencies' enforcement of those laws. ECHO records reported violations, agency inspections of facilities, penalties paid by companies for infractions. It also incorporates information from other sources, such as reported pollutant releases from the Toxics Release Inventory and socio-economic information from EJScreen.
 
 Unfortunately, both the web portal for ECHO (echo.epa.gov) and its API have a number of limitations. First, EPA generally only makes the past 3-5 years worth of data available through these services. Second, EPA typically does not allow aggregating information into meaningful views, such as reports of inspections by Census tract or ZIP code. Instead, searches on echo.epa.gov are usually facility-oriented. This makes it hard to understand the state of environmental enforcement and compliance across an entire geography, company, or industry sector.
```

### Comparing `echo_modules-0.1.2/pyproject.toml` & `echo_modules-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ECHO_modules"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
 	{name = "Steve Hansen", email = "steven.e.hansen@gmail.com"}, 
 	{name="Eric Nost", email="enost@uoguelph.ca" }, 
 	{name="Kelsey Breseman", email="ifoundthemeaningoflife@gmail.com" }, 
 	{name = "EDGI", email = "contact@envirodatagov.org"}
 ]
 readme = "README.md"
```

### Comparing `echo_modules-0.1.2/PKG-INFO` & `echo_modules-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ECHO_modules
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package for analyzing the US Environmental Protection Agency's Enforcement and Compliance History Online database
 Author-email: Steve Hansen <steven.e.hansen@gmail.com>, Eric Nost <enost@uoguelph.ca>, Kelsey Breseman <ifoundthemeaningoflife@gmail.com>, EDGI <contact@envirodatagov.org>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Dist: folium>=0.14.0
@@ -20,15 +20,15 @@
 Project-URL: Issues, https://github.com/edgi-govdata-archiving/ECHO_modules/issues
 
 ECHO_modules 
 ===============================
 [![Download Latest Version from PyPI](https://img.shields.io/pypi/v/echo-modules.svg)](https://pypi.python.org/pypi/echo-modules)
 [![Code of Conduct](https://img.shields.io/badge/%E2%9D%A4-code%20of%20conduct-blue.svg?style=flat)](https://github.com/edgi-govdata-archiving/overview/blob/main/CONDUCT.md)
 
-*ECHO_modules* is a Python package repository for analyzing a copy of the US Environmental Protection Agency's (EPA) Enforcement and Compliance History Online (ECHO) database.
+*ECHO_modules* is a Python package for analyzing a copy of the US Environmental Protection Agency's (EPA) Enforcement and Compliance History Online (ECHO) database.
 
 Background
 --------------------------
 The US EPA collects a wide variety of data concerning environmental pollution and makes this available through several portals. The ECHO database collates information on industrial facilities' compliance with environmental protection laws like the Clean Water Act and regulatory agencies' enforcement of those laws. ECHO records reported violations, agency inspections of facilities, penalties paid by companies for infractions. It also incorporates information from other sources, such as reported pollutant releases from the Toxics Release Inventory and socio-economic information from EJScreen.
 
 Unfortunately, both the web portal for ECHO (echo.epa.gov) and its API have a number of limitations. First, EPA generally only makes the past 3-5 years worth of data available through these services. Second, EPA typically does not allow aggregating information into meaningful views, such as reports of inspections by Census tract or ZIP code. Instead, searches on echo.epa.gov are usually facility-oriented. This makes it hard to understand the state of environmental enforcement and compliance across an entire geography, company, or industry sector.
```

