# Comparing `tmp/reviutils-1.4.0a7.tar.gz` & `tmp/reviutils-1.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reviutils-1.4.0a7.tar", last modified: Wed Apr 17 01:42:31 2024, max compression
+gzip compressed data, was "reviutils-1.4.0b1.tar", last modified: Wed Apr 17 07:06:21 2024, max compression
```

## Comparing `reviutils-1.4.0a7.tar` & `reviutils-1.4.0b1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 01:42:31.315166 reviutils-1.4.0a7/
--rw-rw-rw-   0        0        0    11558 2024-03-14 03:50:07.000000 reviutils-1.4.0a7/LICENSE
--rw-rw-rw-   0        0        0     2872 2024-04-17 01:42:31.314165 reviutils-1.4.0a7/PKG-INFO
--rw-rw-rw-   0        0        0     2546 2024-04-11 07:45:45.000000 reviutils-1.4.0a7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 01:42:31.277888 reviutils-1.4.0a7/reviutils/
-drwxrwxrwx   0        0        0        0 2024-04-17 01:42:31.290888 reviutils-1.4.0a7/reviutils/api/
--rw-rw-rw-   0        0        0       57 2024-03-27 06:31:11.000000 reviutils-1.4.0a7/reviutils/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 01:42:31.292889 reviutils-1.4.0a7/reviutils/api/amap/
--rw-rw-rw-   0        0        0     2497 2024-04-11 08:50:46.000000 reviutils-1.4.0a7/reviutils/api/amap/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-11 08:36:43.000000 reviutils-1.4.0a7/reviutils/api/amap/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-17 01:42:31.295888 reviutils-1.4.0a7/reviutils/audio/
--rw-rw-rw-   0        0        0      116 2024-03-20 03:20:30.000000 reviutils-1.4.0a7/reviutils/audio/__init__.py
--rw-rw-rw-   0        0        0     3232 2024-03-18 03:19:04.000000 reviutils-1.4.0a7/reviutils/audio/clipper.py
--rw-rw-rw-   0        0        0     1534 2024-03-20 03:42:36.000000 reviutils-1.4.0a7/reviutils/audio/reader.py
-drwxrwxrwx   0        0        0        0 2024-04-17 01:42:31.296888 reviutils-1.4.0a7/reviutils/common/
--rw-rw-rw-   0        0        0     3467 2024-03-15 02:38:48.000000 reviutils-1.4.0a7/reviutils/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 01:42:31.301106 reviutils-1.4.0a7/reviutils/gis/
--rw-rw-rw-   0        0        0      106 2024-04-11 06:29:44.000000 reviutils-1.4.0a7/reviutils/gis/__init__.py
--rw-rw-rw-   0        0        0     6807 2024-04-11 08:35:09.000000 reviutils-1.4.0a7/reviutils/gis/convertor.py
--rw-rw-rw-   0        0        0      558 2024-04-11 06:29:44.000000 reviutils-1.4.0a7/reviutils/gis/main.py
-drwxrwxrwx   0        0        0        0 2024-04-17 01:42:31.308165 reviutils-1.4.0a7/reviutils/noisepollution/
--rw-rw-rw-   0        0        0      314 2024-03-20 03:21:45.000000 reviutils-1.4.0a7/reviutils/noisepollution/__init__.py
--rw-rw-rw-   0        0        0     1994 2024-03-14 08:34:09.000000 reviutils-1.4.0a7/reviutils/noisepollution/evaluation.py
--rw-rw-rw-   0        0        0     4114 2024-03-19 08:00:42.000000 reviutils-1.4.0a7/reviutils/noisepollution/funcarea.py
--rw-rw-rw-   0        0        0     1043 2024-03-20 03:33:29.000000 reviutils-1.4.0a7/reviutils/noisepollution/hourhelper.py
--rw-rw-rw-   0        0        0     7313 2024-03-15 02:38:48.000000 reviutils-1.4.0a7/reviutils/noisepollution/splhelper.py
-drwxrwxrwx   0        0        0        0 2024-04-17 01:42:31.309164 reviutils-1.4.0a7/reviutils/omap/
--rw-rw-rw-   0        0        0       22 2024-04-16 08:13:41.000000 reviutils-1.4.0a7/reviutils/omap/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 01:42:31.310166 reviutils-1.4.0a7/reviutils/omap/constants/
--rw-rw-rw-   0        0        0     3701 2024-04-17 01:41:17.000000 reviutils-1.4.0a7/reviutils/omap/constants/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 01:42:31.313166 reviutils-1.4.0a7/reviutils/omap/samples/
--rw-rw-rw-   0        0        0     1131 2024-04-16 02:18:53.000000 reviutils-1.4.0a7/reviutils/omap/samples/Base.py
--rw-rw-rw-   0        0        0       19 2024-04-16 08:13:29.000000 reviutils-1.4.0a7/reviutils/omap/samples/__init__.py
--rw-rw-rw-   0        0        0    12655 2024-04-17 01:24:32.000000 reviutils-1.4.0a7/reviutils/omap/samples/main.py
-drwxrwxrwx   0        0        0        0 2024-04-17 01:42:31.289888 reviutils-1.4.0a7/reviutils.egg-info/
--rw-rw-rw-   0        0        0     2872 2024-04-17 01:42:31.000000 reviutils-1.4.0a7/reviutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      843 2024-04-17 01:42:31.000000 reviutils-1.4.0a7/reviutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 01:42:31.000000 reviutils-1.4.0a7/reviutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 01:42:31.000000 reviutils-1.4.0a7/reviutils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       91 2024-04-17 01:42:31.000000 reviutils-1.4.0a7/reviutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-17 01:42:31.000000 reviutils-1.4.0a7/reviutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 01:42:31.315166 reviutils-1.4.0a7/setup.cfg
--rw-rw-rw-   0        0        0     2371 2024-04-17 01:42:27.000000 reviutils-1.4.0a7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:06:21.288217 reviutils-1.4.0b1/
+-rw-rw-rw-   0        0        0    11558 2024-03-14 03:50:07.000000 reviutils-1.4.0b1/LICENSE
+-rw-rw-rw-   0        0        0     2942 2024-04-17 07:06:21.287217 reviutils-1.4.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0     2616 2024-04-17 02:27:29.000000 reviutils-1.4.0b1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 07:06:21.247236 reviutils-1.4.0b1/reviutils/
+drwxrwxrwx   0        0        0        0 2024-04-17 07:06:21.261220 reviutils-1.4.0b1/reviutils/api/
+-rw-rw-rw-   0        0        0       57 2024-03-27 06:31:11.000000 reviutils-1.4.0b1/reviutils/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:06:21.263235 reviutils-1.4.0b1/reviutils/api/amap/
+-rw-rw-rw-   0        0        0     2497 2024-04-11 08:50:46.000000 reviutils-1.4.0b1/reviutils/api/amap/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-11 08:36:43.000000 reviutils-1.4.0b1/reviutils/api/amap/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:06:21.267218 reviutils-1.4.0b1/reviutils/audio/
+-rw-rw-rw-   0        0        0      116 2024-03-20 03:20:30.000000 reviutils-1.4.0b1/reviutils/audio/__init__.py
+-rw-rw-rw-   0        0        0     3232 2024-03-18 03:19:04.000000 reviutils-1.4.0b1/reviutils/audio/clipper.py
+-rw-rw-rw-   0        0        0     1534 2024-03-20 03:42:36.000000 reviutils-1.4.0b1/reviutils/audio/reader.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:06:21.268217 reviutils-1.4.0b1/reviutils/common/
+-rw-rw-rw-   0        0        0     3467 2024-03-15 02:38:48.000000 reviutils-1.4.0b1/reviutils/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:06:21.273235 reviutils-1.4.0b1/reviutils/gis/
+-rw-rw-rw-   0        0        0      106 2024-04-11 06:29:44.000000 reviutils-1.4.0b1/reviutils/gis/__init__.py
+-rw-rw-rw-   0        0        0     6807 2024-04-11 08:35:09.000000 reviutils-1.4.0b1/reviutils/gis/convertor.py
+-rw-rw-rw-   0        0        0      558 2024-04-11 06:29:44.000000 reviutils-1.4.0b1/reviutils/gis/main.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:06:21.279217 reviutils-1.4.0b1/reviutils/noisepollution/
+-rw-rw-rw-   0        0        0      314 2024-03-20 03:21:45.000000 reviutils-1.4.0b1/reviutils/noisepollution/__init__.py
+-rw-rw-rw-   0        0        0     1994 2024-03-14 08:34:09.000000 reviutils-1.4.0b1/reviutils/noisepollution/evaluation.py
+-rw-rw-rw-   0        0        0     4114 2024-03-19 08:00:42.000000 reviutils-1.4.0b1/reviutils/noisepollution/funcarea.py
+-rw-rw-rw-   0        0        0     1043 2024-03-20 03:33:29.000000 reviutils-1.4.0b1/reviutils/noisepollution/hourhelper.py
+-rw-rw-rw-   0        0        0     7313 2024-03-15 02:38:48.000000 reviutils-1.4.0b1/reviutils/noisepollution/splhelper.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:06:21.281217 reviutils-1.4.0b1/reviutils/omap/
+-rw-rw-rw-   0        0        0      725 2024-04-17 07:01:15.000000 reviutils-1.4.0b1/reviutils/omap/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:06:21.282235 reviutils-1.4.0b1/reviutils/omap/constants/
+-rw-rw-rw-   0        0        0     3751 2024-04-17 03:20:28.000000 reviutils-1.4.0b1/reviutils/omap/constants/__init__.py
+-rw-rw-rw-   0        0        0     1906 2024-04-17 07:05:36.000000 reviutils-1.4.0b1/reviutils/omap/demo.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:06:21.286220 reviutils-1.4.0b1/reviutils/omap/samples/
+-rw-rw-rw-   0        0        0     1131 2024-04-16 02:18:53.000000 reviutils-1.4.0b1/reviutils/omap/samples/Base.py
+-rw-rw-rw-   0        0        0       19 2024-04-16 08:13:29.000000 reviutils-1.4.0b1/reviutils/omap/samples/__init__.py
+-rw-rw-rw-   0        0        0    12837 2024-04-17 07:04:25.000000 reviutils-1.4.0b1/reviutils/omap/samples/main.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:06:21.260220 reviutils-1.4.0b1/reviutils.egg-info/
+-rw-rw-rw-   0        0        0     2942 2024-04-17 07:06:21.000000 reviutils-1.4.0b1/reviutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      866 2024-04-17 07:06:21.000000 reviutils-1.4.0b1/reviutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 07:06:21.000000 reviutils-1.4.0b1/reviutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 07:06:21.000000 reviutils-1.4.0b1/reviutils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       91 2024-04-17 07:06:21.000000 reviutils-1.4.0b1/reviutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-17 07:06:21.000000 reviutils-1.4.0b1/reviutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 07:06:21.288217 reviutils-1.4.0b1/setup.cfg
+-rw-rw-rw-   0        0        0     2371 2024-04-17 07:06:15.000000 reviutils-1.4.0b1/setup.py
```

### Comparing `reviutils-1.4.0a7/LICENSE` & `reviutils-1.4.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a7/PKG-INFO` & `reviutils-1.4.0b1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviutils
-Version: 1.4.0a7
+Version: 1.4.0b1
 Summary: A common library frequently used on python
 Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI
 Author-email: reviy-top@outlook.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: audio
@@ -67,14 +67,18 @@
 
   提供读取音频文件的能力。此功能允许您将音频文件加载到应用程序中进行进一步处理或分析。
 
 ### reviutils.gis
 
     提供经纬度转换器。
 
+### reviutils.omap
+
+    用于管理与生成Omap地图对象。
+
 ## 安装
 
 #### 常规模块安装
 
 ```
 pip install --upgrade pip
 pip install reviutils
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reviutils Version: 1.4.0a7 Summary: A common
+Metadata-Version: 2.1 Name: reviutils Version: 1.4.0b1 Summary: A common
 library frequently used on python Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
 Description-Content-Type: text/markdown Provides-Extra: audio License-File:
 LICENSE
                             ************ rreevviiuuttiillss ************
                            ä¸ä¸ªå¸¸ç¨çPythonåº
                             _ç_®__ä_½__ä_¸_­_æ__ï½ _E_n_g_l_i_s_h
@@ -23,11 +23,12 @@
 å°æ¶æ°æ®å¤çï¼å¯å¯¹å°æ¶æ°æ®è¿è¡å¤çï¼åºåç½å¤©åå¤ææ¶æ®µã
 - #### reviutils.noisepollution.splhelper
 å£°åçº§ï¼SPLï¼è®¡ç®ï¼æä¾ä»æ°æ®è®¡ç®å£°åçº§çåè½ã ###
 reviutils.audio > éè¦é¢å¤çå®è£ - #### reviutils.audio.clipper
 æä¾è£åªæå¡«åé³é¢æä»¶çåè½ãæ¨å¯ä»¥ä½¿ç¨æ­¤åè½æ¥ä¿®åªé³é¢çæ®µæå¨é³é¢çå¼å¤´æç»å°¾æ·»å éé³ã
 - #### reviutils.audio.reader
 æä¾è¯»åé³é¢æä»¶çè½åãæ­¤åè½åè®¸æ¨å°é³é¢æä»¶å è½½å°åºç¨ç¨åºä¸­è¿è¡è¿ä¸æ­¥å¤çæåæã
-### reviutils.gis æä¾ç»çº¬åº¦è½¬æ¢å¨ã ## å®è£ #### å¸¸è§æ¨¡åå®è£
-``` pip install --upgrade pip pip install reviutils ``` #### é¢å¤å®è£ ```
-pip install reviutils[audio] ``` ### è®¸å¯è¯
+### reviutils.gis æä¾ç»çº¬åº¦è½¬æ¢å¨ã ### reviutils.omap
+ç¨äºç®¡çä¸çæOmapå°å¾å¯¹è±¡ã ## å®è£ #### å¸¸è§æ¨¡åå®è£ ```
+pip install --upgrade pip pip install reviutils ``` #### é¢å¤å®è£ ``` pip
+install reviutils[audio] ``` ### è®¸å¯è¯
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_l_i_c_e_n_s_e_-_A_p_a_c_h_e_-_-_2_._0_-_y_e_l_l_o_w_]
```

### Comparing `reviutils-1.4.0a7/README.md` & `reviutils-1.4.0b1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,18 @@
 
   提供读取音频文件的能力。此功能允许您将音频文件加载到应用程序中进行进一步处理或分析。
 
 ### reviutils.gis
 
     提供经纬度转换器。
 
+### reviutils.omap
+
+    用于管理与生成Omap地图对象。
+
 ## 安装
 
 #### 常规模块安装
 
 ```
 pip install --upgrade pip
 pip install reviutils
```

#### html2text {}

```diff
@@ -18,11 +18,12 @@
 å°æ¶æ°æ®å¤çï¼å¯å¯¹å°æ¶æ°æ®è¿è¡å¤çï¼åºåç½å¤©åå¤ææ¶æ®µã
 - #### reviutils.noisepollution.splhelper
 å£°åçº§ï¼SPLï¼è®¡ç®ï¼æä¾ä»æ°æ®è®¡ç®å£°åçº§çåè½ã ###
 reviutils.audio > éè¦é¢å¤çå®è£ - #### reviutils.audio.clipper
 æä¾è£åªæå¡«åé³é¢æä»¶çåè½ãæ¨å¯ä»¥ä½¿ç¨æ­¤åè½æ¥ä¿®åªé³é¢çæ®µæå¨é³é¢çå¼å¤´æç»å°¾æ·»å éé³ã
 - #### reviutils.audio.reader
 æä¾è¯»åé³é¢æä»¶çè½åãæ­¤åè½åè®¸æ¨å°é³é¢æä»¶å è½½å°åºç¨ç¨åºä¸­è¿è¡è¿ä¸æ­¥å¤çæåæã
-### reviutils.gis æä¾ç»çº¬åº¦è½¬æ¢å¨ã ## å®è£ #### å¸¸è§æ¨¡åå®è£
-``` pip install --upgrade pip pip install reviutils ``` #### é¢å¤å®è£ ```
-pip install reviutils[audio] ``` ### è®¸å¯è¯
+### reviutils.gis æä¾ç»çº¬åº¦è½¬æ¢å¨ã ### reviutils.omap
+ç¨äºç®¡çä¸çæOmapå°å¾å¯¹è±¡ã ## å®è£ #### å¸¸è§æ¨¡åå®è£ ```
+pip install --upgrade pip pip install reviutils ``` #### é¢å¤å®è£ ``` pip
+install reviutils[audio] ``` ### è®¸å¯è¯
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_l_i_c_e_n_s_e_-_A_p_a_c_h_e_-_-_2_._0_-_y_e_l_l_o_w_]
```

### Comparing `reviutils-1.4.0a7/reviutils/api/amap/__init__.py` & `reviutils-1.4.0b1/reviutils/api/amap/__init__.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a7/reviutils/audio/clipper.py` & `reviutils-1.4.0b1/reviutils/audio/clipper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a7/reviutils/audio/reader.py` & `reviutils-1.4.0b1/reviutils/audio/reader.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a7/reviutils/common/__init__.py` & `reviutils-1.4.0b1/reviutils/common/__init__.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a7/reviutils/gis/convertor.py` & `reviutils-1.4.0b1/reviutils/gis/convertor.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a7/reviutils/gis/main.py` & `reviutils-1.4.0b1/reviutils/gis/main.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a7/reviutils/noisepollution/evaluation.py` & `reviutils-1.4.0b1/reviutils/noisepollution/evaluation.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a7/reviutils/noisepollution/funcarea.py` & `reviutils-1.4.0b1/reviutils/noisepollution/funcarea.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a7/reviutils/noisepollution/hourhelper.py` & `reviutils-1.4.0b1/reviutils/noisepollution/hourhelper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a7/reviutils/noisepollution/splhelper.py` & `reviutils-1.4.0b1/reviutils/noisepollution/splhelper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a7/reviutils/omap/constants/__init__.py` & `reviutils-1.4.0b1/reviutils/omap/constants/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     Pink = Color(name="粉色", id=4202692863)
     Green = Color(name="绿色", id=4194369280)
     Blue = Color(name="蓝色", id=4211015680)
     Red = Color(name="红色", id=4194304255)
     Yellow = Color(name="黄色", id=4194369535)
     Cyan = Color(name="青色", id=4211080960)
     Purple = Color(name="紫色", id=4211015808)
+    Orange = Color(name="橙色", id=4194304511)
 # endregion
 
 
 # region 对象类型
 class ObjectType(ConstantsBase):
     """
     Object type class
```

### Comparing `reviutils-1.4.0a7/reviutils/omap/samples/Base.py` & `reviutils-1.4.0b1/reviutils/omap/samples/Base.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a7/reviutils/omap/samples/main.py` & `reviutils-1.4.0b1/reviutils/omap/samples/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,27 +90,27 @@
 class Polyline(ItemBase):
     def __init__(
         self,
         name: str,
         polyline_type: PolylineTypes,
         latlng: List[float],
         is_gcj02: bool,
-        line_color: Colors = Colors.Default,
+        line_color: Union[Colors,int] = Colors.Default,
         line_width: int = 1,
         line_alpha: int = 100,
         show_name: bool = False,
         edit: bool = False,
         parent_id: int = 1,
     ):
         # 检查坐标数量是否符合要求
         if len(latlng) % 2 != 0:
             raise ValueError("Polyline coordinates should be even number")
         assert len(latlng)>=polyline_type.value.length_min*2 and len(latlng)<=polyline_type.value.length_max*2, f"Polyline coordinates should be between {polyline_type.value.length_min*2} and {polyline_type.value.length_max*2}"
         tdo = TrackDrawObject(
-            LineClr=line_color.value.id,
+            LineClr=line_color.value.id if isinstance(line_color, Colors) else line_color,
             LineWidth=line_width,
             LineAlpha=line_alpha,
             ShowType=polyline_type.value.ShowType,
         )
         detail = PolylineDetail(
             Gcj02=is_gcj02,
             Mtp = len(latlng)//2 if polyline_type == PolylineTypes.Polyline else polyline_type.value.Mtp,
@@ -184,20 +184,20 @@
     def __init__(
         self,
         name: str,
         lng: float,
         lat: float,
         is_gcj02: bool,
         font_size:int = 16,
-        color: Colors = Colors.Default,
+        color: Union[Colors,int] = Colors.Default,
         rotation: int = 0,
         parent_id: int = 1,
     ):
         extinfo = ExtInfoObject(
-            FontClr=color.value.id,
+            FontClr=color.value.id if isinstance(color, Colors) else color,
             FontRotateAngle=rotation,
             FontSize=font_size
         )
         detail = TextDetail(Lng=lng, Lat=lat, Gcj02=is_gcj02, ExtInfo=extinfo)
         obj = ObjectBase(
             name=name, obj_detail=detail, type_id=ObjectTypes.Point.value.id
         )
@@ -276,17 +276,19 @@
             raise NotImplementedError(f"Unsupported child type: {type(child)}")
 
 
 class Folder(ItemBase):
     def __init__(
         self,
         name: str,
-        detail: FolderDetail,
+        detail: FolderDetail=None,
         parent_id: int = 1,
     ):
+        if detail is None:
+            detail = FolderDetail()
         obj = ObjectBase(
             name=name, obj_detail=detail, type_id=ObjectTypes.Folder.value.id
         )
         super().__init__(
             obj=obj,
             parent_id=parent_id,
             type_id=ObjectTypes.Folder.value.id,
```

### Comparing `reviutils-1.4.0a7/reviutils.egg-info/PKG-INFO` & `reviutils-1.4.0b1/reviutils.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviutils
-Version: 1.4.0a7
+Version: 1.4.0b1
 Summary: A common library frequently used on python
 Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI
 Author-email: reviy-top@outlook.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: audio
@@ -67,14 +67,18 @@
 
   提供读取音频文件的能力。此功能允许您将音频文件加载到应用程序中进行进一步处理或分析。
 
 ### reviutils.gis
 
     提供经纬度转换器。
 
+### reviutils.omap
+
+    用于管理与生成Omap地图对象。
+
 ## 安装
 
 #### 常规模块安装
 
 ```
 pip install --upgrade pip
 pip install reviutils
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reviutils Version: 1.4.0a7 Summary: A common
+Metadata-Version: 2.1 Name: reviutils Version: 1.4.0b1 Summary: A common
 library frequently used on python Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
 Description-Content-Type: text/markdown Provides-Extra: audio License-File:
 LICENSE
                             ************ rreevviiuuttiillss ************
                            ä¸ä¸ªå¸¸ç¨çPythonåº
                             _ç_®__ä_½__ä_¸_­_æ__ï½ _E_n_g_l_i_s_h
@@ -23,11 +23,12 @@
 å°æ¶æ°æ®å¤çï¼å¯å¯¹å°æ¶æ°æ®è¿è¡å¤çï¼åºåç½å¤©åå¤ææ¶æ®µã
 - #### reviutils.noisepollution.splhelper
 å£°åçº§ï¼SPLï¼è®¡ç®ï¼æä¾ä»æ°æ®è®¡ç®å£°åçº§çåè½ã ###
 reviutils.audio > éè¦é¢å¤çå®è£ - #### reviutils.audio.clipper
 æä¾è£åªæå¡«åé³é¢æä»¶çåè½ãæ¨å¯ä»¥ä½¿ç¨æ­¤åè½æ¥ä¿®åªé³é¢çæ®µæå¨é³é¢çå¼å¤´æç»å°¾æ·»å éé³ã
 - #### reviutils.audio.reader
 æä¾è¯»åé³é¢æä»¶çè½åãæ­¤åè½åè®¸æ¨å°é³é¢æä»¶å è½½å°åºç¨ç¨åºä¸­è¿è¡è¿ä¸æ­¥å¤çæåæã
-### reviutils.gis æä¾ç»çº¬åº¦è½¬æ¢å¨ã ## å®è£ #### å¸¸è§æ¨¡åå®è£
-``` pip install --upgrade pip pip install reviutils ``` #### é¢å¤å®è£ ```
-pip install reviutils[audio] ``` ### è®¸å¯è¯
+### reviutils.gis æä¾ç»çº¬åº¦è½¬æ¢å¨ã ### reviutils.omap
+ç¨äºç®¡çä¸çæOmapå°å¾å¯¹è±¡ã ## å®è£ #### å¸¸è§æ¨¡åå®è£ ```
+pip install --upgrade pip pip install reviutils ``` #### é¢å¤å®è£ ``` pip
+install reviutils[audio] ``` ### è®¸å¯è¯
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_l_i_c_e_n_s_e_-_A_p_a_c_h_e_-_-_2_._0_-_y_e_l_l_o_w_]
```

### Comparing `reviutils-1.4.0a7/reviutils.egg-info/SOURCES.txt` & `reviutils-1.4.0b1/reviutils.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -19,11 +19,12 @@
 reviutils/gis/main.py
 reviutils/noisepollution/__init__.py
 reviutils/noisepollution/evaluation.py
 reviutils/noisepollution/funcarea.py
 reviutils/noisepollution/hourhelper.py
 reviutils/noisepollution/splhelper.py
 reviutils/omap/__init__.py
+reviutils/omap/demo.py
 reviutils/omap/constants/__init__.py
 reviutils/omap/samples/Base.py
 reviutils/omap/samples/__init__.py
 reviutils/omap/samples/main.py
```

### Comparing `reviutils-1.4.0a7/setup.py` & `reviutils-1.4.0b1/setup.py`

 * *Files identical despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 import os, shutil
 from setuptools import setup
 
 
 name = "reviutils"
-version = "1.4.0a7"
+version = "1.4.0b1"
 packages = [
     "reviutils.common",
     "reviutils.noisepollution",
     "reviutils.audio",
     "reviutils.api",
     "reviutils.api.amap",
     "reviutils.gis",
```

