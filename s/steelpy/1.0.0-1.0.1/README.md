# Comparing `tmp/steelpy-1.0.0.tar.gz` & `tmp/steelpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steelpy-1.0.0.tar", max compression
+gzip compressed data, was "steelpy-1.0.1.tar", max compression
```

## Comparing `steelpy-1.0.0.tar` & `steelpy-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11558 2024-04-15 00:15:35.250711 steelpy-1.0.0/license.txt
--rw-r--r--   0        0        0      489 2024-04-15 00:56:17.482306 steelpy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1491 2024-04-14 19:17:05.548477 steelpy-1.0.0/README.md
--rw-r--r--   0        0        0       25 2024-04-15 00:07:30.681181 steelpy-1.0.0/steelpy/__init__.py
--rw-r--r--   0        0        0    11358 2024-04-15 00:44:17.980620 steelpy-1.0.0/steelpy/LICENSE.md
--rw-r--r--   0        0        0       10 2024-04-15 00:44:17.980620 steelpy-1.0.0/steelpy/README.md
--rw-r--r--   0        0        0     6148 2024-04-13 14:24:11.525081 steelpy-1.0.0/steelpy/shape files/.DS_Store
--rw-r--r--   0        0        0    11454 2024-04-13 14:22:22.387676 steelpy-1.0.0/steelpy/shape files/C_shapes.xlsx
--rw-r--r--   0        0        0    55958 2024-04-13 14:22:22.517421 steelpy-1.0.0/steelpy/shape files/DBL_L_shapes.xlsx
--rw-r--r--   0        0        0     8761 2024-04-13 14:22:22.531852 steelpy-1.0.0/steelpy/shape files/HP_shapes.xlsx
--rw-r--r--   0        0        0    19577 2024-04-13 14:22:22.685953 steelpy-1.0.0/steelpy/shape files/HSS_R_shapes.xlsx
--rw-r--r--   0        0        0    53674 2024-04-13 14:22:22.648944 steelpy-1.0.0/steelpy/shape files/HSS_shapes.xlsx
--rw-r--r--   0        0        0    32880 2024-04-13 14:22:22.749414 steelpy-1.0.0/steelpy/shape files/L_shapes.xlsx
--rw-r--r--   0        0        0     7785 2024-04-13 14:22:22.761931 steelpy-1.0.0/steelpy/shape files/M_shapes.xlsx
--rw-r--r--   0        0        0    12974 2024-04-13 14:22:22.783967 steelpy-1.0.0/steelpy/shape files/MC_shapes.xlsx
--rw-r--r--   0        0        0     6841 2024-04-13 14:22:22.794757 steelpy-1.0.0/steelpy/shape files/MT_shapes.xlsx
--rw-r--r--   0        0        0     9052 2024-04-13 14:22:22.809959 steelpy-1.0.0/steelpy/shape files/PIPE_shapes.xlsx
--rw-r--r--   0        0        0     9556 2024-04-13 14:22:22.825993 steelpy-1.0.0/steelpy/shape files/S_shapes.xlsx
--rw-r--r--   0        0        0     8516 2024-04-13 14:22:22.839824 steelpy-1.0.0/steelpy/shape files/ST_shapes.xlsx
--rw-r--r--   0        0        0    51977 2024-04-13 14:22:22.946043 steelpy-1.0.0/steelpy/shape files/W_shapes.xlsx
--rw-r--r--   0        0        0    46395 2024-04-13 14:22:23.030673 steelpy-1.0.0/steelpy/shape files/WT_shapes.xlsx
--rw-r--r--   0        0        0     1829 2024-04-15 00:07:31.541137 steelpy-1.0.0/steelpy/steelpy.py
--rw-r--r--   0        0        0     2011 1970-01-01 00:00:00.000000 steelpy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-15 00:15:35.250711 steelpy-1.0.1/license.txt
+-rw-r--r--   0        0        0      488 2024-04-16 23:54:26.912611 steelpy-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1491 2024-04-14 19:17:05.548477 steelpy-1.0.1/README.md
+-rw-r--r--   0        0        0       25 2024-04-15 00:07:30.681181 steelpy-1.0.1/steelpy/__init__.py
+-rw-r--r--   0        0        0    11358 2024-04-15 00:44:17.980620 steelpy-1.0.1/steelpy/LICENSE.md
+-rw-r--r--   0        0        0       10 2024-04-15 00:44:17.980620 steelpy-1.0.1/steelpy/README.md
+-rw-r--r--   0        0        0     6148 2024-04-13 14:24:11.525081 steelpy-1.0.1/steelpy/shape files/.DS_Store
+-rw-r--r--   0        0        0    11454 2024-04-13 14:22:22.387676 steelpy-1.0.1/steelpy/shape files/C_shapes.xlsx
+-rw-r--r--   0        0        0    55958 2024-04-13 14:22:22.517421 steelpy-1.0.1/steelpy/shape files/DBL_L_shapes.xlsx
+-rw-r--r--   0        0        0     8761 2024-04-13 14:22:22.531852 steelpy-1.0.1/steelpy/shape files/HP_shapes.xlsx
+-rw-r--r--   0        0        0    19577 2024-04-13 14:22:22.685953 steelpy-1.0.1/steelpy/shape files/HSS_R_shapes.xlsx
+-rw-r--r--   0        0        0    53674 2024-04-13 14:22:22.648944 steelpy-1.0.1/steelpy/shape files/HSS_shapes.xlsx
+-rw-r--r--   0        0        0    32880 2024-04-13 14:22:22.749414 steelpy-1.0.1/steelpy/shape files/L_shapes.xlsx
+-rw-r--r--   0        0        0     7785 2024-04-13 14:22:22.761931 steelpy-1.0.1/steelpy/shape files/M_shapes.xlsx
+-rw-r--r--   0        0        0    12974 2024-04-13 14:22:22.783967 steelpy-1.0.1/steelpy/shape files/MC_shapes.xlsx
+-rw-r--r--   0        0        0     6841 2024-04-13 14:22:22.794757 steelpy-1.0.1/steelpy/shape files/MT_shapes.xlsx
+-rw-r--r--   0        0        0     9052 2024-04-13 14:22:22.809959 steelpy-1.0.1/steelpy/shape files/PIPE_shapes.xlsx
+-rw-r--r--   0        0        0     9556 2024-04-13 14:22:22.825993 steelpy-1.0.1/steelpy/shape files/S_shapes.xlsx
+-rw-r--r--   0        0        0     8516 2024-04-13 14:22:22.839824 steelpy-1.0.1/steelpy/shape files/ST_shapes.xlsx
+-rw-r--r--   0        0        0    51977 2024-04-13 14:22:22.946043 steelpy-1.0.1/steelpy/shape files/W_shapes.xlsx
+-rw-r--r--   0        0        0    46395 2024-04-13 14:22:23.030673 steelpy-1.0.1/steelpy/shape files/WT_shapes.xlsx
+-rw-r--r--   0        0        0     1829 2024-04-16 23:47:01.477340 steelpy-1.0.1/steelpy/steelpy.py
+-rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 steelpy-1.0.1/PKG-INFO
```

### Comparing `steelpy-1.0.0/license.txt` & `steelpy-1.0.1/license.txt`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/README.md` & `steelpy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/LICENSE.md` & `steelpy-1.0.1/steelpy/LICENSE.md`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/shape files/.DS_Store` & `steelpy-1.0.1/steelpy/shape files/.DS_Store`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/shape files/C_shapes.xlsx` & `steelpy-1.0.1/steelpy/shape files/C_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/shape files/DBL_L_shapes.xlsx` & `steelpy-1.0.1/steelpy/shape files/DBL_L_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/shape files/HP_shapes.xlsx` & `steelpy-1.0.1/steelpy/shape files/HP_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/shape files/HSS_R_shapes.xlsx` & `steelpy-1.0.1/steelpy/shape files/HSS_R_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/shape files/HSS_shapes.xlsx` & `steelpy-1.0.1/steelpy/shape files/HSS_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/shape files/L_shapes.xlsx` & `steelpy-1.0.1/steelpy/shape files/L_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/shape files/M_shapes.xlsx` & `steelpy-1.0.1/steelpy/shape files/M_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/shape files/MC_shapes.xlsx` & `steelpy-1.0.1/steelpy/shape files/MC_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/shape files/MT_shapes.xlsx` & `steelpy-1.0.1/steelpy/shape files/MT_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/shape files/PIPE_shapes.xlsx` & `steelpy-1.0.1/steelpy/shape files/PIPE_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/shape files/S_shapes.xlsx` & `steelpy-1.0.1/steelpy/shape files/S_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/shape files/ST_shapes.xlsx` & `steelpy-1.0.1/steelpy/shape files/ST_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/shape files/W_shapes.xlsx` & `steelpy-1.0.1/steelpy/shape files/W_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/shape files/WT_shapes.xlsx` & `steelpy-1.0.1/steelpy/shape files/WT_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.0/steelpy/steelpy.py` & `steelpy-1.0.1/steelpy/steelpy.py`

 * *Files identical despite different names*

