# Comparing `tmp/p_eo-0.3.0-py3-none-any.whl.zip` & `tmp/p_eo-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 14715 bytes, number of entries: 16
--rw-r--r--  2.0 unx      250 b- defN 24-Mar-01 02:00 P_EO/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-01 02:00 P_EO/common/__init__.py
--rw-r--r--  2.0 unx      387 b- defN 24-Mar-01 02:00 P_EO/common/config.py
--rw-r--r--  2.0 unx     1619 b- defN 24-Mar-01 02:00 P_EO/common/error.py
--rw-r--r--  2.0 unx     1709 b- defN 24-Mar-01 02:00 P_EO/common/log.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-01 02:00 P_EO/core/__init__.py
--rw-r--r--  2.0 unx    10402 b- defN 24-Mar-01 02:00 P_EO/core/action.py
--rw-r--r--  2.0 unx     5372 b- defN 24-Mar-01 02:00 P_EO/core/driver.py
--rw-r--r--  2.0 unx     6456 b- defN 24-Mar-01 02:00 P_EO/core/elements.py
--rw-r--r--  2.0 unx     1161 b- defN 24-Mar-01 02:00 P_EO/core/javascript.py
--rw-r--r--  2.0 unx     1315 b- defN 24-Mar-01 02:00 P_EO/core/page.py
--rw-r--r--  2.0 unx    11558 b- defN 24-Mar-01 02:00 p_eo-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      319 b- defN 24-Mar-01 02:00 p_eo-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-01 02:00 p_eo-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Mar-01 02:00 p_eo-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1208 b- defN 24-Mar-01 02:00 p_eo-0.3.0.dist-info/RECORD
-16 files, 41853 bytes uncompressed, 12753 bytes compressed:  69.5%
+Zip file size: 14773 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      250 b- defN 24-Apr-17 09:59 P_EO/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 09:59 P_EO/common/__init__.py
+-rw-r--r--  2.0 unx      387 b- defN 24-Apr-17 09:59 P_EO/common/config.py
+-rw-r--r--  2.0 unx     1619 b- defN 24-Apr-17 09:59 P_EO/common/error.py
+-rw-r--r--  2.0 unx     1709 b- defN 24-Apr-17 09:59 P_EO/common/log.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 09:59 P_EO/core/__init__.py
+-rw-r--r--  2.0 unx    10508 b- defN 24-Apr-17 09:59 P_EO/core/action.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-Apr-17 09:59 P_EO/core/driver.py
+-rw-r--r--  2.0 unx     6456 b- defN 24-Apr-17 09:59 P_EO/core/elements.py
+-rw-r--r--  2.0 unx     1161 b- defN 24-Apr-17 09:59 P_EO/core/javascript.py
+-rw-r--r--  2.0 unx     1315 b- defN 24-Apr-17 09:59 P_EO/core/page.py
+-rw-r--r--  2.0 unx    11558 b- defN 24-Apr-17 09:59 p_eo-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      319 b- defN 24-Apr-17 09:59 p_eo-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 09:59 p_eo-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-17 09:59 p_eo-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1208 b- defN 24-Apr-17 09:59 p_eo-0.3.1.dist-info/RECORD
+16 files, 41959 bytes uncompressed, 12811 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: P_EO/core/javascript.py
 Comment: 
 
 Filename: P_EO/core/page.py
 Comment: 
 
-Filename: p_eo-0.3.0.dist-info/LICENSE
+Filename: p_eo-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: p_eo-0.3.0.dist-info/METADATA
+Filename: p_eo-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: p_eo-0.3.0.dist-info/WHEEL
+Filename: p_eo-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: p_eo-0.3.0.dist-info/top_level.txt
+Filename: p_eo-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: p_eo-0.3.0.dist-info/RECORD
+Filename: p_eo-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## P_EO/__init__.py

```diff
@@ -1,12 +1,12 @@
 from P_EO.common.config import Default, LogConfig
 from P_EO.core.elements import Element, Elements, IFrame
 from P_EO.core.page import Page
 
-VERSION = '0.3.0'
+VERSION = '0.3.1'
 
 __all__ = [
     Element,
     Elements,
     IFrame,
     Page,
     Default,
```

## P_EO/core/action.py

```diff
@@ -109,15 +109,16 @@
 
     def action_chains(self, wait=Default.ACTION_WAIT):
         """
         元素滚动到可见，并返回一个ActionChains对象
         :param wait:
         :return:
         """
-        ActionChains(self.driver).scroll_to_element(self.ele()).perform()
+        self.scrolled_into_view()
+        # ActionChains(self.driver).scroll_to_element(self.ele()).perform()  # selenium==3.141.0 好像没有这个语法，>=4以上好像才有
         time.sleep(wait)
         return ActionChains(self.driver)
 
     def click_by_action_chains(self, wait=Default.ACTION_WAIT):
         """
         元素滚动并点击
         :param wait:
```

## Comparing `p_eo-0.3.0.dist-info/LICENSE` & `p_eo-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `p_eo-0.3.0.dist-info/RECORD` & `p_eo-0.3.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-P_EO/__init__.py,sha256=OTFJTOT7KkYF20D17YdE5cQUjMbSdh2dI7Yw2Cjk-NI,250
+P_EO/__init__.py,sha256=uPB9dpTLr7rP7RQ_W1PgiGZfwbFe_jkR4ekbHAlwGA0,250
 P_EO/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 P_EO/common/config.py,sha256=J-AF4NgApJPT4SMlI2sfaErZfFhReXXobmr2nKenBXA,387
 P_EO/common/error.py,sha256=eoaHHTSo5sy6g1dtTfiRJNvwNc1ruDgv0tzHI67_lrE,1619
 P_EO/common/log.py,sha256=j6I7Cv8pXWMzeDr0tQ0AAvjBTBISnf2ojEfK_zn2sBs,1709
 P_EO/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-P_EO/core/action.py,sha256=VsUmDkuFePHpm7DXzhagZFZRmDGfi1RrqNmL2mKzmP8,10402
+P_EO/core/action.py,sha256=Va1fqwMvbNi-IwHmoK-R-7iOWEAv-FcM-o5J3qHS4RA,10508
 P_EO/core/driver.py,sha256=nSaEp4xniNJYU9Q8NTrx_X1BmMA5OqxrPtXCyr7971M,5372
 P_EO/core/elements.py,sha256=btoewjpUxst-tlU8x_TeKt9LFmbAHExshi3wOGbJCFA,6456
 P_EO/core/javascript.py,sha256=PqmqW_iq9GM4rdfGWXtdhmnP10WT0F2_Y9IFP4wlv38,1161
 P_EO/core/page.py,sha256=JuHxK9ERu0vZ_y7JOwL2ZQRTH221CUzQXVg7bcYo7V4,1315
-p_eo-0.3.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-p_eo-0.3.0.dist-info/METADATA,sha256=kbbWJa2T6bdV0Tvd1Ybcd7dztsKWnGM4EpOnGjyjOog,319
-p_eo-0.3.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-p_eo-0.3.0.dist-info/top_level.txt,sha256=l3zgFCnD5y70VQdYdQwMMn9JMvcXF1Qfn7Xnr6_2Nq8,5
-p_eo-0.3.0.dist-info/RECORD,,
+p_eo-0.3.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+p_eo-0.3.1.dist-info/METADATA,sha256=-hVSsUGBodfBRys6v9hu5Sw7FzZSwa2S__Y7aMLT73s,319
+p_eo-0.3.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+p_eo-0.3.1.dist-info/top_level.txt,sha256=l3zgFCnD5y70VQdYdQwMMn9JMvcXF1Qfn7Xnr6_2Nq8,5
+p_eo-0.3.1.dist-info/RECORD,,
```

