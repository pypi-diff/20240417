# Comparing `tmp/pkscreener-0.44.20240417.269.tar.gz` & `tmp/pkscreener-0.44.20240417.270.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240417.269.tar", last modified: Wed Apr 17 06:12:11 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240417.270.tar", last modified: Wed Apr 17 09:12:31 2024, max compression
```

## Comparing `pkscreener-0.44.20240417.269.tar` & `pkscreener-0.44.20240417.270.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 06:12:11.835329 pkscreener-0.44.20240417.269/
--rw-rw-rw-   0        0        0     1086 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-17 06:12:11.835329 pkscreener-0.44.20240417.269/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 06:12:11.819731 pkscreener-0.44.20240417.269/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:12:11.835329 pkscreener-0.44.20240417.269/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     3237 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27587 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8037 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48885 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   113854 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    46266 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    77525 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-17 06:12:05.000000 pkscreener-0.44.20240417.269/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   115333 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    19391 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:12:11.819731 pkscreener-0.44.20240417.269/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-17 06:12:11.000000 pkscreener-0.44.20240417.269/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1282 2024-04-17 06:12:11.000000 pkscreener-0.44.20240417.269/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 06:12:11.000000 pkscreener-0.44.20240417.269/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-17 06:12:11.000000 pkscreener-0.44.20240417.269/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 06:12:11.000000 pkscreener-0.44.20240417.269/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-17 06:12:11.000000 pkscreener-0.44.20240417.269/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-17 06:12:11.835329 pkscreener-0.44.20240417.269/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-17 06:08:25.000000 pkscreener-0.44.20240417.269/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:12:31.541771 pkscreener-0.44.20240417.270/
+-rw-rw-rw-   0        0        0     1086 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-17 09:12:31.541771 pkscreener-0.44.20240417.270/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 09:12:31.526145 pkscreener-0.44.20240417.270/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:12:31.541771 pkscreener-0.44.20240417.270/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     3237 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27587 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8037 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48912 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   113854 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    46266 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    78109 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-17 09:12:22.000000 pkscreener-0.44.20240417.270/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   115366 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    19391 2024-04-17 09:08:20.000000 pkscreener-0.44.20240417.270/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:12:31.526145 pkscreener-0.44.20240417.270/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-17 09:12:31.000000 pkscreener-0.44.20240417.270/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1282 2024-04-17 09:12:31.000000 pkscreener-0.44.20240417.270/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 09:12:31.000000 pkscreener-0.44.20240417.270/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-17 09:12:31.000000 pkscreener-0.44.20240417.270/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 09:12:31.000000 pkscreener-0.44.20240417.270/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-17 09:12:31.000000 pkscreener-0.44.20240417.270/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-17 09:12:31.541771 pkscreener-0.44.20240417.270/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-17 09:08:21.000000 pkscreener-0.44.20240417.270/setup.py
```

### Comparing `pkscreener-0.44.20240417.269/LICENSE` & `pkscreener-0.44.20240417.270/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/LICENSE-Others` & `pkscreener-0.44.20240417.270/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/PKG-INFO` & `pkscreener-0.44.20240417.270/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240417.269
+Version: 0.44.20240417.270
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240417.269.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240417.270.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.269/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.269/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.269/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240417.269/README.md` & `pkscreener-0.44.20240417.270/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.269/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.269/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.269/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240417.269/pkscreener/__init__.py` & `pkscreener-0.44.20240417.270/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/PortfolioXRay.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,16 +91,18 @@
     return reports
 
 
 def bestStrategiesFromSummaryForReport(reportName: None, summary=False,includeLargestDatasets=False):
     dfs = []
     insights = None
     if "PKDevTools_Default_Log_Level" not in os.environ.keys():
-        if (("RUNNER" not in os.environ.keys()) or not configManager.showPastStrategyData):
+        if (("RUNNER" not in os.environ.keys())):
             return None
+    if not configManager.showPastStrategyData:
+        return None
     try:
         dfs = pd.read_html(
             "https://pkjmesra.github.io/PKScreener/Backtest-Reports/{0}".format(
                 reportName.replace("_X_", "_B_").replace("_G_", "_B_").replace("_S_", "_B_")
             ),encoding="UTF-8", attrs = {'id': 'resultsTable'}
         )
     except Exception as e: # pragma: no cover
```

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/Utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,22 +281,22 @@
         return x
 
     def formatRatio(ratio, volumeRatio):
         if ratio >= volumeRatio and ratio != np.nan and (not math.isinf(ratio)):
             return colorText.BOLD + colorText.GREEN + str(ratio) + "x" + colorText.END
         return colorText.BOLD + colorText.FAIL + str(ratio) + "x" + colorText.END
 
-    def addQuickWatermark(sourceImage:Image, xVertical=None, dataSrc=""):
+    def addQuickWatermark(sourceImage:Image, xVertical=None, dataSrc="", dataSrcFontSize=10):
         width, height = sourceImage.size
         watermarkText = f"© {datetime.date.today().year} pkjmesra | PKScreener"
         message_length = len(watermarkText)
         # load font (tweak ratio based on a particular font)
         FONT_RATIO = 1.5
         DIAGONAL_PERCENTAGE = .85
-        DATASRC_FONTSIZE = 10
+        DATASRC_FONTSIZE = dataSrcFontSize
         dataSrc = f"Src: {dataSrc}"
         diagonal_length = int(math.sqrt((width**2) + (height**2)))
         diagonal_to_use = diagonal_length * DIAGONAL_PERCENTAGE
         height_to_use = height * DIAGONAL_PERCENTAGE
         font_size = int(diagonal_to_use / (message_length / FONT_RATIO))
         font_size_vertical = int(height_to_use / (message_length / FONT_RATIO))
         fontPath = tools.setupReportFont()
@@ -418,18 +418,20 @@
         summaryLabel = None,
         detailLabel = None
     ):
         if "PKDevTools_Default_Log_Level" not in os.environ.keys():
             if (("RUNNER" in os.environ.keys() and os.environ["RUNNER"] == "LOCAL_RUN_SCANNER")):
                 return
         warnings.filterwarnings("ignore", category=DeprecationWarning)
+        ART_FONT_SIZE = 30
+        STD_FONT_SIZE = 60
         # First 4 lines are headers. Last 1 line is bottom grid line
         fontPath = tools.setupReportFont()
-        artfont = ImageFont.truetype(fontPath, 30)
-        stdfont = ImageFont.truetype(fontPath, 60)
+        artfont = ImageFont.truetype(fontPath, ART_FONT_SIZE)
+        stdfont = ImageFont.truetype(fontPath, STD_FONT_SIZE)
         
         bgColor, gridColor, artColor, menuColor = tools.getDefaultColors()
 
         dfs_to_print = [styledTable, backtestSummary, backtestDetail]
         unstyled_dfs = [table, backtestSummary, backtestDetail]
         reportTitle = f"[+] As of {PKDateUtilities.currentDateTime().strftime('%d-%m-%y %H.%M.%S')} IST > You chose {label}"
         titleLabels = [
@@ -602,47 +604,49 @@
         draw.text(
             (colPixelRunValue, rowPixelRunValue + 1),
             repoText,
             font=artfont,
             fill=menuColor,
         )
         # Legend text
-        legendLineNumber = 0
         rowPixelRunValue += 2 * stdFont_oneLinelabel_height + 20
-        legendLines = legendText.split("\n")
+        legendLines = legendText.splitlines()
+        legendSeperator = "***"
+        col_width_sep, _ = artfont.getsize_multiline(legendSeperator)
         for line in legendLines:
             colPixelRunValue = startColValue
             _, artfont_line_height = artfont.getsize_multiline(line)
-            cellStyles, cellCleanValues = tools.getCellColors(
-                line, defaultCellFillColor=gridColor
-            )
-            valCounter = 0
-            for style in cellStyles:
-                cleanValue = cellCleanValues[valCounter]
-                valCounter += 1
-                if bgColor == "white" and style == "yellow":
-                    # Yellow on a white background is difficult to read
-                    style = "blue"
-                elif bgColor == "black" and style == "blue":
-                    # blue on a black background is difficult to read
-                    style = "yellow"
-                col_width, _ = artfont.getsize_multiline(cleanValue)
+            lineitems = line.split(legendSeperator)
+            red = True
+            for lineitem in lineitems:
+                if lineitem == "" or not red:
+                    draw.text(
+                        (colPixelRunValue, rowPixelRunValue),
+                        legendSeperator,
+                        font=artfont,
+                        fill=gridColor,
+                    )
+                    colPixelRunValue += col_width_sep + 1
+                style = "red" if not red else gridColor
+                red = not red
                 draw.text(
                     (colPixelRunValue, rowPixelRunValue),
-                    cleanValue,
+                    lineitem,
                     font=artfont,
                     fill=style,
                 )
+                col_width, _ = artfont.getsize_multiline(lineitem)
                 # Move to the next text in the same line
-                colPixelRunValue += col_width + 2
+                colPixelRunValue += col_width + 1
+                
             # Let's go to the next line
             rowPixelRunValue += artfont_line_height + 1
 
         im = im.resize(im.size, Image.ANTIALIAS, reducing_gap=2)
-        im = tools.addQuickWatermark(im,xVertical,dataSrc="Yahoo; Morningstar, Inc; National Stock Exchange of India Ltd;")
+        im = tools.addQuickWatermark(im,xVertical,dataSrc="Yahoo; Morningstar, Inc; National Stock Exchange of India Ltd;",dataSrcFontSize=ART_FONT_SIZE)
         im.save(filename, format="png", bitmap_format="png", optimize=True, quality=20)
         # if 'RUNNER' not in os.environ.keys() and 'PKDevTools_Default_Log_Level' in os.environ.keys():
         # im.show()
 
     def wrapFitLegendText(table, backtestSummary, legendText):
         wrapper = textwrap.TextWrapper(
             width=2
@@ -689,18 +693,18 @@
         legendText = f"{legendText} last 22 trading sessions. Their strength is displayed depending on the steepness of the trendlines. (Strong / Weak) Up / Down shows how high/low the demand is respectively. A Sideways trend is the horizontal price movement that occurs when the forces of supply and demand are nearly equal. T:▲ or T:▼ shows the general moving average uptrend/downtrend from a 200 day MA perspective"
         legendText = f"{legendText} if the current 200DMA is more/less than the last 20/80/100 days' 200DMA. Similarly, t:▲ or t:▼ shows for 50DMA based on 9/14/20 days' 50DMA trend. MFI:▲ or MFI:▼ shows"
         legendText = f"{legendText} if the overall top 5 mutual funds and top 5 institutional investors ownership went up or down on the closing of the last month. *** 10. Pattern ***:This shows if the chart or the candle (from the candlestick chart) is"
         legendText = f"{legendText} forming any known pattern in the recent timeframe or as per the selected screening options. Do a google search for the shown pattern names to learn. *** 11. CCI ***: The Commodity Channel Index (CCI) is a technical indicator that measures the difference between the current price and the historical average price of the given stock. Generally below '- 100' is considered oversold"
         legendText = f"{legendText} and above 100 is considered overbought. If the CCI is < '-100' or CCI is > 100 and the Trend(22Prds) is Strong/Weak Up, it is shown in green. Otherwise it's in red. *** 12. 1-Pd/2-Pd etc. ***: 60.29% of (413) under 1-Pd in green shows that the given scan option was correct 60.23% of the times for 413 stocks that scanner found in the last 22 trading sessions under the same scan"
         legendText = f"{legendText} options. Similarly, 61.69 % of (154) in green under 22-Pd, means we found that 61.56% of 154 stocks (~95 stocks) prices found under the same scan options increased in 22 trading periods. 57.87% of (2661) under 'Overall' means that over the last 22 trading sessions we found 2661 stock instances under the same scanning options (for example, Momentum Gainers), out of which 57.87%"
         legendText = f"{legendText} of the stock prices increased in one or more of the last 1 or 2 or 3 or 4 or 5 or 10 or 22 or 22 trading sessions. If you want to see by what percent the prices increased, you should see the details. *** 13. 1 to 30 period gain/loss % ***: 4.17% under 1-Pd in green in the gain/loss table/grid means the stock price increased by 4.17% in the next 1 trading session. If this is in"
-        legendText = f"{legendText} red, example, -5.67%, it means the price actually decreased by 5.67%. Gains are in green and losses are in red in this grid. The Date column has the date(s) on which that specific stock was found under the chosen scan options in the past 22 trading sessions. *** 14. 52Wk H/L ***: These have 52 weeks high/low prices within 10% of LTP:Yellow, above high:Green. Below 90% High:Red."
-        legendText = f"{legendText} *** 15. 1-Pd-% ***: Shows the 1 period gain in percent from the given date. Similarly 2-Pd-%, 3-Pd-% etc shows 2 day, 3 days gain etc. *** 16. 1-Pd-10k ***: Shows 1 period/day portfolio value if you would have invested 10,000 on the given date. *** 17. [T][_trend_] ***: [T] is for Trends followed by the trend name in the filter. *** 18. [BO] ***: Shows the Breakout filter value."
-        legendText = f"{legendText} *** 19. [P] ***: [P] shows pattern name. *** 20. MFI ***: Top 5 Mutual fund ownership and top 5 Institutional investor ownership status as on the last day of the last month, based on analysis from Morningstar. *** 21. FairValue ***: Morningstar Fair value of a given stock as of last trading day as determined by 3rd party analysis based on fundamentals. *** 20. MCapWt% ***: This "
-        legendText = f"{legendText} shows the market-cap weighted portfolio weight to consider investing.\n"
+        legendText = f"{legendText} red, example, -5.67%, it means the price actually decreased by 5.67%. Gains are in green and losses are in red in this grid. The Date column has the date(s) on which that specific stock was found under the chosen scan options in the past 22 trading sessions. *** 14. 52Wk H/L ***: These have 52 weeks high/low prices and will be shown in red, green or yellow based on how close the"
+        legendText = f"{legendText} price is to the 52 wk high/low value.If the 52 week high/low value is within 10% of LTP:Yellow, LTP is above 52 week high:Green. If the LTP is below 90% of 52 week high:Red.*** 15. 1-Pd-% ***: Shows the 1 period gain in percent from the given date. Similarly 2-Pd-%, 3-Pd-% etc shows 2 day, 3 days gain etc. *** 16. 1-Pd-10k ***: Shows 1 period/day portfolio value if you would"
+        legendText = f"{legendText} have invested 10,000 on the given date. *** 17. [T][_trend_] ***: [T] is for Trends followed by the trend name in the filter. *** 18. [BO] ***: This Shows the Breakout filter value from the backtest reports and will be available only if 'showpaststrategydata' configuration is turned on. *** 19. [P] ***: [P] shows pattern name. *** 20. MFI ***: Top 5 Mutual fund ownership and "
+        legendText = f"{legendText} top 5 Institutional investor ownership status as on the last day of the last month, based on analysis from Morningstar. *** 21. FairValue ***: Morningstar Fair value of a given stock as of last trading day as determined by 3rd party analysis based on fundamentals. *** 22. MCapWt% ***: This shows the market-cap weighted portfolio weight to consider investing.\n"
         legendText = tools.wrapFitLegendText(table,backtestSummary, legendText)
         # legendText = legendText.replace("***:", colorText.END + colorText.WHITE)
         # legendText = legendText.replace("*** ", colorText.END + colorText.FAIL)
         # return colorText.WHITE + legendText + colorText.END
         return legendText
 
     def getRepoHelpText(table,backtestSummary):
@@ -793,15 +797,17 @@
             queueCounter += 1
         
         if len(tasksList) > 0:
             PKScheduler.scheduleTasks(tasksList=tasksList, label=f"Downloading latest data (Total={len(stockCodes)} records in {len(tasksList)} batches){'Be Patient!' if len(stockCodes)> 2000 else ''}",timeout=10,minAcceptableCompletionPercentage=80)
             for task in tasksList:
                 if task.result is not None:
                     for stock in task.userData:
-                        stockDict[stock] = task.result[f"{stock}{exchangeSuffix}"].to_dict("split")
+                        taskResult = task.result.get(f"{stock}{exchangeSuffix}")
+                        if taskResult is not None:
+                            stockDict[stock] = taskResult.to_dict("split")
         return stockDict
 
     def loadStockData(
         stockDict,
         configManager,
         downloadOnly=False,
         defaultAnswer=None,
@@ -813,15 +819,15 @@
         forceRedownload=False
     ):
         isIntraday = isIntraday or configManager.isIntradayConfig()
         exists, cache_file = tools.afterMarketStockDataExists(
             isIntraday, forceLoad=forceLoad
         )
         initialLoadCount = len(stockDict)
-        isTrading = PKDateUtilities.isTradingTime()
+        isTrading = PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()
         if (stockCodes is not None and len(stockCodes) > 0) and (isTrading or downloadOnly):
             stockDict = tools.downloadLatestData(stockDict,configManager,stockCodes,exchangeSuffix=exchangeSuffix)
             # return stockDict
 
         default_logger().info(
             f"Stock data cache file:{cache_file} exists ->{str(exists)}"
         )
```

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/classes/keys.py` & `pkscreener-0.44.20240417.270/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/courbd.ttf` & `pkscreener-0.44.20240417.270/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/globals.py` & `pkscreener-0.44.20240417.270/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1891,16 +1891,18 @@
                     if col in screenResults.columns:
                         screenResults.drop(col, axis=1, inplace=True, errors="ignore")
     return summaryReturns
 
 
 def tabulateBacktestResults(saveResults, maxAllowed=0, force=False):
     if "PKDevTools_Default_Log_Level" not in os.environ.keys():
-        if ("RUNNER" not in os.environ.keys()) or ("RUNNER" in os.environ.keys() and not force) or not configManager.showPastStrategyData:
+        if ("RUNNER" not in os.environ.keys()) or ("RUNNER" in os.environ.keys() and not force):
             return None, None
+    if not configManager.showPastStrategyData:
+        return None, None
     tabulated_backtest_summary = ""
     tabulated_backtest_detail = ""
     summarydf, detaildf = getSummaryCorrectnessOfStrategy(saveResults)
     if summarydf is not None and len(summarydf) > 0:
         tabulated_backtest_summary = colorText.miniTabulator().tabulate(
             summarydf,
             headers="keys",
```

### Comparing `pkscreener-0.44.20240417.269/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240417.270/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240417.270/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240417.270/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240417.270/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240417.269
+Version: 0.44.20240417.270
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240417.269.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240417.270.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.269/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.269/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.268/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240417.269/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240417.269/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240417.270/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240417.269/setup.py` & `pkscreener-0.44.20240417.270/setup.py`

 * *Files identical despite different names*

