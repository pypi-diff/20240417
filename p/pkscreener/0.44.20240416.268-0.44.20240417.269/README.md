# Comparing `tmp/pkscreener-0.44.20240416.268.tar.gz` & `tmp/pkscreener-0.44.20240417.269.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240416.268.tar", last modified: Tue Apr 16 19:39:05 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240417.269.tar", last modified: Wed Apr 17 06:12:11 2024, max compression
```

## Comparing `pkscreener-0.44.20240416.268.tar` & `pkscreener-0.44.20240417.269.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 19:39:05.558606 pkscreener-0.44.20240416.268/
--rw-rw-rw-   0        0        0     1086 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-16 19:39:05.558606 pkscreener-0.44.20240416.268/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 19:39:05.542984 pkscreener-0.44.20240416.268/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 19:39:05.558606 pkscreener-0.44.20240416.268/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     3237 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27587 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8037 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48885 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   113854 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    46266 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    77523 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-16 19:38:57.000000 pkscreener-0.44.20240416.268/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   115333 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    19391 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-16 19:39:05.542984 pkscreener-0.44.20240416.268/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-16 19:39:05.000000 pkscreener-0.44.20240416.268/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1282 2024-04-16 19:39:05.000000 pkscreener-0.44.20240416.268/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 19:39:05.000000 pkscreener-0.44.20240416.268/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-16 19:39:05.000000 pkscreener-0.44.20240416.268/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 19:39:05.000000 pkscreener-0.44.20240416.268/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-16 19:39:05.000000 pkscreener-0.44.20240416.268/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-16 19:39:05.558606 pkscreener-0.44.20240416.268/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-16 19:35:10.000000 pkscreener-0.44.20240416.268/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:12:11.835329 pkscreener-0.44.20240417.269/
+-rw-rw-rw-   0        0        0     1086 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-17 06:12:11.835329 pkscreener-0.44.20240417.269/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 06:12:11.819731 pkscreener-0.44.20240417.269/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:12:11.835329 pkscreener-0.44.20240417.269/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     3237 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27587 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8037 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48885 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   113854 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    46266 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    77525 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-17 06:12:05.000000 pkscreener-0.44.20240417.269/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   115333 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    19391 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:12:11.819731 pkscreener-0.44.20240417.269/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-17 06:12:11.000000 pkscreener-0.44.20240417.269/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1282 2024-04-17 06:12:11.000000 pkscreener-0.44.20240417.269/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 06:12:11.000000 pkscreener-0.44.20240417.269/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-17 06:12:11.000000 pkscreener-0.44.20240417.269/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 06:12:11.000000 pkscreener-0.44.20240417.269/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-17 06:12:11.000000 pkscreener-0.44.20240417.269/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-17 06:12:11.835329 pkscreener-0.44.20240417.269/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/setup.py
```

### Comparing `pkscreener-0.44.20240416.268/LICENSE` & `pkscreener-0.44.20240417.269/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/LICENSE-Others` & `pkscreener-0.44.20240417.269/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/PKG-INFO` & `pkscreener-0.44.20240417.269/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240416.268
+Version: 0.44.20240417.269
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240416.268.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240417.269.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.267/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.267/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.267/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240416.268/README.md` & `pkscreener-0.44.20240417.269/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.267/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.267/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.267/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240416.268/pkscreener/__init__.py` & `pkscreener-0.44.20240417.269/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,15 +637,15 @@
             # Let's go to the next line
             rowPixelRunValue += artfont_line_height + 1
 
         im = im.resize(im.size, Image.ANTIALIAS, reducing_gap=2)
         im = tools.addQuickWatermark(im,xVertical,dataSrc="Yahoo; Morningstar, Inc; National Stock Exchange of India Ltd;")
         im.save(filename, format="png", bitmap_format="png", optimize=True, quality=20)
         # if 'RUNNER' not in os.environ.keys() and 'PKDevTools_Default_Log_Level' in os.environ.keys():
-        im.show()
+        # im.show()
 
     def wrapFitLegendText(table, backtestSummary, legendText):
         wrapper = textwrap.TextWrapper(
             width=2
             * int(
                 len(table.split("\n")[0])
                 if len(table) > 0
```

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/classes/keys.py` & `pkscreener-0.44.20240417.269/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/courbd.ttf` & `pkscreener-0.44.20240417.269/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/globals.py` & `pkscreener-0.44.20240417.269/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240417.269/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240417.269/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240417.269/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240417.269/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240416.268
+Version: 0.44.20240417.269
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240416.268.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240417.269.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.267/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.267/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.267/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240416.268/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240417.269/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.268/setup.py` & `pkscreener-0.44.20240417.269/setup.py`

 * *Files identical despite different names*

