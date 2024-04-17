# Comparing `tmp/PKNSETools-0.1.20240417.85.tar.gz` & `tmp/PKNSETools-0.1.20240417.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKNSETools-0.1.20240417.85.tar", last modified: Wed Apr 17 21:31:55 2024, max compression
+gzip compressed data, was "PKNSETools-0.1.20240417.86.tar", last modified: Wed Apr 17 21:36:01 2024, max compression
```

## Comparing `PKNSETools-0.1.20240417.85.tar` & `PKNSETools-0.1.20240417.86.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 21:31:55.158485 PKNSETools-0.1.20240417.85/
--rw-rw-rw-   0        0        0     2661 2024-04-17 21:31:55.158485 PKNSETools-0.1.20240417.85/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 21:31:55.158485 PKNSETools-0.1.20240417.85/PKNSETools/
-drwxrwxrwx   0        0        0        0 2024-04-17 21:31:55.158485 PKNSETools-0.1.20240417.85/PKNSETools/Benny/
--rw-rw-rw-   0        0        0    34274 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/Benny/NSE.py
--rw-rw-rw-   0        0        0     1198 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/Benny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 21:31:55.158485 PKNSETools-0.1.20240417.85/PKNSETools/Nasdaq/
--rw-rw-rw-   0        0        0     3392 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/Nasdaq/PKNasdaqIndex.py
--rw-rw-rw-   0        0        0     1225 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/Nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4806 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/PKAllStocks.py
--rw-rw-rw-   0        0        0    10032 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/PKCompanyGeneral.py
--rw-rw-rw-   0        0        0     3303 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/PKCompanyStock.py
--rw-rw-rw-   0        0        0     2223 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/PKConstants.py
--rw-rw-rw-   0        0        0     5168 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/PKIntraDay.py
--rw-rw-rw-   0        0        0     6446 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    12667 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/PKNSEStockDataFetcher.py
--rw-rw-rw-   0        0        0       30 2024-04-17 21:31:50.000000 PKNSETools-0.1.20240417.85/PKNSETools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 21:31:55.158485 PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/
--rw-rw-rw-   0        0        0     1830 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/NSEStockDB.py
--rw-rw-rw-   0        0        0     1848 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/NSEStockFairValueDB.py
--rw-rw-rw-   0        0        0     1836 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/NSEStockMFIDB.py
--rw-rw-rw-   0        0        0    61965 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
--rw-rw-rw-   0        0        0     1378 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/error.py
--rw-rw-rw-   0        0        0    40060 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/funds.py
--rw-rw-rw-   0        0        0    22036 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/search.py
--rw-rw-rw-   0        0        0    13495 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/security.py
--rw-rw-rw-   0        0        0    29930 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/stock.py
--rw-rw-rw-   0        0        0    23246 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-17 21:31:55.158485 PKNSETools-0.1.20240417.85/PKNSETools.egg-info/
--rw-rw-rw-   0        0        0     2661 2024-04-17 21:31:55.000000 PKNSETools-0.1.20240417.85/PKNSETools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1041 2024-04-17 21:31:55.000000 PKNSETools-0.1.20240417.85/PKNSETools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 21:31:55.000000 PKNSETools-0.1.20240417.85/PKNSETools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 21:31:49.000000 PKNSETools-0.1.20240417.85/PKNSETools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2024-04-17 21:31:55.000000 PKNSETools-0.1.20240417.85/PKNSETools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-17 21:31:55.000000 PKNSETools-0.1.20240417.85/PKNSETools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1884 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/README.md
--rw-rw-rw-   0        0        0       86 2024-04-17 21:31:55.158485 PKNSETools-0.1.20240417.85/setup.cfg
--rw-rw-rw-   0        0        0     3832 2024-04-17 21:30:33.000000 PKNSETools-0.1.20240417.85/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:36:01.769641 PKNSETools-0.1.20240417.86/
+-rw-rw-rw-   0        0        0     2661 2024-04-17 21:36:01.769641 PKNSETools-0.1.20240417.86/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 21:36:01.769641 PKNSETools-0.1.20240417.86/PKNSETools/
+drwxrwxrwx   0        0        0        0 2024-04-17 21:36:01.769641 PKNSETools-0.1.20240417.86/PKNSETools/Benny/
+-rw-rw-rw-   0        0        0    34274 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/Benny/NSE.py
+-rw-rw-rw-   0        0        0     1198 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/Benny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:36:01.769641 PKNSETools-0.1.20240417.86/PKNSETools/Nasdaq/
+-rw-rw-rw-   0        0        0     3392 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/Nasdaq/PKNasdaqIndex.py
+-rw-rw-rw-   0        0        0     1225 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/Nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4806 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/PKAllStocks.py
+-rw-rw-rw-   0        0        0    10032 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/PKCompanyGeneral.py
+-rw-rw-rw-   0        0        0     3303 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/PKCompanyStock.py
+-rw-rw-rw-   0        0        0     2223 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/PKConstants.py
+-rw-rw-rw-   0        0        0     5168 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/PKIntraDay.py
+-rw-rw-rw-   0        0        0     6446 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    12681 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/PKNSEStockDataFetcher.py
+-rw-rw-rw-   0        0        0       30 2024-04-17 21:35:58.000000 PKNSETools-0.1.20240417.86/PKNSETools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:36:01.769641 PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/
+-rw-rw-rw-   0        0        0     1830 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/NSEStockDB.py
+-rw-rw-rw-   0        0        0     1848 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/NSEStockFairValueDB.py
+-rw-rw-rw-   0        0        0     1836 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/NSEStockMFIDB.py
+-rw-rw-rw-   0        0        0    61965 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
+-rw-rw-rw-   0        0        0     1378 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/error.py
+-rw-rw-rw-   0        0        0    40060 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/funds.py
+-rw-rw-rw-   0        0        0    22038 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/search.py
+-rw-rw-rw-   0        0        0    13495 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/security.py
+-rw-rw-rw-   0        0        0    29930 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/stock.py
+-rw-rw-rw-   0        0        0    23246 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:36:01.769641 PKNSETools-0.1.20240417.86/PKNSETools.egg-info/
+-rw-rw-rw-   0        0        0     2661 2024-04-17 21:36:01.000000 PKNSETools-0.1.20240417.86/PKNSETools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1041 2024-04-17 21:36:01.000000 PKNSETools-0.1.20240417.86/PKNSETools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 21:36:01.000000 PKNSETools-0.1.20240417.86/PKNSETools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 21:35:56.000000 PKNSETools-0.1.20240417.86/PKNSETools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2024-04-17 21:36:01.000000 PKNSETools-0.1.20240417.86/PKNSETools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-17 21:36:01.000000 PKNSETools-0.1.20240417.86/PKNSETools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1884 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-17 21:36:01.785266 PKNSETools-0.1.20240417.86/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2024-04-17 21:34:16.000000 PKNSETools-0.1.20240417.86/setup.py
```

### Comparing `PKNSETools-0.1.20240417.85/PKG-INFO` & `PKNSETools-0.1.20240417.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240417.85
+Version: 0.1.20240417.86
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240417.85.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240417.86.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/Benny/NSE.py` & `PKNSETools-0.1.20240417.86/PKNSETools/Benny/NSE.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/Benny/__init__.py` & `PKNSETools-0.1.20240417.86/PKNSETools/Benny/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/Nasdaq/PKNasdaqIndex.py` & `PKNSETools-0.1.20240417.86/PKNSETools/Nasdaq/PKNasdaqIndex.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/Nasdaq/__init__.py` & `PKNSETools-0.1.20240417.86/PKNSETools/Nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/PKAllStocks.py` & `PKNSETools-0.1.20240417.86/PKNSETools/PKAllStocks.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/PKCompanyGeneral.py` & `PKNSETools-0.1.20240417.86/PKNSETools/PKCompanyGeneral.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/PKCompanyStock.py` & `PKNSETools-0.1.20240417.86/PKNSETools/PKCompanyStock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/PKConstants.py` & `PKNSETools-0.1.20240417.86/PKNSETools/PKConstants.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/PKIntraDay.py` & `PKNSETools-0.1.20240417.86/PKNSETools/PKIntraDay.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/PKMultiProcessorClient.py` & `PKNSETools-0.1.20240417.86/PKNSETools/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/PKNSEStockDataFetcher.py` & `PKNSETools-0.1.20240417.86/PKNSETools/PKNSEStockDataFetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,50 +110,50 @@
                         + colorText.FAIL
                         + "[+] Enter Stock Code(s) for screening (Multiple codes should be seperated by ,): "
                     )
                 ).upper()
             stockCode = stockCode.replace(" ", "")
             listStockCodes = stockCode.split(",")
         else:
-            OutputControls.printOutput(colorText.BOLD + "[+] Getting Stock Codes From NSE... ", end="")
+            OutputControls().printOutput(colorText.BOLD + "[+] Getting Stock Codes From NSE... ", end="")
             listStockCodes = self.fetchNiftyCodes(tickerOption)
             if len(listStockCodes) > 10:
-                OutputControls.printOutput(
+                OutputControls().printOutput(
                     colorText.GREEN
                     + ("=> Done! Fetched %d stock codes." % len(listStockCodes))
                     + colorText.END
                 )
                 if self.configManager.shuffleEnabled:
                     random.shuffle(listStockCodes)
-                    OutputControls.printOutput(
+                    OutputControls().printOutput(
                         colorText.BLUE
                         + "[+] Stock shuffling is active."
                         + colorText.END
                     )
                 else:
-                    OutputControls.printOutput(
+                    OutputControls().printOutput(
                         colorText.FAIL
                         + "[+] Stock shuffling is inactive."
                         + colorText.END
                     )
                 if self.configManager.stageTwo:
-                    OutputControls.printOutput(
+                    OutputControls().printOutput(
                         colorText.BLUE
                         + "[+] Screening only for the stocks in Stage-2! Edit User Config to change this."
                         + colorText.END
                     )
                 else:
-                    OutputControls.printOutput(
+                    OutputControls().printOutput(
                         colorText.FAIL
                         + "[+] Screening only for the stocks in all Stages! Edit User Config to change this."
                         + colorText.END
                     )
 
             else:
-                OutputControls.printOutput(
+                OutputControls().printOutput(
                     colorText.FAIL
                     + "=> Error getting stock codes from NSE!"
                     + colorText.END
                 )
 
         return listStockCodes
```

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/NSEStockDB.py` & `PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/NSEStockDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/NSEStockFairValueDB.py` & `PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/NSEStockFairValueDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/NSEStockMFIDB.py` & `PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/NSEStockMFIDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/PKMorningstarDataFetcher.py` & `PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/PKMorningstarDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/__init__.py` & `PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/error.py` & `PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/error.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/funds.py` & `PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/funds.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/search.py` & `PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,15 @@
   }
 
   result = general_search(params, proxies=proxies)
 
   if result['rows']:
     return result['rows']
   else:
-    OutputControls.printOutput('0 fund found with the term %s' % (term))
+    OutputControls().printOutput('0 fund found with the term %s' % (term))
     return {}
 
 def search_stock(term,field,exchange, pageSize =10,currency ='INR', filters={}, proxies={}):
   """
   This function will use the screener of morningstar.co.uk to find stocks which include the term.
 
   Args:
```

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/security.py` & `PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/security.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/stock.py` & `PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/stock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools/morningstartools/utils.py` & `PKNSETools-0.1.20240417.86/PKNSETools/morningstartools/utils.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools.egg-info/PKG-INFO` & `PKNSETools-0.1.20240417.86/PKNSETools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240417.85
+Version: 0.1.20240417.86
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240417.85.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240417.86.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240417.85/PKNSETools.egg-info/SOURCES.txt` & `PKNSETools-0.1.20240417.86/PKNSETools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/README.md` & `PKNSETools-0.1.20240417.86/README.md`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240417.85/setup.py` & `PKNSETools-0.1.20240417.86/setup.py`

 * *Files identical despite different names*
