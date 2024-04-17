# Comparing `tmp/pyriksdagen-1.0.0rc1.tar.gz` & `tmp/pyriksdagen-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriksdagen-1.0.0rc1.tar", max compression
+gzip compressed data, was "pyriksdagen-1.1.0.tar", max compression
```

## Comparing `pyriksdagen-1.0.0rc1.tar` & `pyriksdagen-1.1.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0     1107 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0      247 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/README.md
--rw-r--r--   0        0        0      850 2024-03-26 10:48:29.578000 pyriksdagen-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0       84 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/__init__.py
--rw-r--r--   0        0        0      286 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/alias.rq
--rw-r--r--   0        0        0      539 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/external_identifiers.rq
--rw-r--r--   0        0        0      494 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/government.rq
--rw-r--r--   0        0        0      777 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/member_of_parliament.rq
--rw-r--r--   0        0        0      148 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/member_of_parliament.txt
--rw-r--r--   0        0        0     1621 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/minister.rq
--rw-r--r--   0        0        0      235 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/minister.txt
--rw-r--r--   0        0        0      301 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/name_location_specifier.rq
--rw-r--r--   0        0        0      527 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/party_affiliation.rq
--rw-r--r--   0        0        0      588 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/person.rq
--rw-r--r--   0        0        0      277 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/place_of_birth.rq
--rw-r--r--   0        0        0      277 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/place_of_death.rq
--rw-r--r--   0        0        0      251 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/portraits.rq
--rw-r--r--   0        0        0      663 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/speaker.rq
--rw-r--r--   0        0        0      253 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/speaker.txt
--rw-r--r--   0        0        0      247 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/twitter.rq
--rw-r--r--   0        0        0      959 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/wiki_id.rq
--rw-r--r--   0        0        0      225 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/alias.rq
--rw-r--r--   0        0        0      482 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/government.rq
--rw-r--r--   0        0        0      722 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/member_of_parliament.rq
--rw-r--r--   0        0        0     1380 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/minister.rq
--rw-r--r--   0        0        0     1013 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/name_location_specifier.rq
--rw-r--r--   0        0        0     1230 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/party_affiliation.rq
--rw-r--r--   0        0        0     1412 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/person.rq
--rw-r--r--   0        0        0      616 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/speaker.rq
--rw-r--r--   0        0        0      959 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/twitter.rq
--rw-r--r--   0        0        0      798 2024-03-26 10:47:51.937759 pyriksdagen-1.0.0rc1/pyriksdagen/data/segmentation/detection.csv
--rw-r--r--   0        0        0     3355 2024-03-26 10:47:51.941759 pyriksdagen-1.0.0rc1/pyriksdagen/data/segmentation/patterns.json
--rw-r--r--   0        0        0     2195 2024-03-26 10:47:51.941759 pyriksdagen-1.0.0rc1/pyriksdagen/dataset.py
--rw-r--r--   0        0        0    19802 2024-03-26 10:47:51.941759 pyriksdagen-1.0.0rc1/pyriksdagen/date_handling.py
--rw-r--r--   0        0        0     7026 2024-03-26 10:47:51.941759 pyriksdagen-1.0.0rc1/pyriksdagen/db.py
--rw-r--r--   0        0        0     8159 2024-03-26 10:47:51.941759 pyriksdagen-1.0.0rc1/pyriksdagen/download.py
--rw-r--r--   0        0        0     5649 2024-03-26 10:47:51.941759 pyriksdagen-1.0.0rc1/pyriksdagen/export.py
--rw-r--r--   0        0        0     5222 2024-03-26 10:47:51.941759 pyriksdagen-1.0.0rc1/pyriksdagen/match_mp.py
--rw-r--r--   0        0        0    12084 2024-03-26 10:47:51.941759 pyriksdagen-1.0.0rc1/pyriksdagen/metadata.py
--rw-r--r--   0        0        0    11120 2024-03-26 10:47:51.941759 pyriksdagen-1.0.0rc1/pyriksdagen/mp.py
--rw-r--r--   0        0        0    17780 2024-03-26 10:47:51.941759 pyriksdagen-1.0.0rc1/pyriksdagen/refine.py
--rwxr-xr-x   0        0        0      237 2024-03-26 10:47:51.941759 pyriksdagen-1.0.0rc1/pyriksdagen/requirements.txt
--rw-r--r--   0        0        0     8441 2024-03-26 10:47:51.941759 pyriksdagen-1.0.0rc1/pyriksdagen/segmentation.py
--rw-r--r--   0        0        0    10156 2024-03-26 10:47:51.941759 pyriksdagen-1.0.0rc1/pyriksdagen/swerik_catalog.py
--rw-r--r--   0        0        0    10364 2024-03-26 10:47:51.941759 pyriksdagen-1.0.0rc1/pyriksdagen/utils.py
--rw-r--r--   0        0        0     5682 2024-03-26 10:47:51.941759 pyriksdagen-1.0.0rc1/pyriksdagen/wikidata.py
--rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 pyriksdagen-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1107 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/LICENSE
+-rw-r--r--   0        0        0      247 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/README.md
+-rw-r--r--   0        0        0      847 2024-04-17 11:48:52.538331 pyriksdagen-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/__init__.py
+-rw-r--r--   0        0        0      286 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/alias.rq
+-rw-r--r--   0        0        0      432 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/explicit_no_party.rq
+-rw-r--r--   0        0        0      539 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/external_identifiers.rq
+-rw-r--r--   0        0        0      494 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/government.rq
+-rw-r--r--   0        0        0      777 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/member_of_parliament.rq
+-rw-r--r--   0        0        0      148 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/member_of_parliament.txt
+-rw-r--r--   0        0        0     1621 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/minister.rq
+-rw-r--r--   0        0        0      235 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/minister.txt
+-rw-r--r--   0        0        0      301 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/name_location_specifier.rq
+-rw-r--r--   0        0        0      527 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/party_affiliation.rq
+-rw-r--r--   0        0        0      588 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/person.rq
+-rw-r--r--   0        0        0      277 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/place_of_birth.rq
+-rw-r--r--   0        0        0      277 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/place_of_death.rq
+-rw-r--r--   0        0        0      251 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/portraits.rq
+-rw-r--r--   0        0        0      663 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/speaker.rq
+-rw-r--r--   0        0        0      253 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/speaker.txt
+-rw-r--r--   0        0        0      247 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/twitter.rq
+-rw-r--r--   0        0        0      959 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/wiki_id.rq
+-rw-r--r--   0        0        0      225 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/alias.rq
+-rw-r--r--   0        0        0      482 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/government.rq
+-rw-r--r--   0        0        0      722 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/member_of_parliament.rq
+-rw-r--r--   0        0        0     1380 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/minister.rq
+-rw-r--r--   0        0        0     1013 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/name_location_specifier.rq
+-rw-r--r--   0        0        0     1230 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/party_affiliation.rq
+-rw-r--r--   0        0        0     1412 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/person.rq
+-rw-r--r--   0        0        0      616 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/speaker.rq
+-rw-r--r--   0        0        0      959 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/twitter.rq
+-rw-r--r--   0        0        0      798 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/segmentation/detection.csv
+-rw-r--r--   0        0        0     3355 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/segmentation/patterns.json
+-rw-r--r--   0        0        0     2195 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/dataset.py
+-rw-r--r--   0        0        0    19798 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/date_handling.py
+-rw-r--r--   0        0        0     7026 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/db.py
+-rw-r--r--   0        0        0     8159 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/download.py
+-rw-r--r--   0        0        0     5649 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/export.py
+-rw-r--r--   0        0        0     5222 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/match_mp.py
+-rw-r--r--   0        0        0    13611 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/metadata.py
+-rw-r--r--   0        0        0    11120 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/mp.py
+-rw-r--r--   0        0        0    17780 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/refine.py
+-rwxr-xr-x   0        0        0      237 2024-04-17 11:48:09.765917 pyriksdagen-1.1.0/pyriksdagen/requirements.txt
+-rw-r--r--   0        0        0     8441 2024-04-17 11:48:09.765917 pyriksdagen-1.1.0/pyriksdagen/segmentation.py
+-rw-r--r--   0        0        0    10156 2024-04-17 11:48:09.765917 pyriksdagen-1.1.0/pyriksdagen/swerik_catalog.py
+-rw-r--r--   0        0        0    10395 2024-04-17 11:48:09.765917 pyriksdagen-1.1.0/pyriksdagen/utils.py
+-rw-r--r--   0        0        0     5682 2024-04-17 11:48:09.765917 pyriksdagen-1.1.0/pyriksdagen/wikidata.py
+-rw-r--r--   0        0        0     1578 1970-01-01 00:00:00.000000 pyriksdagen-1.1.0/PKG-INFO
```

### Comparing `pyriksdagen-1.0.0rc1/LICENSE` & `pyriksdagen-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyproject.toml` & `pyriksdagen-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyriksdagen"
-version = "1.0.0rc1"
+version = "1.1.0"
 description = "Access the Riksdagen corpus"
 authors = ["ninpnin <vainoyrjanainen@icloud.com>"]
 repository = "https://github.com/welfare-state-analytics/riksdagen-corpus"
 readme = "README.md"
 license = "MIT"
 packages = [
     { include = "pyriksdagen", from = "" }
```

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/external_identifiers.rq` & `pyriksdagen-1.1.0/pyriksdagen/data/queries/external_identifiers.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/member_of_parliament.rq` & `pyriksdagen-1.1.0/pyriksdagen/data/queries/member_of_parliament.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/minister.rq` & `pyriksdagen-1.1.0/pyriksdagen/data/queries/minister.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/party_affiliation.rq` & `pyriksdagen-1.1.0/pyriksdagen/data/queries/party_affiliation.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/person.rq` & `pyriksdagen-1.1.0/pyriksdagen/data/queries/person.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/speaker.rq` & `pyriksdagen-1.1.0/pyriksdagen/data/queries/speaker.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/queries/wiki_id.rq` & `pyriksdagen-1.1.0/pyriksdagen/data/queries/wiki_id.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/member_of_parliament.rq` & `pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/member_of_parliament.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/minister.rq` & `pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/minister.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/name_location_specifier.rq` & `pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/name_location_specifier.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/party_affiliation.rq` & `pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/party_affiliation.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/person.rq` & `pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/person.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/speaker.rq` & `pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/speaker.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/queries_backup/twitter.rq` & `pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/twitter.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/segmentation/detection.csv` & `pyriksdagen-1.1.0/pyriksdagen/data/segmentation/detection.csv`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/data/segmentation/patterns.json` & `pyriksdagen-1.1.0/pyriksdagen/data/segmentation/patterns.json`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/dataset.py` & `pyriksdagen-1.1.0/pyriksdagen/dataset.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/date_handling.py` & `pyriksdagen-1.1.0/pyriksdagen/date_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
                                 parliament_years.append(a)
     return list(set(parliament_years))
 
 
 
 def yearize_date(date, riksmote):
     """
-    takes a date and a dataframe of riksdagen-politicians/data/riksdag-year.csv
+    takes a date and a dataframe of riksdagen-persons/data/riksdag-year.csv
     """
     parliament_years = riksmote["parliament_year"].unique()
     parliament_years = [str(_) for _ in parliament_years]
     if len(date) == 10:
         date_p = "day"
     elif len(date) == 4:
         date_p = "year"
```

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/db.py` & `pyriksdagen-1.1.0/pyriksdagen/db.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/download.py` & `pyriksdagen-1.1.0/pyriksdagen/download.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/export.py` & `pyriksdagen-1.1.0/pyriksdagen/export.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/match_mp.py` & `pyriksdagen-1.1.0/pyriksdagen/match_mp.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/metadata.py` & `pyriksdagen-1.1.0/pyriksdagen/metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,14 +39,54 @@
 			(db['start'] > gov_start) &\
 			(db['end'].isna())
 	db.loc[idx, 'end'] = gov_db['end'].max()
 	return db
 
 
 def impute_member_dates(db, metadata_folder):
+	def _fill_na(row, **kwargs):
+		if row['start'] == 'nan' and row['end'] == 'nan':
+			return row
+		elif pd.isna(row['start']) and pd.isna(row['end']):
+			return row
+		else:
+			riksmote = pd.read_csv(f"{metadata_folder}/riksdag-year.csv")
+			if pd.isna(row['start']) or row['start'] == 'nan':
+				try:
+					py = riksmote.loc[
+							(riksmote['start'] <= row['end']) &
+							(riksmote['end'] >= row['end'])
+						].copy()
+					row['start'] = py['start'].unique()[0]
+				except:
+					#pass
+					print("no bueno ---------------------> end:", row['end'], row['person_id'])
+			elif pd.isna(row['end']) or row['end'] == 'nan':
+				if int(row['start'][:4]) < 1867:
+					return row
+				try:
+					py = riksmote.loc[
+							(riksmote['start'] <= row['start']) &
+							(riksmote['end'] > row['start'])
+						].copy()
+					row['end'] = py['end'].unique()[0]
+				except:
+					py = riksmote.loc[
+							riksmote['end'].str.startswith(row['start'][:4])
+						].copy()
+					rs = sorted(py['end'].unique(), reverse=True)[0]
+					if rs < row['start']:
+						py = riksmote.loc[
+								riksmote['end'].str.startswith(
+									str(int(row['start'][:4])+1))
+							].copy()
+						rs = sorted(py['end'].unique(), reverse=True)[0]
+					row['end'] = rs
+		return row
+
 	def _impute_start(date, **kwargs):
 		riksmote = kwargs['riksmote']
 		if len(date) == 10:
 			return date
 		elif len(date) == 7:
 			s = sorted(list(riksmote.loc[riksmote['start'].str.startswith(date, na=False), 'start']))
 			if len(s) > 0:
@@ -81,14 +121,19 @@
 				print(f"Problem with end date: {date} not in riksmote")
 				return date + '-12-31'
 
 	riksmote = pd.read_csv(f"{metadata_folder}/riksdag-year.csv")
 	riksmote[['start', 'end']] = riksmote[['start', 'end']].astype(str)
 
 	idx = (db['source'] == 'member_of_parliament') &\
+			(((pd.isna(db['start'])) | (db['start'] == 'nan')) |\
+			((pd.isna(db['end'])) | (db['end'] == 'nan')))
+	db.loc[idx] = db.loc[idx].apply(lambda x: _fill_na(x, riksmote=riksmote), axis = 1)
+
+	idx = (db['source'] == 'member_of_parliament') &\
 			(pd.notnull(db['start'])) & (db['start'] != 'nan')
 	db.loc[idx, 'start'] = db.loc[idx, 'start'].apply(_impute_start, riksmote=riksmote)
 
 	idx = (db['source'] == 'member_of_parliament') &\
 			(pd.notnull(db['start'])) &\
 			(pd.notnull(db['end']))  & (db['end'] != 'nan')
 	db.loc[idx, 'end'] = db.loc[idx, 'end'].apply(_impute_end, riksmote=riksmote)
@@ -133,15 +178,15 @@
 		if 'member_of_parliament' in sources:
 			#db = impute_member_date(db, gov_db)
 			db = impute_member_dates(db, metadata_folder)
 
 		db['start'] = db['start'].apply(increase_date_precision, start=True)
 		db['end'] = db['end'].apply(increase_date_precision, start=False)
 		db[["start", "end"]] = db[["start", "end"]].apply(pd.to_datetime, format='%Y-%m-%d')
-		# Impute current governments end date
+
 		gov_db = pd.read_csv(f'{metadata_folder}/government.csv')
 		gov_db[["start", "end"]] = gov_db[["start", "end"]].apply(pd.to_datetime, format='%Y-%m-%d')
 		idx = gov_db['start'].idxmax()
 		gov_db.loc[idx, 'end'] = gov_db.loc[idx, 'start'] + datetime.timedelta(days = 365*4)
 
 		if 'member_of_parliament' in sources:
 			db = impute_member_date(db, gov_db)
@@ -343,11 +388,12 @@
 	corpus['person_id'] = corpus['person_id']
 
 	# Drop individuals with missing names
 	corpus = corpus[corpus['name'].notna()]
 
 	# Remove redundancy and split file
 	corpus = corpus.drop_duplicates()
+	#print( corpus.loc[(pd.isna(corpus['start'])) | (pd.isna(corpus['end']))] )
 	corpus = corpus.dropna(subset=['name', 'start', 'end'])
 	corpus = corpus.sort_values(['person_id', 'start', 'end', 'name'])
 
 	return corpus
```

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/mp.py` & `pyriksdagen-1.1.0/pyriksdagen/mp.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/refine.py` & `pyriksdagen-1.1.0/pyriksdagen/refine.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/segmentation.py` & `pyriksdagen-1.1.0/pyriksdagen/segmentation.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/swerik_catalog.py` & `pyriksdagen-1.1.0/pyriksdagen/swerik_catalog.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/utils.py` & `pyriksdagen-1.1.0/pyriksdagen/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Provides useful utilities for the other modules as well as for general use.
 """
 
 import lxml
 from lxml import etree
 import xmlschema
 from bs4 import BeautifulSoup
-from pathlib import Path
+from pathlib import Path, PurePath
 from pyparlaclarin.refine import format_texts
 from datetime import datetime
 import hashlib, uuid, base58, requests, tqdm
 import zipfile
 import os
 from trainerlog import get_logger
 
@@ -143,38 +143,36 @@
         document_type (str): type of document (prot, mot, etc.). If None, fetches all types
         start (int): start year
         end (int): end year
 
     Returns:
         iterator of the protocols as relative paths to current location
     """
-    if corpus_root is None:
-        corpus_root = get_data_location("records")
-
     folder = Path(corpus_root)
+    if folder.is_absolute():
+        folder = folder.relative_to(Path(".").resolve(), walk_up=True)
     docs = folder.glob("**/*.xml")
     if document_type is not None:
         docs = folder.glob(f"**/{document_type}*.xml")
     for protocol in sorted(docs):
         metadata = infer_metadata(protocol.name)
         if "year" not in metadata:
             continue
-        path = protocol.relative_to(".")
+        _path = protocol.relative_to(".")
         assert (start is None) == (
             end is None
         ), "Provide both start and end year or neither"
         if start is not None and end is not None:
             metadata = infer_metadata(protocol.name)
             year = metadata["year"]
             if not year:
                 continue
             secondary_year = metadata.get("secondary_year", year)
             if start <= year and end >= secondary_year:
                 yield str(protocol.relative_to("."))
-
         else:
             yield str(protocol.relative_to("."))
 
 def parse_date(s):
     """
     Parse datetimes with special error handling
 
@@ -331,7 +329,8 @@
     valid_partitions = ["records", "motions", "metadata"]
     assert partition in valid_partitions, f"Provide valid partition of the dataset ({valid_partitions})"
     d = {}
     d["records"] = os.environ.get("RECORDS_PATH", "data")
     d["motions"] = os.environ.get("MOTIONS_PATH", "data")
     d["metadata"] = os.environ.get("METADATA_PATH", "data")
     return d[partition]
+
```

### Comparing `pyriksdagen-1.0.0rc1/pyriksdagen/wikidata.py` & `pyriksdagen-1.1.0/pyriksdagen/wikidata.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.0.0rc1/PKG-INFO` & `pyriksdagen-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriksdagen
-Version: 1.0.0rc1
+Version: 1.1.0
 Summary: Access the Riksdagen corpus
 Home-page: https://github.com/welfare-state-analytics/riksdagen-corpus
 License: MIT
 Author: ninpnin
 Author-email: vainoyrjanainen@icloud.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

