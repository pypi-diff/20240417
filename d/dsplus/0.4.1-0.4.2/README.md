# Comparing `tmp/dsplus-0.4.1.tar.gz` & `tmp/dsplus-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsplus-0.4.1.tar", last modified: Mon Apr 15 02:59:38 2024, max compression
+gzip compressed data, was "dsplus-0.4.2.tar", last modified: Wed Apr 17 03:57:11 2024, max compression
```

## Comparing `dsplus-0.4.1.tar` & `dsplus-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 02:59:38.208908 dsplus-0.4.1/
--rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.4.1/LICENSE
--rw-rw-rw-   0        0        0      690 2024-04-15 02:59:38.205417 dsplus-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       99 2024-02-24 21:14:11.000000 dsplus-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 02:59:38.182100 dsplus-0.4.1/dsplus/
--rw-rw-rw-   0        0        0      171 2024-04-15 02:59:18.000000 dsplus-0.4.1/dsplus/__init__.py
--rw-rw-rw-   0        0        0    24320 2024-04-02 22:58:04.000000 dsplus-0.4.1/dsplus/pb_functions_general.py
--rw-rw-rw-   0        0        0    41884 2024-04-15 02:58:21.000000 dsplus-0.4.1/dsplus/pb_functions_pandas.py
--rw-rw-rw-   0        0        0    56894 2024-04-02 22:58:04.000000 dsplus-0.4.1/dsplus/pb_functions_plotly.py
--rw-rw-rw-   0        0        0    44406 2024-04-12 03:03:10.000000 dsplus-0.4.1/dsplus/pb_functions_spatial.py
-drwxrwxrwx   0        0        0        0 2024-04-15 02:59:38.194354 dsplus-0.4.1/dsplus.egg-info/
--rw-rw-rw-   0        0        0      690 2024-04-15 02:59:37.000000 dsplus-0.4.1/dsplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-04-15 02:59:38.000000 dsplus-0.4.1/dsplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 02:59:37.000000 dsplus-0.4.1/dsplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-15 02:59:37.000000 dsplus-0.4.1/dsplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 02:59:38.208908 dsplus-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1650 2024-03-29 02:13:48.000000 dsplus-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 02:59:38.200574 dsplus-0.4.1/tests/
--rw-rw-rw-   0        0        0    12143 2024-03-29 17:35:19.000000 dsplus-0.4.1/tests/Test_pandas.py
+drwxrwxrwx   0        0        0        0 2024-04-17 03:57:11.741144 dsplus-0.4.2/
+-rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0      690 2024-04-17 03:57:11.735693 dsplus-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2024-02-24 21:14:11.000000 dsplus-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 03:57:11.707527 dsplus-0.4.2/dsplus/
+-rw-rw-rw-   0        0        0      171 2024-04-17 03:56:55.000000 dsplus-0.4.2/dsplus/__init__.py
+-rw-rw-rw-   0        0        0    24320 2024-04-02 22:58:04.000000 dsplus-0.4.2/dsplus/pb_functions_general.py
+-rw-rw-rw-   0        0        0    42751 2024-04-17 00:36:26.000000 dsplus-0.4.2/dsplus/pb_functions_pandas.py
+-rw-rw-rw-   0        0        0    56894 2024-04-02 22:58:04.000000 dsplus-0.4.2/dsplus/pb_functions_plotly.py
+-rw-rw-rw-   0        0        0    44406 2024-04-12 03:03:10.000000 dsplus-0.4.2/dsplus/pb_functions_spatial.py
+drwxrwxrwx   0        0        0        0 2024-04-17 03:57:11.726224 dsplus-0.4.2/dsplus.egg-info/
+-rw-rw-rw-   0        0        0      690 2024-04-17 03:57:11.000000 dsplus-0.4.2/dsplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-04-17 03:57:11.000000 dsplus-0.4.2/dsplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 03:57:11.000000 dsplus-0.4.2/dsplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-17 03:57:11.000000 dsplus-0.4.2/dsplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 03:57:11.741144 dsplus-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1650 2024-03-29 02:13:48.000000 dsplus-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 03:57:11.730037 dsplus-0.4.2/tests/
+-rw-rw-rw-   0        0        0    12530 2024-04-17 03:55:44.000000 dsplus-0.4.2/tests/Test_pandas.py
```

### Comparing `dsplus-0.4.1/LICENSE` & `dsplus-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.1/PKG-INFO` & `dsplus-0.4.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.4.1
+Version: 0.4.2
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.4.1/dsplus/pb_functions_general.py` & `dsplus-0.4.2/dsplus/pb_functions_general.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.1/dsplus/pb_functions_pandas.py` & `dsplus-0.4.2/dsplus/pb_functions_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,37 +127,40 @@
         - 'cols' is comprised of individual pieces separated by comma.
             - Whitespaces before and after comma are ignored.
         - Each piece can be a column name, a slice, a pandas string function, or an asterisk (*).
         - Slice means a two column names separated by a colon. eg. 'v1:v5' means all columns from 'v1' to 'v5' (inclusive).
             - If the first columnn name is omitted, it means everything before. For eg. ':v5' means all column upto and including 'v5'.
             - If the last column name is omitted, it means everything after. For eg. 'v1:' means all column anmes from and including 'v1'.
         - To specify pandas string function, the piece should start with 'str.'. For eg. 'str.startswith("v2")'.
-            - The function should return True or False values on all columns of 'df'. Only
+            - The function should return True or False values on all columns of 'df'.
+        - To specify data type, the piece should start with 'select_dtypes('. For eg. 'select_dtypes("category")'.
         - An asterisk (*) means all other columnn names.
             - All other column except for all other inclusions and exclusions (before or after the asterisk) will be placed in place of the asterisk (*).
         - Any piece can be negated adding a '-' in front. These columns are excluded. Examples:
             - '-v1' means exclude column 'v1'.
             - '-v1:v5' means exclude columns from 'v1' to 'v5' (inclusive).
             - '-:v5' means exclude all columns upto and including 'v5'.
             - '-v1:' means exclude all columns from and including 'v1'.
         - If any columns to keep are repeated, only the first occurence is kept.
         - Any columns to be excluded will be excluded. Exclusion takes precedence over inclusion.
         - If no inclusions are provided, all columns are taken as inclusions.
             - This is useful when only exclusions are provided.
 
     Examples:
-        >>> df = pd.DataFrame(columns = ['v'+str(_) for _ in range(21)])
+        >>> df = pd.DataFrame(columns = ['v'+str(_) for _ in range(21)]).astype(dict(v5=int, v15=int, v0='category'))
         >>> pd_cols(df, ':v2, v4:v6, *, v9:v10, -v12:v13, -v11, -v17:')
         >>> pd_cols(df, 'v1:v2, v4:v6, *, v9:v10')
         >>> pd_cols(df, 'v4:')
         >>> pd_cols(df, ':v9, -v2')
         >>> pd_cols(df, 'v9:, -v12')
         >>> pd_cols(df, '*, -v12, -v4:v9')
         >>> pd_cols(df, 'v15:, *')
         >>> pd_cols(df, 'str.contains("v2"), *, -str.startswith("v1"), -v8')
+        >>> pd_cols(df, '-select_dtypes("category")')
+        >>> pd_cols(df, 'select_dtypes("number"), *')
         >>> pd_cols(df, '-v2:')
         >>> df[lambda _: pd_cols(_, 'v15:, *')]
     '''
     v_cols_all = df.columns.to_series()
 
     cols_split = [_.strip() for _ in cols.split(',')]
 
@@ -167,14 +170,18 @@
     for col in cols_split:
         if col=='*':
             temp_v_cols = ['*']
         elif col[0:4] == 'str.':
             temp_v_cols = eval('df.columns[df.columns.' + col + ']').tolist()
         elif col[0:5] == '-str.':
             temp_v_cols = eval('df.columns[df.columns.' + col[1:] + ']').tolist()
+        elif col[0:14] == 'select_dtypes(':
+            temp_v_cols = eval('df.' + col + '.columns.tolist()')
+        elif col[0:15] == '-select_dtypes(':
+            temp_v_cols = eval('df.' + col[1:] + '.columns.tolist()')
         elif ':' in col:
             temp_v_cols = [_.strip().replace('-', '') for _ in col.split(':')]
             if temp_v_cols[0] == '':
                 index_from = 0
             else:
                 index_from = v_cols_all.tolist().index(temp_v_cols[0])
             if temp_v_cols[1] == '':
@@ -225,37 +232,41 @@
         - 'cols' is comprised of individual pieces separated by comma.
             - Whitespaces before and after comma are ignored.
         - Each piece can be a column name, a slice, a pandas string function, or an asterisk (*).
         - Slice means a two column names separated by a colon. eg. 'v1:v5' means all columns from 'v1' to 'v5' (inclusive).
             - If the first columnn name is omitted, it means everything before. For eg. ':v5' means all column upto and including 'v5'.
             - If the last column name is omitted, it means everything after. For eg. 'v1:' means all column anmes from and including 'v1'.
         - To specify pandas string function, the piece should start with 'str.'. For eg. 'str.startswith("v2")'.
+            - The function should return True or False values on all columns of 'df'.
+        - To specify data type, the piece should start with 'select_dtypes('. For eg. 'select_dtypes("category")'.
         - An asterisk (*) means all other columnn names.
             - All other column except for all other inclusions and exclusions (before or after the asterisk) will be placed in place of the asterisk (*).
         - Any piece can be negated adding a '-' in front. These columns are excluded. Examples:
             - '-v1' means exclude column 'v1'.
             - '-v1:v5' means exclude columns from 'v1' to 'v5' (inclusive).
             - '-:v5' means exclude all columns upto and including 'v5'.
             - '-v1:' means exclude all columns from and including 'v1'.
         - If any columns to keep are repeated, only the first occurence is kept.
         - Any columns to be excluded will be excluded. Exclusion takes precedence over inclusion.
         - If no inclusions are provided, all columns are taken as inclusions.
             - This is useful when only exclusions are provided.
 
     Examples:
-        >>> df = pd.DataFrame(columns = ['v'+str(_) for _ in range(21)])
+        >>> df = pd.DataFrame(columns = ['v'+str(_) for _ in range(21)]).astype(dict(v5=int, v15=int, v0='category'))
         >>> df.pipe(pd_select, ':v2, v4:v6, *, v9:v10, -v12:v13, -v11, -v17:')
         >>> df.pipe(pd_select, 'v1:v2, v4:v6, *, v9:v10')
         >>> df.pipe(pd_select, 'v4:')
         >>> df.pipe(pd_select, ':v9, -v2')
         >>> df.pipe(pd_select, 'v9:, -v12')
         >>> df.pipe(pd_select, '*, -v12, -v4:v9')
         >>> df.pipe(pd_select, 'v15:, *')
         >>> df.pipe(pd_select, 'str.startswith("v2"), *')
         >>> df.pipe(pd_select, 'str.contains("v2"), *, -str.startswith("v1"), -v8')
+        >>> df.pipe(pd_select, '-select_dtypes("category")')
+        >>> df.pipe(pd_select, 'select_dtypes("number"), *')
         >>> df.pipe(pd_select, '-v2:')
     '''
     return df[lambda _: pd_cols(_, cols)]
 
 #%%
 def pd_select_simple(df: pd.DataFrame,
                      cols_before: str|list|np.ndarray|pd.Series=None,
```

### Comparing `dsplus-0.4.1/dsplus/pb_functions_plotly.py` & `dsplus-0.4.2/dsplus/pb_functions_plotly.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.1/dsplus/pb_functions_spatial.py` & `dsplus-0.4.2/dsplus/pb_functions_spatial.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.1/dsplus.egg-info/PKG-INFO` & `dsplus-0.4.2/dsplus.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.4.1
+Version: 0.4.2
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.4.1/setup.py` & `dsplus-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.1/tests/Test_pandas.py` & `dsplus-0.4.2/tests/Test_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,22 @@
 def test_pd_select_2():
     df = pd.DataFrame(columns = ['v'+str(_) for _ in range(21)])
 
     df_select = df.pipe(ds.pd_select, '-:v5, -v8:')
 
     assert df_select.columns.tolist() == ['v6', 'v7']
 
+#%%
+def test_pd_select_3():
+    df = pd.DataFrame(columns = ['v'+str(_) for _ in range(21)]).astype(dict(v5=int, v15=int, v0='category'))
+
+    df_select = df.pipe(ds.pd_select, 'select_dtypes("number"), *, -v8:v13, -select_dtypes("category")')
+
+    assert df_select.columns.tolist() == ['v5', 'v15', 'v1', 'v2', 'v3', 'v4', 'v6', 'v7', 'v14', 'v16', 'v17', 'v18', 'v19', 'v20']
+
 #endregion -----------------------------------------------------------------------------------------
 #region Concat
 
 #%%
 def test_pd_concat_series_1():
     assert ds.pd_concat_series(pd.Series([1,2,3]), 4).tolist() == [1,2,3,4]
```

