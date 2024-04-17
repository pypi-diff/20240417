# Comparing `tmp/autofile-0.0.7.tar.gz` & `tmp/autofile-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofile-0.0.7.tar", last modified: Sun Oct 31 16:15:42 2021, max compression
+gzip compressed data, was "autofile-0.0.8.tar", last modified: Sun Oct 31 20:42:49 2021, max compression
```

## Comparing `autofile-0.0.7.tar` & `autofile-0.0.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2021-10-31 16:15:42.992998 autofile-0.0.7/
--rw-r--r--   0 rhet       (501) staff       (20)     1070 2021-10-11 04:53:47.000000 autofile-0.0.7/LICENSE
--rw-r--r--   0 rhet       (501) staff       (20)       75 2021-10-25 03:10:46.000000 autofile-0.0.7/MANIFEST.in
--rw-r--r--   0 rhet       (501) staff       (20)    35867 2021-10-31 16:15:42.966086 autofile-0.0.7/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)    34921 2021-10-31 16:15:12.000000 autofile-0.0.7/README.md
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2021-10-31 16:15:42.749982 autofile-0.0.7/autofile/
--rw-r--r--   0 rhet       (501) staff       (20)      189 2021-10-24 21:11:15.000000 autofile-0.0.7/autofile/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)       30 2021-10-11 05:35:20.000000 autofile-0.0.7/autofile/__main__.py
--rw-r--r--   0 rhet       (501) staff       (20)       51 2021-10-31 16:15:14.000000 autofile-0.0.7/autofile/_version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5155 2021-10-31 15:47:53.000000 autofile-0.0.7/autofile/autofile.py
--rw-r--r--   0 rhet       (501) staff       (20)    11376 2021-10-25 01:06:06.000000 autofile-0.0.7/autofile/cli.py
--rw-r--r--   0 rhet       (501) staff       (20)      359 2021-10-22 04:59:10.000000 autofile-0.0.7/autofile/constants.py
--rw-r--r--   0 rhet       (501) staff       (20)     1624 2021-10-18 04:22:34.000000 autofile-0.0.7/autofile/datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     5960 2021-10-20 12:46:01.000000 autofile-0.0.7/autofile/datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    17145 2021-10-24 05:23:22.000000 autofile-0.0.7/autofile/exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)      878 2021-10-24 21:10:35.000000 autofile-0.0.7/autofile/hookspecs.py
--rw-r--r--   0 rhet       (501) staff       (20)     2824 2021-10-24 15:09:54.000000 autofile-0.0.7/autofile/path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8119 2021-10-24 15:24:02.000000 autofile-0.0.7/autofile/pathlibutil.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2021-10-31 16:15:42.803660 autofile-0.0.7/autofile/plugins/
--rw-r--r--   0 rhet       (501) staff       (20)        0 2021-10-17 20:53:11.000000 autofile-0.0.7/autofile/plugins/__init__.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2021-10-31 16:15:42.961787 autofile-0.0.7/autofile/plugins/templates/
--rw-r--r--   0 rhet       (501) staff       (20)       45 2021-10-22 04:51:31.000000 autofile-0.0.7/autofile/plugins/templates/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)     2782 2021-10-25 01:14:42.000000 autofile-0.0.7/autofile/plugins/templates/audio.py
--rw-r--r--   0 rhet       (501) staff       (20)     6260 2021-10-31 15:11:30.000000 autofile-0.0.7/autofile/plugins/templates/docx.py
--rw-r--r--   0 rhet       (501) staff       (20)     7385 2021-10-24 21:12:39.000000 autofile-0.0.7/autofile/plugins/templates/exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     4292 2021-10-31 04:30:55.000000 autofile-0.0.7/autofile/plugins/templates/filedates.py
--rw-r--r--   0 rhet       (501) staff       (20)     2943 2021-10-24 21:13:51.000000 autofile-0.0.7/autofile/plugins/templates/filepath.py
--rw-r--r--   0 rhet       (501) staff       (20)     1438 2021-10-24 21:13:43.000000 autofile-0.0.7/autofile/plugins/templates/filestat.py
--rw-r--r--   0 rhet       (501) staff       (20)     1653 2021-10-24 21:13:43.000000 autofile-0.0.7/autofile/plugins/templates/finder.py
--rw-r--r--   0 rhet       (501) staff       (20)     2792 2021-10-24 21:13:43.000000 autofile-0.0.7/autofile/plugins/templates/format.py
--rw-r--r--   0 rhet       (501) staff       (20)     2549 2021-10-25 02:30:03.000000 autofile-0.0.7/autofile/plugins/templates/mdls.py
--rw-r--r--   0 rhet       (501) staff       (20)     1979 2021-10-24 21:13:43.000000 autofile-0.0.7/autofile/plugins/templates/punctuation.py
--rw-r--r--   0 rhet       (501) staff       (20)    27697 2021-10-24 21:13:43.000000 autofile-0.0.7/autofile/plugins/templates/uti.py
--rw-r--r--   0 rhet       (501) staff       (20)     1369 2021-10-23 04:18:21.000000 autofile-0.0.7/autofile/renderoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     8331 2021-10-31 16:09:38.000000 autofile-0.0.7/autofile/template.md
--rw-r--r--   0 rhet       (501) staff       (20)    23330 2021-10-31 16:06:44.000000 autofile-0.0.7/autofile/template.py
--rw-r--r--   0 rhet       (501) staff       (20)     1950 2021-10-31 15:58:38.000000 autofile-0.0.7/autofile/template.tx
--rw-r--r--   0 rhet       (501) staff       (20)     1118 2021-10-23 18:01:15.000000 autofile-0.0.7/autofile/utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2021-10-31 16:15:42.802925 autofile-0.0.7/autofile.egg-info/
--rw-r--r--   0 rhet       (501) staff       (20)    35867 2021-10-31 16:15:42.000000 autofile-0.0.7/autofile.egg-info/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)     1090 2021-10-31 16:15:42.000000 autofile-0.0.7/autofile.egg-info/SOURCES.txt
--rw-r--r--   0 rhet       (501) staff       (20)        1 2021-10-31 16:15:42.000000 autofile-0.0.7/autofile.egg-info/dependency_links.txt
--rw-r--r--   0 rhet       (501) staff       (20)       47 2021-10-31 16:15:42.000000 autofile-0.0.7/autofile.egg-info/entry_points.txt
--rw-r--r--   0 rhet       (501) staff       (20)      375 2021-10-31 16:15:42.000000 autofile-0.0.7/autofile.egg-info/requires.txt
--rw-r--r--   0 rhet       (501) staff       (20)        9 2021-10-31 16:15:42.000000 autofile-0.0.7/autofile.egg-info/top_level.txt
--rw-r--r--   0 rhet       (501) staff       (20)       38 2021-10-31 16:15:42.993219 autofile-0.0.7/setup.cfg
--rwxr--r--   0 rhet       (501) staff       (20)     2557 2021-10-31 15:15:16.000000 autofile-0.0.7/setup.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2021-10-31 20:42:49.112015 autofile-0.0.8/
+-rw-r--r--   0 rhet       (501) staff       (20)     1070 2021-10-11 04:53:47.000000 autofile-0.0.8/LICENSE
+-rw-r--r--   0 rhet       (501) staff       (20)       75 2021-10-25 03:10:46.000000 autofile-0.0.8/MANIFEST.in
+-rw-r--r--   0 rhet       (501) staff       (20)    36191 2021-10-31 20:42:49.109169 autofile-0.0.8/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)    35245 2021-10-31 20:41:43.000000 autofile-0.0.8/README.md
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2021-10-31 20:42:48.816749 autofile-0.0.8/autofile/
+-rw-r--r--   0 rhet       (501) staff       (20)      189 2021-10-24 21:11:15.000000 autofile-0.0.8/autofile/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)       30 2021-10-11 05:35:20.000000 autofile-0.0.8/autofile/__main__.py
+-rw-r--r--   0 rhet       (501) staff       (20)       51 2021-10-31 20:40:27.000000 autofile-0.0.8/autofile/_version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5155 2021-10-31 15:47:53.000000 autofile-0.0.8/autofile/autofile.py
+-rw-r--r--   0 rhet       (501) staff       (20)    11376 2021-10-25 01:06:06.000000 autofile-0.0.8/autofile/cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)      359 2021-10-22 04:59:10.000000 autofile-0.0.8/autofile/constants.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1624 2021-10-18 04:22:34.000000 autofile-0.0.8/autofile/datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5960 2021-10-20 12:46:01.000000 autofile-0.0.8/autofile/datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17145 2021-10-24 05:23:22.000000 autofile-0.0.8/autofile/exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)      878 2021-10-24 21:10:35.000000 autofile-0.0.8/autofile/hookspecs.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2824 2021-10-24 15:09:54.000000 autofile-0.0.8/autofile/path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8119 2021-10-24 15:24:02.000000 autofile-0.0.8/autofile/pathlibutil.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2021-10-31 20:42:49.059545 autofile-0.0.8/autofile/plugins/
+-rw-r--r--   0 rhet       (501) staff       (20)        0 2021-10-17 20:53:11.000000 autofile-0.0.8/autofile/plugins/__init__.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2021-10-31 20:42:49.101688 autofile-0.0.8/autofile/plugins/templates/
+-rw-r--r--   0 rhet       (501) staff       (20)       45 2021-10-22 04:51:31.000000 autofile-0.0.8/autofile/plugins/templates/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2782 2021-10-25 01:14:42.000000 autofile-0.0.8/autofile/plugins/templates/audio.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6260 2021-10-31 15:11:30.000000 autofile-0.0.8/autofile/plugins/templates/docx.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7385 2021-10-24 21:12:39.000000 autofile-0.0.8/autofile/plugins/templates/exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4292 2021-10-31 04:30:55.000000 autofile-0.0.8/autofile/plugins/templates/filedates.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2943 2021-10-24 21:13:51.000000 autofile-0.0.8/autofile/plugins/templates/filepath.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1438 2021-10-24 21:13:43.000000 autofile-0.0.8/autofile/plugins/templates/filestat.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1653 2021-10-24 21:13:43.000000 autofile-0.0.8/autofile/plugins/templates/finder.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2792 2021-10-24 21:13:43.000000 autofile-0.0.8/autofile/plugins/templates/format.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2549 2021-10-25 02:30:03.000000 autofile-0.0.8/autofile/plugins/templates/mdls.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1979 2021-10-24 21:13:43.000000 autofile-0.0.8/autofile/plugins/templates/punctuation.py
+-rw-r--r--   0 rhet       (501) staff       (20)    27697 2021-10-24 21:13:43.000000 autofile-0.0.8/autofile/plugins/templates/uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1369 2021-10-23 04:18:21.000000 autofile-0.0.8/autofile/renderoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8515 2021-10-31 20:40:11.000000 autofile-0.0.8/autofile/template.md
+-rw-r--r--   0 rhet       (501) staff       (20)    24283 2021-10-31 20:40:19.000000 autofile-0.0.8/autofile/template.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1954 2021-10-31 20:28:33.000000 autofile-0.0.8/autofile/template.tx
+-rw-r--r--   0 rhet       (501) staff       (20)     1118 2021-10-23 18:01:15.000000 autofile-0.0.8/autofile/utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2021-10-31 20:42:49.043017 autofile-0.0.8/autofile.egg-info/
+-rw-r--r--   0 rhet       (501) staff       (20)    36191 2021-10-31 20:42:48.000000 autofile-0.0.8/autofile.egg-info/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)     1090 2021-10-31 20:42:48.000000 autofile-0.0.8/autofile.egg-info/SOURCES.txt
+-rw-r--r--   0 rhet       (501) staff       (20)        1 2021-10-31 20:42:48.000000 autofile-0.0.8/autofile.egg-info/dependency_links.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       47 2021-10-31 20:42:48.000000 autofile-0.0.8/autofile.egg-info/entry_points.txt
+-rw-r--r--   0 rhet       (501) staff       (20)      375 2021-10-31 20:42:48.000000 autofile-0.0.8/autofile.egg-info/requires.txt
+-rw-r--r--   0 rhet       (501) staff       (20)        9 2021-10-31 20:42:48.000000 autofile-0.0.8/autofile.egg-info/top_level.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       38 2021-10-31 20:42:49.112910 autofile-0.0.8/setup.cfg
+-rwxr--r--   0 rhet       (501) staff       (20)     2557 2021-10-31 15:15:16.000000 autofile-0.0.8/setup.py
```

### Comparing `autofile-0.0.7/LICENSE` & `autofile-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/PKG-INFO` & `autofile-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofile
-Version: 0.0.7
+Version: 0.0.8
 Summary: Use templates to automatically move files into directories
 Home-page: https://github.com/RhetTbull/autofile
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Download-URL: https://github.com/RhetTbull/autofile
 Project-URL: GitHub, https://github.com/RhetTbull/autofile
@@ -255,18 +255,22 @@
  • upper: Convert value to upper case, e.g. 'Value' => 'VALUE'.                
  • strip: Strip whitespace from beginning/end of value, e.g. ' Value ' =>      
    'Value'.                                                                    
  • titlecase: Convert value to title case, e.g. 'my value' => 'My Value'.      
  • capitalize: Capitalize first word of value and convert other words to lower 
    case, e.g. 'MY VALUE' => 'My value'.                                        
  • braces: Enclose value in curly braces, e.g. 'value => '{value}'.            
- • parens: Enclose value in parentheses, e.g. 'value' => '(value')             
- • brackets: Enclose value in brackets, e.g. 'value' => '[value]'              
+ • parens: Enclose value in parentheses, e.g. 'value' => '(value').            
+ • brackets: Enclose value in brackets, e.g. 'value' => '[value]'.             
  • split(delim): Split value into a list of values using delim as delimiter,   
-   e.g. 'value1;value2' => ['value1', 'value2'] if used with split(;)          
+   e.g. 'value1;value2' => ['value1', 'value2'] if used with split(;).         
+ • chop(x): Remove x characters off the end of value, e.g. chop(1): 'Value' => 
+   'Valu'.                                                                     
+ • chomp(x): Remove x characters from the beginning of value, e.g. chomp(1):   
+   'Value' => 'alue'.                                                          
 
 e.g. if file keywords are ["FOO","bar"]:                                       
 
  • "{exiftool:Keywords|lower}" renders to "foo", "bar"                         
  • "{exiftool:Keywords|upper}" renders to: "FOO", "BAR"                        
  • "{exiftool:Keywords|capitalize}" renders to: "Foo", "Bar"                   
  • "{exiftool:Keywords|lower|parens}" renders to: "(foo)", "(bar)"
```

### Comparing `autofile-0.0.7/README.md` & `autofile-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -231,18 +231,22 @@
  • upper: Convert value to upper case, e.g. 'Value' => 'VALUE'.                
  • strip: Strip whitespace from beginning/end of value, e.g. ' Value ' =>      
    'Value'.                                                                    
  • titlecase: Convert value to title case, e.g. 'my value' => 'My Value'.      
  • capitalize: Capitalize first word of value and convert other words to lower 
    case, e.g. 'MY VALUE' => 'My value'.                                        
  • braces: Enclose value in curly braces, e.g. 'value => '{value}'.            
- • parens: Enclose value in parentheses, e.g. 'value' => '(value')             
- • brackets: Enclose value in brackets, e.g. 'value' => '[value]'              
+ • parens: Enclose value in parentheses, e.g. 'value' => '(value').            
+ • brackets: Enclose value in brackets, e.g. 'value' => '[value]'.             
  • split(delim): Split value into a list of values using delim as delimiter,   
-   e.g. 'value1;value2' => ['value1', 'value2'] if used with split(;)          
+   e.g. 'value1;value2' => ['value1', 'value2'] if used with split(;).         
+ • chop(x): Remove x characters off the end of value, e.g. chop(1): 'Value' => 
+   'Valu'.                                                                     
+ • chomp(x): Remove x characters from the beginning of value, e.g. chomp(1):   
+   'Value' => 'alue'.                                                          
 
 e.g. if file keywords are ["FOO","bar"]:                                       
 
  • "{exiftool:Keywords|lower}" renders to "foo", "bar"                         
  • "{exiftool:Keywords|upper}" renders to: "FOO", "BAR"                        
  • "{exiftool:Keywords|capitalize}" renders to: "Foo", "Bar"                   
  • "{exiftool:Keywords|lower|parens}" renders to: "(foo)", "(bar)"
```

### Comparing `autofile-0.0.7/autofile/autofile.py` & `autofile-0.0.8/autofile/autofile.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/cli.py` & `autofile-0.0.8/autofile/cli.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/datetime_formatter.py` & `autofile-0.0.8/autofile/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/datetime_utils.py` & `autofile-0.0.8/autofile/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/exiftool.py` & `autofile-0.0.8/autofile/exiftool.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/hookspecs.py` & `autofile-0.0.8/autofile/hookspecs.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/path_utils.py` & `autofile-0.0.8/autofile/path_utils.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/pathlibutil.py` & `autofile-0.0.8/autofile/pathlibutil.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/plugins/templates/audio.py` & `autofile-0.0.8/autofile/plugins/templates/audio.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/plugins/templates/docx.py` & `autofile-0.0.8/autofile/plugins/templates/docx.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/plugins/templates/exiftool.py` & `autofile-0.0.8/autofile/plugins/templates/exiftool.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/plugins/templates/filedates.py` & `autofile-0.0.8/autofile/plugins/templates/filedates.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/plugins/templates/filepath.py` & `autofile-0.0.8/autofile/plugins/templates/filepath.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/plugins/templates/filestat.py` & `autofile-0.0.8/autofile/plugins/templates/filestat.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/plugins/templates/finder.py` & `autofile-0.0.8/autofile/plugins/templates/finder.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/plugins/templates/format.py` & `autofile-0.0.8/autofile/plugins/templates/format.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/plugins/templates/mdls.py` & `autofile-0.0.8/autofile/plugins/templates/mdls.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/plugins/templates/punctuation.py` & `autofile-0.0.8/autofile/plugins/templates/punctuation.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/plugins/templates/uti.py` & `autofile-0.0.8/autofile/plugins/templates/uti.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/renderoptions.py` & `autofile-0.0.8/autofile/renderoptions.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile/template.md` & `autofile-0.0.8/autofile/template.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,19 @@
 
 - lower: Convert value to lower case, e.g. 'Value' => 'value'.
 - upper: Convert value to upper case, e.g. 'Value' => 'VALUE'.
 - strip: Strip whitespace from beginning/end of value, e.g. ' Value ' => 'Value'.
 - titlecase: Convert value to title case, e.g. 'my value' => 'My Value'.
 - capitalize: Capitalize first word of value and convert other words to lower case, e.g. 'MY VALUE' => 'My value'.
 - braces: Enclose value in curly braces, e.g. 'value => '{value}'.
-- parens: Enclose value in parentheses, e.g. 'value' => '(value')
-- brackets: Enclose value in brackets, e.g. 'value' => '[value]'
-- split(delim): Split value into a list of values using delim as delimiter, e.g. 'value1;value2' => ['value1', 'value2'] if used with split(;)
+- parens: Enclose value in parentheses, e.g. 'value' => '(value').
+- brackets: Enclose value in brackets, e.g. 'value' => '[value]'.
+- split(delim): Split value into a list of values using delim as delimiter, e.g. 'value1;value2' => ['value1', 'value2'] if used with split(;).
+- chop(x): Remove x characters off the end of value, e.g. chop(1): 'Value' => 'Valu'.
+- chomp(x): Remove x characters from the beginning of value, e.g. chomp(1): 'Value' => 'alue'.
 
 <!-- - shell_quote: Quotes the value for safe usage in the shell, e.g. My file.jpeg => 'My file.jpeg'; only adds quotes if needed.
 - function: Run custom python function to filter value; use in format 'function:/path/to/file.py::function_name'. See example at https://github.com/RhetTbull/osxfiles/blob/master/examples/template_filter.py
 -->
 
 e.g. if file keywords are `["FOO","bar"]`:
```

### Comparing `autofile-0.0.7/autofile/template.py` & `autofile-0.0.8/autofile/template.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,17 @@
     "strip": "Strip whitespace from beginning/end of value, e.g. ' Value ' => 'Value'.",
     "titlecase": "Convert value to title case, e.g. 'my value' => 'My Value'.",
     "capitalize": "Capitalize first word of value and convert other words to lower case, e.g. 'MY VALUE' => 'My value'.",
     "braces": "Enclose value in curly braces, e.g. 'value => '{value}'.",
     "parens": "Enclose value in parentheses, e.g. 'value' => '(value').",
     "brackets": "Enclose value in brackets, e.g. 'value' => '[value]'.",
     "shell_quote": "Quotes the value for safe usage in the shell, e.g. My file.jpeg => 'My file.jpeg'; only adds quotes if needed.",
-    "split(str)": "Splits the value into a list using 'str' as delimiter, e.g. split(;) would split 'foo;bar' into [foo, bar]."
+    "split(str)": "Splits the value into a list using 'str' as delimiter, e.g. split(;) would split 'foo;bar' into [foo, bar].",
+    "chop(x)": "Remove x characters off the end of value, e.g. chop(1): 'Value' => 'Valu'.",
+    "chomp(x)": "Remove x characters from the beginning of value, e.g. chomp(1): 'Value' => 'alue'.",
     # "function": "Run custom python function to filter value; use in format 'function:/path/to/file.py::function_name'. See example at https://github.com/RhetTbull/osxphotos/blob/master/examples/template_filter.py",
 }
 
 # PATH_SEP_DEFAULT = os.path.sep
 
 
 class FileTemplateParser:
@@ -495,22 +497,39 @@
                 value = ["[" + values + "]"] if values else []
         elif filter_ == "shell_quote":
             if values and type(values) == list:
                 value = [shlex.quote(v) for v in values]
             else:
                 value = [shlex.quote(values)] if values else []
         elif filter_.startswith("split"):
+            # split on delimiter
             delim = filter_.split("split")[1][1:-1]
             if delim:
                 new_values = []
                 for v in values:
                     new_values.extend(v.split(delim))
                 value = new_values
             else:
                 value = values
+        elif filter_.startswith("chop"):
+            # chop off characters from the end
+            chop = filter_.split("chop")[1][1:-1]
+            try:
+                chop = int(chop)
+            except ValueError:
+                raise ValueError(f"Invalid value for chop: {chop}")
+            value = [v[:-chop] for v in values] if chop else values
+        elif filter_.startswith("chomp"):
+            # chop off characters from the beginning
+            chomp = filter_.split("chomp")[1][1:-1]
+            try:
+                chomp = int(chomp)
+            except ValueError:
+                raise ValueError(f"Invalid value for chomp: {chomp}")
+            value = [v[chomp:] for v in values] if chomp else values
         # elif filter_.startswith("function:"):
         # value = self.get_template_value_filter_function(filter_, values)
         else:
             raise ValueError(f"Unhandled filter: {filter_}")
         return value
```

### Comparing `autofile-0.0.7/autofile/template.tx` & `autofile-0.0.8/autofile/template.tx`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     (
     "|"-
     (value+=FILTER_FUNCTION['|'])?
     )?
 ;
 
 FILTER_FUNCTION:
-    /[\.\w:\/]+(\(.*\))?/
+    /[\.\w:\/]+(\([^\)]*\))?/
 ;
 
 Conditional:
     (
     (" "+)-
     (negation=NEGATION)?
     (operator=OPERATOR)
```

### Comparing `autofile-0.0.7/autofile/utils.py` & `autofile-0.0.8/autofile/utils.py`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/autofile.egg-info/PKG-INFO` & `autofile-0.0.8/autofile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofile
-Version: 0.0.7
+Version: 0.0.8
 Summary: Use templates to automatically move files into directories
 Home-page: https://github.com/RhetTbull/autofile
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Download-URL: https://github.com/RhetTbull/autofile
 Project-URL: GitHub, https://github.com/RhetTbull/autofile
@@ -255,18 +255,22 @@
  • upper: Convert value to upper case, e.g. 'Value' => 'VALUE'.                
  • strip: Strip whitespace from beginning/end of value, e.g. ' Value ' =>      
    'Value'.                                                                    
  • titlecase: Convert value to title case, e.g. 'my value' => 'My Value'.      
  • capitalize: Capitalize first word of value and convert other words to lower 
    case, e.g. 'MY VALUE' => 'My value'.                                        
  • braces: Enclose value in curly braces, e.g. 'value => '{value}'.            
- • parens: Enclose value in parentheses, e.g. 'value' => '(value')             
- • brackets: Enclose value in brackets, e.g. 'value' => '[value]'              
+ • parens: Enclose value in parentheses, e.g. 'value' => '(value').            
+ • brackets: Enclose value in brackets, e.g. 'value' => '[value]'.             
  • split(delim): Split value into a list of values using delim as delimiter,   
-   e.g. 'value1;value2' => ['value1', 'value2'] if used with split(;)          
+   e.g. 'value1;value2' => ['value1', 'value2'] if used with split(;).         
+ • chop(x): Remove x characters off the end of value, e.g. chop(1): 'Value' => 
+   'Valu'.                                                                     
+ • chomp(x): Remove x characters from the beginning of value, e.g. chomp(1):   
+   'Value' => 'alue'.                                                          
 
 e.g. if file keywords are ["FOO","bar"]:                                       
 
  • "{exiftool:Keywords|lower}" renders to "foo", "bar"                         
  • "{exiftool:Keywords|upper}" renders to: "FOO", "BAR"                        
  • "{exiftool:Keywords|capitalize}" renders to: "Foo", "Bar"                   
  • "{exiftool:Keywords|lower|parens}" renders to: "(foo)", "(bar)"
```

### Comparing `autofile-0.0.7/autofile.egg-info/SOURCES.txt` & `autofile-0.0.8/autofile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autofile-0.0.7/setup.py` & `autofile-0.0.8/setup.py`

 * *Files identical despite different names*

