# Comparing `tmp/adata-1.2.4.tar.gz` & `tmp/adata-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adata-1.2.4.tar", last modified: Fri Feb  2 14:58:48 2024, max compression
+gzip compressed data, was "adata-2.0.0b0.tar", last modified: Wed Apr 17 10:30:56 2024, max compression
```

## Comparing `adata-1.2.4.tar` & `adata-2.0.0b0.tar`

### file list

```diff
@@ -1,140 +1,137 @@
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.578661 adata-1.2.4/
--rw-r--r--   0 inchaos    (501) staff       (20)    11357 2023-06-10 14:18:58.000000 adata-1.2.4/LICENSE
--rw-r--r--   0 inchaos    (501) staff       (20)      124 2024-01-25 02:00:51.000000 adata-1.2.4/MANIFEST.in
--rw-r--r--   0 inchaos    (501) staff       (20)    19851 2024-02-02 14:58:48.577746 adata-1.2.4/PKG-INFO
--rw-r--r--   0 inchaos    (501) staff       (20)    19026 2024-01-25 02:00:51.000000 adata-1.2.4/README.md
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.423512 adata-1.2.4/adata/
--rw-r--r--   0 inchaos    (501) staff       (20)     1140 2024-01-25 02:00:51.000000 adata-1.2.4/adata/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)      712 2024-02-02 14:56:45.000000 adata-1.2.4/adata/__version__.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.431321 adata-1.2.4/adata/bond/
--rw-r--r--   0 inchaos    (501) staff       (20)      244 2023-06-10 14:18:58.000000 adata-1.2.4/adata/bond/__init__.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.432711 adata-1.2.4/adata/bond/cache/
--rw-r--r--   0 inchaos    (501) staff       (20)       96 2023-08-06 12:21:45.000000 adata-1.2.4/adata/bond/cache/__init__.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.434608 adata-1.2.4/adata/bond/info/
--rw-r--r--   0 inchaos    (501) staff       (20)      244 2024-01-25 02:00:51.000000 adata-1.2.4/adata/bond/info/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)     2136 2023-06-10 14:18:58.000000 adata-1.2.4/adata/bond/info/bond_code.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.437891 adata-1.2.4/adata/bond/market/
--rw-r--r--   0 inchaos    (501) staff       (20)       97 2023-06-10 14:18:58.000000 adata-1.2.4/adata/bond/market/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)      189 2023-06-10 14:18:58.000000 adata-1.2.4/adata/bond/market/bond_market.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.439086 adata-1.2.4/adata/common/
--rw-r--r--   0 inchaos    (501) staff       (20)      141 2023-06-10 14:18:58.000000 adata-1.2.4/adata/common/__init__.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.443130 adata-1.2.4/adata/common/base/
--rw-r--r--   0 inchaos    (501) staff       (20)      126 2023-06-10 14:18:58.000000 adata-1.2.4/adata/common/base/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)      182 2023-08-17 02:11:28.000000 adata-1.2.4/adata/common/base/base_req.py
--rw-r--r--   0 inchaos    (501) staff       (20)     2919 2023-08-17 07:44:30.000000 adata-1.2.4/adata/common/base/base_ths.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.450102 adata-1.2.4/adata/common/exception/
--rw-r--r--   0 inchaos    (501) staff       (20)       90 2023-07-07 22:15:59.000000 adata-1.2.4/adata/common/exception/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)      367 2023-08-06 12:21:45.000000 adata-1.2.4/adata/common/exception/exception_msg.py
--rw-r--r--   0 inchaos    (501) staff       (20)      331 2023-08-17 02:11:28.000000 adata-1.2.4/adata/common/exception/handler.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.458971 adata-1.2.4/adata/common/headers/
--rw-r--r--   0 inchaos    (501) staff       (20)     6319 2023-07-07 23:50:12.000000 adata-1.2.4/adata/common/headers/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)     5733 2023-06-10 14:18:58.000000 adata-1.2.4/adata/common/headers/baidu_headers.py
--rw-r--r--   0 inchaos    (501) staff       (20)      554 2023-08-17 02:11:28.000000 adata-1.2.4/adata/common/headers/east_headers.py
--rw-r--r--   0 inchaos    (501) staff       (20)      583 2023-06-10 14:18:58.000000 adata-1.2.4/adata/common/headers/sina_headers.py
--rw-r--r--   0 inchaos    (501) staff       (20)     3043 2023-08-09 13:29:20.000000 adata-1.2.4/adata/common/headers/ths_headers.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.463497 adata-1.2.4/adata/common/js/
--rw-r--r--   0 inchaos    (501) staff       (20)       92 2023-06-10 14:18:58.000000 adata-1.2.4/adata/common/js/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)    15427 2023-08-06 12:21:45.000000 adata-1.2.4/adata/common/js/hexin.js
--rw-r--r--   0 inchaos    (501) staff       (20)    38785 2023-06-29 09:36:49.000000 adata-1.2.4/adata/common/js/ths.js
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.475956 adata-1.2.4/adata/common/utils/
--rw-r--r--   0 inchaos    (501) staff       (20)      179 2023-07-07 22:50:29.000000 adata-1.2.4/adata/common/utils/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)      478 2024-01-25 02:00:51.000000 adata-1.2.4/adata/common/utils/code_utils.py
--rw-r--r--   0 inchaos    (501) staff       (20)      842 2024-01-25 02:00:51.000000 adata-1.2.4/adata/common/utils/cookie.py
--rw-r--r--   0 inchaos    (501) staff       (20)     2937 2023-06-10 14:18:58.000000 adata-1.2.4/adata/common/utils/snowflake.py
--rw-r--r--   0 inchaos    (501) staff       (20)     2798 2023-08-06 12:21:45.000000 adata-1.2.4/adata/common/utils/sunrequests.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.477387 adata-1.2.4/adata/fund/
--rw-r--r--   0 inchaos    (501) staff       (20)      241 2023-06-10 14:18:58.000000 adata-1.2.4/adata/fund/__init__.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.478567 adata-1.2.4/adata/fund/cache/
--rw-r--r--   0 inchaos    (501) staff       (20)       96 2023-08-06 12:21:45.000000 adata-1.2.4/adata/fund/cache/__init__.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.481357 adata-1.2.4/adata/fund/info/
--rw-r--r--   0 inchaos    (501) staff       (20)      243 2024-01-25 02:00:51.000000 adata-1.2.4/adata/fund/info/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)     5130 2023-08-06 12:21:45.000000 adata-1.2.4/adata/fund/info/fund_info.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.484170 adata-1.2.4/adata/fund/market/
--rw-r--r--   0 inchaos    (501) staff       (20)      197 2024-01-25 02:00:51.000000 adata-1.2.4/adata/fund/market/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)      187 2023-06-10 14:18:58.000000 adata-1.2.4/adata/fund/market/etf_market.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.485741 adata-1.2.4/adata/message/
--rw-r--r--   0 inchaos    (501) staff       (20)       96 2023-06-10 14:18:58.000000 adata-1.2.4/adata/message/__init__.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.494494 adata-1.2.4/adata/sentiment/
--rw-r--r--   0 inchaos    (501) staff       (20)      446 2023-08-06 12:21:45.000000 adata-1.2.4/adata/sentiment/__init__.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.496054 adata-1.2.4/adata/sentiment/cache/
--rw-r--r--   0 inchaos    (501) staff       (20)       96 2023-08-06 12:21:45.000000 adata-1.2.4/adata/sentiment/cache/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)     9422 2023-09-02 14:54:53.000000 adata-1.2.4/adata/sentiment/north_flow.py
--rw-r--r--   0 inchaos    (501) staff       (20)     3647 2023-08-17 07:16:27.000000 adata-1.2.4/adata/sentiment/securities_margin.py
--rw-r--r--   0 inchaos    (501) staff       (20)     4174 2023-08-09 13:29:20.000000 adata-1.2.4/adata/sentiment/stock_lifting.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.497811 adata-1.2.4/adata/stock/
--rw-r--r--   0 inchaos    (501) staff       (20)      399 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/__init__.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.500784 adata-1.2.4/adata/stock/cache/
--rw-r--r--   0 inchaos    (501) staff       (20)      254 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/cache/__init__.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.532789 adata-1.2.4/adata/stock/cache/calendar/
--rw-r--r--   0 inchaos    (501) staff       (20)       33 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2004.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5508 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2005.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5508 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2006.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5508 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2007.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5523 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2008.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5508 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2009.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5508 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2010.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5508 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2011.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5523 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2012.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5508 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2013.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5508 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2014.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5508 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2015.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5523 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2016.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5493 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2017.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5508 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2018.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5508 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2019.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5523 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2020.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5508 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2021.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5508 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2022.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5508 2023-07-07 22:04:53.000000 adata-1.2.4/adata/stock/cache/calendar/2023.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     5522 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/cache/calendar/2024.csv
--rw-r--r--   0 inchaos    (501) staff       (20)      410 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/cache/calendar/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)   169206 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/cache/code.csv
--rw-r--r--   0 inchaos    (501) staff       (20)     8623 2023-06-10 14:18:58.000000 adata-1.2.4/adata/stock/cache/index_code_rel_ths.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.536582 adata-1.2.4/adata/stock/index/
--rw-r--r--   0 inchaos    (501) staff       (20)      250 2023-06-10 14:18:58.000000 adata-1.2.4/adata/stock/index/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)      194 2023-06-10 14:18:58.000000 adata-1.2.4/adata/stock/index/cal_index.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.541484 adata-1.2.4/adata/stock/info/
--rw-r--r--   0 inchaos    (501) staff       (20)      481 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/info/__init__.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.546834 adata-1.2.4/adata/stock/info/concept/
--rw-r--r--   0 inchaos    (501) staff       (20)       79 2023-08-06 12:21:45.000000 adata-1.2.4/adata/stock/info/concept/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)      465 2023-08-06 12:24:11.000000 adata-1.2.4/adata/stock/info/concept/stock_concept.py
--rw-r--r--   0 inchaos    (501) staff       (20)     5488 2024-02-02 14:48:08.000000 adata-1.2.4/adata/stock/info/concept/stock_concept_east.py
--rw-r--r--   0 inchaos    (501) staff       (20)      444 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/info/concept/stock_concept_template.py
--rw-r--r--   0 inchaos    (501) staff       (20)    14832 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/info/concept/stock_concept_ths.py
--rw-r--r--   0 inchaos    (501) staff       (20)     5640 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/info/stock_code.py
--rw-r--r--   0 inchaos    (501) staff       (20)    10466 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/info/stock_index.py
--rw-r--r--   0 inchaos    (501) staff       (20)     2250 2023-11-09 09:36:11.000000 adata-1.2.4/adata/stock/info/trade_calendar.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.548452 adata-1.2.4/adata/stock/market/
--rw-r--r--   0 inchaos    (501) staff       (20)      530 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/market/__init__.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.557246 adata-1.2.4/adata/stock/market/concepth_market/
--rw-r--r--   0 inchaos    (501) staff       (20)      371 2023-08-09 13:29:20.000000 adata-1.2.4/adata/stock/market/concepth_market/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)     6899 2023-08-09 13:29:20.000000 adata-1.2.4/adata/stock/market/concepth_market/concept_market_east.py
--rw-r--r--   0 inchaos    (501) staff       (20)      679 2023-08-09 13:29:20.000000 adata-1.2.4/adata/stock/market/concepth_market/concept_market_template.py
--rw-r--r--   0 inchaos    (501) staff       (20)     9429 2023-08-09 13:29:20.000000 adata-1.2.4/adata/stock/market/concepth_market/concept_market_ths.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.561975 adata-1.2.4/adata/stock/market/index_market/
--rw-r--r--   0 inchaos    (501) staff       (20)       90 2023-08-06 12:44:28.000000 adata-1.2.4/adata/stock/market/index_market/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)     2163 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/market/index_market/market_index.py
--rw-r--r--   0 inchaos    (501) staff       (20)     6734 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/market/index_market/market_index_east.py
--rw-r--r--   0 inchaos    (501) staff       (20)     1701 2023-08-09 13:29:20.000000 adata-1.2.4/adata/stock/market/index_market/market_index_template.py
--rw-r--r--   0 inchaos    (501) staff       (20)     8085 2023-08-09 13:29:20.000000 adata-1.2.4/adata/stock/market/index_market/market_index_ths.py
--rw-r--r--   0 inchaos    (501) staff       (20)     3114 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/market/stock_dividend.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.568761 adata-1.2.4/adata/stock/market/stock_market/
--rw-r--r--   0 inchaos    (501) staff       (20)      167 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/market/stock_market/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)     3424 2023-09-14 09:03:28.000000 adata-1.2.4/adata/stock/market/stock_market/stock_market.py
--rw-r--r--   0 inchaos    (501) staff       (20)    11174 2024-01-25 02:00:51.000000 adata-1.2.4/adata/stock/market/stock_market/stock_market_baidu.py
--rw-r--r--   0 inchaos    (501) staff       (20)     5282 2023-09-14 01:54:47.000000 adata-1.2.4/adata/stock/market/stock_market/stock_market_qq.py
--rw-r--r--   0 inchaos    (501) staff       (20)     2593 2023-07-06 10:32:27.000000 adata-1.2.4/adata/stock/market/stock_market/stock_market_sina.py
--rw-r--r--   0 inchaos    (501) staff       (20)     2584 2023-09-14 01:54:47.000000 adata-1.2.4/adata/stock/market/stock_market/stock_market_template.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.576645 adata-1.2.4/adata.egg-info/
--rw-r--r--   0 inchaos    (501) staff       (20)    19851 2024-02-02 14:58:48.000000 adata-1.2.4/adata.egg-info/PKG-INFO
--rw-r--r--   0 inchaos    (501) staff       (20)     3645 2024-02-02 14:58:48.000000 adata-1.2.4/adata.egg-info/SOURCES.txt
--rw-r--r--   0 inchaos    (501) staff       (20)        1 2024-02-02 14:58:48.000000 adata-1.2.4/adata.egg-info/dependency_links.txt
--rw-r--r--   0 inchaos    (501) staff       (20)       75 2024-02-02 14:58:48.000000 adata-1.2.4/adata.egg-info/requires.txt
--rw-r--r--   0 inchaos    (501) staff       (20)        6 2024-02-02 14:58:48.000000 adata-1.2.4/adata.egg-info/top_level.txt
--rw-r--r--   0 inchaos    (501) staff       (20)       38 2024-02-02 14:58:48.578904 adata-1.2.4/setup.cfg
--rw-r--r--   0 inchaos    (501) staff       (20)     1773 2024-01-25 02:00:51.000000 adata-1.2.4/setup.py
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.415954 adata-1.2.4/tests/
-drwxr-xr-x   0 inchaos    (501) staff       (20)        0 2024-02-02 14:58:48.574818 adata-1.2.4/tests/other/
--rw-r--r--   0 inchaos    (501) staff       (20)       80 2023-06-29 09:36:49.000000 adata-1.2.4/tests/other/__init__.py
--rw-r--r--   0 inchaos    (501) staff       (20)     1310 2023-06-29 09:36:49.000000 adata-1.2.4/tests/other/bs4_test.py
--rw-r--r--   0 inchaos    (501) staff       (20)      581 2023-06-29 09:36:49.000000 adata-1.2.4/tests/other/year_test.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.418604 adata-2.0.0b0/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 05:48:39.000000 adata-2.0.0b0/LICENSE
+-rw-rw-rw-   0        0        0      126 2023-10-23 06:31:33.000000 adata-2.0.0b0/MANIFEST.in
+-rw-rw-rw-   0        0        0    21039 2024-04-17 10:30:56.418604 adata-2.0.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0    20328 2024-04-17 10:27:23.000000 adata-2.0.0b0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.306074 adata-2.0.0b0/adata/
+-rw-rw-rw-   0        0        0     1189 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/__init__.py
+-rw-rw-rw-   0        0        0      737 2024-04-17 10:30:41.000000 adata-2.0.0b0/adata/__version__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.312075 adata-2.0.0b0/adata/bond/
+-rw-rw-rw-   0        0        0      261 2023-06-05 11:07:12.000000 adata-2.0.0b0/adata/bond/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.313076 adata-2.0.0b0/adata/bond/cache/
+-rw-rw-rw-   0        0        0      103 2023-08-18 09:30:57.000000 adata-2.0.0b0/adata/bond/cache/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.315076 adata-2.0.0b0/adata/bond/info/
+-rw-rw-rw-   0        0        0      261 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/bond/info/__init__.py
+-rw-rw-rw-   0        0        0     2200 2023-05-31 08:21:01.000000 adata-2.0.0b0/adata/bond/info/bond_code.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.317076 adata-2.0.0b0/adata/bond/market/
+-rw-rw-rw-   0        0        0      104 2023-05-31 08:12:06.000000 adata-2.0.0b0/adata/bond/market/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-04-07 05:48:39.000000 adata-2.0.0b0/adata/bond/market/bond_market.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.318076 adata-2.0.0b0/adata/common/
+-rw-rw-rw-   0        0        0      150 2023-04-07 05:48:39.000000 adata-2.0.0b0/adata/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.321077 adata-2.0.0b0/adata/common/base/
+-rw-rw-rw-   0        0        0      133 2023-06-05 03:44:57.000000 adata-2.0.0b0/adata/common/base/__init__.py
+-rw-rw-rw-   0        0        0      195 2023-08-14 05:47:34.000000 adata-2.0.0b0/adata/common/base/base_req.py
+-rw-rw-rw-   0        0        0     3015 2023-08-18 09:30:57.000000 adata-2.0.0b0/adata/common/base/base_ths.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.325078 adata-2.0.0b0/adata/common/exception/
+-rw-rw-rw-   0        0        0       97 2023-07-10 08:15:13.000000 adata-2.0.0b0/adata/common/exception/__init__.py
+-rw-rw-rw-   0        0        0      379 2023-08-01 09:58:42.000000 adata-2.0.0b0/adata/common/exception/exception_msg.py
+-rw-rw-rw-   0        0        0      350 2023-08-14 06:04:13.000000 adata-2.0.0b0/adata/common/exception/handler.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.330081 adata-2.0.0b0/adata/common/headers/
+-rw-rw-rw-   0        0        0     6407 2023-07-10 08:15:13.000000 adata-2.0.0b0/adata/common/headers/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-07 05:48:39.000000 adata-2.0.0b0/adata/common/headers/baidu_headers.py
+-rw-rw-rw-   0        0        0      571 2023-08-14 05:47:34.000000 adata-2.0.0b0/adata/common/headers/east_headers.py
+-rw-rw-rw-   0        0        0      602 2023-04-18 11:18:06.000000 adata-2.0.0b0/adata/common/headers/sina_headers.py
+-rw-rw-rw-   0        0        0     3085 2023-08-08 04:51:00.000000 adata-2.0.0b0/adata/common/headers/ths_headers.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.333081 adata-2.0.0b0/adata/common/js/
+-rw-rw-rw-   0        0        0       99 2023-05-05 10:05:38.000000 adata-2.0.0b0/adata/common/js/__init__.py
+-rw-rw-rw-   0        0        0    15792 2023-08-01 09:31:40.000000 adata-2.0.0b0/adata/common/js/hexin.js
+-rw-rw-rw-   0        0        0    39849 2023-06-28 03:35:45.000000 adata-2.0.0b0/adata/common/js/ths.js
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.339080 adata-2.0.0b0/adata/common/utils/
+-rw-rw-rw-   0        0        0      190 2023-07-10 08:15:13.000000 adata-2.0.0b0/adata/common/utils/__init__.py
+-rw-rw-rw-   0        0        0      501 2023-12-04 11:20:28.000000 adata-2.0.0b0/adata/common/utils/code_utils.py
+-rw-rw-rw-   0        0        0      877 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/common/utils/cookie.py
+-rw-rw-rw-   0        0        0     3046 2023-04-07 05:48:39.000000 adata-2.0.0b0/adata/common/utils/snowflake.py
+-rw-rw-rw-   0        0        0     2891 2023-08-07 03:04:02.000000 adata-2.0.0b0/adata/common/utils/sunrequests.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.340595 adata-2.0.0b0/adata/fund/
+-rw-rw-rw-   0        0        0      327 2024-04-17 10:25:02.000000 adata-2.0.0b0/adata/fund/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.341586 adata-2.0.0b0/adata/fund/cache/
+-rw-rw-rw-   0        0        0      103 2023-06-02 06:05:35.000000 adata-2.0.0b0/adata/fund/cache/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.343586 adata-2.0.0b0/adata/fund/info/
+-rw-rw-rw-   0        0        0      260 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/fund/info/__init__.py
+-rw-rw-rw-   0        0        0     5247 2023-08-01 10:31:22.000000 adata-2.0.0b0/adata/fund/info/fund_info.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.348587 adata-2.0.0b0/adata/fund/market/
+-rw-rw-rw-   0        0        0      379 2024-04-17 10:25:02.000000 adata-2.0.0b0/adata/fund/market/__init__.py
+-rw-rw-rw-   0        0        0     2170 2024-04-17 10:25:02.000000 adata-2.0.0b0/adata/fund/market/etf_market.py
+-rw-rw-rw-   0        0        0      657 2024-04-17 10:07:40.000000 adata-2.0.0b0/adata/fund/market/etf_market_template.py
+-rw-rw-rw-   0        0        0     7993 2024-04-17 10:07:40.000000 adata-2.0.0b0/adata/fund/market/etf_market_ths.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.349587 adata-2.0.0b0/adata/message/
+-rw-rw-rw-   0        0        0      103 2023-04-07 05:48:39.000000 adata-2.0.0b0/adata/message/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.355589 adata-2.0.0b0/adata/sentiment/
+-rw-rw-rw-   0        0        0      466 2023-08-01 04:36:50.000000 adata-2.0.0b0/adata/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.356589 adata-2.0.0b0/adata/sentiment/cache/
+-rw-rw-rw-   0        0        0      103 2023-08-18 09:30:57.000000 adata-2.0.0b0/adata/sentiment/cache/__init__.py
+-rw-rw-rw-   0        0        0     9633 2023-08-01 04:08:30.000000 adata-2.0.0b0/adata/sentiment/north_flow.py
+-rw-rw-rw-   0        0        0     3741 2023-08-18 09:30:57.000000 adata-2.0.0b0/adata/sentiment/securities_margin.py
+-rw-rw-rw-   0        0        0     4271 2023-08-08 04:51:00.000000 adata-2.0.0b0/adata/sentiment/stock_lifting.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.357589 adata-2.0.0b0/adata/stock/
+-rw-rw-rw-   0        0        0      420 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/stock/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.361590 adata-2.0.0b0/adata/stock/cache/
+-rw-rw-rw-   0        0        0      267 2023-10-18 11:49:59.000000 adata-2.0.0b0/adata/stock/cache/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.386597 adata-2.0.0b0/adata/stock/cache/calendar/
+-rw-rw-rw-   0        0        0       34 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2004.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2005.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2006.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2007.csv
+-rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2008.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2009.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2010.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2011.csv
+-rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2012.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2013.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2014.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2015.csv
+-rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2016.csv
+-rw-rw-rw-   0        0        0     5858 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2017.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2018.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2019.csv
+-rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2020.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2021.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2022.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2023.csv
+-rw-rw-rw-   0        0        0     5888 2023-12-29 03:33:12.000000 adata-2.0.0b0/adata/stock/cache/calendar/2024.csv
+-rw-rw-rw-   0        0        0      428 2023-12-11 07:21:42.000000 adata-2.0.0b0/adata/stock/cache/calendar/__init__.py
+-rw-rw-rw-   0        0        0   174847 2023-10-18 12:45:02.000000 adata-2.0.0b0/adata/stock/cache/code.csv
+-rw-rw-rw-   0        0        0     8752 2023-06-02 06:45:42.000000 adata-2.0.0b0/adata/stock/cache/index_code_rel_ths.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.389598 adata-2.0.0b0/adata/stock/index/
+-rw-rw-rw-   0        0        0      267 2023-06-02 03:44:46.000000 adata-2.0.0b0/adata/stock/index/__init__.py
+-rw-rw-rw-   0        0        0      207 2023-06-02 03:44:46.000000 adata-2.0.0b0/adata/stock/index/cal_index.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.392597 adata-2.0.0b0/adata/stock/info/
+-rw-rw-rw-   0        0        0      501 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/stock/info/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.398599 adata-2.0.0b0/adata/stock/info/concept/
+-rw-rw-rw-   0        0        0       86 2023-08-07 03:04:02.000000 adata-2.0.0b0/adata/stock/info/concept/__init__.py
+-rw-rw-rw-   0        0        0      485 2023-08-07 03:04:02.000000 adata-2.0.0b0/adata/stock/info/concept/stock_concept.py
+-rw-rw-rw-   0        0        0     5595 2024-02-26 03:31:53.000000 adata-2.0.0b0/adata/stock/info/concept/stock_concept_east.py
+-rw-rw-rw-   0        0        0      463 2023-12-04 11:54:33.000000 adata-2.0.0b0/adata/stock/info/concept/stock_concept_template.py
+-rw-rw-rw-   0        0        0    15126 2023-12-29 03:33:12.000000 adata-2.0.0b0/adata/stock/info/concept/stock_concept_ths.py
+-rw-rw-rw-   0        0        0     5770 2023-10-18 12:46:30.000000 adata-2.0.0b0/adata/stock/info/stock_code.py
+-rw-rw-rw-   0        0        0    10715 2023-10-18 04:49:44.000000 adata-2.0.0b0/adata/stock/info/stock_index.py
+-rw-rw-rw-   0        0        0     2321 2023-08-08 04:46:57.000000 adata-2.0.0b0/adata/stock/info/trade_calendar.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.400600 adata-2.0.0b0/adata/stock/market/
+-rw-rw-rw-   0        0        0      550 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/stock/market/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.403600 adata-2.0.0b0/adata/stock/market/concepth_market/
+-rw-rw-rw-   0        0        0      385 2023-08-07 03:32:53.000000 adata-2.0.0b0/adata/stock/market/concepth_market/__init__.py
+-rw-rw-rw-   0        0        0     7028 2023-08-08 11:22:09.000000 adata-2.0.0b0/adata/stock/market/concepth_market/concept_market_east.py
+-rw-rw-rw-   0        0        0      695 2023-08-08 11:05:55.000000 adata-2.0.0b0/adata/stock/market/concepth_market/concept_market_template.py
+-rw-rw-rw-   0        0        0     9587 2023-08-08 10:57:42.000000 adata-2.0.0b0/adata/stock/market/concepth_market/concept_market_ths.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.409601 adata-2.0.0b0/adata/stock/market/index_market/
+-rw-rw-rw-   0        0        0       97 2023-08-07 03:04:02.000000 adata-2.0.0b0/adata/stock/market/index_market/__init__.py
+-rw-rw-rw-   0        0        0     2218 2023-12-29 03:56:23.000000 adata-2.0.0b0/adata/stock/market/index_market/market_index.py
+-rw-rw-rw-   0        0        0     6865 2023-12-29 03:55:54.000000 adata-2.0.0b0/adata/stock/market/index_market/market_index_east.py
+-rw-rw-rw-   0        0        0     1746 2023-08-08 11:47:56.000000 adata-2.0.0b0/adata/stock/market/index_market/market_index_template.py
+-rw-rw-rw-   0        0        0     8246 2023-08-08 11:48:17.000000 adata-2.0.0b0/adata/stock/market/index_market/market_index_ths.py
+-rw-rw-rw-   0        0        0     3199 2023-10-18 04:50:22.000000 adata-2.0.0b0/adata/stock/market/stock_dividend.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.416602 adata-2.0.0b0/adata/stock/market/stock_market/
+-rw-rw-rw-   0        0        0      176 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/stock/market/stock_market/__init__.py
+-rw-rw-rw-   0        0        0     3519 2024-04-17 10:25:01.000000 adata-2.0.0b0/adata/stock/market/stock_market/stock_market.py
+-rw-rw-rw-   0        0        0    11398 2023-12-04 12:31:36.000000 adata-2.0.0b0/adata/stock/market/stock_market/stock_market_baidu.py
+-rw-rw-rw-   0        0        0     5415 2023-09-18 06:30:43.000000 adata-2.0.0b0/adata/stock/market/stock_market/stock_market_qq.py
+-rw-rw-rw-   0        0        0     2666 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/market/stock_market/stock_market_sina.py
+-rw-rw-rw-   0        0        0     2658 2023-09-13 12:58:10.000000 adata-2.0.0b0/adata/stock/market/stock_market/stock_market_template.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.311075 adata-2.0.0b0/adata.egg-info/
+-rw-rw-rw-   0        0        0    21039 2024-04-17 10:30:56.000000 adata-2.0.0b0/adata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3649 2024-04-17 10:30:56.000000 adata-2.0.0b0/adata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 10:30:56.000000 adata-2.0.0b0/adata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-17 10:30:56.000000 adata-2.0.0b0/adata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-17 10:30:56.000000 adata-2.0.0b0/adata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 10:30:56.418604 adata-2.0.0b0/setup.cfg
+-rw-rw-rw-   0        0        0     1838 2023-12-04 12:31:36.000000 adata-2.0.0b0/setup.py
```

### Comparing `adata-1.2.4/LICENSE` & `adata-2.0.0b0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `adata-1.2.4/PKG-INFO` & `adata-2.0.0b0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,289 +1,304 @@
-Metadata-Version: 2.1
-Name: adata
-Version: 1.2.4
-Summary: A Data,A Stock,ETF,Bond,Quant,Stock Market,K Line
-Home-page: https://github.com/1nchaos/adata
-Author: 1nchaos
-Author-email: 9527@1nchaos.com
-License: Apache License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.16.0
-Requires-Dist: pandas>=0.22.0
-Requires-Dist: beautifulsoup4>=4.0.2
-Requires-Dist: py_mini_racer>=0.6.0
-
-# [AData](https://adata.1nchaos.com)
-
-<p align="center">
-  <a href="https://adata.1nchaos.com/" target="_blank">
-    <img width="180" src="./docs/AData200x200.png" alt="logo">
-  </a>
-</p>
-
-![GitHub language count](https://img.shields.io/github/languages/count/1nchaos/adata)![GitHub top language](https://img.shields.io/github/languages/top/1nchaos/adata)[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/adata?color=d)](https://pypi.org/project/adata/)[![Licence](https://img.shields.io/hexpm/l/apa?color=d)](https://gitee.com/inchaos/adata/blob/main/LICENSE)[![Downloads](https://static.pepy.tech/badge/adata/week)](https://pepy.tech/project/adata)![GitHub Repo stars](https://img.shields.io/github/stars/1nchaos/adata)![GitHub issues](https://img.shields.io/github/issues/1nchaos/adata)![GitHub contributors](https://img.shields.io/github/contributors/1nchaos/adata)![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/1nchaos/adata)[![Downloads](https://static.pepy.tech/badge/adata)](https://pepy.tech/project/adata)![PyPI - Version](https://img.shields.io/pypi/v/adata)
-
-
-
-## 0、[介绍](https://adata.1nchaos.com/idea.html)
-> 专注A股，专注量化，向阳而生；开放、纯净、持续、为Ai(爱)发电。
->
-> 专注股票行情数据，为了保证数据的高可用性，采用多数据源融合切换。
->
-> 目标：支持个人量化行情的需要；众人拾柴火焰高，欢迎加入。
-
-**市场寒冷，发热不易，坚持更难；如有帮助到你，右上角点 ⭐Star 一键三连，谢谢支持和收藏^_^**
-
-## 一、[快速开始](https://adata.1nchaos.com/quickStart.html)
-
-### （1）安装sdk
-
-~~~python
-# 首次安装
-pip install adata
-# 指定镜像源
-pip install adata -i http://mirrors.aliyun.com/pypi/simple/
-
-# 升级版本
-pip install -U adata
-# 指定镜像源
-pip install -U adata -i http://mirrors.aliyun.com/pypi/simple/
-~~~
-
-**注：国内镜像可能存在同步延迟，可使用官方镜像源，以下是镜像源**
-
-阿里云【推荐】：http://mirrors.aliyun.com/pypi/simple/  
-
-清华大学：https://pypi.tuna.tsinghua.edu.cn/simple  
-
-官方镜像源：https://pypi.org/simple
-
-### （2）使用示例
-
-#### 1. 获取股票代码
-
-获取所有的股票代码
-
-~~~python
-import adata
-
-res_df = adata.stock.info.all_code()
-print(res_df)
-~~~
-
-示例结果：
-
-~~~python
-  stock_code short_name exchange
-0        001324       N长青科       SZ
-1        301361       众智科技       SZ
-2        300514        友讯达       SZ
-...         ...        ...      ...
-5490     300367        网力退       SZ
-5491     300372        欣泰退       SZ
-5492     300431        暴风退       SZ
-
-[5493 rows x 3 columns]
-~~~
-
-#### 2. 获取股票的行情
-
-获取到股票代码后，传入对应的stock_code参数，查询对应股票的行情信息。
-
-```python
-import adata
-
-# k_type: k线类型：1.日；2.周；3.月 默认：1 日k
-res_df = adata.stock.market.get_market(stock_code='000001', k_type=1, start_date='2021-01-01')
-print(res_df)
-```
-
-示例结果：
-
-~~~python
-            trade_time   open  close  ... pre_close stock_code  trade_date
-0    2021-01-04 00:00:00  18.69  18.19  ...     18.93     000001  2021-01-04
-1    2021-01-05 00:00:00  17.99  17.76  ...     18.19     000001  2021-01-05
-2    2021-01-06 00:00:00  17.67  19.15  ...     17.76     000001  2021-01-06
-..                   ...    ...    ...  ...       ...        ...         ...
-573  2023-05-18 00:00:00  12.57  12.49  ...     12.49     000001  2023-05-18
-574  2023-05-19 00:00:00  12.43  12.34  ...     12.49     000001  2023-05-19
-575  2023-05-22 00:00:00  12.31  12.38  ...     12.34     000001  2023-05-22
-
-[576 rows :x 13 columns]
-~~~
-
-#### 3. 其它数据使用
-
-请参考下面数据列表和相关字典文档，找到对应的函数并查看对应的函数注释，进行正确使用。
-
-- [数据字典](https://adata.1nchaos.com/dic/stockInfo.html) 
-
-####  4. 代理设置
-
-项目是基于公开接口，可能存在限制等，因此增加代理设置功能
-
-~~~
-import adata
-
-# 设置代理,代理是全局设置,代理失效后可重新设置。参数:ip,proxy_url
-adata.proxy(is_proxy=True, ip='60.167.21.27:1133')
-res_df = adata.stock.info.all_code()
-print(res_df)
-~~~
-
-**注：**
-
-- v0.0.027b0 及以上版本支持；
-- proxy_url: 获取代理Ip的链接；ip和proxy_url方式选择其一；
-- 每次请求获取一次，为节省ip资源建议使用自建的代理池。
-
-## 二、[数据列表](https://adata.1nchaos.com/dic/dataList.html)
-
-整理了最新版本的数据列表和相关使用Api，详细内容和相关使用参数，请参考数据字典文档。
-
-- [数据列表](https://adata.1nchaos.com/dic/dataList.html) 
-- [数据字典](https://adata.1nchaos.com/dic/stockInfo.html)
-
-### （1）股票-Stock
-
-#### 	1. 基本信息
-
-| 数据             | API                                   | 说明                                   | 备注                                                         |
-| ---------------- | ------------------------------------- | -------------------------------------- | ------------------------------------------------------------ |
-| A股代码          | stock.info.all_code()                 | 所有A股代码信息                        |                                                              |
-| **概念**         |                                       |                                        |                                                              |
-| 来源：同花顺     |                                       |                                        |                                                              |
-| 概念代码         | stock.info.all_concept_code_ths()     | 所有A股概念代码信息（同花顺）          | 来源：同花顺公开数据                                         |
-| 概念成分列表     | stock.info.concept_constituent_ths()  | 获取同花顺概念指数的成分股（同花顺）   | 注意：返回结果只有股票代码和股票简称，可根据概念名称查询     |
-| 股票所属概念     | stock.info.get_concept_ths()          | 获取单只股票所属的概念板块             | [F10](https://basic.10jqka.com.cn/300033/concept.html)       |
-| 来源：东方财富   |                                       |                                        |                                                              |
-| 概念代码         | stock.info.all_concept_code_east()    | 所有A股概念代码信息（东方财富）        | 来源：[东方财富](https://data.eastmoney.com/bkzj/gn.html)    |
-| 概念成分列表     | stock.info.concept_constituent_east() | 获取同花顺概念指数的成分股（东方财富） | 注意：返回结果只有股票代码和股票简称，可根据概念名称查询     |
-| 股票所属概念     | stock.info.get_concept_east()         | 获取单只股票所属的概念板块             | [核心题材](https://emweb.securities.eastmoney.com/pc_hsf10/pages/index.html?type=web&code=SZ300059&color=b#/hxtc) |
-| **指数**         |                                       |                                        |                                                              |
-| 指数代码         | stock.info.all_index_code()           | 获取所有A股市场的指数代码              | 来源同花顺，可能存在同花顺对代码重新编码的情况               |
-| 指数对应的成分股 | stock.info.index_constituent()        | 获取对应指数的成分股列表               |                                                              |
-| **其它**         |                                       |                                        |                                                              |
-| 股票交易日历     | stock.info.trade_calendar()           | 获取股票交易日信息                     | 来源：深交所                                                 |
-
-#### 	2. 行情信息
-
-
-| 数据                | API                                            | 说明                                  | 备注                                                         |
-| ------------------- | ---------------------------------------------- | ------------------------------------- | ------------------------------------------------------------ |
-| 分红信息            | stock.market.get_dividend()                    | 获取单只股票的分红信息                |                                                              |
-| 股票行情            | stock.market.get_market()                      | 获取单只股票的行情信息-日、周、月 k线 |                                                              |
-|                     | stock.market.get_market_min()                  | 获取单个股票的今日分时行情            | 只能获取当天                                                 |
-| <u>**实时行情**</u> | stock.market.list_market_current()             | 获取多个股票最新行情信息              | 实时行情<br />数据源：2个，新浪和腾讯                        |
-|                     | stock.market.get_market_five()                 | 获取单个股票的5档行情信息             | 实时行情<br />数据源：2个，腾讯和百度                        |
-|                     | stock.market.get_market_bar()                  | 获取单个股票的分笔成交行情            | 实时行情<br />[股市通](https://gushitong.baidu.com/stock/ab-872925) |
-| 概念行情-同花顺     | stock.market.get_market_concept_ths()          | 获取单个概念的行情信息-日、周、月 k线 | 获取同花顺概念行情时，<br />请注意传入参数是指数代码还是概念代码，<br />指数代码8开头，index_code |
-|                     | stock.market.get_market_concept_min_ths()      | 获取同花顺概念行情-当日分时           | 只能获取当天                                                 |
-|                     | stock.market.get_market_concept_current_ths()  | 获取同花顺当前的概念行情              | 实时行情                                                     |
-| 概念行情-东方财富   | stock.market.get_market_concept_east()         | 获取单个概念的行情信息-日、周、月 k线 | 获取东方财富概念行情时，<br />指数代码BK开头，index_code     |
-|                     | stock.market.get_market_concept_min_east()     | 获取同花顺概念行情-当日分时           | 只能获取当天                                                 |
-|                     | stock.market.get_market_concept_current_east() | 获取同花顺当前的概念行情              | 实时行情                                                     |
-| 指数行情            | stock.market.get_market_index()                | 获取指数的行情信息-日、周、月 k线     |                                                              |
-|                     | stock.market.get_market_index_min()            | 获取指数的行情-当日分时               |                                                              |
-|                     | stock.market.get_market_index_current()        | 获取当前的指数行情                    | 实时行情                                                     |
-
-**注：概念和指数从本质来看是一样的，所以相关的接口和返回结果是一致的，概念是各个厂商自定义的指数，指数是官方或者权威机构定义的，都是一揽子股票的组合。**
-
-### （2）基金-ETF
-
-| 数据           | API                                      | 说明                           | 备注                                                         |
-| -------------- | ---------------------------------------- | ------------------------------ | ------------------------------------------------------------ |
-| ETF（场内）    | fund.info.all_etf_exchange_traded_info() | 获取所有A股市场的ETF信息       | 来源：1. [东方财富](http://quote.eastmoney.com/center/gridlist.html#fund_etf) |
-| 其它数据排期中 | TODO                                     | 若您有相关资源可以一起参与贡献 |                                                              |
-
-### （3）债券-Bond
-
-| 数据           | API                          | 说明                                | 备注                                                   |
-| -------------- | ---------------------------- | ----------------------------------- | ------------------------------------------------------ |
-| 可转债代码     | bond.info.all_convert_code() | 获取所有A股市场的可转换债券代码信息 | 来源：1. [同花顺](http://data.10jqka.com.cn/ipo/bond/) |
-| 其它数据排期中 | TODO                         | 若您有相关资源可以一起参与贡献      |                                                        |
-
-### （4）舆情
-
-| 数据                     | API                                  | 说明                                       | 备注                                                         |
-| ------------------------ | ------------------------------------ | ------------------------------------------ | ------------------------------------------------------------ |
-| 最近一个月的股票解禁列表 | sentiment.stock_lifting_last_month() | 查询最近一个月的股票解禁列表               | 来源：1. [同花顺](http://data.10jqka.com.cn/market/xsjj/)    |
-| 全市场融资融券余额列表   | sentiment.securities_margin()        | 查询全市场融资融券余额列表                 | 来源：1. [东方财富](https://data.eastmoney.com/rzrq/)        |
-| **北向资金-行情**        |                                      |                                            |                                                              |
-|                          | sentiment.north.north_flow_current() | 获取北向资金（沪深港通）当前流入资金的行情 | 来源：1.[东方财富](https://data.eastmoney.com/hsgt/index.html) |
-|                          | sentiment.north.north_flow_min()     | 获取北向资金分时行情                       |                                                              |
-|                          | sentiment.north.north_flow()         | 获取北向资金历史流入行情                   |                                                              |
-| 其它数据排期中           | TODO                                 | 若您有相关资源可以一起参与贡献             |                                                              |
-
-## 三、[数据源](https://adata.1nchaos.com/dataSource.html)
-
-| 数据源     | 板块                                                         | 描述             |
-| ---------- | ------------------------------------------------------------ | ---------------- |
-| 同花顺     | [数据中心](http://data.10jqka.com.cn/)，[行情中心](http://q.10jqka.com.cn/)，[问财](http://www.iwencai.com/unifiedwap/home/index) | 让投资变的更简单 |
-| 百度股市通 | [股市通](https://gushitong.baidu.com/)                       | 科技让投资更简单 |
-| 东方财富   | [数据中心](https://data.eastmoney.com/center/)，[行情中心](http://quote.eastmoney.com/center/) | 财经门户         |
-| 腾讯理财   | [行情中心](https://stockapp.finance.qq.com/mstats/#)         |                  |
-| 新浪财经   | [新浪财经](https://finance.sina.com.cn/stock/)               | 门户网站         |
-
-***--------------------------------------------感谢各位大厂提供的数据----------------------------------------------***
-
-## 四、 其它参考
-
-主要记录查阅过的项目和相关平台，并对此项目产生了深远印象，特此鸣谢。
-
-| [akshare](https://gitee.com/mirrors/akshare) | [聚宽量化](https://www.joinquant.com/) | [baostock](http://baostock.com/baostock/index.php/Python%E5%BC%80%E5%8F%91%E8%B5%84%E6%BA%90) | [MyData](http://api.mairui.club/hsdata.html) |
-| -------------------------------------------- | -------------------------------------- | ------------------------------------------------------------ | -------------------------------------------- |
-
-## 五、发布计划
-
-|      | 版本号 | 内容 | 发布日期     | 备注                           |
-| ---- | ------ | ---- | ------------ | ------------------------------ |
-| ✅    | 0.x.x  | 股票 | 2023-04-05 ~ | 预览版本                       |
-| ✅ ️    | 1.x.x  | 股票 | 2023-10-01   | 中国Ai股                       |
-| ☑️    | 2.x.x  | 基金、债券 | 2024-01-01 | 场内可交易基金：ETF、可转债        |
-| ☑️    | 3.x.x | xxx        | 排期中       |  |
-
-## 六、理念
-
-1. 关于AData，我们只关注交易产生的数据。在A股只有交易数据是真实的，对于量化和AI训练，也只需要关心交易相关的行情数据，做到真正的专注。当然，你可能会说财务数据等也非常有用，但财务数据相对滞后，而且可能ZJ，甚至有XL可能，最终对于普通交易者可能就成了接盘侠。财务数据在我们这里，只做股票池筛选作用，不做实时交易指标推荐。
-
-2. 根据多年的数据治理经验，函数和字典在设计上面，符合标准的数据存储，可根据数据字典建表落地到数据库。
-
-3. 距离15年已过8年，时光匆匆，**抓住底部机会**。
-
-**注：**
-
-- 永久免费开源A股数据库，只有交易相关的数据，专注量化交易。
-- 送给A股的各位朋友一首歌：[谢天笑-向阳花](https://adata.1nchaos.com/向阳花.html)，愿你我向阳而生。
-
-## 参与贡献
-
-1.  Fork 本仓库
-2.  新建 Feat_xxx 分支
-3.  提交代码（注意代码风格和本项目一致即可）
-4.  新建 Pull Request
-
-
-## 特别鸣谢
-
-> 对于项目有支持，包括但不仅限：内容贡献，bug提交，思想交流等等，对项目有影响的个人和机构
-
-| Simon                                         | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https://github.com/LuneZ99) | 匿名用户 | thue | [Triones009](https://github.com/Triones009) |
-| --------------------------------------------- | ------------------------------------------------- | ------------------------------------- | -------- | ---- | ------------------------------------------- |
-| [LeslieWuboy](https://github.com/LeslieWuboy) |                                                   |                                       |          |      |                                             |
-
-----------------------------------------------------------------------
-
-> 
-## Star History
-
-[![Star History Chart](https://api.star-history.com/svg?repos=1nchaos/adata&type=Date)](https://star-history.com/#1nchaos/adata&Date)
+Metadata-Version: 2.1
+Name: adata
+Version: 2.0.0b0
+Summary: A Data,A Stock,ETF,Bond,Quant,Stock Market,K Line
+Home-page: https://github.com/1nchaos/adata
+Author: 1nchaos
+Author-email: 9527@1nchaos.com
+License: Apache License
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# [AData](https://adata.30006124.xyz)
+
+<p align="center">
+  <a href="https://adata.30006124.xyz/" target="_blank">
+    <img width="180" src="./docs/AData200x200.png" alt="logo">
+  </a>
+</p>
+
+![GitHub language count](https://img.shields.io/github/languages/count/1nchaos/adata)![GitHub top language](https://img.shields.io/github/languages/top/1nchaos/adata)[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/adata?color=d)](https://pypi.org/project/adata/)[![Licence](https://img.shields.io/hexpm/l/apa?color=d)](https://gitee.com/inchaos/adata/blob/main/LICENSE)[![Downloads](https://static.pepy.tech/badge/adata/week)](https://pepy.tech/project/adata)![GitHub Repo stars](https://img.shields.io/github/stars/1nchaos/adata)![GitHub issues](https://img.shields.io/github/issues/1nchaos/adata)![GitHub contributors](https://img.shields.io/github/contributors/1nchaos/adata)![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/1nchaos/adata)[![Downloads](https://static.pepy.tech/badge/adata)](https://pepy.tech/project/adata)![PyPI - Version](https://img.shields.io/pypi/v/adata)
+
+
+
+## 0、[介绍](https://adata.30006124.xyz/idea.html)
+> 专注A股，专注量化，向阳而生；开放、纯净、持续、为Ai(爱)发电。
+>
+> 专注股票行情数据，为了保证数据的高可用性，采用多数据源融合切换。
+>
+> 目标：支持个人量化行情的需要；众人拾柴火焰高，欢迎加入。
+
+**市场寒冷，发热不易，坚持更难；如有帮助到你，右上角点 ⭐Star 一键三连，谢谢支持和收藏^_^**
+
+## 一、[快速开始](https://adata.30006124.xyz/quickStart.html)
+
+### （1）安装sdk
+
+~~~python
+# 首次安装
+pip install adata
+# 指定镜像源
+pip install adata -i http://mirrors.aliyun.com/pypi/simple/
+
+# 升级版本
+pip install -U adata
+# 指定镜像源
+pip install -U adata -i http://mirrors.aliyun.com/pypi/simple/
+~~~
+
+**注：国内镜像可能存在同步延迟，可使用官方镜像源，以下是镜像源**
+
+阿里云【推荐】：http://mirrors.aliyun.com/pypi/simple/  
+
+清华大学：https://pypi.tuna.tsinghua.edu.cn/simple  
+
+官方镜像源：https://pypi.org/simple
+
+### （2）使用示例
+
+#### 1. 获取股票代码
+
+获取所有的股票代码
+
+~~~python
+import adata
+
+res_df = adata.stock.info.all_code()
+print(res_df)
+~~~
+
+示例结果：
+
+~~~python
+  stock_code short_name exchange
+0        001324       N长青科       SZ
+1        301361       众智科技       SZ
+2        300514        友讯达       SZ
+...         ...        ...      ...
+5490     300367        网力退       SZ
+5491     300372        欣泰退       SZ
+5492     300431        暴风退       SZ
+
+[5493 rows x 3 columns]
+~~~
+
+#### 2. 获取股票的行情
+
+获取到股票代码后，传入对应的stock_code参数，查询对应股票的行情信息。
+
+```python
+import adata
+
+# k_type: k线类型：1.日；2.周；3.月 默认：1 日k
+res_df = adata.stock.market.get_market(stock_code='000001', k_type=1, start_date='2021-01-01')
+print(res_df)
+```
+
+示例结果：
+
+~~~python
+            trade_time   open  close  ... pre_close stock_code  trade_date
+0    2021-01-04 00:00:00  18.69  18.19  ...     18.93     000001  2021-01-04
+1    2021-01-05 00:00:00  17.99  17.76  ...     18.19     000001  2021-01-05
+2    2021-01-06 00:00:00  17.67  19.15  ...     17.76     000001  2021-01-06
+..                   ...    ...    ...  ...       ...        ...         ...
+573  2023-05-18 00:00:00  12.57  12.49  ...     12.49     000001  2023-05-18
+574  2023-05-19 00:00:00  12.43  12.34  ...     12.49     000001  2023-05-19
+575  2023-05-22 00:00:00  12.31  12.38  ...     12.34     000001  2023-05-22
+
+[576 rows :x 13 columns]
+~~~
+
+#### 3. 其它数据使用
+
+请参考下面数据列表和相关字典文档，找到对应的函数并查看对应的函数注释，进行正确使用。
+
+- [数据字典](https://adata.30006124.xyz/dic/stockInfo.html) 
+
+####  4. 代理设置
+
+项目是基于公开接口，可能存在限制等，因此增加代理设置功能
+
+~~~
+import adata
+
+# 设置代理,代理是全局设置,代理失效后可重新设置。参数:ip,proxy_url
+adata.proxy(is_proxy=True, ip='60.167.21.27:1133')
+res_df = adata.stock.info.all_code()
+print(res_df)
+~~~
+
+**注：**
+
+- proxy_url: 获取代理Ip的链接；ip和proxy_url方式选择其一；
+- 每次请求获取一次，为节省ip资源建议使用自建的代理池。
+
+## 二、[数据列表](https://adata.30006124.xyz/dic/dataList.html)
+
+整理了最新版本的数据列表和相关使用Api，详细内容和相关使用参数，请参考数据字典文档。
+
+- [数据列表](https://adata.30006124.xyz/dic/dataList.html) 
+- [数据字典](https://adata.30006124.xyz/dic/stockInfo.html)
+
+### （1）股票-Stock
+
+#### 	1. 基本信息
+
+| 数据             | API                                   | 说明                                   | 备注                                                         |
+| ---------------- | ------------------------------------- | -------------------------------------- | ------------------------------------------------------------ |
+| A股代码          | stock.info.all_code()                 | 所有A股代码信息                        |                                                              |
+| **概念**         |                                       |                                        |                                                              |
+| 来源：同花顺     |                                       |                                        |                                                              |
+| 概念代码         | stock.info.all_concept_code_ths()     | 所有A股概念代码信息（同花顺）          | 来源：同花顺公开数据                                         |
+| 概念成分列表     | stock.info.concept_constituent_ths()  | 获取同花顺概念指数的成分股（同花顺）   | 注意：返回结果只有股票代码和股票简称，可根据概念名称查询     |
+| 股票所属概念     | stock.info.get_concept_ths()          | 获取单只股票所属的概念板块             | [F10](https://basic.10jqka.com.cn/300033/concept.html)       |
+| 来源：东方财富   |                                       |                                        |                                                              |
+| 概念代码         | stock.info.all_concept_code_east()    | 所有A股概念代码信息（东方财富）        | 来源：[东方财富](https://data.eastmoney.com/bkzj/gn.html)    |
+| 概念成分列表     | stock.info.concept_constituent_east() | 获取同花顺概念指数的成分股（东方财富） | 注意：返回结果只有股票代码和股票简称，可根据概念名称查询     |
+| 股票所属概念     | stock.info.get_concept_east()         | 获取单只股票所属的概念板块             | [核心题材](https://emweb.securities.eastmoney.com/pc_hsf10/pages/index.html?type=web&code=SZ300059&color=b#/hxtc) |
+| **指数**         |                                       |                                        |                                                              |
+| 指数代码         | stock.info.all_index_code()           | 获取所有A股市场的指数代码              | 来源同花顺，可能存在同花顺对代码重新编码的情况               |
+| 指数对应的成分股 | stock.info.index_constituent()        | 获取对应指数的成分股列表               |                                                              |
+| **其它**         |                                       |                                        |                                                              |
+| 股票交易日历     | stock.info.trade_calendar()           | 获取股票交易日信息                     | 来源：深交所                                                 |
+
+#### 	2. 行情信息
+
+
+| 数据                | API                                            | 说明                                  | 备注                                                         |
+| ------------------- | ---------------------------------------------- | ------------------------------------- | ------------------------------------------------------------ |
+| 分红信息            | stock.market.get_dividend()                    | 获取单只股票的分红信息                |                                                              |
+| 股票行情            | stock.market.get_market()                      | 获取单只股票的行情信息-日、周、月 k线 |                                                              |
+|                     | stock.market.get_market_min()                  | 获取单个股票的今日分时行情            | 只能获取当天                                                 |
+| <u>**实时行情**</u> | stock.market.list_market_current()             | 获取多个股票最新行情信息              | 实时行情<br />数据源：2个，新浪和腾讯                        |
+|                     | stock.market.get_market_five()                 | 获取单个股票的5档行情信息             | 实时行情<br />数据源：2个，腾讯和百度                        |
+|                     | stock.market.get_market_bar()                  | 获取单个股票的分笔成交行情            | 实时行情<br />[股市通](https://gushitong.baidu.com/stock/ab-872925) |
+| 概念行情-同花顺     | stock.market.get_market_concept_ths()          | 获取单个概念的行情信息-日、周、月 k线 | 获取同花顺概念行情时，<br />请注意传入参数是指数代码还是概念代码，<br />指数代码8开头，index_code |
+|                     | stock.market.get_market_concept_min_ths()      | 获取同花顺概念行情-当日分时           | 只能获取当天                                                 |
+|                     | stock.market.get_market_concept_current_ths()  | 获取同花顺当前的概念行情              | 实时行情                                                     |
+| 概念行情-东方财富   | stock.market.get_market_concept_east()         | 获取单个概念的行情信息-日、周、月 k线 | 获取东方财富概念行情时，<br />指数代码BK开头，index_code     |
+|                     | stock.market.get_market_concept_min_east()     | 获取同花顺概念行情-当日分时           | 只能获取当天                                                 |
+|                     | stock.market.get_market_concept_current_east() | 获取同花顺当前的概念行情              | 实时行情                                                     |
+| 指数行情            | stock.market.get_market_index()                | 获取指数的行情信息-日、周、月 k线     |                                                              |
+|                     | stock.market.get_market_index_min()            | 获取指数的行情-当日分时               |                                                              |
+|                     | stock.market.get_market_index_current()        | 获取当前的指数行情                    | 实时行情                                                     |
+
+**注：概念和指数从本质来看是一样的，所以相关的接口和返回结果是一致的，概念是各个厂商自定义的指数，指数是官方或者权威机构定义的，都是一揽子股票的组合。**
+
+### （2）基金-ETF
+
+#### 1. 基本信息
+
+| 数据        | API                                      | 说明                     | 备注                                                         |
+| ----------- | ---------------------------------------- | ------------------------ | ------------------------------------------------------------ |
+| ETF（场内） | fund.info.all_etf_exchange_traded_info() | 获取所有A股市场的ETF信息 | 来源：1. [东方财富](http://quote.eastmoney.com/center/gridlist.html#fund_etf) |
+
+#### 2. 行情信息
+
+| 数据    | API                                  | 说明                             | 备注                                     |
+| ------- | ------------------------------------ | -------------------------------- | ---------------------------------------- |
+| ETF行情 | fund.market.get_market_etf()         | 获取ETF的行情信息-日、周、月 k线 | 来源：[同花顺](https://m.10jqka.com.cn/) |
+|         | fund.market.get_market_etf_min()     | 获取ETF的行情-当日分时           |                                          |
+|         | fund.market.get_market_etf_current() | 获取当前的ETF行情                | 实时行情                                 |
+
+### （3）债券-Bond
+
+| 数据           | API                          | 说明                                | 备注                                                   |
+| -------------- | ---------------------------- | ----------------------------------- | ------------------------------------------------------ |
+| 可转债代码     | bond.info.all_convert_code() | 获取所有A股市场的可转换债券代码信息 | 来源：1. [同花顺](http://data.10jqka.com.cn/ipo/bond/) |
+| 其它数据排期中 | TODO                         | 若您有相关资源可以一起参与贡献      |                                                        |
+
+### （4）舆情
+
+| 数据                     | API                                  | 说明                                       | 备注                                                         |
+| ------------------------ | ------------------------------------ | ------------------------------------------ | ------------------------------------------------------------ |
+| 最近一个月的股票解禁列表 | sentiment.stock_lifting_last_month() | 查询最近一个月的股票解禁列表               | 来源：1. [同花顺](http://data.10jqka.com.cn/market/xsjj/)    |
+| 全市场融资融券余额列表   | sentiment.securities_margin()        | 查询全市场融资融券余额列表                 | 来源：1. [东方财富](https://data.eastmoney.com/rzrq/)        |
+| **北向资金-行情**        |                                      |                                            |                                                              |
+|                          | sentiment.north.north_flow_current() | 获取北向资金（沪深港通）当前流入资金的行情 | 来源：1.[东方财富](https://data.eastmoney.com/hsgt/index.html) |
+|                          | sentiment.north.north_flow_min()     | 获取北向资金分时行情                       |                                                              |
+|                          | sentiment.north.north_flow()         | 获取北向资金历史流入行情                   |                                                              |
+| 其它数据排期中           | TODO                                 | 若您有相关资源可以一起参与贡献             |                                                              |
+
+## 三、[数据源](https://adata.30006124.xyz/dataSource.html)
+
+| 数据源     | 板块                                                         | 描述             |
+| ---------- | ------------------------------------------------------------ | ---------------- |
+| 同花顺     | [数据中心](http://data.10jqka.com.cn/)，[行情中心](http://q.10jqka.com.cn/)，[问财](http://www.iwencai.com/unifiedwap/home/index) | 让投资变的更简单 |
+| 百度股市通 | [股市通](https://gushitong.baidu.com/)                       | 科技让投资更简单 |
+| 东方财富   | [数据中心](https://data.eastmoney.com/center/)，[行情中心](http://quote.eastmoney.com/center/) | 财经门户         |
+| 腾讯理财   | [行情中心](https://stockapp.finance.qq.com/mstats/#)         |                  |
+| 新浪财经   | [新浪财经](https://finance.sina.com.cn/stock/)               | 门户网站         |
+
+***--------------------------------------------感谢各位大厂提供的数据----------------------------------------------***
+
+## 四、 其它参考
+
+主要记录查阅过的项目和相关平台，并对此项目产生了深远印象，特此鸣谢。
+
+| [akshare](https://gitee.com/mirrors/akshare) | [聚宽量化](https://www.joinquant.com/) | [baostock](http://baostock.com/baostock/index.php/Python%E5%BC%80%E5%8F%91%E8%B5%84%E6%BA%90) | [MyData](http://api.mairui.club/hsdata.html) |
+| -------------------------------------------- | -------------------------------------- | ------------------------------------------------------------ | -------------------------------------------- |
+
+## 五、发布计划
+
+|      | 版本号 | 内容 | 发布日期     | 备注                           |
+| ---- | ------ | ---- | ------------ | ------------------------------ |
+| ✅    | 0.x.x  | 股票 | 2023-04-05 ~ | 预览版本                       |
+| ✅ ️    | 1.x.x  | 股票 | 2023-10-01   | 中国Ai股                       |
+| ☑️    | 2.x.x  | 基金、债券 | 开发中 | 场内可交易基金：ETF、可转债        |
+| ☑️    | 3.x.x | xxx        | 排期中       |  |
+
+## 六、理念
+
+1. 关于AData，我们只关注交易产生的数据。在A股只有交易数据是真实的，对于量化和AI训练，也只需要关心交易相关的行情数据，做到真正的专注。当然，你可能会说财务数据等也非常有用，但财务数据相对滞后，而且可能ZJ，甚至有XL可能，最终对于普通交易者可能就成了接盘侠。财务数据在我们这里，只做股票池筛选作用，不做实时交易指标推荐。
+
+2. 根据多年的数据治理经验，函数和字典在设计上面，符合标准的数据存储，可根据数据字典建表落地到数据库。
+
+3. 距离15年已过8年，时光匆匆，**抓住底部机会**。
+
+**注：**
+
+- 永久免费开源A股数据库，只有交易相关的数据，专注量化交易。
+- 送给A股的各位朋友一首歌：[谢天笑-向阳花](https://adata.30006124.xyz/向阳花.html)，愿你我向阳而生。
+
+## 参与贡献
+
+1.  Fork 本仓库
+2.  新建 Feat_xxx 分支
+3.  提交代码（注意代码风格和本项目一致即可）
+4.  新建 Pull Request
+
+
+## 特别鸣谢
+
+> 对于项目有支持，包括但不仅限：内容贡献，bug提交，思想交流等等，对项目有影响的个人和机构
+
+| Simon | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https://github.com/LuneZ99) | 匿名用户 | thue | [Triones009](https://github.com/Triones009) | **[adaaaaaa](https://github.com/adaaaaaa)** | **[LeslieWuboy](https://github.com/LeslieWuboy)** |
+| ----- | ------------------------------------------------- | ------------------------------------- | -------- | ---- | ------------------------------------------- | ------------------------------------------- | ------------------------------------------------- |
+|       |                                                   |                                       |          |      |                                             |                                             |                                                   |
+
+----------------------------------------------------------------------
+
+> 
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=1nchaos/adata&type=Date)](https://star-history.com/#1nchaos/adata&Date)
+
+## 欢迎进行交流
+<p align="center">
+  <a href="https://adata.30006124.xyz/" target="_blank">
+    <img width="180" src="./docs/wx.jpg" alt="logo">
+  </a>
+</p>
+
+- 添加wx好友，备注：Adata量化进交流群；
+- 群最近建立，意在提供一个交流的平台，欢迎讨论交流；
+- 一起保卫3000点直到突破6124点。
```

#### html2text {}

```diff
@@ -1,42 +1,40 @@
-Metadata-Version: 2.1 Name: adata Version: 1.2.4 Summary: A Data,A
+Metadata-Version: 2.1 Name: adata Version: 2.0.0b0 Summary: A Data,A
 Stock,ETF,Bond,Quant,Stock Market,K Line Home-page: https://github.com/1nchaos/
 adata Author: 1nchaos Author-email: 9527@1nchaos.com License: Apache License
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: requests>=2.16.0 Requires-Dist: pandas>=0.22.0
-Requires-Dist: beautifulsoup4>=4.0.2 Requires-Dist: py_mini_racer>=0.6.0 #
-[AData](https://adata.1nchaos.com)
+File: LICENSE # [AData](https://adata.30006124.xyz)
                                     _[_l_o_g_o_]
 ![GitHub language count](https://img.shields.io/github/languages/count/1nchaos/
 adata)![GitHub top language](https://img.shields.io/github/languages/top/
 1nchaos/adata)[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 adata?color=d)](https://pypi.org/project/adata/)[![Licence](https://
 img.shields.io/hexpm/l/apa?color=d)](https://gitee.com/inchaos/adata/blob/main/
 LICENSE)[![Downloads](https://static.pepy.tech/badge/adata/week)](https://
 pepy.tech/project/adata)![GitHub Repo stars](https://img.shields.io/github/
 stars/1nchaos/adata)![GitHub issues](https://img.shields.io/github/issues/
 1nchaos/adata)![GitHub contributors](https://img.shields.io/github/
 contributors/1nchaos/adata)![GitHub (Pre-)Release Date](https://img.shields.io/
 github/release-date-pre/1nchaos/adata)[![Downloads](https://static.pepy.tech/
 badge/adata)](https://pepy.tech/project/adata)![PyPI - Version](https://
-img.shields.io/pypi/v/adata) ## 0ã[ä»ç»](https://adata.1nchaos.com/
+img.shields.io/pypi/v/adata) ## 0ã[ä»ç»](https://adata.30006124.xyz/
 idea.html) >
 ä¸æ³¨Aè¡ï¼ä¸æ³¨éåï¼åé³èçï¼å¼æ¾ãçº¯åãæç»­ãä¸ºAi
 (ç±)åçµã > >
 ä¸æ³¨è¡ç¥¨è¡ææ°æ®ï¼ä¸ºäºä¿è¯æ°æ®çé«å¯ç¨æ§ï¼éç¨å¤æ°æ®æºèååæ¢ã
 > >
 ç®æ ï¼æ¯æä¸ªäººéåè¡æçéè¦ï¼ä¼äººæ¾æ´ç«ç°é«ï¼æ¬¢è¿å å¥ã
 **å¸åºå¯å·ï¼åç­ä¸æï¼åææ´é¾ï¼å¦æå¸®å©å°ä½ ï¼å³ä¸è§ç¹
 â­Star ä¸é®ä¸è¿ï¼è°¢è°¢æ¯æåæ¶è^_^** ## ä¸ã[å¿«éå¼å§]
-(https://adata.1nchaos.com/quickStart.html) ### ï¼1ï¼å®è£sdk ~~~python #
+(https://adata.30006124.xyz/quickStart.html) ### ï¼1ï¼å®è£sdk ~~~python #
 é¦æ¬¡å®è£ pip install adata # æå®éåæº pip install adata -i http://
 mirrors.aliyun.com/pypi/simple/ # åçº§çæ¬ pip install -U adata #
 æå®éåæº pip install -U adata -i http://mirrors.aliyun.com/pypi/simple/
 ~~~
 **æ³¨ï¼å½åéåå¯è½å­å¨åæ­¥å»¶è¿ï¼å¯ä½¿ç¨å®æ¹éåæºï¼ä»¥ä¸æ¯éåæº**
 é¿éäºãæ¨èãï¼http://mirrors.aliyun.com/pypi/simple/
 æ¸åå¤§å­¦ï¼https://pypi.tuna.tsinghua.edu.cn/simple
@@ -55,28 +53,27 @@
 18.19 ... 18.93 000001 2021-01-04 1 2021-01-05 00:00:00 17.99 17.76 ... 18.19
 000001 2021-01-05 2 2021-01-06 00:00:00 17.67 19.15 ... 17.76 000001 2021-01-06
 .. ... ... ... ... ... ... ... 573 2023-05-18 00:00:00 12.57 12.49 ... 12.49
 000001 2023-05-18 574 2023-05-19 00:00:00 12.43 12.34 ... 12.49 000001 2023-05-
 19 575 2023-05-22 00:00:00 12.31 12.38 ... 12.34 000001 2023-05-22 [576 rows :
 x 13 columns] ~~~ #### 3. å¶å®æ°æ®ä½¿ç¨
 è¯·åèä¸é¢æ°æ®åè¡¨åç¸å³å­å¸ææ¡£ï¼æ¾å°å¯¹åºçå½æ°å¹¶æ¥çå¯¹åºçå½æ°æ³¨éï¼è¿è¡æ­£ç¡®ä½¿ç¨ã
-- [æ°æ®å­å¸](https://adata.1nchaos.com/dic/stockInfo.html) #### 4.
+- [æ°æ®å­å¸](https://adata.30006124.xyz/dic/stockInfo.html) #### 4.
 ä»£çè®¾ç½®
 é¡¹ç®æ¯åºäºå¬å¼æ¥å£ï¼å¯è½å­å¨éå¶ç­ï¼å æ­¤å¢å ä»£çè®¾ç½®åè½
 ~~~ import adata #
 è®¾ç½®ä»£ç,ä»£çæ¯å¨å±è®¾ç½®,ä»£çå¤±æåå¯éæ°è®¾ç½®ãåæ°:
 ip,proxy_url adata.proxy(is_proxy=True, ip='60.167.21.27:1133') res_df =
-adata.stock.info.all_code() print(res_df) ~~~ **æ³¨ï¼** - v0.0.027b0
-åä»¥ä¸çæ¬æ¯æï¼ - proxy_url:
+adata.stock.info.all_code() print(res_df) ~~~ **æ³¨ï¼** - proxy_url:
 è·åä»£çIpçé¾æ¥ï¼ipåproxy_urlæ¹å¼éæ©å¶ä¸ï¼ -
 æ¯æ¬¡è¯·æ±è·åä¸æ¬¡ï¼ä¸ºèçipèµæºå»ºè®®ä½¿ç¨èªå»ºçä»£çæ± ã
-## äºã[æ°æ®åè¡¨](https://adata.1nchaos.com/dic/dataList.html)
+## äºã[æ°æ®åè¡¨](https://adata.30006124.xyz/dic/dataList.html)
 æ´çäºææ°çæ¬çæ°æ®åè¡¨åç¸å³ä½¿ç¨Apiï¼è¯¦ç»åå®¹åç¸å³ä½¿ç¨åæ°ï¼è¯·åèæ°æ®å­å¸ææ¡£ã
-- [æ°æ®åè¡¨](https://adata.1nchaos.com/dic/dataList.html) - [æ°æ®å­å¸]
-(https://adata.1nchaos.com/dic/stockInfo.html) ### ï¼1ï¼è¡ç¥¨-Stock #### 1.
+- [æ°æ®åè¡¨](https://adata.30006124.xyz/dic/dataList.html) - [æ°æ®å­å¸]
+(https://adata.30006124.xyz/dic/stockInfo.html) ### ï¼1ï¼è¡ç¥¨-Stock #### 1.
 åºæ¬ä¿¡æ¯ | æ°æ® | API | è¯´æ | å¤æ³¨ | | ---------------- | ----------
 --------------------------- | -------------------------------------- | --------
 ---------------------------------------------------- | | Aè¡ä»£ç  |
 stock.info.all_code() | ææAè¡ä»£ç ä¿¡æ¯ | | | **æ¦å¿µ** | | | | |
 æ¥æºï¼åè±é¡º | | | | | æ¦å¿µä»£ç  | stock.info.all_concept_code_ths() |
 ææAè¡æ¦å¿µä»£ç ä¿¡æ¯ï¼åè±é¡ºï¼ | æ¥æºï¼åè±é¡ºå¬å¼æ°æ® |
 | æ¦å¿µæååè¡¨ | stock.info.concept_constituent_ths() |
@@ -132,24 +129,30 @@
 stock.market.get_market_concept_current_east() |
 è·ååè±é¡ºå½åçæ¦å¿µè¡æ | å®æ¶è¡æ | | ææ°è¡æ |
 stock.market.get_market_index() | è·åææ°çè¡æä¿¡æ¯-æ¥ãå¨ãæ
 kçº¿ | | | | stock.market.get_market_index_min() | è·åææ°çè¡æ-
 å½æ¥åæ¶ | | | | stock.market.get_market_index_current() |
 è·åå½åçææ°è¡æ | å®æ¶è¡æ |
 **æ³¨ï¼æ¦å¿µåææ°ä»æ¬è´¨æ¥çæ¯ä¸æ ·çï¼æä»¥ç¸å³çæ¥å£åè¿åç»ææ¯ä¸è´çï¼æ¦å¿µæ¯åä¸ªååèªå®ä¹çææ°ï¼ææ°æ¯å®æ¹æèæå¨æºæå®ä¹çï¼é½æ¯ä¸æ½å­è¡ç¥¨çç»åã**
-### ï¼2ï¼åºé-ETF | æ°æ® | API | è¯´æ | å¤æ³¨ | | -------------- | ---
-------------------------------------- | ------------------------------ | ------
------------------------------------------------------- | | ETFï¼åºåï¼ |
-fund.info.all_etf_exchange_traded_info() | è·åææAè¡å¸åºçETFä¿¡æ¯ |
-æ¥æºï¼1. [ä¸æ¹è´¢å¯](http://quote.eastmoney.com/center/
-gridlist.html#fund_etf) | | å¶å®æ°æ®ææä¸­ | TODO |
-è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® | | ### ï¼3ï¼åºå¸-Bond |
-æ°æ® | API | è¯´æ | å¤æ³¨ | | -------------- | ---------------------------
-- | ----------------------------------- | -------------------------------------
------------------ | | å¯è½¬åºä»£ç  | bond.info.all_convert_code() |
+### ï¼2ï¼åºé-ETF #### 1. åºæ¬ä¿¡æ¯ | æ°æ® | API | è¯´æ | å¤æ³¨ | |
+----------- | ---------------------------------------- | ----------------------
+-- | ------------------------------------------------------------ | |
+ETFï¼åºåï¼ | fund.info.all_etf_exchange_traded_info() |
+è·åææAè¡å¸åºçETFä¿¡æ¯ | æ¥æºï¼1. [ä¸æ¹è´¢å¯](http://
+quote.eastmoney.com/center/gridlist.html#fund_etf) | #### 2. è¡æä¿¡æ¯ |
+æ°æ® | API | è¯´æ | å¤æ³¨ | | ------- | ----------------------------------
+-- | -------------------------------- | ---------------------------------------
+- | | ETFè¡æ | fund.market.get_market_etf() | è·åETFçè¡æä¿¡æ¯-
+æ¥ãå¨ãæ kçº¿ | æ¥æºï¼[åè±é¡º](https://m.10jqka.com.cn/) | | |
+fund.market.get_market_etf_min() | è·åETFçè¡æ-å½æ¥åæ¶ | | | |
+fund.market.get_market_etf_current() | è·åå½åçETFè¡æ | å®æ¶è¡æ
+| ### ï¼3ï¼åºå¸-Bond | æ°æ® | API | è¯´æ | å¤æ³¨ | | -------------- |
+---------------------------- | ----------------------------------- | ----------
+-------------------------------------------- | | å¯è½¬åºä»£ç  |
+bond.info.all_convert_code() |
 è·åææAè¡å¸åºçå¯è½¬æ¢åºå¸ä»£ç ä¿¡æ¯ | æ¥æºï¼1. [åè±é¡º]
 (http://data.10jqka.com.cn/ipo/bond/) | | å¶å®æ°æ®ææä¸­ | TODO |
 è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® | | ### ï¼4ï¼èæ | æ°æ® |
 API | è¯´æ | å¤æ³¨ | | ------------------------ | --------------------------
 ---------- | ------------------------------------------ | ---------------------
 --------------------------------------- | |
 æè¿ä¸ä¸ªæçè¡ç¥¨è§£ç¦åè¡¨ | sentiment.stock_lifting_last_month() |
@@ -159,17 +162,17 @@
 æ¥æºï¼1. [ä¸æ¹è´¢å¯](https://data.eastmoney.com/rzrq/) | |
 **ååèµé-è¡æ** | | | | | | sentiment.north.north_flow_current() |
 è·åååèµéï¼æ²ªæ·±æ¸¯éï¼å½åæµå¥èµéçè¡æ | æ¥æºï¼1.
 [ä¸æ¹è´¢å¯](https://data.eastmoney.com/hsgt/index.html) | | |
 sentiment.north.north_flow_min() | è·åååèµéåæ¶è¡æ | | | |
 sentiment.north.north_flow() | è·åååèµéåå²æµå¥è¡æ | | |
 å¶å®æ°æ®ææä¸­ | TODO | è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® |
-| ## ä¸ã[æ°æ®æº](https://adata.1nchaos.com/dataSource.html) | æ°æ®æº |
-æ¿å | æè¿° | | ---------- | ----------------------------------------------
--------------- | ---------------- | | åè±é¡º | [æ°æ®ä¸­å¿](http://
+| ## ä¸ã[æ°æ®æº](https://adata.30006124.xyz/dataSource.html) | æ°æ®æº
+| æ¿å | æè¿° | | ---------- | --------------------------------------------
+---------------- | ---------------- | | åè±é¡º | [æ°æ®ä¸­å¿](http://
 data.10jqka.com.cn/)ï¼[è¡æä¸­å¿](http://q.10jqka.com.cn/)ï¼[é®è´¢](http:
 //www.iwencai.com/unifiedwap/home/index) | è®©æèµåçæ´ç®å | |
 ç¾åº¦è¡å¸é | [è¡å¸é](https://gushitong.baidu.com/) |
 ç§æè®©æèµæ´ç®å | | ä¸æ¹è´¢å¯ | [æ°æ®ä¸­å¿](https://
 data.eastmoney.com/center/)ï¼[è¡æä¸­å¿](http://quote.eastmoney.com/center/
 ) | è´¢ç»é¨æ· | | è¾è®¯çè´¢ | [è¡æä¸­å¿](https://
 stockapp.finance.qq.com/mstats/#) | | | æ°æµªè´¢ç» | [æ°æµªè´¢ç»](https://
@@ -182,31 +185,37 @@
 Python%E5%BC%80%E5%8F%91%E8%B5%84%E6%BA%90) | [MyData](http://api.mairui.club/
 hsdata.html) | | -------------------------------------------- | ---------------
 ----------------------- | -----------------------------------------------------
 ------- | -------------------------------------------- | ## äºãåå¸è®¡å
 | | çæ¬å· | åå®¹ | åå¸æ¥æ | å¤æ³¨ | | ---- | ------ | ---- | -----
 ------- | ------------------------------ | | â | 0.x.x | è¡ç¥¨ | 2023-04-05
 ~ | é¢è§çæ¬ | | â ï¸ | 1.x.x | è¡ç¥¨ | 2023-10-01 | ä¸­å½Aiè¡ | |
-âï¸ | 2.x.x | åºéãåºå¸ | 2024-01-01 |
+âï¸ | 2.x.x | åºéãåºå¸ | å¼åä¸­ |
 åºåå¯äº¤æåºéï¼ETFãå¯è½¬åº | | âï¸ | 3.x.x | xxx | ææä¸­ |
 | ## å­ãçå¿µ 1.
 å³äºADataï¼æä»¬åªå³æ³¨äº¤æäº§ççæ°æ®ãå¨Aè¡åªæäº¤ææ°æ®æ¯çå®çï¼å¯¹äºéååAIè®­ç»ï¼ä¹åªéè¦å³å¿äº¤æç¸å³çè¡ææ°æ®ï¼åå°çæ­£çä¸æ³¨ãå½ç¶ï¼ä½ å¯è½ä¼è¯´è´¢å¡æ°æ®ç­ä¹éå¸¸æç¨ï¼ä½è´¢å¡æ°æ®ç¸å¯¹æ»åï¼èä¸å¯è½ZJï¼çè³æXLå¯è½ï¼æç»å¯¹äºæ®éäº¤æèå¯è½å°±æäºæ¥çä¾ ãè´¢å¡æ°æ®å¨æä»¬è¿éï¼åªåè¡ç¥¨æ± ç­éä½ç¨ï¼ä¸åå®æ¶äº¤æææ æ¨èã
 2.
 æ ¹æ®å¤å¹´çæ°æ®æ²»çç»éªï¼å½æ°åå­å¸å¨è®¾è®¡ä¸é¢ï¼ç¬¦åæ åçæ°æ®å­å¨ï¼å¯æ ¹æ®æ°æ®å­å¸å»ºè¡¨è½å°å°æ°æ®åºã
 3. è·ç¦»15å¹´å·²è¿8å¹´ï¼æ¶åååï¼**æä½åºé¨æºä¼**ã **æ³¨ï¼**
 -
 æ°¸ä¹åè´¹å¼æºAè¡æ°æ®åºï¼åªæäº¤æç¸å³çæ°æ®ï¼ä¸æ³¨éåäº¤æã
 - éç»Aè¡çåä½æåä¸é¦æ­ï¼[è°¢å¤©ç¬-åé³è±](https://
-adata.1nchaos.com/åé³è±.html)ï¼æ¿ä½ æåé³èçã ## åä¸è´¡ç® 1.
-Fork æ¬ä»åº 2. æ°å»º Feat_xxx åæ¯ 3.
+adata.30006124.xyz/åé³è±.html)ï¼æ¿ä½ æåé³èçã ## åä¸è´¡ç®
+1. Fork æ¬ä»åº 2. æ°å»º Feat_xxx åæ¯ 3.
 æäº¤ä»£ç ï¼æ³¨æä»£ç é£æ ¼åæ¬é¡¹ç®ä¸è´å³å¯ï¼ 4. æ°å»º Pull
 Request ## ç¹å«é¸£è°¢ >
 å¯¹äºé¡¹ç®ææ¯æï¼åæ¬ä½ä¸ä»éï¼åå®¹è´¡ç®ï¼bugæäº¤ï¼ææ³äº¤æµç­ç­ï¼å¯¹é¡¹ç®æå½±åçä¸ªäººåæºæ
 | Simon | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https:/
 /github.com/LuneZ99) | å¿åç¨æ· | thue | [Triones009](https://github.com/
-Triones009) | | --------------------------------------------- | ---------------
----------------------------------- | ------------------------------------- | --
------- | ---- | ------------------------------------------- | | [LeslieWuboy]
-(https://github.com/LeslieWuboy) | | | | | | ----------------------------------
------------------------------------- > ## Star History [![Star History Chart]
-(https://api.star-history.com/svg?repos=1nchaos/adata&type=Date)](https://star-
-history.com/#1nchaos/adata&Date)
+Triones009) | **[adaaaaaa](https://github.com/adaaaaaa)** | **[LeslieWuboy]
+(https://github.com/LeslieWuboy)** | | ----- | --------------------------------
+----------------- | ------------------------------------- | -------- | ---- | -
+------------------------------------------ | ----------------------------------
+--------- | ------------------------------------------------- | | | | | | | | |
+| ---------------------------------------------------------------------- > ##
+Star History [![Star History Chart](https://api.star-history.com/
+svg?repos=1nchaos/adata&type=Date)](https://star-history.com/#1nchaos/
+adata&Date) ## æ¬¢è¿è¿è¡äº¤æµ
+                                    _[_l_o_g_o_]
+- æ·»å wxå¥½åï¼å¤æ³¨ï¼Adataéåè¿äº¤æµç¾¤ï¼ -
+ç¾¤æè¿å»ºç«ï¼æå¨æä¾ä¸ä¸ªäº¤æµçå¹³å°ï¼æ¬¢è¿è®¨è®ºäº¤æµï¼ -
+ä¸èµ·ä¿å«3000ç¹ç´å°çªç ´6124ç¹ã
```

### Comparing `adata-1.2.4/README.md` & `adata-2.0.0b0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,266 +1,285 @@
-# [AData](https://adata.1nchaos.com)
-
-<p align="center">
-  <a href="https://adata.1nchaos.com/" target="_blank">
-    <img width="180" src="./docs/AData200x200.png" alt="logo">
-  </a>
-</p>
-
-![GitHub language count](https://img.shields.io/github/languages/count/1nchaos/adata)![GitHub top language](https://img.shields.io/github/languages/top/1nchaos/adata)[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/adata?color=d)](https://pypi.org/project/adata/)[![Licence](https://img.shields.io/hexpm/l/apa?color=d)](https://gitee.com/inchaos/adata/blob/main/LICENSE)[![Downloads](https://static.pepy.tech/badge/adata/week)](https://pepy.tech/project/adata)![GitHub Repo stars](https://img.shields.io/github/stars/1nchaos/adata)![GitHub issues](https://img.shields.io/github/issues/1nchaos/adata)![GitHub contributors](https://img.shields.io/github/contributors/1nchaos/adata)![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/1nchaos/adata)[![Downloads](https://static.pepy.tech/badge/adata)](https://pepy.tech/project/adata)![PyPI - Version](https://img.shields.io/pypi/v/adata)
-
-
-
-## 0、[介绍](https://adata.1nchaos.com/idea.html)
-> 专注A股，专注量化，向阳而生；开放、纯净、持续、为Ai(爱)发电。
->
-> 专注股票行情数据，为了保证数据的高可用性，采用多数据源融合切换。
->
-> 目标：支持个人量化行情的需要；众人拾柴火焰高，欢迎加入。
-
-**市场寒冷，发热不易，坚持更难；如有帮助到你，右上角点 ⭐Star 一键三连，谢谢支持和收藏^_^**
-
-## 一、[快速开始](https://adata.1nchaos.com/quickStart.html)
-
-### （1）安装sdk
-
-~~~python
-# 首次安装
-pip install adata
-# 指定镜像源
-pip install adata -i http://mirrors.aliyun.com/pypi/simple/
-
-# 升级版本
-pip install -U adata
-# 指定镜像源
-pip install -U adata -i http://mirrors.aliyun.com/pypi/simple/
-~~~
-
-**注：国内镜像可能存在同步延迟，可使用官方镜像源，以下是镜像源**
-
-阿里云【推荐】：http://mirrors.aliyun.com/pypi/simple/  
-
-清华大学：https://pypi.tuna.tsinghua.edu.cn/simple  
-
-官方镜像源：https://pypi.org/simple
-
-### （2）使用示例
-
-#### 1. 获取股票代码
-
-获取所有的股票代码
-
-~~~python
-import adata
-
-res_df = adata.stock.info.all_code()
-print(res_df)
-~~~
-
-示例结果：
-
-~~~python
-  stock_code short_name exchange
-0        001324       N长青科       SZ
-1        301361       众智科技       SZ
-2        300514        友讯达       SZ
-...         ...        ...      ...
-5490     300367        网力退       SZ
-5491     300372        欣泰退       SZ
-5492     300431        暴风退       SZ
-
-[5493 rows x 3 columns]
-~~~
-
-#### 2. 获取股票的行情
-
-获取到股票代码后，传入对应的stock_code参数，查询对应股票的行情信息。
-
-```python
-import adata
-
-# k_type: k线类型：1.日；2.周；3.月 默认：1 日k
-res_df = adata.stock.market.get_market(stock_code='000001', k_type=1, start_date='2021-01-01')
-print(res_df)
-```
-
-示例结果：
-
-~~~python
-            trade_time   open  close  ... pre_close stock_code  trade_date
-0    2021-01-04 00:00:00  18.69  18.19  ...     18.93     000001  2021-01-04
-1    2021-01-05 00:00:00  17.99  17.76  ...     18.19     000001  2021-01-05
-2    2021-01-06 00:00:00  17.67  19.15  ...     17.76     000001  2021-01-06
-..                   ...    ...    ...  ...       ...        ...         ...
-573  2023-05-18 00:00:00  12.57  12.49  ...     12.49     000001  2023-05-18
-574  2023-05-19 00:00:00  12.43  12.34  ...     12.49     000001  2023-05-19
-575  2023-05-22 00:00:00  12.31  12.38  ...     12.34     000001  2023-05-22
-
-[576 rows :x 13 columns]
-~~~
-
-#### 3. 其它数据使用
-
-请参考下面数据列表和相关字典文档，找到对应的函数并查看对应的函数注释，进行正确使用。
-
-- [数据字典](https://adata.1nchaos.com/dic/stockInfo.html) 
-
-####  4. 代理设置
-
-项目是基于公开接口，可能存在限制等，因此增加代理设置功能
-
-~~~
-import adata
-
-# 设置代理,代理是全局设置,代理失效后可重新设置。参数:ip,proxy_url
-adata.proxy(is_proxy=True, ip='60.167.21.27:1133')
-res_df = adata.stock.info.all_code()
-print(res_df)
-~~~
-
-**注：**
-
-- v0.0.027b0 及以上版本支持；
-- proxy_url: 获取代理Ip的链接；ip和proxy_url方式选择其一；
-- 每次请求获取一次，为节省ip资源建议使用自建的代理池。
-
-## 二、[数据列表](https://adata.1nchaos.com/dic/dataList.html)
-
-整理了最新版本的数据列表和相关使用Api，详细内容和相关使用参数，请参考数据字典文档。
-
-- [数据列表](https://adata.1nchaos.com/dic/dataList.html) 
-- [数据字典](https://adata.1nchaos.com/dic/stockInfo.html)
-
-### （1）股票-Stock
-
-#### 	1. 基本信息
-
-| 数据             | API                                   | 说明                                   | 备注                                                         |
-| ---------------- | ------------------------------------- | -------------------------------------- | ------------------------------------------------------------ |
-| A股代码          | stock.info.all_code()                 | 所有A股代码信息                        |                                                              |
-| **概念**         |                                       |                                        |                                                              |
-| 来源：同花顺     |                                       |                                        |                                                              |
-| 概念代码         | stock.info.all_concept_code_ths()     | 所有A股概念代码信息（同花顺）          | 来源：同花顺公开数据                                         |
-| 概念成分列表     | stock.info.concept_constituent_ths()  | 获取同花顺概念指数的成分股（同花顺）   | 注意：返回结果只有股票代码和股票简称，可根据概念名称查询     |
-| 股票所属概念     | stock.info.get_concept_ths()          | 获取单只股票所属的概念板块             | [F10](https://basic.10jqka.com.cn/300033/concept.html)       |
-| 来源：东方财富   |                                       |                                        |                                                              |
-| 概念代码         | stock.info.all_concept_code_east()    | 所有A股概念代码信息（东方财富）        | 来源：[东方财富](https://data.eastmoney.com/bkzj/gn.html)    |
-| 概念成分列表     | stock.info.concept_constituent_east() | 获取同花顺概念指数的成分股（东方财富） | 注意：返回结果只有股票代码和股票简称，可根据概念名称查询     |
-| 股票所属概念     | stock.info.get_concept_east()         | 获取单只股票所属的概念板块             | [核心题材](https://emweb.securities.eastmoney.com/pc_hsf10/pages/index.html?type=web&code=SZ300059&color=b#/hxtc) |
-| **指数**         |                                       |                                        |                                                              |
-| 指数代码         | stock.info.all_index_code()           | 获取所有A股市场的指数代码              | 来源同花顺，可能存在同花顺对代码重新编码的情况               |
-| 指数对应的成分股 | stock.info.index_constituent()        | 获取对应指数的成分股列表               |                                                              |
-| **其它**         |                                       |                                        |                                                              |
-| 股票交易日历     | stock.info.trade_calendar()           | 获取股票交易日信息                     | 来源：深交所                                                 |
-
-#### 	2. 行情信息
-
-
-| 数据                | API                                            | 说明                                  | 备注                                                         |
-| ------------------- | ---------------------------------------------- | ------------------------------------- | ------------------------------------------------------------ |
-| 分红信息            | stock.market.get_dividend()                    | 获取单只股票的分红信息                |                                                              |
-| 股票行情            | stock.market.get_market()                      | 获取单只股票的行情信息-日、周、月 k线 |                                                              |
-|                     | stock.market.get_market_min()                  | 获取单个股票的今日分时行情            | 只能获取当天                                                 |
-| <u>**实时行情**</u> | stock.market.list_market_current()             | 获取多个股票最新行情信息              | 实时行情<br />数据源：2个，新浪和腾讯                        |
-|                     | stock.market.get_market_five()                 | 获取单个股票的5档行情信息             | 实时行情<br />数据源：2个，腾讯和百度                        |
-|                     | stock.market.get_market_bar()                  | 获取单个股票的分笔成交行情            | 实时行情<br />[股市通](https://gushitong.baidu.com/stock/ab-872925) |
-| 概念行情-同花顺     | stock.market.get_market_concept_ths()          | 获取单个概念的行情信息-日、周、月 k线 | 获取同花顺概念行情时，<br />请注意传入参数是指数代码还是概念代码，<br />指数代码8开头，index_code |
-|                     | stock.market.get_market_concept_min_ths()      | 获取同花顺概念行情-当日分时           | 只能获取当天                                                 |
-|                     | stock.market.get_market_concept_current_ths()  | 获取同花顺当前的概念行情              | 实时行情                                                     |
-| 概念行情-东方财富   | stock.market.get_market_concept_east()         | 获取单个概念的行情信息-日、周、月 k线 | 获取东方财富概念行情时，<br />指数代码BK开头，index_code     |
-|                     | stock.market.get_market_concept_min_east()     | 获取同花顺概念行情-当日分时           | 只能获取当天                                                 |
-|                     | stock.market.get_market_concept_current_east() | 获取同花顺当前的概念行情              | 实时行情                                                     |
-| 指数行情            | stock.market.get_market_index()                | 获取指数的行情信息-日、周、月 k线     |                                                              |
-|                     | stock.market.get_market_index_min()            | 获取指数的行情-当日分时               |                                                              |
-|                     | stock.market.get_market_index_current()        | 获取当前的指数行情                    | 实时行情                                                     |
-
-**注：概念和指数从本质来看是一样的，所以相关的接口和返回结果是一致的，概念是各个厂商自定义的指数，指数是官方或者权威机构定义的，都是一揽子股票的组合。**
-
-### （2）基金-ETF
-
-| 数据           | API                                      | 说明                           | 备注                                                         |
-| -------------- | ---------------------------------------- | ------------------------------ | ------------------------------------------------------------ |
-| ETF（场内）    | fund.info.all_etf_exchange_traded_info() | 获取所有A股市场的ETF信息       | 来源：1. [东方财富](http://quote.eastmoney.com/center/gridlist.html#fund_etf) |
-| 其它数据排期中 | TODO                                     | 若您有相关资源可以一起参与贡献 |                                                              |
-
-### （3）债券-Bond
-
-| 数据           | API                          | 说明                                | 备注                                                   |
-| -------------- | ---------------------------- | ----------------------------------- | ------------------------------------------------------ |
-| 可转债代码     | bond.info.all_convert_code() | 获取所有A股市场的可转换债券代码信息 | 来源：1. [同花顺](http://data.10jqka.com.cn/ipo/bond/) |
-| 其它数据排期中 | TODO                         | 若您有相关资源可以一起参与贡献      |                                                        |
-
-### （4）舆情
-
-| 数据                     | API                                  | 说明                                       | 备注                                                         |
-| ------------------------ | ------------------------------------ | ------------------------------------------ | ------------------------------------------------------------ |
-| 最近一个月的股票解禁列表 | sentiment.stock_lifting_last_month() | 查询最近一个月的股票解禁列表               | 来源：1. [同花顺](http://data.10jqka.com.cn/market/xsjj/)    |
-| 全市场融资融券余额列表   | sentiment.securities_margin()        | 查询全市场融资融券余额列表                 | 来源：1. [东方财富](https://data.eastmoney.com/rzrq/)        |
-| **北向资金-行情**        |                                      |                                            |                                                              |
-|                          | sentiment.north.north_flow_current() | 获取北向资金（沪深港通）当前流入资金的行情 | 来源：1.[东方财富](https://data.eastmoney.com/hsgt/index.html) |
-|                          | sentiment.north.north_flow_min()     | 获取北向资金分时行情                       |                                                              |
-|                          | sentiment.north.north_flow()         | 获取北向资金历史流入行情                   |                                                              |
-| 其它数据排期中           | TODO                                 | 若您有相关资源可以一起参与贡献             |                                                              |
-
-## 三、[数据源](https://adata.1nchaos.com/dataSource.html)
-
-| 数据源     | 板块                                                         | 描述             |
-| ---------- | ------------------------------------------------------------ | ---------------- |
-| 同花顺     | [数据中心](http://data.10jqka.com.cn/)，[行情中心](http://q.10jqka.com.cn/)，[问财](http://www.iwencai.com/unifiedwap/home/index) | 让投资变的更简单 |
-| 百度股市通 | [股市通](https://gushitong.baidu.com/)                       | 科技让投资更简单 |
-| 东方财富   | [数据中心](https://data.eastmoney.com/center/)，[行情中心](http://quote.eastmoney.com/center/) | 财经门户         |
-| 腾讯理财   | [行情中心](https://stockapp.finance.qq.com/mstats/#)         |                  |
-| 新浪财经   | [新浪财经](https://finance.sina.com.cn/stock/)               | 门户网站         |
-
-***--------------------------------------------感谢各位大厂提供的数据----------------------------------------------***
-
-## 四、 其它参考
-
-主要记录查阅过的项目和相关平台，并对此项目产生了深远印象，特此鸣谢。
-
-| [akshare](https://gitee.com/mirrors/akshare) | [聚宽量化](https://www.joinquant.com/) | [baostock](http://baostock.com/baostock/index.php/Python%E5%BC%80%E5%8F%91%E8%B5%84%E6%BA%90) | [MyData](http://api.mairui.club/hsdata.html) |
-| -------------------------------------------- | -------------------------------------- | ------------------------------------------------------------ | -------------------------------------------- |
-
-## 五、发布计划
-
-|      | 版本号 | 内容 | 发布日期     | 备注                           |
-| ---- | ------ | ---- | ------------ | ------------------------------ |
-| ✅    | 0.x.x  | 股票 | 2023-04-05 ~ | 预览版本                       |
-| ✅ ️    | 1.x.x  | 股票 | 2023-10-01   | 中国Ai股                       |
-| ☑️    | 2.x.x  | 基金、债券 | 2024-01-01 | 场内可交易基金：ETF、可转债        |
-| ☑️    | 3.x.x | xxx        | 排期中       |  |
-
-## 六、理念
-
-1. 关于AData，我们只关注交易产生的数据。在A股只有交易数据是真实的，对于量化和AI训练，也只需要关心交易相关的行情数据，做到真正的专注。当然，你可能会说财务数据等也非常有用，但财务数据相对滞后，而且可能ZJ，甚至有XL可能，最终对于普通交易者可能就成了接盘侠。财务数据在我们这里，只做股票池筛选作用，不做实时交易指标推荐。
-
-2. 根据多年的数据治理经验，函数和字典在设计上面，符合标准的数据存储，可根据数据字典建表落地到数据库。
-
-3. 距离15年已过8年，时光匆匆，**抓住底部机会**。
-
-**注：**
-
-- 永久免费开源A股数据库，只有交易相关的数据，专注量化交易。
-- 送给A股的各位朋友一首歌：[谢天笑-向阳花](https://adata.1nchaos.com/向阳花.html)，愿你我向阳而生。
-
-## 参与贡献
-
-1.  Fork 本仓库
-2.  新建 Feat_xxx 分支
-3.  提交代码（注意代码风格和本项目一致即可）
-4.  新建 Pull Request
-
-
-## 特别鸣谢
-
-> 对于项目有支持，包括但不仅限：内容贡献，bug提交，思想交流等等，对项目有影响的个人和机构
-
-| Simon                                         | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https://github.com/LuneZ99) | 匿名用户 | thue | [Triones009](https://github.com/Triones009) |
-| --------------------------------------------- | ------------------------------------------------- | ------------------------------------- | -------- | ---- | ------------------------------------------- |
-| [LeslieWuboy](https://github.com/LeslieWuboy) |                                                   |                                       |          |      |                                             |
-
-----------------------------------------------------------------------
-
-> 
-## Star History
-
-[![Star History Chart](https://api.star-history.com/svg?repos=1nchaos/adata&type=Date)](https://star-history.com/#1nchaos/adata&Date)
+# [AData](https://adata.30006124.xyz)
+
+<p align="center">
+  <a href="https://adata.30006124.xyz/" target="_blank">
+    <img width="180" src="./docs/AData200x200.png" alt="logo">
+  </a>
+</p>
+
+![GitHub language count](https://img.shields.io/github/languages/count/1nchaos/adata)![GitHub top language](https://img.shields.io/github/languages/top/1nchaos/adata)[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/adata?color=d)](https://pypi.org/project/adata/)[![Licence](https://img.shields.io/hexpm/l/apa?color=d)](https://gitee.com/inchaos/adata/blob/main/LICENSE)[![Downloads](https://static.pepy.tech/badge/adata/week)](https://pepy.tech/project/adata)![GitHub Repo stars](https://img.shields.io/github/stars/1nchaos/adata)![GitHub issues](https://img.shields.io/github/issues/1nchaos/adata)![GitHub contributors](https://img.shields.io/github/contributors/1nchaos/adata)![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/1nchaos/adata)[![Downloads](https://static.pepy.tech/badge/adata)](https://pepy.tech/project/adata)![PyPI - Version](https://img.shields.io/pypi/v/adata)
+
+
+
+## 0、[介绍](https://adata.30006124.xyz/idea.html)
+> 专注A股，专注量化，向阳而生；开放、纯净、持续、为Ai(爱)发电。
+>
+> 专注股票行情数据，为了保证数据的高可用性，采用多数据源融合切换。
+>
+> 目标：支持个人量化行情的需要；众人拾柴火焰高，欢迎加入。
+
+**市场寒冷，发热不易，坚持更难；如有帮助到你，右上角点 ⭐Star 一键三连，谢谢支持和收藏^_^**
+
+## 一、[快速开始](https://adata.30006124.xyz/quickStart.html)
+
+### （1）安装sdk
+
+~~~python
+# 首次安装
+pip install adata
+# 指定镜像源
+pip install adata -i http://mirrors.aliyun.com/pypi/simple/
+
+# 升级版本
+pip install -U adata
+# 指定镜像源
+pip install -U adata -i http://mirrors.aliyun.com/pypi/simple/
+~~~
+
+**注：国内镜像可能存在同步延迟，可使用官方镜像源，以下是镜像源**
+
+阿里云【推荐】：http://mirrors.aliyun.com/pypi/simple/  
+
+清华大学：https://pypi.tuna.tsinghua.edu.cn/simple  
+
+官方镜像源：https://pypi.org/simple
+
+### （2）使用示例
+
+#### 1. 获取股票代码
+
+获取所有的股票代码
+
+~~~python
+import adata
+
+res_df = adata.stock.info.all_code()
+print(res_df)
+~~~
+
+示例结果：
+
+~~~python
+  stock_code short_name exchange
+0        001324       N长青科       SZ
+1        301361       众智科技       SZ
+2        300514        友讯达       SZ
+...         ...        ...      ...
+5490     300367        网力退       SZ
+5491     300372        欣泰退       SZ
+5492     300431        暴风退       SZ
+
+[5493 rows x 3 columns]
+~~~
+
+#### 2. 获取股票的行情
+
+获取到股票代码后，传入对应的stock_code参数，查询对应股票的行情信息。
+
+```python
+import adata
+
+# k_type: k线类型：1.日；2.周；3.月 默认：1 日k
+res_df = adata.stock.market.get_market(stock_code='000001', k_type=1, start_date='2021-01-01')
+print(res_df)
+```
+
+示例结果：
+
+~~~python
+            trade_time   open  close  ... pre_close stock_code  trade_date
+0    2021-01-04 00:00:00  18.69  18.19  ...     18.93     000001  2021-01-04
+1    2021-01-05 00:00:00  17.99  17.76  ...     18.19     000001  2021-01-05
+2    2021-01-06 00:00:00  17.67  19.15  ...     17.76     000001  2021-01-06
+..                   ...    ...    ...  ...       ...        ...         ...
+573  2023-05-18 00:00:00  12.57  12.49  ...     12.49     000001  2023-05-18
+574  2023-05-19 00:00:00  12.43  12.34  ...     12.49     000001  2023-05-19
+575  2023-05-22 00:00:00  12.31  12.38  ...     12.34     000001  2023-05-22
+
+[576 rows :x 13 columns]
+~~~
+
+#### 3. 其它数据使用
+
+请参考下面数据列表和相关字典文档，找到对应的函数并查看对应的函数注释，进行正确使用。
+
+- [数据字典](https://adata.30006124.xyz/dic/stockInfo.html) 
+
+####  4. 代理设置
+
+项目是基于公开接口，可能存在限制等，因此增加代理设置功能
+
+~~~
+import adata
+
+# 设置代理,代理是全局设置,代理失效后可重新设置。参数:ip,proxy_url
+adata.proxy(is_proxy=True, ip='60.167.21.27:1133')
+res_df = adata.stock.info.all_code()
+print(res_df)
+~~~
+
+**注：**
+
+- proxy_url: 获取代理Ip的链接；ip和proxy_url方式选择其一；
+- 每次请求获取一次，为节省ip资源建议使用自建的代理池。
+
+## 二、[数据列表](https://adata.30006124.xyz/dic/dataList.html)
+
+整理了最新版本的数据列表和相关使用Api，详细内容和相关使用参数，请参考数据字典文档。
+
+- [数据列表](https://adata.30006124.xyz/dic/dataList.html) 
+- [数据字典](https://adata.30006124.xyz/dic/stockInfo.html)
+
+### （1）股票-Stock
+
+#### 	1. 基本信息
+
+| 数据             | API                                   | 说明                                   | 备注                                                         |
+| ---------------- | ------------------------------------- | -------------------------------------- | ------------------------------------------------------------ |
+| A股代码          | stock.info.all_code()                 | 所有A股代码信息                        |                                                              |
+| **概念**         |                                       |                                        |                                                              |
+| 来源：同花顺     |                                       |                                        |                                                              |
+| 概念代码         | stock.info.all_concept_code_ths()     | 所有A股概念代码信息（同花顺）          | 来源：同花顺公开数据                                         |
+| 概念成分列表     | stock.info.concept_constituent_ths()  | 获取同花顺概念指数的成分股（同花顺）   | 注意：返回结果只有股票代码和股票简称，可根据概念名称查询     |
+| 股票所属概念     | stock.info.get_concept_ths()          | 获取单只股票所属的概念板块             | [F10](https://basic.10jqka.com.cn/300033/concept.html)       |
+| 来源：东方财富   |                                       |                                        |                                                              |
+| 概念代码         | stock.info.all_concept_code_east()    | 所有A股概念代码信息（东方财富）        | 来源：[东方财富](https://data.eastmoney.com/bkzj/gn.html)    |
+| 概念成分列表     | stock.info.concept_constituent_east() | 获取同花顺概念指数的成分股（东方财富） | 注意：返回结果只有股票代码和股票简称，可根据概念名称查询     |
+| 股票所属概念     | stock.info.get_concept_east()         | 获取单只股票所属的概念板块             | [核心题材](https://emweb.securities.eastmoney.com/pc_hsf10/pages/index.html?type=web&code=SZ300059&color=b#/hxtc) |
+| **指数**         |                                       |                                        |                                                              |
+| 指数代码         | stock.info.all_index_code()           | 获取所有A股市场的指数代码              | 来源同花顺，可能存在同花顺对代码重新编码的情况               |
+| 指数对应的成分股 | stock.info.index_constituent()        | 获取对应指数的成分股列表               |                                                              |
+| **其它**         |                                       |                                        |                                                              |
+| 股票交易日历     | stock.info.trade_calendar()           | 获取股票交易日信息                     | 来源：深交所                                                 |
+
+#### 	2. 行情信息
+
+
+| 数据                | API                                            | 说明                                  | 备注                                                         |
+| ------------------- | ---------------------------------------------- | ------------------------------------- | ------------------------------------------------------------ |
+| 分红信息            | stock.market.get_dividend()                    | 获取单只股票的分红信息                |                                                              |
+| 股票行情            | stock.market.get_market()                      | 获取单只股票的行情信息-日、周、月 k线 |                                                              |
+|                     | stock.market.get_market_min()                  | 获取单个股票的今日分时行情            | 只能获取当天                                                 |
+| <u>**实时行情**</u> | stock.market.list_market_current()             | 获取多个股票最新行情信息              | 实时行情<br />数据源：2个，新浪和腾讯                        |
+|                     | stock.market.get_market_five()                 | 获取单个股票的5档行情信息             | 实时行情<br />数据源：2个，腾讯和百度                        |
+|                     | stock.market.get_market_bar()                  | 获取单个股票的分笔成交行情            | 实时行情<br />[股市通](https://gushitong.baidu.com/stock/ab-872925) |
+| 概念行情-同花顺     | stock.market.get_market_concept_ths()          | 获取单个概念的行情信息-日、周、月 k线 | 获取同花顺概念行情时，<br />请注意传入参数是指数代码还是概念代码，<br />指数代码8开头，index_code |
+|                     | stock.market.get_market_concept_min_ths()      | 获取同花顺概念行情-当日分时           | 只能获取当天                                                 |
+|                     | stock.market.get_market_concept_current_ths()  | 获取同花顺当前的概念行情              | 实时行情                                                     |
+| 概念行情-东方财富   | stock.market.get_market_concept_east()         | 获取单个概念的行情信息-日、周、月 k线 | 获取东方财富概念行情时，<br />指数代码BK开头，index_code     |
+|                     | stock.market.get_market_concept_min_east()     | 获取同花顺概念行情-当日分时           | 只能获取当天                                                 |
+|                     | stock.market.get_market_concept_current_east() | 获取同花顺当前的概念行情              | 实时行情                                                     |
+| 指数行情            | stock.market.get_market_index()                | 获取指数的行情信息-日、周、月 k线     |                                                              |
+|                     | stock.market.get_market_index_min()            | 获取指数的行情-当日分时               |                                                              |
+|                     | stock.market.get_market_index_current()        | 获取当前的指数行情                    | 实时行情                                                     |
+
+**注：概念和指数从本质来看是一样的，所以相关的接口和返回结果是一致的，概念是各个厂商自定义的指数，指数是官方或者权威机构定义的，都是一揽子股票的组合。**
+
+### （2）基金-ETF
+
+#### 1. 基本信息
+
+| 数据        | API                                      | 说明                     | 备注                                                         |
+| ----------- | ---------------------------------------- | ------------------------ | ------------------------------------------------------------ |
+| ETF（场内） | fund.info.all_etf_exchange_traded_info() | 获取所有A股市场的ETF信息 | 来源：1. [东方财富](http://quote.eastmoney.com/center/gridlist.html#fund_etf) |
+
+#### 2. 行情信息
+
+| 数据    | API                                  | 说明                             | 备注                                     |
+| ------- | ------------------------------------ | -------------------------------- | ---------------------------------------- |
+| ETF行情 | fund.market.get_market_etf()         | 获取ETF的行情信息-日、周、月 k线 | 来源：[同花顺](https://m.10jqka.com.cn/) |
+|         | fund.market.get_market_etf_min()     | 获取ETF的行情-当日分时           |                                          |
+|         | fund.market.get_market_etf_current() | 获取当前的ETF行情                | 实时行情                                 |
+
+### （3）债券-Bond
+
+| 数据           | API                          | 说明                                | 备注                                                   |
+| -------------- | ---------------------------- | ----------------------------------- | ------------------------------------------------------ |
+| 可转债代码     | bond.info.all_convert_code() | 获取所有A股市场的可转换债券代码信息 | 来源：1. [同花顺](http://data.10jqka.com.cn/ipo/bond/) |
+| 其它数据排期中 | TODO                         | 若您有相关资源可以一起参与贡献      |                                                        |
+
+### （4）舆情
+
+| 数据                     | API                                  | 说明                                       | 备注                                                         |
+| ------------------------ | ------------------------------------ | ------------------------------------------ | ------------------------------------------------------------ |
+| 最近一个月的股票解禁列表 | sentiment.stock_lifting_last_month() | 查询最近一个月的股票解禁列表               | 来源：1. [同花顺](http://data.10jqka.com.cn/market/xsjj/)    |
+| 全市场融资融券余额列表   | sentiment.securities_margin()        | 查询全市场融资融券余额列表                 | 来源：1. [东方财富](https://data.eastmoney.com/rzrq/)        |
+| **北向资金-行情**        |                                      |                                            |                                                              |
+|                          | sentiment.north.north_flow_current() | 获取北向资金（沪深港通）当前流入资金的行情 | 来源：1.[东方财富](https://data.eastmoney.com/hsgt/index.html) |
+|                          | sentiment.north.north_flow_min()     | 获取北向资金分时行情                       |                                                              |
+|                          | sentiment.north.north_flow()         | 获取北向资金历史流入行情                   |                                                              |
+| 其它数据排期中           | TODO                                 | 若您有相关资源可以一起参与贡献             |                                                              |
+
+## 三、[数据源](https://adata.30006124.xyz/dataSource.html)
+
+| 数据源     | 板块                                                         | 描述             |
+| ---------- | ------------------------------------------------------------ | ---------------- |
+| 同花顺     | [数据中心](http://data.10jqka.com.cn/)，[行情中心](http://q.10jqka.com.cn/)，[问财](http://www.iwencai.com/unifiedwap/home/index) | 让投资变的更简单 |
+| 百度股市通 | [股市通](https://gushitong.baidu.com/)                       | 科技让投资更简单 |
+| 东方财富   | [数据中心](https://data.eastmoney.com/center/)，[行情中心](http://quote.eastmoney.com/center/) | 财经门户         |
+| 腾讯理财   | [行情中心](https://stockapp.finance.qq.com/mstats/#)         |                  |
+| 新浪财经   | [新浪财经](https://finance.sina.com.cn/stock/)               | 门户网站         |
+
+***--------------------------------------------感谢各位大厂提供的数据----------------------------------------------***
+
+## 四、 其它参考
+
+主要记录查阅过的项目和相关平台，并对此项目产生了深远印象，特此鸣谢。
+
+| [akshare](https://gitee.com/mirrors/akshare) | [聚宽量化](https://www.joinquant.com/) | [baostock](http://baostock.com/baostock/index.php/Python%E5%BC%80%E5%8F%91%E8%B5%84%E6%BA%90) | [MyData](http://api.mairui.club/hsdata.html) |
+| -------------------------------------------- | -------------------------------------- | ------------------------------------------------------------ | -------------------------------------------- |
+
+## 五、发布计划
+
+|      | 版本号 | 内容 | 发布日期     | 备注                           |
+| ---- | ------ | ---- | ------------ | ------------------------------ |
+| ✅    | 0.x.x  | 股票 | 2023-04-05 ~ | 预览版本                       |
+| ✅ ️    | 1.x.x  | 股票 | 2023-10-01   | 中国Ai股                       |
+| ☑️    | 2.x.x  | 基金、债券 | 开发中 | 场内可交易基金：ETF、可转债        |
+| ☑️    | 3.x.x | xxx        | 排期中       |  |
+
+## 六、理念
+
+1. 关于AData，我们只关注交易产生的数据。在A股只有交易数据是真实的，对于量化和AI训练，也只需要关心交易相关的行情数据，做到真正的专注。当然，你可能会说财务数据等也非常有用，但财务数据相对滞后，而且可能ZJ，甚至有XL可能，最终对于普通交易者可能就成了接盘侠。财务数据在我们这里，只做股票池筛选作用，不做实时交易指标推荐。
+
+2. 根据多年的数据治理经验，函数和字典在设计上面，符合标准的数据存储，可根据数据字典建表落地到数据库。
+
+3. 距离15年已过8年，时光匆匆，**抓住底部机会**。
+
+**注：**
+
+- 永久免费开源A股数据库，只有交易相关的数据，专注量化交易。
+- 送给A股的各位朋友一首歌：[谢天笑-向阳花](https://adata.30006124.xyz/向阳花.html)，愿你我向阳而生。
+
+## 参与贡献
+
+1.  Fork 本仓库
+2.  新建 Feat_xxx 分支
+3.  提交代码（注意代码风格和本项目一致即可）
+4.  新建 Pull Request
+
+
+## 特别鸣谢
+
+> 对于项目有支持，包括但不仅限：内容贡献，bug提交，思想交流等等，对项目有影响的个人和机构
+
+| Simon | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https://github.com/LuneZ99) | 匿名用户 | thue | [Triones009](https://github.com/Triones009) | **[adaaaaaa](https://github.com/adaaaaaa)** | **[LeslieWuboy](https://github.com/LeslieWuboy)** |
+| ----- | ------------------------------------------------- | ------------------------------------- | -------- | ---- | ------------------------------------------- | ------------------------------------------- | ------------------------------------------------- |
+|       |                                                   |                                       |          |      |                                             |                                             |                                                   |
+
+----------------------------------------------------------------------
+
+> 
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=1nchaos/adata&type=Date)](https://star-history.com/#1nchaos/adata&Date)
+
+## 欢迎进行交流
+<p align="center">
+  <a href="https://adata.30006124.xyz/" target="_blank">
+    <img width="180" src="./docs/wx.jpg" alt="logo">
+  </a>
+</p>
+
+- 添加wx好友，备注：Adata量化进交流群；
+- 群最近建立，意在提供一个交流的平台，欢迎讨论交流；
+- 一起保卫3000点直到突破6124点。
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
-# [AData](https://adata.1nchaos.com)
+# [AData](https://adata.30006124.xyz)
                                     _[_l_o_g_o_]
 ![GitHub language count](https://img.shields.io/github/languages/count/1nchaos/
 adata)![GitHub top language](https://img.shields.io/github/languages/top/
 1nchaos/adata)[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 adata?color=d)](https://pypi.org/project/adata/)[![Licence](https://
 img.shields.io/hexpm/l/apa?color=d)](https://gitee.com/inchaos/adata/blob/main/
 LICENSE)[![Downloads](https://static.pepy.tech/badge/adata/week)](https://
 pepy.tech/project/adata)![GitHub Repo stars](https://img.shields.io/github/
 stars/1nchaos/adata)![GitHub issues](https://img.shields.io/github/issues/
 1nchaos/adata)![GitHub contributors](https://img.shields.io/github/
 contributors/1nchaos/adata)![GitHub (Pre-)Release Date](https://img.shields.io/
 github/release-date-pre/1nchaos/adata)[![Downloads](https://static.pepy.tech/
 badge/adata)](https://pepy.tech/project/adata)![PyPI - Version](https://
-img.shields.io/pypi/v/adata) ## 0ã[ä»ç»](https://adata.1nchaos.com/
+img.shields.io/pypi/v/adata) ## 0ã[ä»ç»](https://adata.30006124.xyz/
 idea.html) >
 ä¸æ³¨Aè¡ï¼ä¸æ³¨éåï¼åé³èçï¼å¼æ¾ãçº¯åãæç»­ãä¸ºAi
 (ç±)åçµã > >
 ä¸æ³¨è¡ç¥¨è¡ææ°æ®ï¼ä¸ºäºä¿è¯æ°æ®çé«å¯ç¨æ§ï¼éç¨å¤æ°æ®æºèååæ¢ã
 > >
 ç®æ ï¼æ¯æä¸ªäººéåè¡æçéè¦ï¼ä¼äººæ¾æ´ç«ç°é«ï¼æ¬¢è¿å å¥ã
 **å¸åºå¯å·ï¼åç­ä¸æï¼åææ´é¾ï¼å¦æå¸®å©å°ä½ ï¼å³ä¸è§ç¹
 â­Star ä¸é®ä¸è¿ï¼è°¢è°¢æ¯æåæ¶è^_^** ## ä¸ã[å¿«éå¼å§]
-(https://adata.1nchaos.com/quickStart.html) ### ï¼1ï¼å®è£sdk ~~~python #
+(https://adata.30006124.xyz/quickStart.html) ### ï¼1ï¼å®è£sdk ~~~python #
 é¦æ¬¡å®è£ pip install adata # æå®éåæº pip install adata -i http://
 mirrors.aliyun.com/pypi/simple/ # åçº§çæ¬ pip install -U adata #
 æå®éåæº pip install -U adata -i http://mirrors.aliyun.com/pypi/simple/
 ~~~
 **æ³¨ï¼å½åéåå¯è½å­å¨åæ­¥å»¶è¿ï¼å¯ä½¿ç¨å®æ¹éåæºï¼ä»¥ä¸æ¯éåæº**
 é¿éäºãæ¨èãï¼http://mirrors.aliyun.com/pypi/simple/
 æ¸åå¤§å­¦ï¼https://pypi.tuna.tsinghua.edu.cn/simple
@@ -44,28 +44,27 @@
 18.19 ... 18.93 000001 2021-01-04 1 2021-01-05 00:00:00 17.99 17.76 ... 18.19
 000001 2021-01-05 2 2021-01-06 00:00:00 17.67 19.15 ... 17.76 000001 2021-01-06
 .. ... ... ... ... ... ... ... 573 2023-05-18 00:00:00 12.57 12.49 ... 12.49
 000001 2023-05-18 574 2023-05-19 00:00:00 12.43 12.34 ... 12.49 000001 2023-05-
 19 575 2023-05-22 00:00:00 12.31 12.38 ... 12.34 000001 2023-05-22 [576 rows :
 x 13 columns] ~~~ #### 3. å¶å®æ°æ®ä½¿ç¨
 è¯·åèä¸é¢æ°æ®åè¡¨åç¸å³å­å¸ææ¡£ï¼æ¾å°å¯¹åºçå½æ°å¹¶æ¥çå¯¹åºçå½æ°æ³¨éï¼è¿è¡æ­£ç¡®ä½¿ç¨ã
-- [æ°æ®å­å¸](https://adata.1nchaos.com/dic/stockInfo.html) #### 4.
+- [æ°æ®å­å¸](https://adata.30006124.xyz/dic/stockInfo.html) #### 4.
 ä»£çè®¾ç½®
 é¡¹ç®æ¯åºäºå¬å¼æ¥å£ï¼å¯è½å­å¨éå¶ç­ï¼å æ­¤å¢å ä»£çè®¾ç½®åè½
 ~~~ import adata #
 è®¾ç½®ä»£ç,ä»£çæ¯å¨å±è®¾ç½®,ä»£çå¤±æåå¯éæ°è®¾ç½®ãåæ°:
 ip,proxy_url adata.proxy(is_proxy=True, ip='60.167.21.27:1133') res_df =
-adata.stock.info.all_code() print(res_df) ~~~ **æ³¨ï¼** - v0.0.027b0
-åä»¥ä¸çæ¬æ¯æï¼ - proxy_url:
+adata.stock.info.all_code() print(res_df) ~~~ **æ³¨ï¼** - proxy_url:
 è·åä»£çIpçé¾æ¥ï¼ipåproxy_urlæ¹å¼éæ©å¶ä¸ï¼ -
 æ¯æ¬¡è¯·æ±è·åä¸æ¬¡ï¼ä¸ºèçipèµæºå»ºè®®ä½¿ç¨èªå»ºçä»£çæ± ã
-## äºã[æ°æ®åè¡¨](https://adata.1nchaos.com/dic/dataList.html)
+## äºã[æ°æ®åè¡¨](https://adata.30006124.xyz/dic/dataList.html)
 æ´çäºææ°çæ¬çæ°æ®åè¡¨åç¸å³ä½¿ç¨Apiï¼è¯¦ç»åå®¹åç¸å³ä½¿ç¨åæ°ï¼è¯·åèæ°æ®å­å¸ææ¡£ã
-- [æ°æ®åè¡¨](https://adata.1nchaos.com/dic/dataList.html) - [æ°æ®å­å¸]
-(https://adata.1nchaos.com/dic/stockInfo.html) ### ï¼1ï¼è¡ç¥¨-Stock #### 1.
+- [æ°æ®åè¡¨](https://adata.30006124.xyz/dic/dataList.html) - [æ°æ®å­å¸]
+(https://adata.30006124.xyz/dic/stockInfo.html) ### ï¼1ï¼è¡ç¥¨-Stock #### 1.
 åºæ¬ä¿¡æ¯ | æ°æ® | API | è¯´æ | å¤æ³¨ | | ---------------- | ----------
 --------------------------- | -------------------------------------- | --------
 ---------------------------------------------------- | | Aè¡ä»£ç  |
 stock.info.all_code() | ææAè¡ä»£ç ä¿¡æ¯ | | | **æ¦å¿µ** | | | | |
 æ¥æºï¼åè±é¡º | | | | | æ¦å¿µä»£ç  | stock.info.all_concept_code_ths() |
 ææAè¡æ¦å¿µä»£ç ä¿¡æ¯ï¼åè±é¡ºï¼ | æ¥æºï¼åè±é¡ºå¬å¼æ°æ® |
 | æ¦å¿µæååè¡¨ | stock.info.concept_constituent_ths() |
@@ -121,24 +120,30 @@
 stock.market.get_market_concept_current_east() |
 è·ååè±é¡ºå½åçæ¦å¿µè¡æ | å®æ¶è¡æ | | ææ°è¡æ |
 stock.market.get_market_index() | è·åææ°çè¡æä¿¡æ¯-æ¥ãå¨ãæ
 kçº¿ | | | | stock.market.get_market_index_min() | è·åææ°çè¡æ-
 å½æ¥åæ¶ | | | | stock.market.get_market_index_current() |
 è·åå½åçææ°è¡æ | å®æ¶è¡æ |
 **æ³¨ï¼æ¦å¿µåææ°ä»æ¬è´¨æ¥çæ¯ä¸æ ·çï¼æä»¥ç¸å³çæ¥å£åè¿åç»ææ¯ä¸è´çï¼æ¦å¿µæ¯åä¸ªååèªå®ä¹çææ°ï¼ææ°æ¯å®æ¹æèæå¨æºæå®ä¹çï¼é½æ¯ä¸æ½å­è¡ç¥¨çç»åã**
-### ï¼2ï¼åºé-ETF | æ°æ® | API | è¯´æ | å¤æ³¨ | | -------------- | ---
-------------------------------------- | ------------------------------ | ------
------------------------------------------------------- | | ETFï¼åºåï¼ |
-fund.info.all_etf_exchange_traded_info() | è·åææAè¡å¸åºçETFä¿¡æ¯ |
-æ¥æºï¼1. [ä¸æ¹è´¢å¯](http://quote.eastmoney.com/center/
-gridlist.html#fund_etf) | | å¶å®æ°æ®ææä¸­ | TODO |
-è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® | | ### ï¼3ï¼åºå¸-Bond |
-æ°æ® | API | è¯´æ | å¤æ³¨ | | -------------- | ---------------------------
-- | ----------------------------------- | -------------------------------------
------------------ | | å¯è½¬åºä»£ç  | bond.info.all_convert_code() |
+### ï¼2ï¼åºé-ETF #### 1. åºæ¬ä¿¡æ¯ | æ°æ® | API | è¯´æ | å¤æ³¨ | |
+----------- | ---------------------------------------- | ----------------------
+-- | ------------------------------------------------------------ | |
+ETFï¼åºåï¼ | fund.info.all_etf_exchange_traded_info() |
+è·åææAè¡å¸åºçETFä¿¡æ¯ | æ¥æºï¼1. [ä¸æ¹è´¢å¯](http://
+quote.eastmoney.com/center/gridlist.html#fund_etf) | #### 2. è¡æä¿¡æ¯ |
+æ°æ® | API | è¯´æ | å¤æ³¨ | | ------- | ----------------------------------
+-- | -------------------------------- | ---------------------------------------
+- | | ETFè¡æ | fund.market.get_market_etf() | è·åETFçè¡æä¿¡æ¯-
+æ¥ãå¨ãæ kçº¿ | æ¥æºï¼[åè±é¡º](https://m.10jqka.com.cn/) | | |
+fund.market.get_market_etf_min() | è·åETFçè¡æ-å½æ¥åæ¶ | | | |
+fund.market.get_market_etf_current() | è·åå½åçETFè¡æ | å®æ¶è¡æ
+| ### ï¼3ï¼åºå¸-Bond | æ°æ® | API | è¯´æ | å¤æ³¨ | | -------------- |
+---------------------------- | ----------------------------------- | ----------
+-------------------------------------------- | | å¯è½¬åºä»£ç  |
+bond.info.all_convert_code() |
 è·åææAè¡å¸åºçå¯è½¬æ¢åºå¸ä»£ç ä¿¡æ¯ | æ¥æºï¼1. [åè±é¡º]
 (http://data.10jqka.com.cn/ipo/bond/) | | å¶å®æ°æ®ææä¸­ | TODO |
 è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® | | ### ï¼4ï¼èæ | æ°æ® |
 API | è¯´æ | å¤æ³¨ | | ------------------------ | --------------------------
 ---------- | ------------------------------------------ | ---------------------
 --------------------------------------- | |
 æè¿ä¸ä¸ªæçè¡ç¥¨è§£ç¦åè¡¨ | sentiment.stock_lifting_last_month() |
@@ -148,17 +153,17 @@
 æ¥æºï¼1. [ä¸æ¹è´¢å¯](https://data.eastmoney.com/rzrq/) | |
 **ååèµé-è¡æ** | | | | | | sentiment.north.north_flow_current() |
 è·åååèµéï¼æ²ªæ·±æ¸¯éï¼å½åæµå¥èµéçè¡æ | æ¥æºï¼1.
 [ä¸æ¹è´¢å¯](https://data.eastmoney.com/hsgt/index.html) | | |
 sentiment.north.north_flow_min() | è·åååèµéåæ¶è¡æ | | | |
 sentiment.north.north_flow() | è·åååèµéåå²æµå¥è¡æ | | |
 å¶å®æ°æ®ææä¸­ | TODO | è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® |
-| ## ä¸ã[æ°æ®æº](https://adata.1nchaos.com/dataSource.html) | æ°æ®æº |
-æ¿å | æè¿° | | ---------- | ----------------------------------------------
--------------- | ---------------- | | åè±é¡º | [æ°æ®ä¸­å¿](http://
+| ## ä¸ã[æ°æ®æº](https://adata.30006124.xyz/dataSource.html) | æ°æ®æº
+| æ¿å | æè¿° | | ---------- | --------------------------------------------
+---------------- | ---------------- | | åè±é¡º | [æ°æ®ä¸­å¿](http://
 data.10jqka.com.cn/)ï¼[è¡æä¸­å¿](http://q.10jqka.com.cn/)ï¼[é®è´¢](http:
 //www.iwencai.com/unifiedwap/home/index) | è®©æèµåçæ´ç®å | |
 ç¾åº¦è¡å¸é | [è¡å¸é](https://gushitong.baidu.com/) |
 ç§æè®©æèµæ´ç®å | | ä¸æ¹è´¢å¯ | [æ°æ®ä¸­å¿](https://
 data.eastmoney.com/center/)ï¼[è¡æä¸­å¿](http://quote.eastmoney.com/center/
 ) | è´¢ç»é¨æ· | | è¾è®¯çè´¢ | [è¡æä¸­å¿](https://
 stockapp.finance.qq.com/mstats/#) | | | æ°æµªè´¢ç» | [æ°æµªè´¢ç»](https://
@@ -171,31 +176,37 @@
 Python%E5%BC%80%E5%8F%91%E8%B5%84%E6%BA%90) | [MyData](http://api.mairui.club/
 hsdata.html) | | -------------------------------------------- | ---------------
 ----------------------- | -----------------------------------------------------
 ------- | -------------------------------------------- | ## äºãåå¸è®¡å
 | | çæ¬å· | åå®¹ | åå¸æ¥æ | å¤æ³¨ | | ---- | ------ | ---- | -----
 ------- | ------------------------------ | | â | 0.x.x | è¡ç¥¨ | 2023-04-05
 ~ | é¢è§çæ¬ | | â ï¸ | 1.x.x | è¡ç¥¨ | 2023-10-01 | ä¸­å½Aiè¡ | |
-âï¸ | 2.x.x | åºéãåºå¸ | 2024-01-01 |
+âï¸ | 2.x.x | åºéãåºå¸ | å¼åä¸­ |
 åºåå¯äº¤æåºéï¼ETFãå¯è½¬åº | | âï¸ | 3.x.x | xxx | ææä¸­ |
 | ## å­ãçå¿µ 1.
 å³äºADataï¼æä»¬åªå³æ³¨äº¤æäº§ççæ°æ®ãå¨Aè¡åªæäº¤ææ°æ®æ¯çå®çï¼å¯¹äºéååAIè®­ç»ï¼ä¹åªéè¦å³å¿äº¤æç¸å³çè¡ææ°æ®ï¼åå°çæ­£çä¸æ³¨ãå½ç¶ï¼ä½ å¯è½ä¼è¯´è´¢å¡æ°æ®ç­ä¹éå¸¸æç¨ï¼ä½è´¢å¡æ°æ®ç¸å¯¹æ»åï¼èä¸å¯è½ZJï¼çè³æXLå¯è½ï¼æç»å¯¹äºæ®éäº¤æèå¯è½å°±æäºæ¥çä¾ ãè´¢å¡æ°æ®å¨æä»¬è¿éï¼åªåè¡ç¥¨æ± ç­éä½ç¨ï¼ä¸åå®æ¶äº¤æææ æ¨èã
 2.
 æ ¹æ®å¤å¹´çæ°æ®æ²»çç»éªï¼å½æ°åå­å¸å¨è®¾è®¡ä¸é¢ï¼ç¬¦åæ åçæ°æ®å­å¨ï¼å¯æ ¹æ®æ°æ®å­å¸å»ºè¡¨è½å°å°æ°æ®åºã
 3. è·ç¦»15å¹´å·²è¿8å¹´ï¼æ¶åååï¼**æä½åºé¨æºä¼**ã **æ³¨ï¼**
 -
 æ°¸ä¹åè´¹å¼æºAè¡æ°æ®åºï¼åªæäº¤æç¸å³çæ°æ®ï¼ä¸æ³¨éåäº¤æã
 - éç»Aè¡çåä½æåä¸é¦æ­ï¼[è°¢å¤©ç¬-åé³è±](https://
-adata.1nchaos.com/åé³è±.html)ï¼æ¿ä½ æåé³èçã ## åä¸è´¡ç® 1.
-Fork æ¬ä»åº 2. æ°å»º Feat_xxx åæ¯ 3.
+adata.30006124.xyz/åé³è±.html)ï¼æ¿ä½ æåé³èçã ## åä¸è´¡ç®
+1. Fork æ¬ä»åº 2. æ°å»º Feat_xxx åæ¯ 3.
 æäº¤ä»£ç ï¼æ³¨æä»£ç é£æ ¼åæ¬é¡¹ç®ä¸è´å³å¯ï¼ 4. æ°å»º Pull
 Request ## ç¹å«é¸£è°¢ >
 å¯¹äºé¡¹ç®ææ¯æï¼åæ¬ä½ä¸ä»éï¼åå®¹è´¡ç®ï¼bugæäº¤ï¼ææ³äº¤æµç­ç­ï¼å¯¹é¡¹ç®æå½±åçä¸ªäººåæºæ
 | Simon | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https:/
 /github.com/LuneZ99) | å¿åç¨æ· | thue | [Triones009](https://github.com/
-Triones009) | | --------------------------------------------- | ---------------
----------------------------------- | ------------------------------------- | --
------- | ---- | ------------------------------------------- | | [LeslieWuboy]
-(https://github.com/LeslieWuboy) | | | | | | ----------------------------------
------------------------------------- > ## Star History [![Star History Chart]
-(https://api.star-history.com/svg?repos=1nchaos/adata&type=Date)](https://star-
-history.com/#1nchaos/adata&Date)
+Triones009) | **[adaaaaaa](https://github.com/adaaaaaa)** | **[LeslieWuboy]
+(https://github.com/LeslieWuboy)** | | ----- | --------------------------------
+----------------- | ------------------------------------- | -------- | ---- | -
+------------------------------------------ | ----------------------------------
+--------- | ------------------------------------------------- | | | | | | | | |
+| ---------------------------------------------------------------------- > ##
+Star History [![Star History Chart](https://api.star-history.com/
+svg?repos=1nchaos/adata&type=Date)](https://star-history.com/#1nchaos/
+adata&Date) ## æ¬¢è¿è¿è¡äº¤æµ
+                                    _[_l_o_g_o_]
+- æ·»å wxå¥½åï¼å¤æ³¨ï¼Adataéåè¿äº¤æµç¾¤ï¼ -
+ç¾¤æè¿å»ºç«ï¼æå¨æä¾ä¸ä¸ªäº¤æµçå¹³å°ï¼æ¬¢è¿è®¨è®ºäº¤æµï¼ -
+ä¸èµ·ä¿å«3000ç¹ç´å°çªç ´6124ç¹ã
```

### Comparing `adata-1.2.4/adata/__init__.py` & `adata-2.0.0b0/adata/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# -*- coding: utf-8 -*-
-"""
-@desc: adata
-@author: 1nchaos
-@time: 2023/4/4
-"""
-# -*- coding: utf-8 -*-
-
-import logging
-
-from adata.__version__ import __version__
-from adata.bond import bond
-from adata.common.utils.sunrequests import SunProxy
-from adata.fund import fund
-from adata.sentiment import sentiment
-from adata.stock import stock
-
-
-def version():
-    return __version__
-
-
-def proxy(is_proxy=False, ip: str = None, proxy_url: str = None):
-    """
-    设置请求代理
-    :param is_proxy: 是否启用代理，默认：否
-    :param ip: 代理ip地址；格式样例：192.123.123.4:4568
-    :param proxy_url: 能获取到代理的url，返回格式必须和ip一样
-    """
-    SunProxy.set('is_proxy', is_proxy)
-    SunProxy.set('ip', ip)
-    SunProxy.set('proxy_url', proxy_url)
-    return
-
-
-# set up logging
-logger = logging.getLogger("adata")
-
-
-def set_logger():
-    format_string = "%(asctime)s - %(levelname)s - %(message)s"
-    formatter = logging.Formatter(format_string, datefmt="%Y-%m-%dT%H:%M:%S")
-    handler = logging.StreamHandler()
-    handler.setFormatter(formatter)
-
-    logger.addHandler(handler)
-
-
-set_logger()
+# -*- coding: utf-8 -*-
+"""
+@desc: adata
+@author: 1nchaos
+@time: 2023/4/4
+"""
+# -*- coding: utf-8 -*-
+
+import logging
+
+from adata.__version__ import __version__
+from adata.bond import bond
+from adata.common.utils.sunrequests import SunProxy
+from adata.fund import fund
+from adata.sentiment import sentiment
+from adata.stock import stock
+
+
+def version():
+    return __version__
+
+
+def proxy(is_proxy=False, ip: str = None, proxy_url: str = None):
+    """
+    设置请求代理
+    :param is_proxy: 是否启用代理，默认：否
+    :param ip: 代理ip地址；格式样例：192.123.123.4:4568
+    :param proxy_url: 能获取到代理的url，返回格式必须和ip一样
+    """
+    SunProxy.set('is_proxy', is_proxy)
+    SunProxy.set('ip', ip)
+    SunProxy.set('proxy_url', proxy_url)
+    return
+
+
+# set up logging
+logger = logging.getLogger("adata")
+
+
+def set_logger():
+    format_string = "%(asctime)s - %(levelname)s - %(message)s"
+    formatter = logging.Formatter(format_string, datefmt="%Y-%m-%dT%H:%M:%S")
+    handler = logging.StreamHandler()
+    handler.setFormatter(formatter)
+
+    logger.addHandler(handler)
+
+
+set_logger()
```

### Comparing `adata-1.2.4/adata/__version__.py` & `adata-2.0.0b0/adata/__version__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# -*- coding: utf-8 -*-
-
-VERSION = (1, 2, 4)
-PRERELEASE = None  # alpha, beta or rc
-REVISION = None
-
-
-def generate_version(version, prerelease=None, revision=None):
-    version_parts = [".".join(map(str, version))]
-    if prerelease is not None:
-        version_parts.append(f"-{prerelease}")
-    if revision is not None:
-        version_parts.append(f".{revision}")
-    return "".join(version_parts)
-
-
-__title__ = "adata"
-__description__ = "A Data,A Stock,ETF,Bond,Quant,Stock Market,K Line"
-__url__ = "https://github.com/1nchaos/adata"
-__version__ = generate_version(VERSION, prerelease=PRERELEASE, revision=REVISION)
-__author__ = "1nchaos"
-__author_email__ = "9527@1nchaos.com"
-__license__ = "Apache License"
+# -*- coding: utf-8 -*-
+
+VERSION = (2, 0, 0)
+PRERELEASE = 'beta'  # alpha, beta or rc
+REVISION = None
+
+
+def generate_version(version, prerelease=None, revision=None):
+    version_parts = [".".join(map(str, version))]
+    if prerelease is not None:
+        version_parts.append(f"-{prerelease}")
+    if revision is not None:
+        version_parts.append(f".{revision}")
+    return "".join(version_parts)
+
+
+__title__ = "adata"
+__description__ = "A Data,A Stock,ETF,Bond,Quant,Stock Market,K Line"
+__url__ = "https://github.com/1nchaos/adata"
+__version__ = generate_version(VERSION, prerelease=PRERELEASE, revision=REVISION)
+__author__ = "1nchaos"
+__author_email__ = "9527@1nchaos.com"
+__license__ = "Apache License"
```

### Comparing `adata-1.2.4/adata/common/base/base_ths.py` & `adata-2.0.0b0/adata/common/base/base_ths.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-# -*- coding: utf-8 -*-
-"""
-@desc: 同花顺基础类
-@author: 1nchaos
-@time: 2023/6/5
-@log: change log
-"""
-import copy
-import datetime
-import re
-import time
-
-from bs4 import BeautifulSoup
-from py_mini_racer import py_mini_racer
-
-from adata.common import requests
-from adata.common.headers import ths_headers
-from adata.common.utils import cookie
-from adata.common.utils.cookie import get_file_content_ths
-
-
-class BaseThs(object):
-    """同花顺base类"""
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def _get_text(self, api_url, code):
-        """
-        获取同花顺的请求 text
-        :param api_url: url
-        :param code: 代码
-        :return:
-        """
-        headers = copy.deepcopy(ths_headers.text_headers)
-        headers['Host'] = 'd.10jqka.com.cn'
-        headers['Cookie'] = cookie.ths_cookie()
-        text = ''
-        for i in range(2):
-            res = requests.request('get', api_url, headers=headers, proxies={})
-            text = res.text
-            if code in text:
-                break
-            time.sleep(2)
-        return text
-
-    def _get_years_by_start_date(self, start_date):
-        """
-        根据开始时间获取大于开始时间的所有年份的列表
-        例：start_date=2020-10-01 -> years=[2020,2021,2022,2023]
-        :param start_date: 开始时间
-        :return: 年份
-        """
-        years = []
-        if not start_date:
-            years.append('last')
-        else:
-            current_year = datetime.datetime.now().year
-            start_year = datetime.datetime.strptime(start_date, "%Y-%m-%d").year
-            while start_year <= current_year:
-                years.append(start_year - 1)
-                start_year += 1
-            if current_year not in years:
-                years.append(current_year)
-        return years
-
-    def get_wencai_server_time(self):
-        """
-        获取问财服务时间
-        :return: time
-        """
-        url = 'http://www.iwencai.com/unifiedwap/home/index'
-        resp = requests.request(method='get', url=url)
-        resp_text = resp.text
-        soup = BeautifulSoup(resp_text, 'html.parser')
-        js_url = "http:" + soup.find('script')['src']
-        js_resp = requests.request(method='get', url=js_url)
-        js_text = js_resp.text
-        obj = re.compile(r'var TOKEN_SERVER_TIME=(?P<time>.*?);!function')
-        server_time = obj.search(js_text).group('time')
-        return server_time
-
-    def wencai_hexin_v(self, js_path="hexin.js"):
-        """
-        wencai_hexin
-        """
-        js_code = py_mini_racer.MiniRacer()
-        js_content = get_file_content_ths(file_path=js_path)
-        js_content = 'var TOKEN_SERVER_TIME=' + str(self.get_wencai_server_time()) + ";\n" + js_content
-        js_code.eval(js_content)
-        v = js_code.call("rt.updata")
-        return v
-
-
-if __name__ == '__main__':
-    print(BaseThs().wencai_hexin_v())
+# -*- coding: utf-8 -*-
+"""
+@desc: 同花顺基础类
+@author: 1nchaos
+@time: 2023/6/5
+@log: change log
+"""
+import copy
+import datetime
+import re
+import time
+
+from bs4 import BeautifulSoup
+from py_mini_racer import py_mini_racer
+
+from adata.common import requests
+from adata.common.headers import ths_headers
+from adata.common.utils import cookie
+from adata.common.utils.cookie import get_file_content_ths
+
+
+class BaseThs(object):
+    """同花顺base类"""
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def _get_text(self, api_url, code):
+        """
+        获取同花顺的请求 text
+        :param api_url: url
+        :param code: 代码
+        :return:
+        """
+        headers = copy.deepcopy(ths_headers.text_headers)
+        headers['Host'] = 'd.10jqka.com.cn'
+        headers['Cookie'] = cookie.ths_cookie()
+        text = ''
+        for i in range(2):
+            res = requests.request('get', api_url, headers=headers, proxies={})
+            text = res.text
+            if code in text:
+                break
+            time.sleep(2)
+        return text
+
+    def _get_years_by_start_date(self, start_date):
+        """
+        根据开始时间获取大于开始时间的所有年份的列表
+        例：start_date=2020-10-01 -> years=[2020,2021,2022,2023]
+        :param start_date: 开始时间
+        :return: 年份
+        """
+        years = []
+        if not start_date:
+            years.append('last')
+        else:
+            current_year = datetime.datetime.now().year
+            start_year = datetime.datetime.strptime(start_date, "%Y-%m-%d").year
+            while start_year <= current_year:
+                years.append(start_year - 1)
+                start_year += 1
+            if current_year not in years:
+                years.append(current_year)
+        return years
+
+    def get_wencai_server_time(self):
+        """
+        获取问财服务时间
+        :return: time
+        """
+        url = 'http://www.iwencai.com/unifiedwap/home/index'
+        resp = requests.request(method='get', url=url)
+        resp_text = resp.text
+        soup = BeautifulSoup(resp_text, 'html.parser')
+        js_url = "http:" + soup.find('script')['src']
+        js_resp = requests.request(method='get', url=js_url)
+        js_text = js_resp.text
+        obj = re.compile(r'var TOKEN_SERVER_TIME=(?P<time>.*?);!function')
+        server_time = obj.search(js_text).group('time')
+        return server_time
+
+    def wencai_hexin_v(self, js_path="hexin.js"):
+        """
+        wencai_hexin
+        """
+        js_code = py_mini_racer.MiniRacer()
+        js_content = get_file_content_ths(file_path=js_path)
+        js_content = 'var TOKEN_SERVER_TIME=' + str(self.get_wencai_server_time()) + ";\n" + js_content
+        js_code.eval(js_content)
+        v = js_code.call("rt.updata")
+        return v
+
+
+if __name__ == '__main__':
+    print(BaseThs().wencai_hexin_v())
```

### Comparing `adata-1.2.4/adata/common/headers/baidu_headers.py` & `adata-2.0.0b0/adata/common/headers/baidu_headers.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# -*- coding: utf-8 -*-
-"""
-@desc: readme
-@author: 1nchaos
-@time: 2023/3/29
-@log: change log
-"""
-
-json_headers = {
-    'Host': 'finance.pae.baidu.com',
-    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/110.0',
-    'Accept': 'application/vnd.finance-web.v1+json',
-    'Accept-Language': 'zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2',
-    'Accept-Encoding': 'gzip, deflate, br',
-    'Acs-Token': '1680073602136_1680187152773_uZ76rU6tKjd6HavzqUwLS+LsRmCm+fagieEZzD622QiLe/Sfrq5cqVY6phLw7Vm/MGvLdp6eJI1R/Egp6PEB4E6agGNB91g61mfdylADtKBaq4zV4ZC/SOfrjh9TxMb6i6WwY5S1WFg/wPK2fPCoCZMkVSTJ704skNglDoLsPm+9RjCM4PJK68GKE7ZG1p13P5iAMk9ndAJ7HZ3FJAnBQCQeI82Q+fAOAtxrXtGf7eAoblBlgX7OaTJD97PIm9zy1yE37KVyfCngWZNp5VwP3OWGU6jCLeeq2vKpg2hS6TkgbUgqom57ZGSlIezfwQ7vltRiGG3cnpoPSBxrfiEXwz5iulsLGeubIzjOj1yYIBPWVYNBhSn7aM0P/dBq0Ug4cf3xmTvUI/GVMq9PXHGqBss1Px0Yl+hiSc1+vbgz7vQ=',
-    'Origin': 'https://gushitong.baidu.com',
-    'Connection': 'keep-alive',
-    'Referer': 'https://gushitong.baidu.com/',
-    'Cookie': 'BAIDUID=054924A85233268C182D09EC253E676F:SL=0:NR=10:FG=1; BIDUPSID=19DB8A6DEBD5A452CE6A10E90276DE7C; PSTM=1572438578; MCITY=-75%3A; BDUSS=V-UmF5S1pXNVd1Um15S0Y1MXc0S20wZ3FGYzhIVjlUZUFoczVvRlVjUTB1dTVnRVFBQUFBJCQAAAAAAAAAAAEAAADIruQqaV~EwdPjAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAADQtx2A0LcdgS3; __yjs_duid=1_0e624b9d24290650971c8590bcfe96361619270097027; ZFY=KxKVSFoJLIz0l23rNHW:AV1udt6Ern2XM0p4sN7:AJdw8:C; H_PS_PSSID=38185_36546_38409_38470_38439_38468_38289_38380_37931_38382_26350_22157_38282_37881; BDRCVFR[feWj1Vr5u3D]=I67x6TjHwwYf0; delPer=0; PSINO=6; BDORZ=B490B5EBF6F3CD402E515D22BCDA1598; ZD_ENTRY=baidu; __bid_n=184332335315a549634207; FPTOKEN=0G8DZh7ruaz1dUnw7eFAGwkkafhUBvTOkCNkScDsJi6ucyCKBDttk2Tv233PFjFcYDQH/nqo0eEZY9g0psSI5FwqsV/lPlXLoPcGR6EQ3I9iV5fhRVGwx/xKTmJ1O7b09GcBwac2qYSO1tDSfR20KFkYKdZihCdiCAHUPhhniaMVTFa/d2JywSFgXh5ksnMGNkQXY0fS8bKzsP/UTJdtSvg8J8WuYoh7g6EDHeXRVlt5t13dTO8A6DMCNOYlxzGLSDomP/3UOsH+T/4iGsNubZL+y3016UY0ehJa8meg2mAq+wS0DdmsJxYao0qTDaAT/5LfNM4j3LoVRAMUYtOzM/9V4ajJfK7atGKQXFSn+VnANgwuvUvfZGCOdF8oMn4N7Jv6jvQ5XocYTAOb7MZJgOocxgPsL5zDGIcXYmUPAxoPn2/9SsgFLR4mxU+D++F9|c5qXUXOqFRs5f/aOsOlP9AY4If8rgdZFdcLJjdaX0Is=|10|3c9b5f41e931d2d8783fbcce14863165; BAIDU_WISE_UID=wapp_1680175629815_954; arialoadData=false; BCLID=8799370053103418941; BCLID_BFESS=8799370053103418941; BDSFRCVID=A1tOJeC62wVF227f5qXouQCuMHnCdsrTH6aoWSjyl4QjjjGKIQ2REG0Pnf8g0KuMn6bMogKKXgOTHw0F_2uxOjjg8UtVJeC6EG0Ptf8g0f5; BDSFRCVID_BFESS=A1tOJeC62wVF227f5qXouQCuMHnCdsrTH6aoWSjyl4QjjjGKIQ2REG0Pnf8g0KuMn6bMogKKXgOTHw0F_2uxOjjg8UtVJeC6EG0Ptf8g0f5; H_BDCLCKID_SF=JnIOoCIMtID3qnFkKJL_-P4DePLD-URZ5mAqot3C3D_KMnLGKq7o5q_d5tc72fJb-5rnaIQqaM36j4T1jhQ8M4I1yPrIJqj43bRTWJLy5KJvfq6kj45YhP-Uyn7MWh37bbRlMKoaMp78jR093JO4y4Ldj4oxJpOJ5JbMonLafJOKHICweMK; H_BDCLCKID_SF_BFESS=JnIOoCIMtID3qnFkKJL_-P4DePLD-URZ5mAqot3C3D_KMnLGKq7o5q_d5tc72fJb-5rnaIQqaM36j4T1jhQ8M4I1yPrIJqj43bRTWJLy5KJvfq6kj45YhP-Uyn7MWh37bbRlMKoaMp78jR093JO4y4Ldj4oxJpOJ5JbMonLafJOKHICweMK',
-    'Sec-Fetch-Dest': 'empty',
-    'Sec-Fetch-Mode': 'cors',
-    'Sec-Fetch-Site': 'same-site',
-    'TE': 'trailers',
-}
-
-text_headers = {
-    'Host': 'gushitong.baidu.com',
-    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/110.0',
-    'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8',
-    'Accept-Language': 'zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2',
-    'Accept-Encoding': 'gzip, deflate, br',
-    'Connection': 'keep-alive',
-    'Cookie': 'BAIDUID=DC08E09E609EB9778F0574D4518A5507:SL=0:NR=10:FG=1; BIDUPSID=72A958B07427F9F9CB3F63FD8B6C6565; PSTM=1677461180; MCITY=-%3A; BDUSS=toZjl2NTY0NFNwQWVyaUpFREJlSS1NWmVranN5YzdMSXpEcTZkNTRaTjA4amhrSVFBQUFBJCQAAAAAAAAAAAEAAADIruQqaV~EwdPjAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAHRlEWR0ZRFkN0; H_PS_PSSID=38185_36554_38470_38353_38359_38396_38468_38289_36807_38263_37929_38382_26350_38421_38283_37881; BDSFRCVID=5OPOJexroG07v97fK16bU1LKNeKK0PQTDYrEeU9ooveGPK0Vc8uvEG0PtDQMefIb1DMtogKKXgOTHw0F_2uxOjjg8UtVJeC6EG0Ptf8g0M5; H_BDCLCKID_SF=tJPf_CK5JIL3H48k-4QEbbQH-UnLq-jyBgOZ04n-ah02MI5Y04jBynDv3HQrBM69agQN_hcm3UTdsq76Wh35K5tTQP6rLtJHHG74KKJxbn7EKDjHLP5DDbLehUJiBhvMBan7LKJIXKohJh7FM4tW3J0ZyxomtfQxtNRJ0DnjtpChbC_mjT_hjT3BeU5eetjK2CntsJOOaCv-ht5Oy4oWK441DattaljhMm3P5fKhBpvF8nR_06Jk3M04X-o9-hvT-54e2p3FBUQjq66bQft20b0eMeFD0xJaKJRtWb7jWhviep72ybt2QlRX5q79atTMfNTJ-qcH0KQpsIJM5-DWbT8IjHCHtT-tJRkJ_Dvt-5rDHJTg5DTjhPrMyxCjWMT-MTryKKt5JRTCe4To3JblDfAUX4nQBqDfWHnRhlRNB-3iV-OxDUvnyxAZ-pKLQMQxtNRJWbIEtl5THR_x5tnobUPUWMJ9LUvftgcdot5yBbc8eIna5hjkbfJBQttjQn3hfIkj2CKLtK-WbK_wj6t3-t0_qx5Ka43tHD7yWCvdMU7cOR5Jj65ED5-sbx5hBM3kKaID2pvkbUnDSbIC3MA--t4YKGJeQUJ82TAHhDoD5qcHsq0x0h3We-bQypouQb_H0COMahv95h7xO-0xQlPK5JkgMx6MqpQJQeQ-5KQN3KJmfbL9bT3tjjTXjH8JJ60ttR3MB4bH56rjDnCrjfnmXUI82h5y058fbJKf0qkhJJolhqRoX4ovyT8r0JORXRj45GI8Wb7K5l3mOIJK-T7h5xL1Db3J0pou5CcA3DjgB4boepvoW-Jc3MkWD-jdJJQOBKQB0KnGbUQkeq8CQft20b0EeMtjW6LEK5r2SC_XtKDh3j; Hm_lvt_c8bd3584daa59ca83c2ec1247d343576=1679365029; Hm_lpvt_c8bd3584daa59ca83c2ec1247d343576=1680096200; BDORZ=FFFB88E999055A3F8A630C64834BD6D0; ab_sr=1.0.1_OTVlZTQ5MzFhYTMyY2FjZTY5M2NiYTJjMzUwMTVkNTE0OGM1MzUwMWQzZjk4NTNjMmE5NjJiODM3OGI2MzFlNWFlMDZjOTYzNWIxOTE0MmY2MzI4YjM0OGMwNGFmN2NmNzg1MjA1M2E2ODUwYzFlNmI4NThiZmRlNWJiMmU0NDMwOGI0MDY1ZGRiODNjZWM3ZjY0ZDhlM2VmNjIzYTdlOQ==; BA_HECTOR=24akak252l042g848500208u1i28dic1n; delPer=0; PSINO=7; ZFY=a4MO01qoxt3fSy8GE2fVF3isnJZvFcG4BOxTOLYMkmo:C; BDRCVFR[gltLrB7qNCt]=mk3SLVN4HKm',
-    'Upgrade-Insecure-Requests': '1',
-    'Sec-Fetch-Dest': 'document',
-    'Sec-Fetch-Mode': 'navigate',
-    'Sec-Fetch-Site': 'none',
-    'Sec-Fetch-User': '?1',
-}
+# -*- coding: utf-8 -*-
+"""
+@desc: readme
+@author: 1nchaos
+@time: 2023/3/29
+@log: change log
+"""
+
+json_headers = {
+    'Host': 'finance.pae.baidu.com',
+    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/110.0',
+    'Accept': 'application/vnd.finance-web.v1+json',
+    'Accept-Language': 'zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2',
+    'Accept-Encoding': 'gzip, deflate, br',
+    'Acs-Token': '1680073602136_1680187152773_uZ76rU6tKjd6HavzqUwLS+LsRmCm+fagieEZzD622QiLe/Sfrq5cqVY6phLw7Vm/MGvLdp6eJI1R/Egp6PEB4E6agGNB91g61mfdylADtKBaq4zV4ZC/SOfrjh9TxMb6i6WwY5S1WFg/wPK2fPCoCZMkVSTJ704skNglDoLsPm+9RjCM4PJK68GKE7ZG1p13P5iAMk9ndAJ7HZ3FJAnBQCQeI82Q+fAOAtxrXtGf7eAoblBlgX7OaTJD97PIm9zy1yE37KVyfCngWZNp5VwP3OWGU6jCLeeq2vKpg2hS6TkgbUgqom57ZGSlIezfwQ7vltRiGG3cnpoPSBxrfiEXwz5iulsLGeubIzjOj1yYIBPWVYNBhSn7aM0P/dBq0Ug4cf3xmTvUI/GVMq9PXHGqBss1Px0Yl+hiSc1+vbgz7vQ=',
+    'Origin': 'https://gushitong.baidu.com',
+    'Connection': 'keep-alive',
+    'Referer': 'https://gushitong.baidu.com/',
+    'Cookie': 'BAIDUID=054924A85233268C182D09EC253E676F:SL=0:NR=10:FG=1; BIDUPSID=19DB8A6DEBD5A452CE6A10E90276DE7C; PSTM=1572438578; MCITY=-75%3A; BDUSS=V-UmF5S1pXNVd1Um15S0Y1MXc0S20wZ3FGYzhIVjlUZUFoczVvRlVjUTB1dTVnRVFBQUFBJCQAAAAAAAAAAAEAAADIruQqaV~EwdPjAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAADQtx2A0LcdgS3; __yjs_duid=1_0e624b9d24290650971c8590bcfe96361619270097027; ZFY=KxKVSFoJLIz0l23rNHW:AV1udt6Ern2XM0p4sN7:AJdw8:C; H_PS_PSSID=38185_36546_38409_38470_38439_38468_38289_38380_37931_38382_26350_22157_38282_37881; BDRCVFR[feWj1Vr5u3D]=I67x6TjHwwYf0; delPer=0; PSINO=6; BDORZ=B490B5EBF6F3CD402E515D22BCDA1598; ZD_ENTRY=baidu; __bid_n=184332335315a549634207; FPTOKEN=0G8DZh7ruaz1dUnw7eFAGwkkafhUBvTOkCNkScDsJi6ucyCKBDttk2Tv233PFjFcYDQH/nqo0eEZY9g0psSI5FwqsV/lPlXLoPcGR6EQ3I9iV5fhRVGwx/xKTmJ1O7b09GcBwac2qYSO1tDSfR20KFkYKdZihCdiCAHUPhhniaMVTFa/d2JywSFgXh5ksnMGNkQXY0fS8bKzsP/UTJdtSvg8J8WuYoh7g6EDHeXRVlt5t13dTO8A6DMCNOYlxzGLSDomP/3UOsH+T/4iGsNubZL+y3016UY0ehJa8meg2mAq+wS0DdmsJxYao0qTDaAT/5LfNM4j3LoVRAMUYtOzM/9V4ajJfK7atGKQXFSn+VnANgwuvUvfZGCOdF8oMn4N7Jv6jvQ5XocYTAOb7MZJgOocxgPsL5zDGIcXYmUPAxoPn2/9SsgFLR4mxU+D++F9|c5qXUXOqFRs5f/aOsOlP9AY4If8rgdZFdcLJjdaX0Is=|10|3c9b5f41e931d2d8783fbcce14863165; BAIDU_WISE_UID=wapp_1680175629815_954; arialoadData=false; BCLID=8799370053103418941; BCLID_BFESS=8799370053103418941; BDSFRCVID=A1tOJeC62wVF227f5qXouQCuMHnCdsrTH6aoWSjyl4QjjjGKIQ2REG0Pnf8g0KuMn6bMogKKXgOTHw0F_2uxOjjg8UtVJeC6EG0Ptf8g0f5; BDSFRCVID_BFESS=A1tOJeC62wVF227f5qXouQCuMHnCdsrTH6aoWSjyl4QjjjGKIQ2REG0Pnf8g0KuMn6bMogKKXgOTHw0F_2uxOjjg8UtVJeC6EG0Ptf8g0f5; H_BDCLCKID_SF=JnIOoCIMtID3qnFkKJL_-P4DePLD-URZ5mAqot3C3D_KMnLGKq7o5q_d5tc72fJb-5rnaIQqaM36j4T1jhQ8M4I1yPrIJqj43bRTWJLy5KJvfq6kj45YhP-Uyn7MWh37bbRlMKoaMp78jR093JO4y4Ldj4oxJpOJ5JbMonLafJOKHICweMK; H_BDCLCKID_SF_BFESS=JnIOoCIMtID3qnFkKJL_-P4DePLD-URZ5mAqot3C3D_KMnLGKq7o5q_d5tc72fJb-5rnaIQqaM36j4T1jhQ8M4I1yPrIJqj43bRTWJLy5KJvfq6kj45YhP-Uyn7MWh37bbRlMKoaMp78jR093JO4y4Ldj4oxJpOJ5JbMonLafJOKHICweMK',
+    'Sec-Fetch-Dest': 'empty',
+    'Sec-Fetch-Mode': 'cors',
+    'Sec-Fetch-Site': 'same-site',
+    'TE': 'trailers',
+}
+
+text_headers = {
+    'Host': 'gushitong.baidu.com',
+    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/110.0',
+    'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8',
+    'Accept-Language': 'zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2',
+    'Accept-Encoding': 'gzip, deflate, br',
+    'Connection': 'keep-alive',
+    'Cookie': 'BAIDUID=DC08E09E609EB9778F0574D4518A5507:SL=0:NR=10:FG=1; BIDUPSID=72A958B07427F9F9CB3F63FD8B6C6565; PSTM=1677461180; MCITY=-%3A; BDUSS=toZjl2NTY0NFNwQWVyaUpFREJlSS1NWmVranN5YzdMSXpEcTZkNTRaTjA4amhrSVFBQUFBJCQAAAAAAAAAAAEAAADIruQqaV~EwdPjAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAHRlEWR0ZRFkN0; H_PS_PSSID=38185_36554_38470_38353_38359_38396_38468_38289_36807_38263_37929_38382_26350_38421_38283_37881; BDSFRCVID=5OPOJexroG07v97fK16bU1LKNeKK0PQTDYrEeU9ooveGPK0Vc8uvEG0PtDQMefIb1DMtogKKXgOTHw0F_2uxOjjg8UtVJeC6EG0Ptf8g0M5; H_BDCLCKID_SF=tJPf_CK5JIL3H48k-4QEbbQH-UnLq-jyBgOZ04n-ah02MI5Y04jBynDv3HQrBM69agQN_hcm3UTdsq76Wh35K5tTQP6rLtJHHG74KKJxbn7EKDjHLP5DDbLehUJiBhvMBan7LKJIXKohJh7FM4tW3J0ZyxomtfQxtNRJ0DnjtpChbC_mjT_hjT3BeU5eetjK2CntsJOOaCv-ht5Oy4oWK441DattaljhMm3P5fKhBpvF8nR_06Jk3M04X-o9-hvT-54e2p3FBUQjq66bQft20b0eMeFD0xJaKJRtWb7jWhviep72ybt2QlRX5q79atTMfNTJ-qcH0KQpsIJM5-DWbT8IjHCHtT-tJRkJ_Dvt-5rDHJTg5DTjhPrMyxCjWMT-MTryKKt5JRTCe4To3JblDfAUX4nQBqDfWHnRhlRNB-3iV-OxDUvnyxAZ-pKLQMQxtNRJWbIEtl5THR_x5tnobUPUWMJ9LUvftgcdot5yBbc8eIna5hjkbfJBQttjQn3hfIkj2CKLtK-WbK_wj6t3-t0_qx5Ka43tHD7yWCvdMU7cOR5Jj65ED5-sbx5hBM3kKaID2pvkbUnDSbIC3MA--t4YKGJeQUJ82TAHhDoD5qcHsq0x0h3We-bQypouQb_H0COMahv95h7xO-0xQlPK5JkgMx6MqpQJQeQ-5KQN3KJmfbL9bT3tjjTXjH8JJ60ttR3MB4bH56rjDnCrjfnmXUI82h5y058fbJKf0qkhJJolhqRoX4ovyT8r0JORXRj45GI8Wb7K5l3mOIJK-T7h5xL1Db3J0pou5CcA3DjgB4boepvoW-Jc3MkWD-jdJJQOBKQB0KnGbUQkeq8CQft20b0EeMtjW6LEK5r2SC_XtKDh3j; Hm_lvt_c8bd3584daa59ca83c2ec1247d343576=1679365029; Hm_lpvt_c8bd3584daa59ca83c2ec1247d343576=1680096200; BDORZ=FFFB88E999055A3F8A630C64834BD6D0; ab_sr=1.0.1_OTVlZTQ5MzFhYTMyY2FjZTY5M2NiYTJjMzUwMTVkNTE0OGM1MzUwMWQzZjk4NTNjMmE5NjJiODM3OGI2MzFlNWFlMDZjOTYzNWIxOTE0MmY2MzI4YjM0OGMwNGFmN2NmNzg1MjA1M2E2ODUwYzFlNmI4NThiZmRlNWJiMmU0NDMwOGI0MDY1ZGRiODNjZWM3ZjY0ZDhlM2VmNjIzYTdlOQ==; BA_HECTOR=24akak252l042g848500208u1i28dic1n; delPer=0; PSINO=7; ZFY=a4MO01qoxt3fSy8GE2fVF3isnJZvFcG4BOxTOLYMkmo:C; BDRCVFR[gltLrB7qNCt]=mk3SLVN4HKm',
+    'Upgrade-Insecure-Requests': '1',
+    'Sec-Fetch-Dest': 'document',
+    'Sec-Fetch-Mode': 'navigate',
+    'Sec-Fetch-Site': 'none',
+    'Sec-Fetch-User': '?1',
+}
```

### Comparing `adata-1.2.4/adata/common/headers/east_headers.py` & `adata-2.0.0b0/adata/common/headers/east_headers.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# -*- coding: utf-8 -*-
-"""
-@desc: readme
-@author: 1nchaos
-@time: 2023/7/24
-@log: change log
-"""
-json_headers = {
-    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/110.0',
-    'Accept': '*/*',
-    'Content-Type': 'text/plain;charset=UTF-8',
-    'Accept-Language': 'zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2',
-    'Accept-Encoding': 'gzip, deflate, br',
-    'HOST': 'datacenter-web.eastmoney.com',
-    'Connection': 'keep-alive',
-    'Referer': 'https://data.eastmoney.com/rzrq/total.html',
-}
+# -*- coding: utf-8 -*-
+"""
+@desc: readme
+@author: 1nchaos
+@time: 2023/7/24
+@log: change log
+"""
+json_headers = {
+    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/110.0',
+    'Accept': '*/*',
+    'Content-Type': 'text/plain;charset=UTF-8',
+    'Accept-Language': 'zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2',
+    'Accept-Encoding': 'gzip, deflate, br',
+    'HOST': 'datacenter-web.eastmoney.com',
+    'Connection': 'keep-alive',
+    'Referer': 'https://data.eastmoney.com/rzrq/total.html',
+}
```

### Comparing `adata-1.2.4/adata/common/headers/ths_headers.py` & `adata-2.0.0b0/adata/common/headers/ths_headers.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# -*- coding: utf-8 -*-
-"""
-@desc: readme
-@author: 1nchaos
-@time: 2023/3/29
-@log: change log
-"""
-c_headers = {
-    'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
-    'Accept-Encoding': 'gzip, deflate',
-    'Accept-Language': 'zh-CN,zh;q=0.9',
-    'Cache-Control': 'max-age=0',
-    'Connection': 'keep-alive',
-    'Cookie': 'SL_G_WPT_TO=eo; SL_GWPT_Show_Hide_tmp=1; SL_wptGlobTipTmp=1',
-    'Host': 'search.10jqka.com.cn',
-    'Upgrade-Insecure-Requests': '1',
-    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36',
-}
-
-json_headers = {
-    'Host': 'q.10jqka.com.cn',
-    'Referer': 'http://q.10jqka.com.cn/',
-    'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:105.0) Gecko/20100101 Firefox/105.0',
-    'Accept': '*/*',
-    'Accept-Language': 'zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2',
-    'Accept-Encoding': 'gzip, deflate',
-    'Connection': 'keep-alive',
-    'Cookie': 'v=AzCSZkisIBam9fwSniGPJndtB_-HeRW6Nl9qaSqB_nJczN4r0onkU4ZtOEN5; __bid_n=18484da3254140db6d4207; Hm_lvt_78c58f01938e4d85eaf619eae71b4ed1=1680163246; FPTOKEN=E5SR2waOvFusCzMCQVA/i0npfLNEl6RajFMppa8aoQmLTnIl68wGldxUBmPM57Q9yOCUCB1aiKbuSjFdBzV5SnHNhe0uSYQIfJ9t5YdBrYTHtRO06p0Kjf3ck0dxo587GXZ/Lln6kY2EoiWCZBlXHLfwWq6d/uLzQfq+BnkeN8y5zWt6kJAzY84fZaTCNQPf4Vae5qHOYpskzus+szaS5Qm2VNc/Q/t/0U7QQADRzNRLfYf6A/407ZMdD6+1sGvCQhh959iGl+DRavRasWH2ISY3G/osl/olB61tXSIxNI+IL+rAu7u5TvknHHwVtcigMY4jsgE8qBkN2HU4wDvH5QMv+0E89L5jACYIF+BoMaBNN6VkPt9Pksg8+K6O4K9rwElcjiWRuyzNy25YO13lYQ==|sPeLn4kqSDrmYnpF7Wn94V4caIa/qNc5YWTtvQFK+ac=|10|2bc6aba78093d71b50d1b70dd20ef09d; Hm_lpvt_78c58f01938e4d85eaf619eae71b4ed1=1680163469',
-    'Upgrade-Insecure-Requests': '1',
-}
-
-text_headers = {
-    'Host': 'q.10jqka.com.cn',
-    'Referer': 'http://q.10jqka.com.cn/',
-    'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:105.0) Gecko/20100101 Firefox/105.0',
-    'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8',
-    'Accept-Language': 'zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2',
-    'Accept-Encoding': 'gzip, deflate',
-    'Connection': 'keep-alive',
-    'Cookie': 'v=AzCSZkisIBam9fwSniGPJndtB_-HeRW6Nl9qaSqB_nJczN4r0onkU4ZtOEN5; __bid_n=18484da3254140db6d4207; Hm_lvt_78c58f01938e4d85eaf619eae71b4ed1=1680163246; FPTOKEN=E5SR2waOvFusCzMCQVA/i0npfLNEl6RajFMppa8aoQmLTnIl68wGldxUBmPM57Q9yOCUCB1aiKbuSjFdBzV5SnHNhe0uSYQIfJ9t5YdBrYTHtRO06p0Kjf3ck0dxo587GXZ/Lln6kY2EoiWCZBlXHLfwWq6d/uLzQfq+BnkeN8y5zWt6kJAzY84fZaTCNQPf4Vae5qHOYpskzus+szaS5Qm2VNc/Q/t/0U7QQADRzNRLfYf6A/407ZMdD6+1sGvCQhh959iGl+DRavRasWH2ISY3G/osl/olB61tXSIxNI+IL+rAu7u5TvknHHwVtcigMY4jsgE8qBkN2HU4wDvH5QMv+0E89L5jACYIF+BoMaBNN6VkPt9Pksg8+K6O4K9rwElcjiWRuyzNy25YO13lYQ==|sPeLn4kqSDrmYnpF7Wn94V4caIa/qNc5YWTtvQFK+ac=|10|2bc6aba78093d71b50d1b70dd20ef09d; Hm_lpvt_78c58f01938e4d85eaf619eae71b4ed1=1680163469',
-    'Upgrade-Insecure-Requests': '1',
-}
+# -*- coding: utf-8 -*-
+"""
+@desc: readme
+@author: 1nchaos
+@time: 2023/3/29
+@log: change log
+"""
+c_headers = {
+    'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
+    'Accept-Encoding': 'gzip, deflate',
+    'Accept-Language': 'zh-CN,zh;q=0.9',
+    'Cache-Control': 'max-age=0',
+    'Connection': 'keep-alive',
+    'Cookie': 'SL_G_WPT_TO=eo; SL_GWPT_Show_Hide_tmp=1; SL_wptGlobTipTmp=1',
+    'Host': 'search.10jqka.com.cn',
+    'Upgrade-Insecure-Requests': '1',
+    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36',
+}
+
+json_headers = {
+    'Host': 'q.10jqka.com.cn',
+    'Referer': 'http://q.10jqka.com.cn/',
+    'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:105.0) Gecko/20100101 Firefox/105.0',
+    'Accept': '*/*',
+    'Accept-Language': 'zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2',
+    'Accept-Encoding': 'gzip, deflate',
+    'Connection': 'keep-alive',
+    'Cookie': 'v=AzCSZkisIBam9fwSniGPJndtB_-HeRW6Nl9qaSqB_nJczN4r0onkU4ZtOEN5; __bid_n=18484da3254140db6d4207; Hm_lvt_78c58f01938e4d85eaf619eae71b4ed1=1680163246; FPTOKEN=E5SR2waOvFusCzMCQVA/i0npfLNEl6RajFMppa8aoQmLTnIl68wGldxUBmPM57Q9yOCUCB1aiKbuSjFdBzV5SnHNhe0uSYQIfJ9t5YdBrYTHtRO06p0Kjf3ck0dxo587GXZ/Lln6kY2EoiWCZBlXHLfwWq6d/uLzQfq+BnkeN8y5zWt6kJAzY84fZaTCNQPf4Vae5qHOYpskzus+szaS5Qm2VNc/Q/t/0U7QQADRzNRLfYf6A/407ZMdD6+1sGvCQhh959iGl+DRavRasWH2ISY3G/osl/olB61tXSIxNI+IL+rAu7u5TvknHHwVtcigMY4jsgE8qBkN2HU4wDvH5QMv+0E89L5jACYIF+BoMaBNN6VkPt9Pksg8+K6O4K9rwElcjiWRuyzNy25YO13lYQ==|sPeLn4kqSDrmYnpF7Wn94V4caIa/qNc5YWTtvQFK+ac=|10|2bc6aba78093d71b50d1b70dd20ef09d; Hm_lpvt_78c58f01938e4d85eaf619eae71b4ed1=1680163469',
+    'Upgrade-Insecure-Requests': '1',
+}
+
+text_headers = {
+    'Host': 'q.10jqka.com.cn',
+    'Referer': 'http://q.10jqka.com.cn/',
+    'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:105.0) Gecko/20100101 Firefox/105.0',
+    'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8',
+    'Accept-Language': 'zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2',
+    'Accept-Encoding': 'gzip, deflate',
+    'Connection': 'keep-alive',
+    'Cookie': 'v=AzCSZkisIBam9fwSniGPJndtB_-HeRW6Nl9qaSqB_nJczN4r0onkU4ZtOEN5; __bid_n=18484da3254140db6d4207; Hm_lvt_78c58f01938e4d85eaf619eae71b4ed1=1680163246; FPTOKEN=E5SR2waOvFusCzMCQVA/i0npfLNEl6RajFMppa8aoQmLTnIl68wGldxUBmPM57Q9yOCUCB1aiKbuSjFdBzV5SnHNhe0uSYQIfJ9t5YdBrYTHtRO06p0Kjf3ck0dxo587GXZ/Lln6kY2EoiWCZBlXHLfwWq6d/uLzQfq+BnkeN8y5zWt6kJAzY84fZaTCNQPf4Vae5qHOYpskzus+szaS5Qm2VNc/Q/t/0U7QQADRzNRLfYf6A/407ZMdD6+1sGvCQhh959iGl+DRavRasWH2ISY3G/osl/olB61tXSIxNI+IL+rAu7u5TvknHHwVtcigMY4jsgE8qBkN2HU4wDvH5QMv+0E89L5jACYIF+BoMaBNN6VkPt9Pksg8+K6O4K9rwElcjiWRuyzNy25YO13lYQ==|sPeLn4kqSDrmYnpF7Wn94V4caIa/qNc5YWTtvQFK+ac=|10|2bc6aba78093d71b50d1b70dd20ef09d; Hm_lpvt_78c58f01938e4d85eaf619eae71b4ed1=1680163469',
+    'Upgrade-Insecure-Requests': '1',
+}
```

### Comparing `adata-1.2.4/adata/common/js/hexin.js` & `adata-2.0.0b0/adata/common/js/hexin.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,413 +1,413 @@
-var document = {}
-var window = {}
-var duan = ["", 9527, String, Boolean, "eh", "ad", "Bu", "ileds", "1", "\b", Array, "7", "base", "64De", "\u2543\u252b", "etatS", "pa", "e", "FromUrl", "getOrigi", "nFromUrl", "\u255b\u253e", "b?\x18q)", "ic", "k", "sted", "he", "wser", "oNo", "ckw", "ent", "hst", "^And", "RM", "systemL", 5, "\u255f\u0978\u095b\u09f5", "TR8", "!'", "gth", "er", "TP", 83, "r", !0, "v", "v-nixeh", RegExp, "thsi.cn", 'K\x19"]K^xVV', "KXxAPD?\x1b[Y", document, 0, "allow", 1, "; ", "length", "Init", "=", "; domain=", "checkcookie", !1, "eikooCled", "tnemucod", "d", window, "\u2553\u0972\u0959\u09e4\u09bd\u0938\u0980\u09c5\u09b1\u09d1\u09a7\u09dc\u09dd\u09d3\u09c2", "\u2556\u0979\u095e\u09d3\u09b5\u0935\u098f\u09c7\u099d\u09d2\u09b0", 23, "l$P$~", "frames", "ducument", "ydob", "documentElement", "del", "@[\\]^`{|}~]", "base_fileds", "255", 10, "10", 39, "\u2547\u2535\u255a\u252e\u2541\u2535\u254c\u253c\u2559", 8, "4", "3", "de", 3, "11", 2, "203", "22", "111111", "3f", 16, "\x0f", "\u2506\u2537\u2507\u2537", "11111111", "base64Encode", "v\x1d", "ati", "WY", "te", "bo", "rs", "getHost", Date, "{DF", ":", "^{.*}$", "WU<P[C", 52, "1001", "href", "1111101010", "redirect_url", "^\\s*(?:https?:)?\\/{2,}([^\\/\\?\\#\\\\]+)", "i", "\u256c\u252c\u2516\u254b", "@", "ready", "change", "dy", 7, "protocol", "//s.thsi.cn/js/chameleon/time.1", "onerror", "2000", "readyState", null, "^(\\d+\\.)+\\d+$", "^\\s*(?:(https?:))?\\/{2,}([^\\/\\?\\#\\\\]+)", ".", "strToBytes", "isIPAddr", "serverTimeNow", "addEventListener", "th", "wh", "Scro", "mousemove", 55, "evomhcuot", "[[?PVC\x0e", "getMouseMove", '_R"xWB%Po_3YT', "getMouseClick", "ght", "gin", "msD", "ack", "\u2556\u096b\u095f", "Nativ", "^A", "MozSettingsEvent", "safari", "ActiveXObject", "postMessage", "Uint8Array", "WeakMap", "Google Inc.", "vendor", "chrome", "python", "sgAppName", "JX", 6, "me", "LBBROWSER", "w4", "2345Explorer", "TheWorld", "\u2544", 40, "tTr", "\u2506", "navigator", "webdriver", "languages", "taborcA|FDP", "\u2541\u097c\u0949", 95, "1e0", "e Cli", "iso-8859-1", "defaultCharset", "localStorage", "^Win64", "^Linux armv|Android", "^iPhone", "^iPad", "B_{VV", "getPluginNum", "getBrowserFeature", "12", "16", "sE", "10000", "17", "\u2542\u2532\u2556\u2537\u2543\u2526", "\x1cx`R", 2333, "XMLH", "ers", "0", "lo", 57, "ylppa", "error", "target", "click", "unload", "HE9AWT9Y", "\\.", "c?", "$", "/", "fetch", "prototype", "url", "\u2556\u0971\u0956\u09fe\u09a7", "headers", "\u256b\u2554", 79, "?", "^(.*?):[ \\t]*([^\\r\\n]*)\\r?$", "gm", "s", "src", "analysisRst", "\u255e\u0973\u0949\u09f4\u09a2\u0929\u09ac\u09d4\u0992\u09d2\u09b0\u09d4", "appendChild", "Y", "jsonp_ignore", "^", 70, "421", "XH>a", "\u2574\u253c\u257d\u2530\u2575\u2539\u257c\u2533\u257d\u2522\u256e\u2521\u2560\u2524\u2561\u2525", "CHAMELEON_LOADED"]
-var chang = [1, "", 0, "he", "ad", 29, "\x180G\x1f", "?>=<;:\\\\/,+", "ng", "to", "ff", Number, Error, "11", "6", "er", "ro", "code", "co", "_?L", "ed", "@S\x15D*", Object, "len", "gth", "on", "lo", RegExp, "ySta", 13, "eel", "ee", "ouse", "ll", "\u2544\u2530\u2555\u2531", "FCm-", "isTru", "getC", "Pos", "ve", "or", "ae", "^", "On", "Sho", "can", "ont", "roid", "anguage", "\u2502", "ta", "tna", Date, "3", "am", "e", "n+", "f80", "\x1dD", 6, "\u255f\u253a\u2542\u252b\u2545\u2568\u251e", "KCABLLAC_NOELEMAHC", "X-Antispider-Message", 3, ".baidu.", Function, document, !0, "cookie", "; ", "=", 96, "\u255b\u253e\u2550\u2537\u2543\u252b", "\u250c\u252c\u255c\u253d\u2549\u2521\u251c", ";O", "; expires=", "getCookie", "Thu, 01 Jan 1970 00:00:00 GMT", "setCookie", "Z\x18|", "i", "\u255b\u2534\u2557\u2536\u255a\u2509\u257d\u2512\u2560\u2501\u2566\u2503", 52, window, 10, "Init", !1, "set", "v", "eliflmth", '<script>document.w=window<\/script><iframe src="/favicon.icon"></iframe>', "iS.p", "head", "#default#userData", "get", "[!\"#$%&'()*", "g", "^d", "$D", "\u2568\u2537\u2568\u254c\u256a", "]\\P", "___", "le", "th", "prototype", "base_f", 8, "\\R5Z\\R\x14@^Q3G", "ZV%PgQ?Y]S%", 67, "r", "length", "0", 16, "12", "\u2576\u095f\u0979\u09d5\u0995\u091b\u09a9\u09f9\u09bd\u09f7\u0989\u09fd\u09f5\u09f3\u09f9\u0a41\u0a4d\u098f\u0999\u0905\u0975\u09cb\u09a9\u09a9\u099d\u0927\u0933\u0913\u0a6b\u0999\u09a3\u0937\u098b\u09f5\u0933\u0a7b\u091b\u09b1\u0a63\u095f\u09fb\u094d\u0993\u0943\u092b\u0949\u09a3\u09e7\u09cb\u0925\u0993\u09ab\u09f0\u092c\u092c\u0942\u0950\u09c8\u0944\u09c6\u0990\u0944\u09cb\u098e", "i,", "\u2505\u092f", 12, 56, "20", "1000", 2, 5, "11111111", "encode", "\u255b\u0972\u0959", "\u2519", "s", "WY$PYS", "ystate", "1111101000", / /g, ",", "\u250d", '^".*"$', "edoc_sutats", "status_code", "location", "redirect_url", "href", "4294967295", "j", "1200000", "script", "src", "onreadystatechange", "read", "loaded", "readyState", "complete", "interactive", "onload", "undefined", "\\.com\\.cn$|\\.com\\.hk$", ".", "getServerTime", 'YY7YAD?FjD"', "strhash", "random", "getRootDomain", "booleanToDecimal", "timeNow", "\u2559\u253e", "eventBind", "onwh", "\u255b", 46, "DOMM", "cl", "T^5^", "div", "onmousewheel", "mousewheel", 51, "keydown", "clientY", "getKeyDown", "ch", "plu", "\u2543\u252b", "ouc", "art", "^i", "Po", "callPhantom", "max", "Hei", "ActiveXObject", "nd", "yG&Y]\x17\x15ZUG#A]Ez\x15qY5\x1b", "\u2576\u097e\u094e\u09f8\u09a6\u0938\u09b6\u09fe\u0996\u09d7\u09a7\u09d2\u09cc", "Maxthon", "Q", "opr", "chrome", "BIDUBrowser", "QQBro", "[_$ZUR", "UBrowser", "MSGesture", "plugins", "doNotTrack", "ShockwaveFlash.ShockwaveFlash", "]C|\x18", "webgl2", "platform", "name", "^Win32", "^MacIntel", "^Linux [ix]\\d+", "^BlackBerry", "language", "getPlatform", "getBrowserIndex", "1", "10", 4, 9, "1100", "\t\0", "3c", 256, "w", "TTP", "et", "c", "al", "\u255e", "base", "\u2569\u0975\u094e\u09e5\u09a0\u092e\u09d1\u09ed\u09ce", "target", "fh%PTQr", "#", "\u255f\u097c\u0949\u09f9", 97, "rg", "tnemelEcrs", "fn_Ws", "parentNode", "tagName", "A", "submit", "PX%", "me", "host", "\\.?", "d\x19", "Fri, 01 Feb 2050 00:00:00 GMT", "]E%", "toString", "[object Request]", "headers", 83, "&", encodeURIComponent, "open", "getAllResponseHeaders", "4", "tseuqeRpttHLMX", "Window", "\u2564\u095e", "RI", "\u2550\u0953", "(YaZ", "_", "_str", "V587"];
-
-var r, e, a, n;
-r = e = a = n = duan;
-var u, c, s, t;
-u = c = s = t = chang;
-var Zn = {};
-var rt;
-var f = c[3],
-    l = s[4],
-    d = a[5],
-    h = '+,/\\\\:;<=>?',
-    g = c[8],
-    w = c[9],
-    m = r[6],
-    I = u[10],
-    y = a[7],
-    _ = (s[11],
-        c[12],
-        s[13]),
-    C = e[8],
-    E = u[14],
-    A = '0',
-    b = a[11],
-    T = u[15],
-    B = c[16],
-    R = r[12],
-    k = r[13],
-    S = s[17],
-    P = u[18],
-    D = s[23],
-    x = s[24],
-    N = u[25],
-    L = u[26],
-    F = u[28],
-    Y = r[16],
-    j = a[17],
-    H = e[18],
-    $ = e[19],
-    U = r[20],
-    X = s[30],
-    G = s[31],
-    K = s[32],
-    Q = s[33],
-    Z = r[23],
-    q = r[24],
-    J = u[36],
-    nn = a[25],
-    tn = s[37],
-    rn = c[38],
-    en = r[26],
-    an = c[39],
-    on = s[40],
-    un = a[27],
-    cn = u[41],
-    vn = r[28],
-    fn = u[8],
-    ln = s[44],
-    pn = a[29],
-    dn = s[45],
-    hn = a[30],
-    gn = c[46],
-    wn = a[31],
-    mn = a[32],
-    In = s[47],
-    yn = r[33],
-    _n = a[34],
-    Cn = c[48],
-    En = a[8],
-    An = '5',
-    bn = c[50],
-    Tn = c[51],
-    kn = e[39],
-    Sn = u[53],
-    Pn = r[40],
-    Mn = s[54],
-    On = s[55],
-    xn = r[43],
-    Nn = u[57],
-    Ln = e[44];
-! function(n) {
-    var t = u[80],
-        o = 'localStorage',
-        i = s[67],
-        f, l = u[83]['document'],
-        p, d;
-
-    function g(n) {
-        var t = j;
-        return t = dn,
-            i ? y(n) : f ? w(n) : void u[2]
-    }
-
-    function w(n) {
-        E(function() {
-            return n = R(n),
-                f.getAttribute(n)
-        })()
-    }
-
-    function m() {
-        try {
-            return !!(o in s[83] && s[83][o])
-        } catch (n) {
-            return void u[2]
-        }
-    }
-
-    function I(n) {
-        try {
-            f.removeItem(n)
-        } catch (t) {}
-    }
-    n[c[85]] = C;
-
-    function y(n) {
-        try {
-            return f.getItem(n)
-        } catch (t) {
-            return u[86]
-        }
-    }
-    n[c[87]] = B;
-
-    function _(n, t) {
-        try {
-            f.setItem(n, t)
-        } catch (r) {}
-    }
-
-    function C() {
-        var n = e[64],
-            r = u[88];
-        if (i = m(),
-            i)
-            f = a[65][o];
-        else if (l[at(e[66])][at(e[67], a[68])])
-            try {
-                p = new ActiveXObject(Wn(a[69], s[89], l)),
-                    p.open(),
-                    p.write(s[90]),
-                    p.close(),
-                    d = p.w[e[70]][s[2]][e[71]],
-                    f = d.createElement(n + t + r)
-            } catch (c) {
-                f = l.createElement(o),
-                    d = l[Wn(u[91], a[72])] || l.getElementsByTagName(s[92])[s[2]] || l[a[73]]
-            }
-    }
-
-    function E(n) {
-        return function() {
-            d.appendChild(f),
-                f.addBehavior(s[93]),
-                f.load(o);
-            var t = n();
-            return d.removeChild(f),
-                t
-        }
-    }
-    n[c[94]] = g;
-
-    function A(n) {
-        var t, r, e;
-        if (t = r = e = a,
-            i)
-            I(n);
-        else {
-            if (!f)
-                return void e[52];
-            b(n)
-        }
-    }
-
-    function b(n) {
-        E(function() {
-            n = R(n),
-                f.removeAttribute(n),
-                f.save(o)
-        })()
-    }
-
-    function T(n, t) {
-        E(function() {
-            n = R(n),
-                f.setAttribute(n, t),
-                f.save(o)
-        })()
-    }
-    n[a[74]] = A;
-
-    function B(n, t) {
-        if (void 0 === t)
-            return A(n);
-        if (i)
-            _(n, t);
-        else {
-            if (!f)
-                return void u[2];
-            T(n, t)
-        }
-    }
-
-    function R(n) {
-        var t = s[95],
-            e = r[75],
-            a = new r[47](t + h + e, c[96]);
-        return n.replace(new c[27](u[97]), v(s[98], s[99], s[100])).replace(a, c[101])
-    }
-}(Zn);
-var qn = function() {
-    var n, t, r;
-    n = t = r = a;
-    var e, o, i;
-    e = o = i = s;
-    var u = o[15],
-        c = o[102],
-        f = e[103];
-
-    function l(r) {
-        var a = o[102],
-            i = e[103];
-        this[n[76]] = r;
-        for (var u = t[52], c = r[a + g + i]; u < c; u++)
-            this[u] = t[52]
-    }
-    return l[e[104]][w + m + I + u] = function() {
-            for (var a = e[105], u = this[a + y], c = [], s = -e[0], v = o[2], f = u[r[56]]; v < f; v++)
-                for (var l = this[v], p = u[v], d = s += p; c[d] = l & parseInt(t[77], n[78]),
-                    --p != r[52];)
-                    --d,
-                    l >>= parseInt(n[79], i[106]);
-            return c
-        },
-        l['prototype']['decodeBuffer'] = function(n) {
-            for (var r = e[8], a = this[ot(e[108], e[109])], o = t[52], u = e[2], s = a[c + r + f]; u < s; u++) {
-                var v = a[u],
-                    l = i[2];
-                do {
-                    l = (l << t[82]) + n[o++]
-                } while (--v > t[52]);
-                this[u] = l >>> i[2]
-            }
-        },
-        l
-}()
-var zn;
-
-function at() {
-    var n, t, r;
-    n = t = r = u;
-    var a, o, i;
-    a = o = i = e;
-    var c = arguments[o[52]];
-    if (!c)
-        return t[1];
-    for (var s = o[0], v = o[1], f = a[52]; f < c.length; f++) {
-        var l = c.charCodeAt(f),
-            p = l ^ v;
-        v = v * f % n[222] + o[200],
-            s += i[2].fromCharCode(p)
-    }
-    return s
-}! function(n) {
-    var t = s[13],
-        o = c[53],
-        i = r[83],
-        f = r[84],
-        l = s[110],
-        d = r[85],
-        h = r[86];
-
-    function g(n, a, o, i, u) {
-        for (var c = s[13], v = r[87], f = n[s[111]]; a < f;)
-            o[i++] = n[a++] ^ u & parseInt(c + v + t + _, r[88]),
-            u = ~(u * parseInt(e[89], e[82]))
-    }
-
-    function w(n) {
-        for (var t = c[112], i = r[52], v = n[s[111]], f = []; i < v;) {
-            var l = n[i++] << parseInt(C + t, c[113]) | n[i++] << e[82] | n[i++];
-            f.push(m.charAt(l >> parseInt(e[90], e[82])), m.charAt(l >> parseInt(s[114], e[78]) & parseInt(a[91], r[88])), m.charAt(l >> u[59] & parseInt(E + o, a[78])), m.charAt(l & parseInt(a[92], u[113])))
-        }
-        return f.join(e[0])
-    }
-    for (var m = at(u[115], s[116]), I = {}, y = u[2]; y < parseInt(i + A, e[93]); y++)
-        I[m.charAt(y)] = y;
-
-    function O(n) {
-        var t, r, e;
-        t = r = e = s;
-        var o, i, u;
-        o = i = u = a;
-        for (var c = ot(i[94]), l = e[2], p = n[o[56]], d = []; l < p;) {
-            var h = I[n.charAt(l++)] << parseInt(at(t[117]), u[82]) | I[n.charAt(l++)] << parseInt(v(t[118], u[95], e[119]), o[88]) | I[n.charAt(l++)] << t[59] | I[n.charAt(l++)];
-            d.push(h >> parseInt(e[120], t[106]), h >> parseInt(t[121], r[122]) & parseInt(f + b + c, t[106]), h & parseInt(o[96], u[88]))
-        }
-        return d
-    }
-
-    function D(n) {
-        var t = O(n);
-        if (rn,
-            p,
-            t[r[52]] != h)
-            return error = T + B + l,
-                void 0;
-        var a = t[c[0]],
-            o = [];
-        return g(t, +parseInt(e[79], c[122]), o, +u[2], a),
-            x(o) == a ? o : void 0
-    }
-
-    function x(n) {
-        for (var e = c[2], i = a[52], u = n[c[111]]; i < u; i++)
-            e = (e << s[123]) - e + n[i];
-        return e & parseInt(s[124], r[88])
-    }
-
-    function N(n) {
-        var r = x(n),
-            e = [h, r];
-        return g(n, +a[52], e, +a[88], r),
-            w(e)
-    }
-    n[e[97]] = w,
-        n[R + k + S] = O,
-        n[u[125]] = N,
-        n[d + P + "de"] = D
-}(zn || (zn = {})) ! function(n) {
-    var t = e[87],
-        o = a[8],
-        i = e[8],
-        f = s[215],
-        l = r[52],
-        p = s[0],
-        d = parseInt(c[216], u[122]),
-        h = e[86],
-        g = u[217],
-        w = u[123],
-        m = e[165],
-        I = parseInt(t + En, c[122]),
-        y = parseInt(a[79], a[82]),
-        _ = c[218],
-        C = parseInt(a[193], e[82]),
-        E = parseInt(o + i, r[78]),
-        A = parseInt(u[219], s[122]),
-        b = parseInt(f + An, s[106]),
-        T = parseInt(r[194], s[106]),
-        B = parseInt(8),
-        R = parseInt(e[196], u[122]),
-        k = parseInt(e[197], a[78]),
-        S;
-
-    function P() {
-        var n = s[0],
-            t = r[88],
-            e = parseInt(u[13], c[122]),
-            a = s[217];
-        S = new qn([a, a, a, a, n, n, n, e, t, t, t, t, t, t, t, a, t, n]),
-            S[p] = parseInt(TOKEN_SERVER_TIME),
-            M(),
-            S[B] = 0,
-            S[k] = 3,
-            S[R] = 0,
-            S[h] = 505497997,
-            S[b] = 3812,
-            S[g] = 1,
-            S[w] = 10,
-            S[m] = 5
-    }
-
-    function M() {
-        S[l] = Math.random() * parseInt("4294967295", 10) >>> 0
-    }
-
-    function O() {
-        S[R]++,
-            S[p] = parseInt(TOKEN_SERVER_TIME),
-            S[d] = timeNow(),
-            S[B] = 0,
-            S[I] = 0,
-            S[y] = 0,
-            S[_] = 0,
-            S[C] = 0,
-            S[E] = 0,
-            S[A] = 0;
-        var n = S.toBuffer();
-        console.log(zn.encode(n))
-        return zn.encode(n)
-    }
-    P();
-
-    function D() {
-        return O()
-    }
-    n.updata = D
-}(rt || (rt = {}));
-
-function timeNow() {
-    var n = new e[105];
-    try {
-        return time = s[52].now(),
-            time / parseInt(c[131], a[88]) >>> c[2]
-    } catch (t) {
-        return time = n.getTime(),
-            time / parseInt(s[121], s[84]) >>> r[52]
-    }
-}
+var document = {}
+var window = {}
+var duan = ["", 9527, String, Boolean, "eh", "ad", "Bu", "ileds", "1", "\b", Array, "7", "base", "64De", "\u2543\u252b", "etatS", "pa", "e", "FromUrl", "getOrigi", "nFromUrl", "\u255b\u253e", "b?\x18q)", "ic", "k", "sted", "he", "wser", "oNo", "ckw", "ent", "hst", "^And", "RM", "systemL", 5, "\u255f\u0978\u095b\u09f5", "TR8", "!'", "gth", "er", "TP", 83, "r", !0, "v", "v-nixeh", RegExp, "thsi.cn", 'K\x19"]K^xVV', "KXxAPD?\x1b[Y", document, 0, "allow", 1, "; ", "length", "Init", "=", "; domain=", "checkcookie", !1, "eikooCled", "tnemucod", "d", window, "\u2553\u0972\u0959\u09e4\u09bd\u0938\u0980\u09c5\u09b1\u09d1\u09a7\u09dc\u09dd\u09d3\u09c2", "\u2556\u0979\u095e\u09d3\u09b5\u0935\u098f\u09c7\u099d\u09d2\u09b0", 23, "l$P$~", "frames", "ducument", "ydob", "documentElement", "del", "@[\\]^`{|}~]", "base_fileds", "255", 10, "10", 39, "\u2547\u2535\u255a\u252e\u2541\u2535\u254c\u253c\u2559", 8, "4", "3", "de", 3, "11", 2, "203", "22", "111111", "3f", 16, "\x0f", "\u2506\u2537\u2507\u2537", "11111111", "base64Encode", "v\x1d", "ati", "WY", "te", "bo", "rs", "getHost", Date, "{DF", ":", "^{.*}$", "WU<P[C", 52, "1001", "href", "1111101010", "redirect_url", "^\\s*(?:https?:)?\\/{2,}([^\\/\\?\\#\\\\]+)", "i", "\u256c\u252c\u2516\u254b", "@", "ready", "change", "dy", 7, "protocol", "//s.thsi.cn/js/chameleon/time.1", "onerror", "2000", "readyState", null, "^(\\d+\\.)+\\d+$", "^\\s*(?:(https?:))?\\/{2,}([^\\/\\?\\#\\\\]+)", ".", "strToBytes", "isIPAddr", "serverTimeNow", "addEventListener", "th", "wh", "Scro", "mousemove", 55, "evomhcuot", "[[?PVC\x0e", "getMouseMove", '_R"xWB%Po_3YT', "getMouseClick", "ght", "gin", "msD", "ack", "\u2556\u096b\u095f", "Nativ", "^A", "MozSettingsEvent", "safari", "ActiveXObject", "postMessage", "Uint8Array", "WeakMap", "Google Inc.", "vendor", "chrome", "python", "sgAppName", "JX", 6, "me", "LBBROWSER", "w4", "2345Explorer", "TheWorld", "\u2544", 40, "tTr", "\u2506", "navigator", "webdriver", "languages", "taborcA|FDP", "\u2541\u097c\u0949", 95, "1e0", "e Cli", "iso-8859-1", "defaultCharset", "localStorage", "^Win64", "^Linux armv|Android", "^iPhone", "^iPad", "B_{VV", "getPluginNum", "getBrowserFeature", "12", "16", "sE", "10000", "17", "\u2542\u2532\u2556\u2537\u2543\u2526", "\x1cx`R", 2333, "XMLH", "ers", "0", "lo", 57, "ylppa", "error", "target", "click", "unload", "HE9AWT9Y", "\\.", "c?", "$", "/", "fetch", "prototype", "url", "\u2556\u0971\u0956\u09fe\u09a7", "headers", "\u256b\u2554", 79, "?", "^(.*?):[ \\t]*([^\\r\\n]*)\\r?$", "gm", "s", "src", "analysisRst", "\u255e\u0973\u0949\u09f4\u09a2\u0929\u09ac\u09d4\u0992\u09d2\u09b0\u09d4", "appendChild", "Y", "jsonp_ignore", "^", 70, "421", "XH>a", "\u2574\u253c\u257d\u2530\u2575\u2539\u257c\u2533\u257d\u2522\u256e\u2521\u2560\u2524\u2561\u2525", "CHAMELEON_LOADED"]
+var chang = [1, "", 0, "he", "ad", 29, "\x180G\x1f", "?>=<;:\\\\/,+", "ng", "to", "ff", Number, Error, "11", "6", "er", "ro", "code", "co", "_?L", "ed", "@S\x15D*", Object, "len", "gth", "on", "lo", RegExp, "ySta", 13, "eel", "ee", "ouse", "ll", "\u2544\u2530\u2555\u2531", "FCm-", "isTru", "getC", "Pos", "ve", "or", "ae", "^", "On", "Sho", "can", "ont", "roid", "anguage", "\u2502", "ta", "tna", Date, "3", "am", "e", "n+", "f80", "\x1dD", 6, "\u255f\u253a\u2542\u252b\u2545\u2568\u251e", "KCABLLAC_NOELEMAHC", "X-Antispider-Message", 3, ".baidu.", Function, document, !0, "cookie", "; ", "=", 96, "\u255b\u253e\u2550\u2537\u2543\u252b", "\u250c\u252c\u255c\u253d\u2549\u2521\u251c", ";O", "; expires=", "getCookie", "Thu, 01 Jan 1970 00:00:00 GMT", "setCookie", "Z\x18|", "i", "\u255b\u2534\u2557\u2536\u255a\u2509\u257d\u2512\u2560\u2501\u2566\u2503", 52, window, 10, "Init", !1, "set", "v", "eliflmth", '<script>document.w=window<\/script><iframe src="/favicon.icon"></iframe>', "iS.p", "head", "#default#userData", "get", "[!\"#$%&'()*", "g", "^d", "$D", "\u2568\u2537\u2568\u254c\u256a", "]\\P", "___", "le", "th", "prototype", "base_f", 8, "\\R5Z\\R\x14@^Q3G", "ZV%PgQ?Y]S%", 67, "r", "length", "0", 16, "12", "\u2576\u095f\u0979\u09d5\u0995\u091b\u09a9\u09f9\u09bd\u09f7\u0989\u09fd\u09f5\u09f3\u09f9\u0a41\u0a4d\u098f\u0999\u0905\u0975\u09cb\u09a9\u09a9\u099d\u0927\u0933\u0913\u0a6b\u0999\u09a3\u0937\u098b\u09f5\u0933\u0a7b\u091b\u09b1\u0a63\u095f\u09fb\u094d\u0993\u0943\u092b\u0949\u09a3\u09e7\u09cb\u0925\u0993\u09ab\u09f0\u092c\u092c\u0942\u0950\u09c8\u0944\u09c6\u0990\u0944\u09cb\u098e", "i,", "\u2505\u092f", 12, 56, "20", "1000", 2, 5, "11111111", "encode", "\u255b\u0972\u0959", "\u2519", "s", "WY$PYS", "ystate", "1111101000", / /g, ",", "\u250d", '^".*"$', "edoc_sutats", "status_code", "location", "redirect_url", "href", "4294967295", "j", "1200000", "script", "src", "onreadystatechange", "read", "loaded", "readyState", "complete", "interactive", "onload", "undefined", "\\.com\\.cn$|\\.com\\.hk$", ".", "getServerTime", 'YY7YAD?FjD"', "strhash", "random", "getRootDomain", "booleanToDecimal", "timeNow", "\u2559\u253e", "eventBind", "onwh", "\u255b", 46, "DOMM", "cl", "T^5^", "div", "onmousewheel", "mousewheel", 51, "keydown", "clientY", "getKeyDown", "ch", "plu", "\u2543\u252b", "ouc", "art", "^i", "Po", "callPhantom", "max", "Hei", "ActiveXObject", "nd", "yG&Y]\x17\x15ZUG#A]Ez\x15qY5\x1b", "\u2576\u097e\u094e\u09f8\u09a6\u0938\u09b6\u09fe\u0996\u09d7\u09a7\u09d2\u09cc", "Maxthon", "Q", "opr", "chrome", "BIDUBrowser", "QQBro", "[_$ZUR", "UBrowser", "MSGesture", "plugins", "doNotTrack", "ShockwaveFlash.ShockwaveFlash", "]C|\x18", "webgl2", "platform", "name", "^Win32", "^MacIntel", "^Linux [ix]\\d+", "^BlackBerry", "language", "getPlatform", "getBrowserIndex", "1", "10", 4, 9, "1100", "\t\0", "3c", 256, "w", "TTP", "et", "c", "al", "\u255e", "base", "\u2569\u0975\u094e\u09e5\u09a0\u092e\u09d1\u09ed\u09ce", "target", "fh%PTQr", "#", "\u255f\u097c\u0949\u09f9", 97, "rg", "tnemelEcrs", "fn_Ws", "parentNode", "tagName", "A", "submit", "PX%", "me", "host", "\\.?", "d\x19", "Fri, 01 Feb 2050 00:00:00 GMT", "]E%", "toString", "[object Request]", "headers", 83, "&", encodeURIComponent, "open", "getAllResponseHeaders", "4", "tseuqeRpttHLMX", "Window", "\u2564\u095e", "RI", "\u2550\u0953", "(YaZ", "_", "_str", "V587"];
+
+var r, e, a, n;
+r = e = a = n = duan;
+var u, c, s, t;
+u = c = s = t = chang;
+var Zn = {};
+var rt;
+var f = c[3],
+    l = s[4],
+    d = a[5],
+    h = '+,/\\\\:;<=>?',
+    g = c[8],
+    w = c[9],
+    m = r[6],
+    I = u[10],
+    y = a[7],
+    _ = (s[11],
+        c[12],
+        s[13]),
+    C = e[8],
+    E = u[14],
+    A = '0',
+    b = a[11],
+    T = u[15],
+    B = c[16],
+    R = r[12],
+    k = r[13],
+    S = s[17],
+    P = u[18],
+    D = s[23],
+    x = s[24],
+    N = u[25],
+    L = u[26],
+    F = u[28],
+    Y = r[16],
+    j = a[17],
+    H = e[18],
+    $ = e[19],
+    U = r[20],
+    X = s[30],
+    G = s[31],
+    K = s[32],
+    Q = s[33],
+    Z = r[23],
+    q = r[24],
+    J = u[36],
+    nn = a[25],
+    tn = s[37],
+    rn = c[38],
+    en = r[26],
+    an = c[39],
+    on = s[40],
+    un = a[27],
+    cn = u[41],
+    vn = r[28],
+    fn = u[8],
+    ln = s[44],
+    pn = a[29],
+    dn = s[45],
+    hn = a[30],
+    gn = c[46],
+    wn = a[31],
+    mn = a[32],
+    In = s[47],
+    yn = r[33],
+    _n = a[34],
+    Cn = c[48],
+    En = a[8],
+    An = '5',
+    bn = c[50],
+    Tn = c[51],
+    kn = e[39],
+    Sn = u[53],
+    Pn = r[40],
+    Mn = s[54],
+    On = s[55],
+    xn = r[43],
+    Nn = u[57],
+    Ln = e[44];
+! function(n) {
+    var t = u[80],
+        o = 'localStorage',
+        i = s[67],
+        f, l = u[83]['document'],
+        p, d;
+
+    function g(n) {
+        var t = j;
+        return t = dn,
+            i ? y(n) : f ? w(n) : void u[2]
+    }
+
+    function w(n) {
+        E(function() {
+            return n = R(n),
+                f.getAttribute(n)
+        })()
+    }
+
+    function m() {
+        try {
+            return !!(o in s[83] && s[83][o])
+        } catch (n) {
+            return void u[2]
+        }
+    }
+
+    function I(n) {
+        try {
+            f.removeItem(n)
+        } catch (t) {}
+    }
+    n[c[85]] = C;
+
+    function y(n) {
+        try {
+            return f.getItem(n)
+        } catch (t) {
+            return u[86]
+        }
+    }
+    n[c[87]] = B;
+
+    function _(n, t) {
+        try {
+            f.setItem(n, t)
+        } catch (r) {}
+    }
+
+    function C() {
+        var n = e[64],
+            r = u[88];
+        if (i = m(),
+            i)
+            f = a[65][o];
+        else if (l[at(e[66])][at(e[67], a[68])])
+            try {
+                p = new ActiveXObject(Wn(a[69], s[89], l)),
+                    p.open(),
+                    p.write(s[90]),
+                    p.close(),
+                    d = p.w[e[70]][s[2]][e[71]],
+                    f = d.createElement(n + t + r)
+            } catch (c) {
+                f = l.createElement(o),
+                    d = l[Wn(u[91], a[72])] || l.getElementsByTagName(s[92])[s[2]] || l[a[73]]
+            }
+    }
+
+    function E(n) {
+        return function() {
+            d.appendChild(f),
+                f.addBehavior(s[93]),
+                f.load(o);
+            var t = n();
+            return d.removeChild(f),
+                t
+        }
+    }
+    n[c[94]] = g;
+
+    function A(n) {
+        var t, r, e;
+        if (t = r = e = a,
+            i)
+            I(n);
+        else {
+            if (!f)
+                return void e[52];
+            b(n)
+        }
+    }
+
+    function b(n) {
+        E(function() {
+            n = R(n),
+                f.removeAttribute(n),
+                f.save(o)
+        })()
+    }
+
+    function T(n, t) {
+        E(function() {
+            n = R(n),
+                f.setAttribute(n, t),
+                f.save(o)
+        })()
+    }
+    n[a[74]] = A;
+
+    function B(n, t) {
+        if (void 0 === t)
+            return A(n);
+        if (i)
+            _(n, t);
+        else {
+            if (!f)
+                return void u[2];
+            T(n, t)
+        }
+    }
+
+    function R(n) {
+        var t = s[95],
+            e = r[75],
+            a = new r[47](t + h + e, c[96]);
+        return n.replace(new c[27](u[97]), v(s[98], s[99], s[100])).replace(a, c[101])
+    }
+}(Zn);
+var qn = function() {
+    var n, t, r;
+    n = t = r = a;
+    var e, o, i;
+    e = o = i = s;
+    var u = o[15],
+        c = o[102],
+        f = e[103];
+
+    function l(r) {
+        var a = o[102],
+            i = e[103];
+        this[n[76]] = r;
+        for (var u = t[52], c = r[a + g + i]; u < c; u++)
+            this[u] = t[52]
+    }
+    return l[e[104]][w + m + I + u] = function() {
+            for (var a = e[105], u = this[a + y], c = [], s = -e[0], v = o[2], f = u[r[56]]; v < f; v++)
+                for (var l = this[v], p = u[v], d = s += p; c[d] = l & parseInt(t[77], n[78]),
+                    --p != r[52];)
+                    --d,
+                    l >>= parseInt(n[79], i[106]);
+            return c
+        },
+        l['prototype']['decodeBuffer'] = function(n) {
+            for (var r = e[8], a = this[ot(e[108], e[109])], o = t[52], u = e[2], s = a[c + r + f]; u < s; u++) {
+                var v = a[u],
+                    l = i[2];
+                do {
+                    l = (l << t[82]) + n[o++]
+                } while (--v > t[52]);
+                this[u] = l >>> i[2]
+            }
+        },
+        l
+}()
+var zn;
+
+function at() {
+    var n, t, r;
+    n = t = r = u;
+    var a, o, i;
+    a = o = i = e;
+    var c = arguments[o[52]];
+    if (!c)
+        return t[1];
+    for (var s = o[0], v = o[1], f = a[52]; f < c.length; f++) {
+        var l = c.charCodeAt(f),
+            p = l ^ v;
+        v = v * f % n[222] + o[200],
+            s += i[2].fromCharCode(p)
+    }
+    return s
+}! function(n) {
+    var t = s[13],
+        o = c[53],
+        i = r[83],
+        f = r[84],
+        l = s[110],
+        d = r[85],
+        h = r[86];
+
+    function g(n, a, o, i, u) {
+        for (var c = s[13], v = r[87], f = n[s[111]]; a < f;)
+            o[i++] = n[a++] ^ u & parseInt(c + v + t + _, r[88]),
+            u = ~(u * parseInt(e[89], e[82]))
+    }
+
+    function w(n) {
+        for (var t = c[112], i = r[52], v = n[s[111]], f = []; i < v;) {
+            var l = n[i++] << parseInt(C + t, c[113]) | n[i++] << e[82] | n[i++];
+            f.push(m.charAt(l >> parseInt(e[90], e[82])), m.charAt(l >> parseInt(s[114], e[78]) & parseInt(a[91], r[88])), m.charAt(l >> u[59] & parseInt(E + o, a[78])), m.charAt(l & parseInt(a[92], u[113])))
+        }
+        return f.join(e[0])
+    }
+    for (var m = at(u[115], s[116]), I = {}, y = u[2]; y < parseInt(i + A, e[93]); y++)
+        I[m.charAt(y)] = y;
+
+    function O(n) {
+        var t, r, e;
+        t = r = e = s;
+        var o, i, u;
+        o = i = u = a;
+        for (var c = ot(i[94]), l = e[2], p = n[o[56]], d = []; l < p;) {
+            var h = I[n.charAt(l++)] << parseInt(at(t[117]), u[82]) | I[n.charAt(l++)] << parseInt(v(t[118], u[95], e[119]), o[88]) | I[n.charAt(l++)] << t[59] | I[n.charAt(l++)];
+            d.push(h >> parseInt(e[120], t[106]), h >> parseInt(t[121], r[122]) & parseInt(f + b + c, t[106]), h & parseInt(o[96], u[88]))
+        }
+        return d
+    }
+
+    function D(n) {
+        var t = O(n);
+        if (rn,
+            p,
+            t[r[52]] != h)
+            return error = T + B + l,
+                void 0;
+        var a = t[c[0]],
+            o = [];
+        return g(t, +parseInt(e[79], c[122]), o, +u[2], a),
+            x(o) == a ? o : void 0
+    }
+
+    function x(n) {
+        for (var e = c[2], i = a[52], u = n[c[111]]; i < u; i++)
+            e = (e << s[123]) - e + n[i];
+        return e & parseInt(s[124], r[88])
+    }
+
+    function N(n) {
+        var r = x(n),
+            e = [h, r];
+        return g(n, +a[52], e, +a[88], r),
+            w(e)
+    }
+    n[e[97]] = w,
+        n[R + k + S] = O,
+        n[u[125]] = N,
+        n[d + P + "de"] = D
+}(zn || (zn = {})) ! function(n) {
+    var t = e[87],
+        o = a[8],
+        i = e[8],
+        f = s[215],
+        l = r[52],
+        p = s[0],
+        d = parseInt(c[216], u[122]),
+        h = e[86],
+        g = u[217],
+        w = u[123],
+        m = e[165],
+        I = parseInt(t + En, c[122]),
+        y = parseInt(a[79], a[82]),
+        _ = c[218],
+        C = parseInt(a[193], e[82]),
+        E = parseInt(o + i, r[78]),
+        A = parseInt(u[219], s[122]),
+        b = parseInt(f + An, s[106]),
+        T = parseInt(r[194], s[106]),
+        B = parseInt(8),
+        R = parseInt(e[196], u[122]),
+        k = parseInt(e[197], a[78]),
+        S;
+
+    function P() {
+        var n = s[0],
+            t = r[88],
+            e = parseInt(u[13], c[122]),
+            a = s[217];
+        S = new qn([a, a, a, a, n, n, n, e, t, t, t, t, t, t, t, a, t, n]),
+            S[p] = parseInt(TOKEN_SERVER_TIME),
+            M(),
+            S[B] = 0,
+            S[k] = 3,
+            S[R] = 0,
+            S[h] = 505497997,
+            S[b] = 3812,
+            S[g] = 1,
+            S[w] = 10,
+            S[m] = 5
+    }
+
+    function M() {
+        S[l] = Math.random() * parseInt("4294967295", 10) >>> 0
+    }
+
+    function O() {
+        S[R]++,
+            S[p] = parseInt(TOKEN_SERVER_TIME),
+            S[d] = timeNow(),
+            S[B] = 0,
+            S[I] = 0,
+            S[y] = 0,
+            S[_] = 0,
+            S[C] = 0,
+            S[E] = 0,
+            S[A] = 0;
+        var n = S.toBuffer();
+        console.log(zn.encode(n))
+        return zn.encode(n)
+    }
+    P();
+
+    function D() {
+        return O()
+    }
+    n.updata = D
+}(rt || (rt = {}));
+
+function timeNow() {
+    var n = new e[105];
+    try {
+        return time = s[52].now(),
+            time / parseInt(c[131], a[88]) >>> c[2]
+    } catch (t) {
+        return time = n.getTime(),
+            time / parseInt(s[121], s[84]) >>> r[52]
+    }
+}
 var n = rt.updata()
```

### Comparing `adata-1.2.4/adata/common/js/ths.js` & `adata-2.0.0b0/adata/common/js/ths.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,1061 +1,1061 @@
-var TOKEN_SERVER_TIME = 1572845499.629;
-
-function v_cookie(r, n, t, e, a) {
-    var u = n[0],
-        c = n[1],
-        v = a[0],
-        s = t[0],
-        f = t[1],
-        l = r[0],
-        d = hr(a[1], e[0], t[2]),
-        p = t[3],
-        h = e[1],
-        g = yr(a[2], a[3], e[2]),
-        m = yr(a[4], r[1], t[4]),
-        w = r[2],
-        I = a[5],
-        _ = a[6],
-        y = a[7],
-        E = hr(n[2], r[3], r[4]),
-        A = t[5],
-        C = e[3],
-        b = e[4],
-        B = t[6],
-        R = a[8],
-        T = a[9],
-        S = n[3],
-        k = t[7],
-        x = t[8],
-        O = a[10],
-        L = n[4],
-        M = n[5],
-        N = a[11],
-        P = e[5],
-        j = hr(n[6], e[6], t[9], r[5]),
-        D = t[10],
-        W = e[7],
-        $ = r[6],
-        F = yr(r[7], t[11], e[8], n[7]),
-        X = r[8],
-        H = t[12],
-        K = r[9],
-        U = n[8],
-        V = e[9],
-        Y = r[10],
-        J = e[10],
-        q = r[11],
-        Q = a[12],
-        Z = n[9],
-        G = t[13],
-        z = t[14],
-        rr = t[15],
-        nr = n[10],
-        tr = a[13],
-        er = a[14],
-        ar = e[11],
-        or = r[12],
-        ir = yr(t[16], r[13], r[14], r[15]),
-        ur = t[17],
-        cr = t[18];
-
-    function vr() {
-        var r = arguments[n[11]];
-        return r.split(n[12]).reverse().join(e[12])
-    }
-
-    var sr = [new e[13](hr(a[15], n[13], a[16])), new e[13](a[17])];
-
-    function fr() {
-        var n = arguments[a[18]];
-        if (!n) return a[19];
-        for (var o = t[19], i = e[14], u = e[15]; u < n.length; u++) {
-            var c = n.charCodeAt(u),
-                v = c ^ i;
-            i = c,
-                o += r[16].fromCharCode(v)
-        }
-        return o
-    }
-
-    var lr = '',
-        dr;
-    !
-    function(o) {
-        var i = e[18],
-            c = e[19];
-        o[e[20]] = a[21];
-
-        function v(t, a, o, i, u) {
-            var c, v, s;
-            c = v = s = r;
-            var f, l, d;
-            f = l = d = n;
-            var p, h, g;
-            p = h = g = e;
-            var m = t + g[21] + a;
-            i && (m += l[15] + i),
-                u && (m += h[22] + u),
-                o && (m += v[17] + o),
-                l[14][g[23]] = m
-        }
-
-        o[e[24]] = l;
-
-        function s(t, e, a) {
-            var o = n[16];
-            this.setCookie(t, r[18], i + o + c, e, a)
-        }
-
-        o[t[22]] = f;
-
-        function f(o) {
-            var i = vr(e[25], a[22]),
-                c = a[23][n[17]],
-                v = u + i + o + t[23],
-                s = '';
-            if (s == -r[19]) {
-                if (v = o + t[23], c.substr(a[24], v.length) != v) return;
-                s = a[24]
-            }
-            var f = s + v[r[20]],
-                l = '';
-            return l == -e[26] && (l = c[t[24]])
-
-        }
-
-        o[e[27]] = v;
-
-        function l() {
-            var r, t, a;
-            r = t = a = e;
-            var i, u, c;
-            i = u = c = n;
-            var v = u[18];
-            this.setCookie(v, a[28]),
-                this.getCookie(v) || (o[i[19]] = u[20]),
-                this.delCookie(v)
-        }
-
-        o[n[21]] = s
-    }(dr || (dr = {}));
-    var pr;
-
-    function hr() {
-        var r = arguments[a[25]];
-        if (!r) return a[19];
-        for (var e = a[19], o = t[25], i = n[22], u = t[18]; u < r.length; u++) {
-            var c = r.charCodeAt(u);
-            i = (i + t[26]) % o.length,
-                c ^= o.charCodeAt(i),
-                e += String.fromCharCode(c)
-        }
-        return e
-    }
-
-    !
-    function(o) {
-        var i, u, d;
-        i = u = d = a;
-        var p, h, g;
-        p = h = g = t;
-        var m, w, I;
-        m = w = I = r;
-        var _, y, E;
-        _ = y = E = n;
-        var b, B, R;
-        b = B = R = e;
-        var T = B[29],
-            S = y[23],
-            k = m[22],
-            x = w[0],
-            O = E[24],
-            L = (C, Ar, R[30]),
-            M = b[31],
-            N = T + S,
-            P = p[28],
-            j,
-            W = m[23][y[25]],
-            $,
-            F;
-
-        function X(r) {
-            return function() {
-                F.appendChild(j),
-                    j.addBehavior(u[26]),
-                    j.load(N);
-                var n = r();
-                return F.removeChild(j),
-                    n
-            }
-        }
-
-        function H() {
-            var r = A;
-            r = D;
-            try {
-                return !!(N in B[32] && b[32][N])
-            } catch (n) {
-                return void B[15]
-            }
-        }
-
-        function K(r) {
-            return P ? G(r) : j ? Y(r) : void _[26]
-        }
-
-        function U() {
-            if (P = H(), P) j = _[27][N];
-            else if (W[k + c][I[24]]) try {
-                $ = new ActiveXObject(vr(I[25], y[28], w[26])),
-                    $.open(),
-                    $.write(y[29]),
-                    $.close(),
-                    F = $.w[B[33]][I[27]][_[30]],
-                    j = F.createElement(I[28])
-            } catch (r) {
-                j = W.createElement(N),
-                    F = W[vr(I[29], d[27])] || W.getElementsByTagName(b[17])[I[27]] || W[m[30]]
-            }
-        }
-
-        o[w[31]] = U;
-
-        function V(r, n) {
-            var t = J;
-            if (void 0 === n) return Z(r);
-            if (t = sr, P) z(r, n);
-            else {
-                if (!j) return void B[15];
-                Q(r, n)
-            }
-        }
-
-        o[v + x] = V;
-
-        function Y(r) {
-            X(function() {
-                return r = J(r),
-                    j.getAttribute(r)
-            })()
-        }
-
-        function J(r) {
-            var n = z;
-            n = v;
-            var t = vr(Ir, w[32]),
-                e = new y[31](t + O + s + L, b[31]);
-            return r.replace(new B[13](d[28]), b[34]).replace(e, p[29])
-        }
-
-        function q(r) {
-            try {
-                j.removeItem(r)
-            } catch (n) {}
-        }
-
-        o[M + f + l] = K;
-
-        function Q(r, n) {
-            var t = G;
-            t = cr,
-                X(function() {
-                    var t = M;
-                    r = J(r),
-                        t = K;
-                    try {
-                        j.setAttribute(r, n),
-                            j.save(N)
-                    } catch (e) {}
-                })()
-        }
-
-        function Z(r) {
-            var n, t, e;
-            if (n = t = e = g, P) q(r);
-            else {
-                if (!j) return void t[18];
-                rr(r)
-            }
-        }
-
-        function G(r) {
-            try {
-                return j.getItem(r)
-            } catch (n) {
-                return y[20]
-            }
-        }
-
-        o[fr(w[33], p[30], R[35])] = Z;
-
-        function z(r, n) {
-            try {
-                j.setItem(r, n)
-            } catch (t) {}
-        }
-
-        function rr(r) {
-            X(function() {
-                r = J(r),
-                    j.removeAttribute(r),
-                    j.save(N)
-            })()
-        }
-    }(pr || (pr = {}));
-    var gr = function() {
-            var o, i, u;
-            o = i = u = e;
-            var c, v, s;
-            c = v = s = a;
-            var f, l, g;
-            f = l = g = n;
-            var m, w, I;
-            m = w = I = t;
-            var _, E, A;
-            _ = E = A = r;
-            var C = yr(Cr, U, _[34]),
-                b = vr(A[35], m[31]),
-                R = hr(g[32], c[29], i[36]),
-                T = hr(l[33], g[34], i[37], tr);
-
-            function S(r) {
-                this[m[32]] = r;
-                for (var n = o[15], t = r[i[38]]; t > n; n++) this[n] = i[15]
-            }
-
-            return S[d + p + C][b + h] = function() {
-                    for (var r = this[vr(h, E[36], E[37])], n = [], t = -I[26], e = o[15], a = r[A[20]]; a > e; e++)
-                        for (var u = this[e], f = r[e], d = t += f; n[d] = u & parseInt(v[30], l[35]), --f != s[24];) --d,
-                            u >>= parseInt(i[39], c[31]);
-                    return n
-                },
-                S[vr(w[33], v[32])][_[38]] = function(r) {
-                    var n = dr,
-                        t = this[vr(y, l[36], A[39])],
-                        e = f[26];
-                    n = B;
-                    for (var a = v[24], o = t[l[37]]; o > a; a++) {
-                        var i = t[a],
-                            u = l[26];
-                        do u = (u << parseInt(R + T, g[35])) + r[e++];
-                        while (--i > w[18]);
-                        this[a] = u >>> w[18]
-                    }
-                },
-                S
-        }(),
-        mr;
-    !
-    function(o) {
-        var i, u, c;
-        i = u = c = n;
-        var v, s, f;
-        v = s = f = e;
-        var l, d, p;
-        l = d = p = a;
-        var h, w, I;
-        h = w = I = r;
-        var _, y, E;
-        _ = y = E = t;
-        var A = y[34],
-            C = (nr, U, h[40]),
-            b = p[25];
-
-        function B(r) {
-            for (var n = y[35], t = f[15], e = r[vr(c[38], I[41], H)], a = []; e > t;) {
-                var o = k[r.charAt(t++)] << parseInt(g + A, d[31]) | k[r.charAt(t++)] << parseInt(n + m, h[42]) | k[r.charAt(t++)] << parseInt(I[43], i[35]) | k[r.charAt(t++)];
-                a.push(o >> parseInt(_[36], h[42]), o >> l[31] & parseInt(u[39], i[40]), o & parseInt(d[30], c[35]))
-            }
-            return a
-        }
-
-        function T(r) {
-            for (var n = (O, R, p[24]), t = I[27], e = r[E[24]]; e > t; t++) n = (n << E[37]) - n + r[t];
-            return n & parseInt(E[38], p[33])
-        }
-
-        for (var S = s[40], k = {},
-                x = s[15]; x < parseInt(I[44], l[34]); x++) k[S.charAt(x)] = x;
-
-        function L(r) {
-            var n = B(r),
-                t = n[u[26]];
-            if (t != b) return error = yr(V, u[41], s[41], v[42]),
-                void 0;
-            var e = n[s[26]],
-                a = [];
-            return P(n, +_[39], a, +_[18], e),
-                T(a) == e ? a : void 0
-        }
-
-        function M(r) {
-            var n = T(r),
-                t = [b, n];
-            return P(r, +l[24], t, +p[25], n),
-                N(t)
-        }
-
-        function N(r) {
-            var n, t, e;
-            n = t = e = f;
-            var a, o, u;
-            a = o = u = y;
-            var c, v, s;
-            c = v = s = h;
-            var d, p, g;
-            d = p = g = l;
-            var m, w, I;
-            m = w = I = i;
-            for (var _ = m[42], E = d[24], A = r[c[20]], b = []; A > E;) {
-                var B = r[E++] << parseInt(fr(Z, d[35]), o[39]) | r[E++] << g[31] | r[E++];
-                b.push(S.charAt(B >> parseInt(m[43], t[43])), S.charAt(B >> parseInt(p[36], o[40]) & parseInt(I[44], I[45])), S.charAt(B >> n[44] & parseInt(_ + C, n[42])), S.charAt(B & parseInt(fr(d[37], c[45], or), a[41])))
-            }
-            return b.join(o[19])
-        }
-
-        function P(r, n, t, e, a) {
-            var o, i, u;
-            o = i = u = w;
-            var c, v, s;
-            c = v = s = E;
-            for (var f = r[v[24]]; f > n;) t[e++] = r[n++] ^ a & parseInt(u[46], s[42]),
-                a = ~(a * parseInt(v[43], v[40]))
-        }
-
-        o[E[44]] = N,
-            o[_[45]] = B,
-            o[v[45]] = M,
-            o[y[46]] = L
-    }(mr || (mr = {}));
-    var wr;
-    !
-    function(o) {
-        var i = a[38],
-            u = r[47],
-            c = t[47],
-            v = vr(n[46], a[39], a[40]),
-            s = e[46],
-            f = e[47],
-            l = a[41],
-            d = a[42];
-
-        function p(o) {
-            var i = a[43],
-                u = vr(n[47], e[48], n[48]),
-                c = {},
-                v = function(o, c) {
-                    var s, f, l, d;
-                    for (c = c.replace(n[49], n[12]), c = c.substring(e[26], c[e[38]] - e[26]), s = c.split(e[49]), l = a[24]; l < s[yr(v, sr, t[48])]; l++)
-                        if (f = s[l].split(n[50]), f && !(f[a[44]] < t[39])) {
-                            for (d = n[35]; d < f[r[20]]; d++) f[n[11]] = f[n[11]] + r[48] + f[d];
-                            f[n[26]] = new a[45](r[49]).test(f[n[26]]) ? f[e[15]].substring(r[19], f[e[15]][a[44]] - n[11]) : f[n[26]],
-                                f[n[11]] = new r[50](i + u + w).test(f[n[11]]) ? f[e[26]].substring(t[26], f[r[19]][n[37]] - t[26]) : f[a[18]],
-                                o[f[r[27]]] = f[n[11]]
-                        }
-                    return o
-                };
-            return new a[45](I + _).test(o) && (c = v(c, o)),
-                c
-        }
-
-        function h(n) {
-            for (var t = [], e = a[24]; e < n[r[20]]; e++) t.push(n.charCodeAt(e));
-            return t
-        }
-
-        function g(o) {
-            var u = a[46];
-            if (typeof o === vr(O, a[47], or) && o[a[48]]) try {
-                var c = parseInt(o[a[48]]);
-                switch (c) {
-                    case parseInt(i + u, t[42]):
-                        break;
-                    case parseInt(yr(t[49], r[51], e[50]), e[43]):
-                        top[t[50]][n[51]] = o[e[51]];
-                        break;
-                    case parseInt(yr(a[25], j, e[52]), n[52]):
-                        top[n[53]][t[51]] = o[t[52]]
-                }
-            } catch (v) {}
-        }
-
-        function m(r, n, t) {
-
-        }
-
-        function L() {
-            var e, a, o;
-            e = a = o = r;
-            var i, u, c;
-            i = u = c = n;
-            var v, s, f;
-            v = s = f = t;
-            var l = f[53],
-                d = c[54],
-                p = new e[52];
-            return typeof TOKEN_SERVER_TIME == y + l + d ? s[18] : (time = parseInt(TOKEN_SERVER_TIME), time)
-        }
-
-        function M() {
-            var o = new t[54];
-            try {
-                return time = n[2].now(),
-                    time / parseInt(fr(a[50], a[51], r[53]), t[40]) >>> e[15]
-            } catch (i) {
-                return time = o.getTime(),
-                    time / parseInt(e[53], a[25]) >>> r[27]
-            }
-        }
-
-        function N(r) {
-            for (var a = t[18], o = r[t[24]] - n[11]; o >= e[15]; o--) a = a << e[26] | +r[o];
-            return a
-        }
-
-        function P(a) {
-            var o = new r[50](n[55]);
-            if (K(a)) return a;
-            var i = o.test(a) ? -e[54] : -t[39],
-                u = a.split(r[54]);
-            return u.slice(i).join(fr(n[56], t[55], E))
-        }
-
-        function j(t) {
-            for (var o = n[26], i = e[15], u = t[vr(r[55], a[52], D)]; u > i; i++) o = (o << r[56]) - o + t.charCodeAt(i),
-                o >>>= n[26];
-            return o
-        }
-
-        function W(n, o) {
-            var i = new a[45](t[56], yr(r[57], $, t[57], r[58])),
-                u = new a[45](t[58]);
-            if (n) {
-                var c = n.match(i);
-                if (c) {
-                    var v = c[e[26]];
-                    return o && u.test(v) && (v = v.split(t[59]).pop().split(r[48])[e[15]]),
-                        v
-                }
-            }
-        }
-
-        function $(o) {
-            var i = n[57],
-                u = vr(e[55], e[56]),
-                f = e[4];
-            if (!(o > t[60])) {
-                o = o || a[24];
-                var l = parseInt(E + c + A, r[42]),
-                    d = n[14].createElement(e[57]);
-                d[r[59]] = n[58] + parseInt((new a[53]).getTime() / l) + r[60],
-                    d[r[61]] = function() {
-                        var n = a[46];
-                        cr = r[19],
-                            setTimeout(function() {
-                                    $(++o)
-                                },
-                                o * parseInt(C + n, a[33]))
-                    },
-                    d[t[61]] = d[hr(a[54], a[55], t[62])] = function() {
-                        var a = n[59];
-                        this[i + v + u + b] && this[e[58]] !== n[60] && this[s + B + a + f] !== e[59] && this[t[63]] !== n[61] || (cr = e[15], d[hr(N, r[62], n[62], e[25])] = d[t[64]] = r[63])
-                    },
-                    e[60][e[61]].appendChild(d)
-            }
-        }
-
-        function F() {
-            var r = a[56];
-            return Math.random() * parseInt(R + T + f + r, t[42]) >>> n[26]
-        }
-
-        function X(r) {
-            var e = new n[31](fr(t[65], t[66], a[57]), yr(c, n[63], t[57]));
-            if (r) {
-                var o = r.match(e);
-                return o
-            }
-        }
-
-        o[S + k] = p,
-            o[r[64]] = $,
-            o[t[67]] = g,
-            o[t[68]] = h,
-            o[t[69]] = j,
-            o[t[70]] = F,
-            o[r[65]] = K,
-            o[x + l] = P,
-            o[t[71]] = W,
-            o[t[72]] = X,
-            o[hr(r[66], t[73], r[67], C)] = N,
-            o[t[74]] = M,
-            o[d + O] = L;
-
-        function K(n) {
-            return new r[50](t[75]).test(n)
-        }
-
-        o[r[68]] = m
-    }(wr || (wr = {}));
-    var Ir;
-    !
-    function(o) {
-        var i = t[76],
-            u = t[77],
-            c = n[65],
-            v = t[78],
-            s = a[24],
-            f = n[26],
-            l = t[18],
-            d = t[18],
-            p = e[15],
-            h = a[24],
-            g = r[69],
-            m = '';
-        wr.eventBind(e[60], n[67], E),
-            wr.eventBind(r[71], t[79], E),
-            wr.eventBind(t[20], hr(e[64], A, a[59]), b),
-            wr.eventBind(e[60], r[72], y);
-
-        function w() {
-            return f
-        }
-
-        function I(r) {
-            f++
-        }
-
-        function _() {
-            return {
-                x: p,
-                y: h,
-                trusted: g
-            }
-        }
-
-        function y(r) {
-            d++
-        }
-
-        function E(r) {
-            s++
-        }
-
-        function C() {
-            return l
-        }
-
-        function b(r) {
-            var o, i, u;
-            o = i = u = n;
-            var c, s, f;
-            c = s = f = t;
-            var d, m, w;
-            d = m = w = e;
-            var I, _, y;
-            I = _ = y = a;
-            var E = I[60],
-                A = d[65];
-            l++,
-            g = void 0 == r[E + A + v] || r[yr(f[80], s[81], i[68])],
-                p = r[s[82]],
-                h = r[c[83]]
-        }
-
-        function B() {
-            return d
-        }
-
-        function R() {
-            return s
-        }
-
-        o[r[73]] = R,
-            o[a[61]] = w,
-            o[fr(a[62], n[69])] = C,
-            o[n[70]] = B,
-            o[r[74]] = _
-    }(Ir || (Ir = {}));
-    var _r;
-    !
-    function(u) {
-        var v = fr(n[71], t[84]),
-            s = r[75],
-            f = yr(dr, n[72], e[66], $),
-            l = r[76],
-            d = e[67],
-            p = r[77],
-            h = hr(dr, r[78], a[63], n[73]),
-            g = r[79],
-            m = n[74];
-        BROWSER_LIST = {};
-
-        function w() {
-            var t, e, a;
-            t = e = a = r;
-            var o, i, u;
-            o = i = u = n;
-            return wr.booleanToDecimal(c)
-        }
-
-        function I(t) {
-            for (var o = n[26]; o < y[e[38]]; o++) {
-                var i = y[o][r[94]];
-                if (t.test(i)) return !a[24]
-            }
-            return !a[18]
-        }
-
-        function E(t) {
-
-        }
-
-        function A() {
-            return a[73]
-        }
-
-        function B() {
-            return n[20]
-        }
-
-        function T() {
-            return I(new t[93](r[96]))
-        }
-
-        function S() {
-            return I(new a[45](t[98], r[97]))
-        }
-
-        function k() {
-            for (var r in BROWSER_LIST)
-                if (BROWSER_LIST.hasOwnProperty(r)) {
-                    var n = BROWSER_LIST[r];
-                    if (n()) return +r.substr(a[18])
-                }
-            return e[15]
-        }
-
-        function x() {
-            var n, a, o;
-            n = a = o = r;
-            var i, u, c;
-            i = u = c = t;
-            var v, s, f;
-            v = s = f = e;
-            var l = s[75],
-                d = s[76];
-            return I(new u[93](o[98], v[71])) || E(l + F + d + X)
-        }
-
-        function O() {
-
-        }
-
-        function L() {
-            var r, n, t;
-            r = n = t = a;
-            var o, i, u;
-            o = i = u = e;
-            var c = l;
-            return c = p
-        }
-
-        function M() {
-            var r, n, a;
-            r = n = a = t;
-            var o, i, u;
-            o = i = u = e;
-            var c;
-            try {
-                c = i[60].createElement(a[99]).getContext(i[78])
-            } catch (v) {}
-            return !!c
-        }
-
-
-        function J() {
-            var t, e, o;
-            t = e = o = n;
-            var i, u, c;
-            i = u = c = a;
-            var v, s, f;
-            return v = s = f = r,
-                -parseInt(s[100], c[31]) === (new e[2]).getTimezoneOffset()
-        }
-
-        function Q() {
-            try {} catch (e) {
-                return r[101]
-            }
-        }
-
-        function Z() {
-            var n, a, o;
-            n = a = o = e;
-            var i, u, c;
-            i = u = c = r;
-            var v, s, f;
-            return v = s = f = t,
-                plugin_num = s[18],
-                plugin_num
-        }
-
-        var z = [R, x, S, T, L, Q, b, V, O, J, M, q, Y, B, tr, A];
-
-        var nr = [new e[13](n[85]), new n[31](e[82]), new r[50](e[83]), new r[50](t[102]), new n[31](e[84]), new a[45](a[78]), new a[45](e[85]), new e[13](t[103]), new a[45](r[103]), new t[93](r[104]), new a[45](r[105])];
-
-        function tr() {
-            return e[86]
-        }
-
-        u[e[87]] = rr,
-            u[a[79]] = k,
-            u[yr(c, e[88], r[106])] = Z,
-            u[K + U + m] = w
-    }(_r || (_r = {}));
-
-    function yr() {
-        var o = arguments[a[25]];
-        if (!o) return t[19];
-        for (var i = a[19], u = e[14], c = r[27]; c < o.length; c++) {
-            var v = o.charCodeAt(c),
-                s = v ^ u;
-            u = u * c % a[80] + e[89],
-                i += n[86].fromCharCode(s)
-        }
-        return i
-    }
-
-    var Er;
-    !
-    function(o) {
-        var i = a[81],
-            u = t[35],
-            c = r[107],
-            v = vr(S, a[56]),
-            f = r[27],
-            l = r[19],
-            d = a[25],
-            p = n[87],
-            h = parseInt(e[90], r[108]),
-            g = a[82],
-            m = parseInt(vr(s, t[104]), t[39]),
-            w = r[109],
-            I = t[40],
-            _ = parseInt(i + V, n[45]),
-            y = parseInt(u + c, n[52]),
-            E = parseInt(t[105], r[42]),
-            A = e[91],
-            C = parseInt(Y + v, r[42]),
-            b = parseInt(e[92], e[93]),
-            B = t[106],
-            R = parseInt(vr(e[94], e[95]), t[41]),
-            T = parseInt(a[83], e[93]),
-            k;
-
-        function x() {
-            var r = M();
-            return r
-        }
-
-        function O() {
-            var r = t[26],
-                a = n[35],
-                o = e[54],
-                i = n[88];
-            k = new gr([i, i, i, i, r, r, r, o, a, a, a, a, a, a, a, i, a, r]),
-                k[l] = wr.serverTimeNow(),
-                L(),
-                k[B] = cr,
-                k[T] = ur,
-                k[R] = e[15],
-                k[C] = _r.getBrowserFeature(),
-                k[g] = _r.getBrowserIndex(),
-                k[m] = _r.getPluginNum()
-        }
-
-        function L() {
-            var a = dr.getCookie(tr) || pr.get(ar);
-            if (a && a[r[20]] == parseInt(e[96], n[52])) {
-                var o = mr.decode(a);
-                if (o && (k.decodeBuffer(o), k[f] != t[18])) return
-            }
-            k[f] = wr.random()
-        }
-
-        o[a[84]] = O;
-
-        function M() {
-            k[R]++,
-                k[l] = wr.serverTimeNow(),
-                k[d] = wr.timeNow(),
-                k[B] = cr,
-                k[w] = Ir.getMouseMove(),
-                k[I] = Ir.getMouseClick(),
-                k[_] = Ir.getMouseWhell(),
-                k[y] = Ir.getKeyDown(),
-                k[E] = Ir.getClickPos().x,
-                k[A] = Ir.getClickPos().y;
-            var r = k.toBuffer();
-            return mr.encode(r)
-        }
-
-        o[yr(r[3], n[89], e[97])] = x
-    }(Er || (Er = {}));
-    var Ar;
-    !
-    function(o) {
-        var i = n[90],
-            u = a[85],
-            v = r[110],
-            s = a[86],
-            f = t[107],
-            p,
-            h,
-            m,
-            w,
-            I,
-            _;
-
-        function E(r) {
-            return N(r) && dr[a[87]]
-        }
-
-        function A(o) {
-            var i = wr.getOriginFromUrl(o);
-            return i ? !new n[31](yr(r[42], c, t[110]) + w).test(i[r[108]]) || !new e[13](I).test(i[a[18]]) : t[111]
-        }
-
-        function C(e) {
-            var o = (_r, g, Er.update());
-            return e + (new r[50](vr(a[88], a[89])).test(e) ? n[91] : vr(P, a[90], t[112])) + er + t[23] + r[111](o)
-        }
-
-        function b(o, i, u) {
-            if (r[112] in i) return i.apply(o, u);
-            switch (u[n[37]]) {
-                case n[26]:
-                    return i();
-                case a[18]:
-                    return i(u[n[26]]);
-                case r[108]:
-                    return i(u[e[15]], u[r[19]]);
-                default:
-                    return i(u[n[26]], u[r[108]], u[t[17]])
-            }
-        }
-
-        function B() {
-            var r = Er.update();
-            return r
-        }
-
-        function k(r, e, o) {
-            if (!r) return n[20];
-            var i = r[e];
-            if (!i) return t[111];
-            var u = o(i);
-            return d || (u[a[97]] = i + t[19]),
-                u[n[97]] = i,
-                r[e] = u,
-                a[21]
-        }
-
-        function M(o) {
-            var i, u, c;
-            i = u = c = n;
-            var v, s, l;
-            v = s = l = r;
-            var d, p, h;
-            d = p = h = e;
-            var g, m, w;
-            g = m = w = a;
-            var I, _, y;
-            I = _ = y = t;
-            var R = hr(I[121], w[106], d[109]),
-                T;
-            k(o, _[122],
-                    function(r) {
-                        var n = w[107];
-                        return function() {
-                            var t, e, a;
-                            t = e = a = _;
-                            var o, i, u;
-                            o = i = u = l;
-                            var c, v, s;
-                            c = v = s = w;
-                            var f = s[108];
-                            try {
-                                A(arguments[s[18]]) && !E(arguments[o[19]]) ? arguments[a[26]] = C(arguments[s[18]]) : T = B(),
-                                    r.apply(this, arguments),
-                                    A(arguments[i[19]]) || this.setRequestHeader(ar, T)
-                            } catch (d) {
-                                return n + f
-                            }
-                        }
-                    }),
-                k(o, g[109],
-                    function(r) {
-                        var n = b;
-                        n = M;
-                        var t = vr(_[123], u[107]);
-                        return function() {
-                            var n = fr(f, c[108], I[124]),
-                                e = s[122];
-                            try {
-                                if (parseInt(this.status) === parseInt(h[110], v[123])) {
-                                    for (var a = r.apply(this, arguments), o = new p[13](i[109], n + R), u, l, d = {}; u = o.exec(a);) d[u[m[18]].toLowerCase()] = u[v[108]];
-                                    wr.analysisRst(wr.parse(d[ir.toLowerCase()]))
-                                }
-                            } catch (g) {
-                                return e + t
-                            }
-                            return r.apply(this, arguments)
-                        }
-                    })
-        }
-
-        function N(r) {
-            var n = wr.getHostFromUrl(r, e[28]);
-            return n ? _.test(n) : e[28]
-        }
-
-        function j() {
-            var cookie_v;
-            cookie_v = B()
-            return cookie_v
-        }
-
-        o[n[111]] = j
-    }(Ar || (Ar = {}));
-    var Cr;
-    var cookie = (function(a) {
-        function _() {
-            var cookie_v;
-            Er.Init();
-            cookie_v = Ar.Init();
-            return cookie_v
-        }
-
-        return function y() {
-            try {
-                return _()
-            } catch (r) {
-                return r
-            }
-        }
-    })()
-    return cookie()
-}
-
-function v() {
-    var v;
-    v = v_cookie(
-        ["t", 34, '"$', 36, "\fb", 55, "ure", "lJ#K", "Flash", "getBro", "1", "analys", "CHAMELEON_CALLBACK", 30, "\u256f\u0930\u097b\u09ff\u09a4\u0934\u099d\u09c1\u099d\u09d9\u09a7\u09c3\u0995\u09f0\u09d3\u0a62\u0a6f\u09bc\u09ad\u0934", "F,sp-", String, "; expires=", "", 1, "length", "; ", '', '', "addBehavior", ";^l", ">*]+", 0, "div", "&~!", "", "Init", "('&%$#\"![", ">NJ", "\u254e\u096d\u095f", "W$R", "sdelif_esab", "Or)E", "decodeBuffer", 84, "f", "htgnel", 8, "110", "40", "\u2504\u2562", "255", "o", ":", '^".*"$', RegExp, 40, Date, "e9", ".", 19, 5, "t8JOi", "}B", "src", ".js", "onerror", "*q:", null, "getServerTime", "isIPAddr", "8-", "ZX9Y]V8aWs3VQZ7Y", "eventBind", !0, "wheel", '', "keydown", "getMouseMove", "getClickPos", "vent", "me", "MSG", 41, "th", "safari", "ActiveXObject", "maxHeight", "head", "Google Inc.", "vendor", "sgAppName", "opr", 94, "tugw`pj", "chrome", "2345Explorer", "ome", "TheWorld", "name", "\u2553\u253c\u2572\u251d\u2569\u253d\u254f\u252e\u254d\u2526", "Native Client", "i", "Shockwave", "systemLanguage", "740", !1, "plugins", "^ARM", "^iPod", "^BlackBerry", "\u2550\u0978\u094e\u09c1\u09bc\u0928\u0989\u09d8\u099a\u09f3\u09b7\u09dc", "0", 2, 7, "c", encodeURIComponent, "apply", "headers", "8S:+", "\u2560\u2509\u2567\u2503\u256c\u251b", "\u255e\u2530\u2543\u2526\u2554\u2520\u2562\u2507\u2561\u250e\u257c\u2519", "a", 14, ":dB2", "href", "click", "err", 16, "hostname", "`60w", "\fbf", "&X "],
-        [";", "Element", Date, "par", "i", "DOMMous", 21, "xmT", "wserFe", "h", !0, 1, "", Boolean, '', "; domain=", "n 1970 00:", "cookie", "checkcookie", "allow", !1, "delCookie", 2333, "torage", ")*+,/\\\\:;", '', 0, '', "eliflmth", '', "ducument", RegExp, "W", "qsU", 61, 2, "sdelif_esab", "length", "I", "ff", 16, 45, "3", "10010", "77", 8, "6e%d", "DT{e", "$", / /g, ":", "href", 10, "location", "ned", "\\.com\\.cn$|\\.com\\.hk$", 63, "rea", "https://s.thsi.cn/js/chameleon/time.1", "tat", "loaded", "interactive", "WY:ZYS", "E?`a", "addEventListener", "eScroll", "onmousewheel", "mousemove", "\u255e\u096e\u096e\u09e3\u09a5\u092e\u099a\u09d4\u0990", "\u2550\u2535\u2541\u250c\u2563\u2516\u2565\u2500\u2543\u252f\u2546\u2525\u254e", "getKeyDown", "H69<J", "v~g-", "", "ature", "callPhantom", "ActiveXObject", "Uint8Array", "WeakMap", "JX%<", "chrome", "@L:!", "20", "language", "localStorage", "^Win32", String, 3, 4, "=XAE", "hea", "&", "/", "\\R$", '^R"VP', "s", "include", "_raw", "x.", "isRst", "SCRIPT", "ta", "base", "$?", "^_self$", "#", "unload", "ro", "\u2550", "^(.*?):[ \\t]*([^\\r\\n]*)\\r?$", "g", "Init", "t6?x}", "\u2574\u0955\u097b\u09dc\u0995\u0911\u09ab\u09fe\u09ba\u09e2\u098e\u09fe\u09f9\u09f9\u09f3\u0a55", "=d' "],
-        ["<=>?@[\\]^", "e", "HE9", "tot", "\u2503", "0", "dyS", "se", "getRoot", "NR", "nd", 60, "ng", "s", "get", "mit", 13, 3, 0, "", '', "\u255f\u253a\u255b\u253f", "getCookie", "=", "length", "V587", 1, String, !0, "___", "\u2553\u2536\u255a", "uBot", "base_fileds", 32, "2", "1", "20", 5, "255", 2, 8, 16, 10, "203", "base64Encode", "base64Decode", "decode", "760", "\u255b\u0978\u0954\u09f6\u09a4\u0935", 70, "location", "href", "redirect_url", "efi", Date, "\u2519", "^\\s*(?:https?:)?\\/{2,}([^\\/\\?\\#\\\\]+)", "\u255e", "[@:]", "@", 7, "onload", 'WY$PYS/FLV"P[_7[_R', "readyState", "onreadystatechange", '"^w', "\u2569\u2535\u2546\u256c\u2544\u257b\u2541\u2569\u2501\u2575\u2501\u2571\u2502\u253d\u2507\u252e\u2507\u2538\u2564\u254b\u2530\u2502\u252e\u2553\u257b\u2520\u257e\u2522\u250d\u2551\u256e\u2532\u2511\u254d\u2511\u254c\u2567\u254e", "analysisRst", "strToBytes", "strhash", "random", "getHostFromUrl", "getOriginFromUrl", 83, "timeNow", "^(\\d+\\.)+\\d+$", "d", "v", "ted", "touchmove", 85, "F(K9i", "clientX", "clientY", "\u257a\u2515\u256f\u253c", "postMessage", '', "ActiveXObject", "Apple Computer, Inc.", "Q", "chr", "\u2558\u2535\u2550", "BIDUBrowser", RegExp, "QQBrowser", "ro", "aef", "msDoNotTrack", "PDF|Acrobat", "canvas", "yE", "\u255b\u253a\u2554\u2533\u2546\u2527\u2540\u2525\u2556", "^Android", "^Linux [ix]\\d+", "011", "13", 15, "sub", "addEventListener", "jsonp_ignore", "\u2569", !1, 'L"', "Sj", "T{_,", "q*", "i", "tagName", "et", "{'K", "Pp<", "#x'", "open", "rS", "KN3", "#", "protocol", "\\.", "DEDAOL_NOELEMAHC"],
-        [83, "ffer", "\u2505", "20", "e", "ngsE", Error, "est", "\u2552\u095b\u0956\u09f0\u09a3\u0935\u09c0\u09e2", "1", "sr", "hexin-v", "", RegExp, 9527, 0, "**l>", "head", "Thu, 01 Ja", "00:00 GMT", "allow", "=", "; path=", "cookie", "Init", 33, 1, "setCookie", !0, "localS", "`{|}~]", "g", '', "frames", "___$&", 56, "	", "\b", "length", "10", "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789-_", "\u2552\u096f\u0948\u09fe\u09a2", 16, 2, 6, "encode", "rea", "729", "*.", ",", "\u2506\u092c\u090b\u09a0\u09e1\u096d\u09df\u0981\u09c4\u098c", "redirect_url", "\u2506\u092d\u090a\u09a3", "1111101000", 3, 47, "tat", "script", "readyState", "complete", '', "body", "onwheel", "mousewheel", 37, "rus", "\u2554\u0975", "chr", "ActiveXObject", "WeakMap", "aT1Kg", "i", 24, "\u2554\u253c\u254e\u2521\u254c\u2529", "\u2547\u0971\u094f\u09f6\u09b9\u0933\u099d", "Shockwav", "hockwave", "$cdc_asdjflasutopfhvcZLmcfl_", "webgl2", "2>n|", "plugins", "platform", "^Win64", "^Linux armv|Android", "^iPhone", "^MacIntel", !1, "getPlatform", "6Y,", 2333, "100", 12, "14", 10, 36, "01", "60", "\u2542\u096d\u095e\u09f0\u09a4\u0938", "j", 17, "Request", "prototype", "`z}lc", "error", "s", "r", "target", "\u255e", "A", "U", "193", "host", "$"],
-        ["se", "g@g?", Array, "*Y", Number, "^{.", "*}$", "und", "429", "496", "imeNow", "etti", "rg", "v", "hexin-v", Error, "L_%\\T8", ".baidu.", 1, "", Function, !0, " ", '', 0, 2, "#default#userData", "ydob", "^d", 89, "11111111", 8, "epytotorp", 10, 16, "\u2506\u2536\u2506\u2536\u2506", "14", 13, "10", "Syd", 44, "Domain", "serverT", '^"', "length", RegExp, "00", "tcejbo", "status_code", "n", 66, "\u2506\u2531\u2504\u2534", "htgnel", Date, "L%", 67, "5", "?)'", '', "[[?VS", "isT", "getMouseWhell", "}}", "TR", "ActiveXObject", "WE", "python", "Maxthon", 97, "chrome", "Ryp", "UBrowser", 54, !1, "ontouchstart", "\u254d\u0975\u0917\u09f2\u09be", "iso-8859-1", "defaultCharset", "^iPad", "getBrowserIndex", 256, "1", 5, "17", "Init", "XMLHttp", "tar", "allow", "@*", "?\\", "?", "\u2571\u2503\u256a\u2546\u2566\u2556\u2567\u2547\u2501\u2564\u2506\u2526\u2514\u2524\u2511\u2521\u2501\u2531\u2501\u253b\u250b\u253b\u2501\u2531\u2501\u2521\u2566\u252b\u257f", "den", "tia", 94, "ls", "\u2554\u2526\u2543", "_str", 37, "append", "Child", "\u255f", "\u2569\u0975\u094e\u09e5\u09a0\u092e\u09d1\u09ed\u09ce", "srcElement", "parentNode", "\u2543\u2522\u2545\u250b\u256a\u2507\u2562", "}*", "err", "or", "getAllResponseHeaders", "\\.?", "\\."]
-    );
-    return v
+var TOKEN_SERVER_TIME = 1572845499.629;
+
+function v_cookie(r, n, t, e, a) {
+    var u = n[0],
+        c = n[1],
+        v = a[0],
+        s = t[0],
+        f = t[1],
+        l = r[0],
+        d = hr(a[1], e[0], t[2]),
+        p = t[3],
+        h = e[1],
+        g = yr(a[2], a[3], e[2]),
+        m = yr(a[4], r[1], t[4]),
+        w = r[2],
+        I = a[5],
+        _ = a[6],
+        y = a[7],
+        E = hr(n[2], r[3], r[4]),
+        A = t[5],
+        C = e[3],
+        b = e[4],
+        B = t[6],
+        R = a[8],
+        T = a[9],
+        S = n[3],
+        k = t[7],
+        x = t[8],
+        O = a[10],
+        L = n[4],
+        M = n[5],
+        N = a[11],
+        P = e[5],
+        j = hr(n[6], e[6], t[9], r[5]),
+        D = t[10],
+        W = e[7],
+        $ = r[6],
+        F = yr(r[7], t[11], e[8], n[7]),
+        X = r[8],
+        H = t[12],
+        K = r[9],
+        U = n[8],
+        V = e[9],
+        Y = r[10],
+        J = e[10],
+        q = r[11],
+        Q = a[12],
+        Z = n[9],
+        G = t[13],
+        z = t[14],
+        rr = t[15],
+        nr = n[10],
+        tr = a[13],
+        er = a[14],
+        ar = e[11],
+        or = r[12],
+        ir = yr(t[16], r[13], r[14], r[15]),
+        ur = t[17],
+        cr = t[18];
+
+    function vr() {
+        var r = arguments[n[11]];
+        return r.split(n[12]).reverse().join(e[12])
+    }
+
+    var sr = [new e[13](hr(a[15], n[13], a[16])), new e[13](a[17])];
+
+    function fr() {
+        var n = arguments[a[18]];
+        if (!n) return a[19];
+        for (var o = t[19], i = e[14], u = e[15]; u < n.length; u++) {
+            var c = n.charCodeAt(u),
+                v = c ^ i;
+            i = c,
+                o += r[16].fromCharCode(v)
+        }
+        return o
+    }
+
+    var lr = '',
+        dr;
+    !
+    function(o) {
+        var i = e[18],
+            c = e[19];
+        o[e[20]] = a[21];
+
+        function v(t, a, o, i, u) {
+            var c, v, s;
+            c = v = s = r;
+            var f, l, d;
+            f = l = d = n;
+            var p, h, g;
+            p = h = g = e;
+            var m = t + g[21] + a;
+            i && (m += l[15] + i),
+                u && (m += h[22] + u),
+                o && (m += v[17] + o),
+                l[14][g[23]] = m
+        }
+
+        o[e[24]] = l;
+
+        function s(t, e, a) {
+            var o = n[16];
+            this.setCookie(t, r[18], i + o + c, e, a)
+        }
+
+        o[t[22]] = f;
+
+        function f(o) {
+            var i = vr(e[25], a[22]),
+                c = a[23][n[17]],
+                v = u + i + o + t[23],
+                s = '';
+            if (s == -r[19]) {
+                if (v = o + t[23], c.substr(a[24], v.length) != v) return;
+                s = a[24]
+            }
+            var f = s + v[r[20]],
+                l = '';
+            return l == -e[26] && (l = c[t[24]])
+
+        }
+
+        o[e[27]] = v;
+
+        function l() {
+            var r, t, a;
+            r = t = a = e;
+            var i, u, c;
+            i = u = c = n;
+            var v = u[18];
+            this.setCookie(v, a[28]),
+                this.getCookie(v) || (o[i[19]] = u[20]),
+                this.delCookie(v)
+        }
+
+        o[n[21]] = s
+    }(dr || (dr = {}));
+    var pr;
+
+    function hr() {
+        var r = arguments[a[25]];
+        if (!r) return a[19];
+        for (var e = a[19], o = t[25], i = n[22], u = t[18]; u < r.length; u++) {
+            var c = r.charCodeAt(u);
+            i = (i + t[26]) % o.length,
+                c ^= o.charCodeAt(i),
+                e += String.fromCharCode(c)
+        }
+        return e
+    }
+
+    !
+    function(o) {
+        var i, u, d;
+        i = u = d = a;
+        var p, h, g;
+        p = h = g = t;
+        var m, w, I;
+        m = w = I = r;
+        var _, y, E;
+        _ = y = E = n;
+        var b, B, R;
+        b = B = R = e;
+        var T = B[29],
+            S = y[23],
+            k = m[22],
+            x = w[0],
+            O = E[24],
+            L = (C, Ar, R[30]),
+            M = b[31],
+            N = T + S,
+            P = p[28],
+            j,
+            W = m[23][y[25]],
+            $,
+            F;
+
+        function X(r) {
+            return function() {
+                F.appendChild(j),
+                    j.addBehavior(u[26]),
+                    j.load(N);
+                var n = r();
+                return F.removeChild(j),
+                    n
+            }
+        }
+
+        function H() {
+            var r = A;
+            r = D;
+            try {
+                return !!(N in B[32] && b[32][N])
+            } catch (n) {
+                return void B[15]
+            }
+        }
+
+        function K(r) {
+            return P ? G(r) : j ? Y(r) : void _[26]
+        }
+
+        function U() {
+            if (P = H(), P) j = _[27][N];
+            else if (W[k + c][I[24]]) try {
+                $ = new ActiveXObject(vr(I[25], y[28], w[26])),
+                    $.open(),
+                    $.write(y[29]),
+                    $.close(),
+                    F = $.w[B[33]][I[27]][_[30]],
+                    j = F.createElement(I[28])
+            } catch (r) {
+                j = W.createElement(N),
+                    F = W[vr(I[29], d[27])] || W.getElementsByTagName(b[17])[I[27]] || W[m[30]]
+            }
+        }
+
+        o[w[31]] = U;
+
+        function V(r, n) {
+            var t = J;
+            if (void 0 === n) return Z(r);
+            if (t = sr, P) z(r, n);
+            else {
+                if (!j) return void B[15];
+                Q(r, n)
+            }
+        }
+
+        o[v + x] = V;
+
+        function Y(r) {
+            X(function() {
+                return r = J(r),
+                    j.getAttribute(r)
+            })()
+        }
+
+        function J(r) {
+            var n = z;
+            n = v;
+            var t = vr(Ir, w[32]),
+                e = new y[31](t + O + s + L, b[31]);
+            return r.replace(new B[13](d[28]), b[34]).replace(e, p[29])
+        }
+
+        function q(r) {
+            try {
+                j.removeItem(r)
+            } catch (n) {}
+        }
+
+        o[M + f + l] = K;
+
+        function Q(r, n) {
+            var t = G;
+            t = cr,
+                X(function() {
+                    var t = M;
+                    r = J(r),
+                        t = K;
+                    try {
+                        j.setAttribute(r, n),
+                            j.save(N)
+                    } catch (e) {}
+                })()
+        }
+
+        function Z(r) {
+            var n, t, e;
+            if (n = t = e = g, P) q(r);
+            else {
+                if (!j) return void t[18];
+                rr(r)
+            }
+        }
+
+        function G(r) {
+            try {
+                return j.getItem(r)
+            } catch (n) {
+                return y[20]
+            }
+        }
+
+        o[fr(w[33], p[30], R[35])] = Z;
+
+        function z(r, n) {
+            try {
+                j.setItem(r, n)
+            } catch (t) {}
+        }
+
+        function rr(r) {
+            X(function() {
+                r = J(r),
+                    j.removeAttribute(r),
+                    j.save(N)
+            })()
+        }
+    }(pr || (pr = {}));
+    var gr = function() {
+            var o, i, u;
+            o = i = u = e;
+            var c, v, s;
+            c = v = s = a;
+            var f, l, g;
+            f = l = g = n;
+            var m, w, I;
+            m = w = I = t;
+            var _, E, A;
+            _ = E = A = r;
+            var C = yr(Cr, U, _[34]),
+                b = vr(A[35], m[31]),
+                R = hr(g[32], c[29], i[36]),
+                T = hr(l[33], g[34], i[37], tr);
+
+            function S(r) {
+                this[m[32]] = r;
+                for (var n = o[15], t = r[i[38]]; t > n; n++) this[n] = i[15]
+            }
+
+            return S[d + p + C][b + h] = function() {
+                    for (var r = this[vr(h, E[36], E[37])], n = [], t = -I[26], e = o[15], a = r[A[20]]; a > e; e++)
+                        for (var u = this[e], f = r[e], d = t += f; n[d] = u & parseInt(v[30], l[35]), --f != s[24];) --d,
+                            u >>= parseInt(i[39], c[31]);
+                    return n
+                },
+                S[vr(w[33], v[32])][_[38]] = function(r) {
+                    var n = dr,
+                        t = this[vr(y, l[36], A[39])],
+                        e = f[26];
+                    n = B;
+                    for (var a = v[24], o = t[l[37]]; o > a; a++) {
+                        var i = t[a],
+                            u = l[26];
+                        do u = (u << parseInt(R + T, g[35])) + r[e++];
+                        while (--i > w[18]);
+                        this[a] = u >>> w[18]
+                    }
+                },
+                S
+        }(),
+        mr;
+    !
+    function(o) {
+        var i, u, c;
+        i = u = c = n;
+        var v, s, f;
+        v = s = f = e;
+        var l, d, p;
+        l = d = p = a;
+        var h, w, I;
+        h = w = I = r;
+        var _, y, E;
+        _ = y = E = t;
+        var A = y[34],
+            C = (nr, U, h[40]),
+            b = p[25];
+
+        function B(r) {
+            for (var n = y[35], t = f[15], e = r[vr(c[38], I[41], H)], a = []; e > t;) {
+                var o = k[r.charAt(t++)] << parseInt(g + A, d[31]) | k[r.charAt(t++)] << parseInt(n + m, h[42]) | k[r.charAt(t++)] << parseInt(I[43], i[35]) | k[r.charAt(t++)];
+                a.push(o >> parseInt(_[36], h[42]), o >> l[31] & parseInt(u[39], i[40]), o & parseInt(d[30], c[35]))
+            }
+            return a
+        }
+
+        function T(r) {
+            for (var n = (O, R, p[24]), t = I[27], e = r[E[24]]; e > t; t++) n = (n << E[37]) - n + r[t];
+            return n & parseInt(E[38], p[33])
+        }
+
+        for (var S = s[40], k = {},
+                x = s[15]; x < parseInt(I[44], l[34]); x++) k[S.charAt(x)] = x;
+
+        function L(r) {
+            var n = B(r),
+                t = n[u[26]];
+            if (t != b) return error = yr(V, u[41], s[41], v[42]),
+                void 0;
+            var e = n[s[26]],
+                a = [];
+            return P(n, +_[39], a, +_[18], e),
+                T(a) == e ? a : void 0
+        }
+
+        function M(r) {
+            var n = T(r),
+                t = [b, n];
+            return P(r, +l[24], t, +p[25], n),
+                N(t)
+        }
+
+        function N(r) {
+            var n, t, e;
+            n = t = e = f;
+            var a, o, u;
+            a = o = u = y;
+            var c, v, s;
+            c = v = s = h;
+            var d, p, g;
+            d = p = g = l;
+            var m, w, I;
+            m = w = I = i;
+            for (var _ = m[42], E = d[24], A = r[c[20]], b = []; A > E;) {
+                var B = r[E++] << parseInt(fr(Z, d[35]), o[39]) | r[E++] << g[31] | r[E++];
+                b.push(S.charAt(B >> parseInt(m[43], t[43])), S.charAt(B >> parseInt(p[36], o[40]) & parseInt(I[44], I[45])), S.charAt(B >> n[44] & parseInt(_ + C, n[42])), S.charAt(B & parseInt(fr(d[37], c[45], or), a[41])))
+            }
+            return b.join(o[19])
+        }
+
+        function P(r, n, t, e, a) {
+            var o, i, u;
+            o = i = u = w;
+            var c, v, s;
+            c = v = s = E;
+            for (var f = r[v[24]]; f > n;) t[e++] = r[n++] ^ a & parseInt(u[46], s[42]),
+                a = ~(a * parseInt(v[43], v[40]))
+        }
+
+        o[E[44]] = N,
+            o[_[45]] = B,
+            o[v[45]] = M,
+            o[y[46]] = L
+    }(mr || (mr = {}));
+    var wr;
+    !
+    function(o) {
+        var i = a[38],
+            u = r[47],
+            c = t[47],
+            v = vr(n[46], a[39], a[40]),
+            s = e[46],
+            f = e[47],
+            l = a[41],
+            d = a[42];
+
+        function p(o) {
+            var i = a[43],
+                u = vr(n[47], e[48], n[48]),
+                c = {},
+                v = function(o, c) {
+                    var s, f, l, d;
+                    for (c = c.replace(n[49], n[12]), c = c.substring(e[26], c[e[38]] - e[26]), s = c.split(e[49]), l = a[24]; l < s[yr(v, sr, t[48])]; l++)
+                        if (f = s[l].split(n[50]), f && !(f[a[44]] < t[39])) {
+                            for (d = n[35]; d < f[r[20]]; d++) f[n[11]] = f[n[11]] + r[48] + f[d];
+                            f[n[26]] = new a[45](r[49]).test(f[n[26]]) ? f[e[15]].substring(r[19], f[e[15]][a[44]] - n[11]) : f[n[26]],
+                                f[n[11]] = new r[50](i + u + w).test(f[n[11]]) ? f[e[26]].substring(t[26], f[r[19]][n[37]] - t[26]) : f[a[18]],
+                                o[f[r[27]]] = f[n[11]]
+                        }
+                    return o
+                };
+            return new a[45](I + _).test(o) && (c = v(c, o)),
+                c
+        }
+
+        function h(n) {
+            for (var t = [], e = a[24]; e < n[r[20]]; e++) t.push(n.charCodeAt(e));
+            return t
+        }
+
+        function g(o) {
+            var u = a[46];
+            if (typeof o === vr(O, a[47], or) && o[a[48]]) try {
+                var c = parseInt(o[a[48]]);
+                switch (c) {
+                    case parseInt(i + u, t[42]):
+                        break;
+                    case parseInt(yr(t[49], r[51], e[50]), e[43]):
+                        top[t[50]][n[51]] = o[e[51]];
+                        break;
+                    case parseInt(yr(a[25], j, e[52]), n[52]):
+                        top[n[53]][t[51]] = o[t[52]]
+                }
+            } catch (v) {}
+        }
+
+        function m(r, n, t) {
+
+        }
+
+        function L() {
+            var e, a, o;
+            e = a = o = r;
+            var i, u, c;
+            i = u = c = n;
+            var v, s, f;
+            v = s = f = t;
+            var l = f[53],
+                d = c[54],
+                p = new e[52];
+            return typeof TOKEN_SERVER_TIME == y + l + d ? s[18] : (time = parseInt(TOKEN_SERVER_TIME), time)
+        }
+
+        function M() {
+            var o = new t[54];
+            try {
+                return time = n[2].now(),
+                    time / parseInt(fr(a[50], a[51], r[53]), t[40]) >>> e[15]
+            } catch (i) {
+                return time = o.getTime(),
+                    time / parseInt(e[53], a[25]) >>> r[27]
+            }
+        }
+
+        function N(r) {
+            for (var a = t[18], o = r[t[24]] - n[11]; o >= e[15]; o--) a = a << e[26] | +r[o];
+            return a
+        }
+
+        function P(a) {
+            var o = new r[50](n[55]);
+            if (K(a)) return a;
+            var i = o.test(a) ? -e[54] : -t[39],
+                u = a.split(r[54]);
+            return u.slice(i).join(fr(n[56], t[55], E))
+        }
+
+        function j(t) {
+            for (var o = n[26], i = e[15], u = t[vr(r[55], a[52], D)]; u > i; i++) o = (o << r[56]) - o + t.charCodeAt(i),
+                o >>>= n[26];
+            return o
+        }
+
+        function W(n, o) {
+            var i = new a[45](t[56], yr(r[57], $, t[57], r[58])),
+                u = new a[45](t[58]);
+            if (n) {
+                var c = n.match(i);
+                if (c) {
+                    var v = c[e[26]];
+                    return o && u.test(v) && (v = v.split(t[59]).pop().split(r[48])[e[15]]),
+                        v
+                }
+            }
+        }
+
+        function $(o) {
+            var i = n[57],
+                u = vr(e[55], e[56]),
+                f = e[4];
+            if (!(o > t[60])) {
+                o = o || a[24];
+                var l = parseInt(E + c + A, r[42]),
+                    d = n[14].createElement(e[57]);
+                d[r[59]] = n[58] + parseInt((new a[53]).getTime() / l) + r[60],
+                    d[r[61]] = function() {
+                        var n = a[46];
+                        cr = r[19],
+                            setTimeout(function() {
+                                    $(++o)
+                                },
+                                o * parseInt(C + n, a[33]))
+                    },
+                    d[t[61]] = d[hr(a[54], a[55], t[62])] = function() {
+                        var a = n[59];
+                        this[i + v + u + b] && this[e[58]] !== n[60] && this[s + B + a + f] !== e[59] && this[t[63]] !== n[61] || (cr = e[15], d[hr(N, r[62], n[62], e[25])] = d[t[64]] = r[63])
+                    },
+                    e[60][e[61]].appendChild(d)
+            }
+        }
+
+        function F() {
+            var r = a[56];
+            return Math.random() * parseInt(R + T + f + r, t[42]) >>> n[26]
+        }
+
+        function X(r) {
+            var e = new n[31](fr(t[65], t[66], a[57]), yr(c, n[63], t[57]));
+            if (r) {
+                var o = r.match(e);
+                return o
+            }
+        }
+
+        o[S + k] = p,
+            o[r[64]] = $,
+            o[t[67]] = g,
+            o[t[68]] = h,
+            o[t[69]] = j,
+            o[t[70]] = F,
+            o[r[65]] = K,
+            o[x + l] = P,
+            o[t[71]] = W,
+            o[t[72]] = X,
+            o[hr(r[66], t[73], r[67], C)] = N,
+            o[t[74]] = M,
+            o[d + O] = L;
+
+        function K(n) {
+            return new r[50](t[75]).test(n)
+        }
+
+        o[r[68]] = m
+    }(wr || (wr = {}));
+    var Ir;
+    !
+    function(o) {
+        var i = t[76],
+            u = t[77],
+            c = n[65],
+            v = t[78],
+            s = a[24],
+            f = n[26],
+            l = t[18],
+            d = t[18],
+            p = e[15],
+            h = a[24],
+            g = r[69],
+            m = '';
+        wr.eventBind(e[60], n[67], E),
+            wr.eventBind(r[71], t[79], E),
+            wr.eventBind(t[20], hr(e[64], A, a[59]), b),
+            wr.eventBind(e[60], r[72], y);
+
+        function w() {
+            return f
+        }
+
+        function I(r) {
+            f++
+        }
+
+        function _() {
+            return {
+                x: p,
+                y: h,
+                trusted: g
+            }
+        }
+
+        function y(r) {
+            d++
+        }
+
+        function E(r) {
+            s++
+        }
+
+        function C() {
+            return l
+        }
+
+        function b(r) {
+            var o, i, u;
+            o = i = u = n;
+            var c, s, f;
+            c = s = f = t;
+            var d, m, w;
+            d = m = w = e;
+            var I, _, y;
+            I = _ = y = a;
+            var E = I[60],
+                A = d[65];
+            l++,
+            g = void 0 == r[E + A + v] || r[yr(f[80], s[81], i[68])],
+                p = r[s[82]],
+                h = r[c[83]]
+        }
+
+        function B() {
+            return d
+        }
+
+        function R() {
+            return s
+        }
+
+        o[r[73]] = R,
+            o[a[61]] = w,
+            o[fr(a[62], n[69])] = C,
+            o[n[70]] = B,
+            o[r[74]] = _
+    }(Ir || (Ir = {}));
+    var _r;
+    !
+    function(u) {
+        var v = fr(n[71], t[84]),
+            s = r[75],
+            f = yr(dr, n[72], e[66], $),
+            l = r[76],
+            d = e[67],
+            p = r[77],
+            h = hr(dr, r[78], a[63], n[73]),
+            g = r[79],
+            m = n[74];
+        BROWSER_LIST = {};
+
+        function w() {
+            var t, e, a;
+            t = e = a = r;
+            var o, i, u;
+            o = i = u = n;
+            return wr.booleanToDecimal(c)
+        }
+
+        function I(t) {
+            for (var o = n[26]; o < y[e[38]]; o++) {
+                var i = y[o][r[94]];
+                if (t.test(i)) return !a[24]
+            }
+            return !a[18]
+        }
+
+        function E(t) {
+
+        }
+
+        function A() {
+            return a[73]
+        }
+
+        function B() {
+            return n[20]
+        }
+
+        function T() {
+            return I(new t[93](r[96]))
+        }
+
+        function S() {
+            return I(new a[45](t[98], r[97]))
+        }
+
+        function k() {
+            for (var r in BROWSER_LIST)
+                if (BROWSER_LIST.hasOwnProperty(r)) {
+                    var n = BROWSER_LIST[r];
+                    if (n()) return +r.substr(a[18])
+                }
+            return e[15]
+        }
+
+        function x() {
+            var n, a, o;
+            n = a = o = r;
+            var i, u, c;
+            i = u = c = t;
+            var v, s, f;
+            v = s = f = e;
+            var l = s[75],
+                d = s[76];
+            return I(new u[93](o[98], v[71])) || E(l + F + d + X)
+        }
+
+        function O() {
+
+        }
+
+        function L() {
+            var r, n, t;
+            r = n = t = a;
+            var o, i, u;
+            o = i = u = e;
+            var c = l;
+            return c = p
+        }
+
+        function M() {
+            var r, n, a;
+            r = n = a = t;
+            var o, i, u;
+            o = i = u = e;
+            var c;
+            try {
+                c = i[60].createElement(a[99]).getContext(i[78])
+            } catch (v) {}
+            return !!c
+        }
+
+
+        function J() {
+            var t, e, o;
+            t = e = o = n;
+            var i, u, c;
+            i = u = c = a;
+            var v, s, f;
+            return v = s = f = r,
+                -parseInt(s[100], c[31]) === (new e[2]).getTimezoneOffset()
+        }
+
+        function Q() {
+            try {} catch (e) {
+                return r[101]
+            }
+        }
+
+        function Z() {
+            var n, a, o;
+            n = a = o = e;
+            var i, u, c;
+            i = u = c = r;
+            var v, s, f;
+            return v = s = f = t,
+                plugin_num = s[18],
+                plugin_num
+        }
+
+        var z = [R, x, S, T, L, Q, b, V, O, J, M, q, Y, B, tr, A];
+
+        var nr = [new e[13](n[85]), new n[31](e[82]), new r[50](e[83]), new r[50](t[102]), new n[31](e[84]), new a[45](a[78]), new a[45](e[85]), new e[13](t[103]), new a[45](r[103]), new t[93](r[104]), new a[45](r[105])];
+
+        function tr() {
+            return e[86]
+        }
+
+        u[e[87]] = rr,
+            u[a[79]] = k,
+            u[yr(c, e[88], r[106])] = Z,
+            u[K + U + m] = w
+    }(_r || (_r = {}));
+
+    function yr() {
+        var o = arguments[a[25]];
+        if (!o) return t[19];
+        for (var i = a[19], u = e[14], c = r[27]; c < o.length; c++) {
+            var v = o.charCodeAt(c),
+                s = v ^ u;
+            u = u * c % a[80] + e[89],
+                i += n[86].fromCharCode(s)
+        }
+        return i
+    }
+
+    var Er;
+    !
+    function(o) {
+        var i = a[81],
+            u = t[35],
+            c = r[107],
+            v = vr(S, a[56]),
+            f = r[27],
+            l = r[19],
+            d = a[25],
+            p = n[87],
+            h = parseInt(e[90], r[108]),
+            g = a[82],
+            m = parseInt(vr(s, t[104]), t[39]),
+            w = r[109],
+            I = t[40],
+            _ = parseInt(i + V, n[45]),
+            y = parseInt(u + c, n[52]),
+            E = parseInt(t[105], r[42]),
+            A = e[91],
+            C = parseInt(Y + v, r[42]),
+            b = parseInt(e[92], e[93]),
+            B = t[106],
+            R = parseInt(vr(e[94], e[95]), t[41]),
+            T = parseInt(a[83], e[93]),
+            k;
+
+        function x() {
+            var r = M();
+            return r
+        }
+
+        function O() {
+            var r = t[26],
+                a = n[35],
+                o = e[54],
+                i = n[88];
+            k = new gr([i, i, i, i, r, r, r, o, a, a, a, a, a, a, a, i, a, r]),
+                k[l] = wr.serverTimeNow(),
+                L(),
+                k[B] = cr,
+                k[T] = ur,
+                k[R] = e[15],
+                k[C] = _r.getBrowserFeature(),
+                k[g] = _r.getBrowserIndex(),
+                k[m] = _r.getPluginNum()
+        }
+
+        function L() {
+            var a = dr.getCookie(tr) || pr.get(ar);
+            if (a && a[r[20]] == parseInt(e[96], n[52])) {
+                var o = mr.decode(a);
+                if (o && (k.decodeBuffer(o), k[f] != t[18])) return
+            }
+            k[f] = wr.random()
+        }
+
+        o[a[84]] = O;
+
+        function M() {
+            k[R]++,
+                k[l] = wr.serverTimeNow(),
+                k[d] = wr.timeNow(),
+                k[B] = cr,
+                k[w] = Ir.getMouseMove(),
+                k[I] = Ir.getMouseClick(),
+                k[_] = Ir.getMouseWhell(),
+                k[y] = Ir.getKeyDown(),
+                k[E] = Ir.getClickPos().x,
+                k[A] = Ir.getClickPos().y;
+            var r = k.toBuffer();
+            return mr.encode(r)
+        }
+
+        o[yr(r[3], n[89], e[97])] = x
+    }(Er || (Er = {}));
+    var Ar;
+    !
+    function(o) {
+        var i = n[90],
+            u = a[85],
+            v = r[110],
+            s = a[86],
+            f = t[107],
+            p,
+            h,
+            m,
+            w,
+            I,
+            _;
+
+        function E(r) {
+            return N(r) && dr[a[87]]
+        }
+
+        function A(o) {
+            var i = wr.getOriginFromUrl(o);
+            return i ? !new n[31](yr(r[42], c, t[110]) + w).test(i[r[108]]) || !new e[13](I).test(i[a[18]]) : t[111]
+        }
+
+        function C(e) {
+            var o = (_r, g, Er.update());
+            return e + (new r[50](vr(a[88], a[89])).test(e) ? n[91] : vr(P, a[90], t[112])) + er + t[23] + r[111](o)
+        }
+
+        function b(o, i, u) {
+            if (r[112] in i) return i.apply(o, u);
+            switch (u[n[37]]) {
+                case n[26]:
+                    return i();
+                case a[18]:
+                    return i(u[n[26]]);
+                case r[108]:
+                    return i(u[e[15]], u[r[19]]);
+                default:
+                    return i(u[n[26]], u[r[108]], u[t[17]])
+            }
+        }
+
+        function B() {
+            var r = Er.update();
+            return r
+        }
+
+        function k(r, e, o) {
+            if (!r) return n[20];
+            var i = r[e];
+            if (!i) return t[111];
+            var u = o(i);
+            return d || (u[a[97]] = i + t[19]),
+                u[n[97]] = i,
+                r[e] = u,
+                a[21]
+        }
+
+        function M(o) {
+            var i, u, c;
+            i = u = c = n;
+            var v, s, l;
+            v = s = l = r;
+            var d, p, h;
+            d = p = h = e;
+            var g, m, w;
+            g = m = w = a;
+            var I, _, y;
+            I = _ = y = t;
+            var R = hr(I[121], w[106], d[109]),
+                T;
+            k(o, _[122],
+                    function(r) {
+                        var n = w[107];
+                        return function() {
+                            var t, e, a;
+                            t = e = a = _;
+                            var o, i, u;
+                            o = i = u = l;
+                            var c, v, s;
+                            c = v = s = w;
+                            var f = s[108];
+                            try {
+                                A(arguments[s[18]]) && !E(arguments[o[19]]) ? arguments[a[26]] = C(arguments[s[18]]) : T = B(),
+                                    r.apply(this, arguments),
+                                    A(arguments[i[19]]) || this.setRequestHeader(ar, T)
+                            } catch (d) {
+                                return n + f
+                            }
+                        }
+                    }),
+                k(o, g[109],
+                    function(r) {
+                        var n = b;
+                        n = M;
+                        var t = vr(_[123], u[107]);
+                        return function() {
+                            var n = fr(f, c[108], I[124]),
+                                e = s[122];
+                            try {
+                                if (parseInt(this.status) === parseInt(h[110], v[123])) {
+                                    for (var a = r.apply(this, arguments), o = new p[13](i[109], n + R), u, l, d = {}; u = o.exec(a);) d[u[m[18]].toLowerCase()] = u[v[108]];
+                                    wr.analysisRst(wr.parse(d[ir.toLowerCase()]))
+                                }
+                            } catch (g) {
+                                return e + t
+                            }
+                            return r.apply(this, arguments)
+                        }
+                    })
+        }
+
+        function N(r) {
+            var n = wr.getHostFromUrl(r, e[28]);
+            return n ? _.test(n) : e[28]
+        }
+
+        function j() {
+            var cookie_v;
+            cookie_v = B()
+            return cookie_v
+        }
+
+        o[n[111]] = j
+    }(Ar || (Ar = {}));
+    var Cr;
+    var cookie = (function(a) {
+        function _() {
+            var cookie_v;
+            Er.Init();
+            cookie_v = Ar.Init();
+            return cookie_v
+        }
+
+        return function y() {
+            try {
+                return _()
+            } catch (r) {
+                return r
+            }
+        }
+    })()
+    return cookie()
+}
+
+function v() {
+    var v;
+    v = v_cookie(
+        ["t", 34, '"$', 36, "\fb", 55, "ure", "lJ#K", "Flash", "getBro", "1", "analys", "CHAMELEON_CALLBACK", 30, "\u256f\u0930\u097b\u09ff\u09a4\u0934\u099d\u09c1\u099d\u09d9\u09a7\u09c3\u0995\u09f0\u09d3\u0a62\u0a6f\u09bc\u09ad\u0934", "F,sp-", String, "; expires=", "", 1, "length", "; ", '', '', "addBehavior", ";^l", ">*]+", 0, "div", "&~!", "", "Init", "('&%$#\"![", ">NJ", "\u254e\u096d\u095f", "W$R", "sdelif_esab", "Or)E", "decodeBuffer", 84, "f", "htgnel", 8, "110", "40", "\u2504\u2562", "255", "o", ":", '^".*"$', RegExp, 40, Date, "e9", ".", 19, 5, "t8JOi", "}B", "src", ".js", "onerror", "*q:", null, "getServerTime", "isIPAddr", "8-", "ZX9Y]V8aWs3VQZ7Y", "eventBind", !0, "wheel", '', "keydown", "getMouseMove", "getClickPos", "vent", "me", "MSG", 41, "th", "safari", "ActiveXObject", "maxHeight", "head", "Google Inc.", "vendor", "sgAppName", "opr", 94, "tugw`pj", "chrome", "2345Explorer", "ome", "TheWorld", "name", "\u2553\u253c\u2572\u251d\u2569\u253d\u254f\u252e\u254d\u2526", "Native Client", "i", "Shockwave", "systemLanguage", "740", !1, "plugins", "^ARM", "^iPod", "^BlackBerry", "\u2550\u0978\u094e\u09c1\u09bc\u0928\u0989\u09d8\u099a\u09f3\u09b7\u09dc", "0", 2, 7, "c", encodeURIComponent, "apply", "headers", "8S:+", "\u2560\u2509\u2567\u2503\u256c\u251b", "\u255e\u2530\u2543\u2526\u2554\u2520\u2562\u2507\u2561\u250e\u257c\u2519", "a", 14, ":dB2", "href", "click", "err", 16, "hostname", "`60w", "\fbf", "&X "],
+        [";", "Element", Date, "par", "i", "DOMMous", 21, "xmT", "wserFe", "h", !0, 1, "", Boolean, '', "; domain=", "n 1970 00:", "cookie", "checkcookie", "allow", !1, "delCookie", 2333, "torage", ")*+,/\\\\:;", '', 0, '', "eliflmth", '', "ducument", RegExp, "W", "qsU", 61, 2, "sdelif_esab", "length", "I", "ff", 16, 45, "3", "10010", "77", 8, "6e%d", "DT{e", "$", / /g, ":", "href", 10, "location", "ned", "\\.com\\.cn$|\\.com\\.hk$", 63, "rea", "https://s.thsi.cn/js/chameleon/time.1", "tat", "loaded", "interactive", "WY:ZYS", "E?`a", "addEventListener", "eScroll", "onmousewheel", "mousemove", "\u255e\u096e\u096e\u09e3\u09a5\u092e\u099a\u09d4\u0990", "\u2550\u2535\u2541\u250c\u2563\u2516\u2565\u2500\u2543\u252f\u2546\u2525\u254e", "getKeyDown", "H69<J", "v~g-", "", "ature", "callPhantom", "ActiveXObject", "Uint8Array", "WeakMap", "JX%<", "chrome", "@L:!", "20", "language", "localStorage", "^Win32", String, 3, 4, "=XAE", "hea", "&", "/", "\\R$", '^R"VP', "s", "include", "_raw", "x.", "isRst", "SCRIPT", "ta", "base", "$?", "^_self$", "#", "unload", "ro", "\u2550", "^(.*?):[ \\t]*([^\\r\\n]*)\\r?$", "g", "Init", "t6?x}", "\u2574\u0955\u097b\u09dc\u0995\u0911\u09ab\u09fe\u09ba\u09e2\u098e\u09fe\u09f9\u09f9\u09f3\u0a55", "=d' "],
+        ["<=>?@[\\]^", "e", "HE9", "tot", "\u2503", "0", "dyS", "se", "getRoot", "NR", "nd", 60, "ng", "s", "get", "mit", 13, 3, 0, "", '', "\u255f\u253a\u255b\u253f", "getCookie", "=", "length", "V587", 1, String, !0, "___", "\u2553\u2536\u255a", "uBot", "base_fileds", 32, "2", "1", "20", 5, "255", 2, 8, 16, 10, "203", "base64Encode", "base64Decode", "decode", "760", "\u255b\u0978\u0954\u09f6\u09a4\u0935", 70, "location", "href", "redirect_url", "efi", Date, "\u2519", "^\\s*(?:https?:)?\\/{2,}([^\\/\\?\\#\\\\]+)", "\u255e", "[@:]", "@", 7, "onload", 'WY$PYS/FLV"P[_7[_R', "readyState", "onreadystatechange", '"^w', "\u2569\u2535\u2546\u256c\u2544\u257b\u2541\u2569\u2501\u2575\u2501\u2571\u2502\u253d\u2507\u252e\u2507\u2538\u2564\u254b\u2530\u2502\u252e\u2553\u257b\u2520\u257e\u2522\u250d\u2551\u256e\u2532\u2511\u254d\u2511\u254c\u2567\u254e", "analysisRst", "strToBytes", "strhash", "random", "getHostFromUrl", "getOriginFromUrl", 83, "timeNow", "^(\\d+\\.)+\\d+$", "d", "v", "ted", "touchmove", 85, "F(K9i", "clientX", "clientY", "\u257a\u2515\u256f\u253c", "postMessage", '', "ActiveXObject", "Apple Computer, Inc.", "Q", "chr", "\u2558\u2535\u2550", "BIDUBrowser", RegExp, "QQBrowser", "ro", "aef", "msDoNotTrack", "PDF|Acrobat", "canvas", "yE", "\u255b\u253a\u2554\u2533\u2546\u2527\u2540\u2525\u2556", "^Android", "^Linux [ix]\\d+", "011", "13", 15, "sub", "addEventListener", "jsonp_ignore", "\u2569", !1, 'L"', "Sj", "T{_,", "q*", "i", "tagName", "et", "{'K", "Pp<", "#x'", "open", "rS", "KN3", "#", "protocol", "\\.", "DEDAOL_NOELEMAHC"],
+        [83, "ffer", "\u2505", "20", "e", "ngsE", Error, "est", "\u2552\u095b\u0956\u09f0\u09a3\u0935\u09c0\u09e2", "1", "sr", "hexin-v", "", RegExp, 9527, 0, "**l>", "head", "Thu, 01 Ja", "00:00 GMT", "allow", "=", "; path=", "cookie", "Init", 33, 1, "setCookie", !0, "localS", "`{|}~]", "g", '', "frames", "___$&", 56, "	", "\b", "length", "10", "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789-_", "\u2552\u096f\u0948\u09fe\u09a2", 16, 2, 6, "encode", "rea", "729", "*.", ",", "\u2506\u092c\u090b\u09a0\u09e1\u096d\u09df\u0981\u09c4\u098c", "redirect_url", "\u2506\u092d\u090a\u09a3", "1111101000", 3, 47, "tat", "script", "readyState", "complete", '', "body", "onwheel", "mousewheel", 37, "rus", "\u2554\u0975", "chr", "ActiveXObject", "WeakMap", "aT1Kg", "i", 24, "\u2554\u253c\u254e\u2521\u254c\u2529", "\u2547\u0971\u094f\u09f6\u09b9\u0933\u099d", "Shockwav", "hockwave", "$cdc_asdjflasutopfhvcZLmcfl_", "webgl2", "2>n|", "plugins", "platform", "^Win64", "^Linux armv|Android", "^iPhone", "^MacIntel", !1, "getPlatform", "6Y,", 2333, "100", 12, "14", 10, 36, "01", "60", "\u2542\u096d\u095e\u09f0\u09a4\u0938", "j", 17, "Request", "prototype", "`z}lc", "error", "s", "r", "target", "\u255e", "A", "U", "193", "host", "$"],
+        ["se", "g@g?", Array, "*Y", Number, "^{.", "*}$", "und", "429", "496", "imeNow", "etti", "rg", "v", "hexin-v", Error, "L_%\\T8", ".baidu.", 1, "", Function, !0, " ", '', 0, 2, "#default#userData", "ydob", "^d", 89, "11111111", 8, "epytotorp", 10, 16, "\u2506\u2536\u2506\u2536\u2506", "14", 13, "10", "Syd", 44, "Domain", "serverT", '^"', "length", RegExp, "00", "tcejbo", "status_code", "n", 66, "\u2506\u2531\u2504\u2534", "htgnel", Date, "L%", 67, "5", "?)'", '', "[[?VS", "isT", "getMouseWhell", "}}", "TR", "ActiveXObject", "WE", "python", "Maxthon", 97, "chrome", "Ryp", "UBrowser", 54, !1, "ontouchstart", "\u254d\u0975\u0917\u09f2\u09be", "iso-8859-1", "defaultCharset", "^iPad", "getBrowserIndex", 256, "1", 5, "17", "Init", "XMLHttp", "tar", "allow", "@*", "?\\", "?", "\u2571\u2503\u256a\u2546\u2566\u2556\u2567\u2547\u2501\u2564\u2506\u2526\u2514\u2524\u2511\u2521\u2501\u2531\u2501\u253b\u250b\u253b\u2501\u2531\u2501\u2521\u2566\u252b\u257f", "den", "tia", 94, "ls", "\u2554\u2526\u2543", "_str", 37, "append", "Child", "\u255f", "\u2569\u0975\u094e\u09e5\u09a0\u092e\u09d1\u09ed\u09ce", "srcElement", "parentNode", "\u2543\u2522\u2545\u250b\u256a\u2507\u2562", "}*", "err", "or", "getAllResponseHeaders", "\\.?", "\\."]
+    );
+    return v
 }
```

### Comparing `adata-1.2.4/adata/common/utils/cookie.py` & `adata-2.0.0b0/adata/common/utils/cookie.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# -*- coding: utf-8 -*-
-"""
-@desc: 获取cookie的工具类
-@author: 1nchaos
-@time: 2023/5/5
-@log: change log
-"""
-import os
-
-from py_mini_racer import py_mini_racer
-
-
-def ths_cookie(js_path="ths.js"):
-    """获取同花顺cookie"""
-    js_code = py_mini_racer.MiniRacer()
-    js_content = get_file_content_ths(file_path=js_path)
-    js_code.eval(js_content)
-    return 'v=' + js_code.call("v") + ";"
-
-
-def get_file_content_ths(file_path: str = None) -> str:
-    """
-    获取 JS 文件的内容
-    :param file_path:  JS 文件名
-    :return: 文件内容
-    """
-    _curpath = os.path.normpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
-    f_path = _curpath.replace('utils', 'js/') + file_path
-    with open(f_path) as f:
-        file_data = f.read()
-    return file_data
-
-
-if __name__ == '__main__':
-    print(ths_cookie())
+# -*- coding: utf-8 -*-
+"""
+@desc: 获取cookie的工具类
+@author: 1nchaos
+@time: 2023/5/5
+@log: change log
+"""
+import os
+
+from py_mini_racer import py_mini_racer
+
+
+def ths_cookie(js_path="ths.js"):
+    """获取同花顺cookie"""
+    js_code = py_mini_racer.MiniRacer()
+    js_content = get_file_content_ths(file_path=js_path)
+    js_code.eval(js_content)
+    return 'v=' + js_code.call("v") + ";"
+
+
+def get_file_content_ths(file_path: str = None) -> str:
+    """
+    获取 JS 文件的内容
+    :param file_path:  JS 文件名
+    :return: 文件内容
+    """
+    _curpath = os.path.normpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
+    f_path = _curpath.replace('utils', 'js/') + file_path
+    with open(f_path) as f:
+        file_data = f.read()
+    return file_data
+
+
+if __name__ == '__main__':
+    print(ths_cookie())
```

### Comparing `adata-1.2.4/adata/common/utils/snowflake.py` & `adata-2.0.0b0/adata/common/utils/snowflake.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-# -*- coding: utf-8 -*-
-"""
-@desc: 雪花算法 生成唯一 全局id
-       使用方式 单例模式使用
-       import worker
-@author: 1nchaos
-@time: 2022/4/8
-@log: change log
-"""
-
-import logging
-import random
-import time
-
-# 64位ID的划分
-WORKER_ID_BITS = 5
-DATACENTER_ID_BITS = 5
-SEQUENCE_BITS = 12
-
-# 最大取值计算 # 2**5-1 0b11111
-MAX_WORKER_ID = -1 ^ (-1 << WORKER_ID_BITS)
-MAX_DATACENTER_ID = -1 ^ (-1 << DATACENTER_ID_BITS)
-
-# 移位偏移计算
-WORKER_ID_SHIFT = SEQUENCE_BITS
-DATACENTER_ID_SHIFT = SEQUENCE_BITS + WORKER_ID_BITS
-TIMESTAMP_LEFT_SHIFT = SEQUENCE_BITS + WORKER_ID_BITS + DATACENTER_ID_BITS
-
-# 序号循环掩码
-SEQUENCE_MASK = -1 ^ (-1 << SEQUENCE_BITS)
-
-# Twitter元年时间戳
-TWEPOCH = 1580885600337
-
-logger = logging.getLogger('flask.app')
-
-
-class _IdWorker(object):
-    """
-    用于生成雪花算法 id的对象
-    """
-
-    def __init__(self, datacenter_id=1, worker_id=1, sequence=0):
-        """
-        初始化
-        :param datacenter_id: 数据中心（机器区域）ID
-        :param worker_id: 机器ID
-        :param sequence: 其实序号
-        """
-        # sanity check
-        if worker_id > MAX_WORKER_ID or worker_id < 0:
-            raise ValueError('worker_id值越界')
-        if datacenter_id > MAX_DATACENTER_ID or datacenter_id < 0:
-            raise ValueError('datacenter_id值越界')
-
-        self.worker_id = worker_id
-        self.datacenter_id = datacenter_id
-        self.sequence = sequence
-        # 上次计算的时间戳
-        self.last_timestamp = -1
-
-
-    def _gen_timestamp(self):
-        """
-        生成整数时间戳
-        :return:int timestamp
-        """
-        return int(time.time() * 1000)
-
-    def _til_next_millis(self, last_timestamp):
-        """
-        等到下一毫秒
-        """
-        timestamp = self._gen_timestamp()
-        while timestamp <= last_timestamp:
-            timestamp = self._gen_timestamp()
-        return timestamp
-
-    def id(self):
-        """
-        获取新ID
-        :return:
-        """
-        timestamp = self._gen_timestamp()
-
-        # 时钟回拨
-        if timestamp < self.last_timestamp:
-            logging.error('clock is moving backwards. Rejecting requests until {}'.format(self.last_timestamp))
-            raise
-
-        if timestamp == self.last_timestamp:
-            self.sequence = (self.sequence + 1) & SEQUENCE_MASK
-            if self.sequence == 0:
-                timestamp = self._til_next_millis(self.last_timestamp)
-        else:
-            self.sequence = 0
-
-        self.last_timestamp = timestamp
-
-        new_id = ((timestamp - TWEPOCH) << TIMESTAMP_LEFT_SHIFT) | (self.datacenter_id << DATACENTER_ID_SHIFT) | \
-                 (self.worker_id << WORKER_ID_SHIFT) | self.sequence
-        return new_id
-
-
-# 随机分配机器id 和 数据中心
-worker = _IdWorker(random.randint(0, 31), random.randint(0, 31))
-
-if __name__ == '__main__':
-    print(worker.id())
+# -*- coding: utf-8 -*-
+"""
+@desc: 雪花算法 生成唯一 全局id
+       使用方式 单例模式使用
+       import worker
+@author: 1nchaos
+@time: 2022/4/8
+@log: change log
+"""
+
+import logging
+import random
+import time
+
+# 64位ID的划分
+WORKER_ID_BITS = 5
+DATACENTER_ID_BITS = 5
+SEQUENCE_BITS = 12
+
+# 最大取值计算 # 2**5-1 0b11111
+MAX_WORKER_ID = -1 ^ (-1 << WORKER_ID_BITS)
+MAX_DATACENTER_ID = -1 ^ (-1 << DATACENTER_ID_BITS)
+
+# 移位偏移计算
+WORKER_ID_SHIFT = SEQUENCE_BITS
+DATACENTER_ID_SHIFT = SEQUENCE_BITS + WORKER_ID_BITS
+TIMESTAMP_LEFT_SHIFT = SEQUENCE_BITS + WORKER_ID_BITS + DATACENTER_ID_BITS
+
+# 序号循环掩码
+SEQUENCE_MASK = -1 ^ (-1 << SEQUENCE_BITS)
+
+# Twitter元年时间戳
+TWEPOCH = 1580885600337
+
+logger = logging.getLogger('flask.app')
+
+
+class _IdWorker(object):
+    """
+    用于生成雪花算法 id的对象
+    """
+
+    def __init__(self, datacenter_id=1, worker_id=1, sequence=0):
+        """
+        初始化
+        :param datacenter_id: 数据中心（机器区域）ID
+        :param worker_id: 机器ID
+        :param sequence: 其实序号
+        """
+        # sanity check
+        if worker_id > MAX_WORKER_ID or worker_id < 0:
+            raise ValueError('worker_id值越界')
+        if datacenter_id > MAX_DATACENTER_ID or datacenter_id < 0:
+            raise ValueError('datacenter_id值越界')
+
+        self.worker_id = worker_id
+        self.datacenter_id = datacenter_id
+        self.sequence = sequence
+        # 上次计算的时间戳
+        self.last_timestamp = -1
+
+
+    def _gen_timestamp(self):
+        """
+        生成整数时间戳
+        :return:int timestamp
+        """
+        return int(time.time() * 1000)
+
+    def _til_next_millis(self, last_timestamp):
+        """
+        等到下一毫秒
+        """
+        timestamp = self._gen_timestamp()
+        while timestamp <= last_timestamp:
+            timestamp = self._gen_timestamp()
+        return timestamp
+
+    def id(self):
+        """
+        获取新ID
+        :return:
+        """
+        timestamp = self._gen_timestamp()
+
+        # 时钟回拨
+        if timestamp < self.last_timestamp:
+            logging.error('clock is moving backwards. Rejecting requests until {}'.format(self.last_timestamp))
+            raise
+
+        if timestamp == self.last_timestamp:
+            self.sequence = (self.sequence + 1) & SEQUENCE_MASK
+            if self.sequence == 0:
+                timestamp = self._til_next_millis(self.last_timestamp)
+        else:
+            self.sequence = 0
+
+        self.last_timestamp = timestamp
+
+        new_id = ((timestamp - TWEPOCH) << TIMESTAMP_LEFT_SHIFT) | (self.datacenter_id << DATACENTER_ID_SHIFT) | \
+                 (self.worker_id << WORKER_ID_SHIFT) | self.sequence
+        return new_id
+
+
+# 随机分配机器id 和 数据中心
+worker = _IdWorker(random.randint(0, 31), random.randint(0, 31))
+
+if __name__ == '__main__':
+    print(worker.id())
```

### Comparing `adata-1.2.4/adata/common/utils/sunrequests.py` & `adata-2.0.0b0/adata/common/utils/sunrequests.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-# -*- coding: utf-8 -*-
-"""
-代理:https://jahttp.zhimaruanjian.com/getapi/
-
-@desc: adata 请求工具类
-@author: 1nchaos
-@time:2023/3/30
-@log: 封装请求次数
-"""
-
-import threading
-import time
-
-import requests
-
-
-class SunProxy(object):
-    _data = {}
-    _instance_lock = threading.Lock()
-
-    def __init__(self):
-        pass
-
-    def __new__(cls, *args, **kwargs):
-        if not hasattr(SunProxy, "_instance"):
-            with SunProxy._instance_lock:
-                if not hasattr(SunProxy, "_instance"):
-                    SunProxy._instance = object.__new__(cls)
-
-    @classmethod
-    def set(cls, key, value):
-        cls._data[key] = value
-
-    @classmethod
-    def get(cls, key):
-        return cls._data.get(key)
-
-    @classmethod
-    def delete(cls, key):
-        if key in cls._data:
-            del cls._data[key]
-
-
-class SunRequests(object):
-    def __init__(self, sun_proxy: SunProxy = None) -> None:
-        super().__init__()
-        self.sun_proxy = sun_proxy
-
-    def request(self, method='get', url=None, times=3, retry_wait_time=1588, proxies=None, wait_time=None, **kwargs):
-        """
-        简单封装的请求，参考requests，增加循环次数和次数之间的等待时间
-        :param proxies: 代理配置
-        :param method: 请求方法： get；post
-        :param url: url
-        :param times: 次数，int
-        :param retry_wait_time: 重试等待时间，毫秒
-        :param wait_time: 等待时间：毫秒；表示每个请求的间隔时间，在请求之前等待sleep，主要用于防止请求太频繁的限制。
-        :param kwargs: 其它 requests 参数，用法相同
-        :return: res
-        """
-        # 1. 获取设置代理
-        proxies = self.__get_proxies(proxies)
-        # 2. 请求数据结果
-        res = None
-        for i in range(times):
-            if wait_time:
-                time.sleep(wait_time / 1000)
-            res = requests.request(method=method, url=url, proxies=proxies, **kwargs)
-            if res.status_code in (200, 404):
-                return res
-            time.sleep(retry_wait_time / 1000)
-            if i == times - 1:
-                return res
-        return res
-
-    def __get_proxies(self, proxies):
-        """
-        获取代理配置
-        """
-        if proxies is None:
-            proxies = {}
-        is_proxy = SunProxy.get('is_proxy')
-        ip = SunProxy.get('ip')
-        proxy_url = SunProxy.get('proxy_url')
-        if not ip and is_proxy and proxy_url:
-            ip = requests.get(url=proxy_url).text.replace('\r\n', '') \
-                .replace('\r', '').replace('\n', '').replace('\t', '')
-        if is_proxy and ip:
-            proxies = {'https': f"http://{ip}", 'http': f"http://{ip}"}
-        return proxies
-
-
-sun_requests = SunRequests()
+# -*- coding: utf-8 -*-
+"""
+代理:https://jahttp.zhimaruanjian.com/getapi/
+
+@desc: adata 请求工具类
+@author: 1nchaos
+@time:2023/3/30
+@log: 封装请求次数
+"""
+
+import threading
+import time
+
+import requests
+
+
+class SunProxy(object):
+    _data = {}
+    _instance_lock = threading.Lock()
+
+    def __init__(self):
+        pass
+
+    def __new__(cls, *args, **kwargs):
+        if not hasattr(SunProxy, "_instance"):
+            with SunProxy._instance_lock:
+                if not hasattr(SunProxy, "_instance"):
+                    SunProxy._instance = object.__new__(cls)
+
+    @classmethod
+    def set(cls, key, value):
+        cls._data[key] = value
+
+    @classmethod
+    def get(cls, key):
+        return cls._data.get(key)
+
+    @classmethod
+    def delete(cls, key):
+        if key in cls._data:
+            del cls._data[key]
+
+
+class SunRequests(object):
+    def __init__(self, sun_proxy: SunProxy = None) -> None:
+        super().__init__()
+        self.sun_proxy = sun_proxy
+
+    def request(self, method='get', url=None, times=3, retry_wait_time=1588, proxies=None, wait_time=None, **kwargs):
+        """
+        简单封装的请求，参考requests，增加循环次数和次数之间的等待时间
+        :param proxies: 代理配置
+        :param method: 请求方法： get；post
+        :param url: url
+        :param times: 次数，int
+        :param retry_wait_time: 重试等待时间，毫秒
+        :param wait_time: 等待时间：毫秒；表示每个请求的间隔时间，在请求之前等待sleep，主要用于防止请求太频繁的限制。
+        :param kwargs: 其它 requests 参数，用法相同
+        :return: res
+        """
+        # 1. 获取设置代理
+        proxies = self.__get_proxies(proxies)
+        # 2. 请求数据结果
+        res = None
+        for i in range(times):
+            if wait_time:
+                time.sleep(wait_time / 1000)
+            res = requests.request(method=method, url=url, proxies=proxies, **kwargs)
+            if res.status_code in (200, 404):
+                return res
+            time.sleep(retry_wait_time / 1000)
+            if i == times - 1:
+                return res
+        return res
+
+    def __get_proxies(self, proxies):
+        """
+        获取代理配置
+        """
+        if proxies is None:
+            proxies = {}
+        is_proxy = SunProxy.get('is_proxy')
+        ip = SunProxy.get('ip')
+        proxy_url = SunProxy.get('proxy_url')
+        if not ip and is_proxy and proxy_url:
+            ip = requests.get(url=proxy_url).text.replace('\r\n', '') \
+                .replace('\r', '').replace('\n', '').replace('\t', '')
+        if is_proxy and ip:
+            proxies = {'https': f"http://{ip}", 'http': f"http://{ip}"}
+        return proxies
+
+
+sun_requests = SunRequests()
```

### Comparing `adata-1.2.4/adata/fund/info/fund_info.py` & `adata-2.0.0b0/adata/fund/info/fund_info.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-# -*- coding: utf-8 -*-
-"""
-@desc: 基金信息 etf
-
-http://quote.eastmoney.com/center/gridlist.html#fund_etf
-
-@author: 1nchaos
-@time: 2023/5/31
-@log: change log
-"""
-import json
-import math
-
-import pandas as pd
-
-from adata.common import requests
-from adata.common.base.base_ths import BaseThs
-from adata.common.exception.exception_msg import THS_IP_LIMIT_RES, THS_IP_LIMIT_MSG
-
-
-class FundInfo(BaseThs):
-    """
-    基金信息
-    """
-    __ETF_INFO_COLUMNS = ['fund_code', 'short_name', 'net_value']
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def all_etf_exchange_traded_info(self, wait_time=None):
-        """
-        获取所有etl（场内）的信息
-        :return: ['fund_code', 'short_name', 'net_value']
-        fund_code: 基金代码
-        short_name: 简称
-        net_value: 最新净值
-        """
-        return self.__all_etf_exchange_traded_info_east(wait_time=wait_time)
-
-    def __all_etf_exchange_traded_info_ths(self, wait_time):
-        """
-        http://www.iwencai.com/customized/chart/get-robot-data
-        """
-        wc_url = 'http://www.iwencai.com/customized/chart/get-robot-data'
-        # 1. url拼接页码等参数
-        data = []
-        total_pages = 1
-        curr_page = 1
-        while curr_page <= total_pages:
-            params = {'source': "Ths_iwencai_Xuangu", 'version': '2.0', 'query_area': '', 'block_list': '',
-                      'add_info': '{\"urp\":{\"scene\":1,\"company\":1,\"business\":1},\"contentType\":\"json\",\"searchInfo\":true}',
-                      'question': '基金市场类型包含ETF(场内)', 'perpage': 100, 'page': curr_page, 'secondary_intent': 'fund',
-                      'log_info': '{\"input_type\":\"typewrite\"}',
-                      'rsh': 'Ths_iwencai_Xuangu_kn63wc5it6hwdapiye6hplx8h86di15p'}
-
-            headers = {'Host': 'www.iwencai.com', 'Content-Type': 'application/json',
-                       'Origin': 'http://www.iwencai.com',
-                       'Accept': 'application/json, text/plain, */*', 'hexin-v': self.wencai_hexin_v()}
-            res = requests.request(method='post', url=wc_url, headers=headers, data=json.dumps(params),
-                                   wait_time=wait_time)
-            curr_page += 1
-            # 2. 判断请求是否成功
-            if res.status_code != 200:
-                continue
-            text = res.text.encode('utf-8').decode('unicode escape')
-            if THS_IP_LIMIT_RES in text:
-                return Exception(THS_IP_LIMIT_MSG)
-            if 'ETF(场内)' not in text:
-                break
-            res_json = res.json()
-            data_dic = res_json['answer']['components'][0]['data']
-            # 3 .获取总的页数
-            if total_pages == 1:
-                total_pages = math.ceil(data_dic['meta']['extra']['code_count'] / 100)
-            # 4. 解析数据
-            page_data = []
-            data_list = data_dic['datas']
-            for one in data_list:
-                if 'ETF(场内)' in one['基金@基金市场类型']:
-                    page_data.append({'fund_code': one['code'], 'short_name': one['基金简称'],
-                                      'net_value': one['基金@最新单位净值'], 'net_date': one['基金@最新净值日期'],
-                                      'exchange': one['基金代码'].split('.')[1]})
-            data.extend(page_data)
-            # 5. 封装数据
-            if not data:
-                return pd.DataFrame(data=data, columns=self.__ETF_INFO_COLUMNS)
-        result_df = pd.DataFrame(data=data, columns=self.__ETF_INFO_COLUMNS)
-        data.clear()
-        return result_df[self.__ETF_INFO_COLUMNS]
-
-    def __all_etf_exchange_traded_info_east(self, wait_time):
-        """
-        http://68.push2.eastmoney.com/api/qt/clist/get?cb=jQuery1124047482019788167995_1690884441114&pn=1&pz=500&po=1&np=1&ut=bd1d9ddb04089700cf9c27f6f7426281&fltt=2&invt=2&wbp2u=|0|0|0|web&fid=f3&fs=b:MK0021,b:MK0022,b:MK0023,b:MK0024&fields=f12,f14,f2&_=1690884441121
-        :param wait_time: 等待时间
-        :return:
-        """
-        curr_page = 1
-        data = []
-        while curr_page < 5:
-            url = f"http://68.push2.eastmoney.com/api/qt/clist/get?cb=jQuery1124047482019788167995_1690884441114" \
-                  f"&pn={curr_page}&pz=500&po=1&np=1&ut=bd1d9ddb04089700cf9c27f6f7426281&fltt=2&invt=2&wbp2u=|0|0|0|web" \
-                  f"&fid=f3&fs=b:MK0021,b:MK0022,b:MK0023,b:MK0024&fields=f12,f14,f2&_=1690884441121"
-            text = requests.request('get', url, headers={}, proxies={}, wait_time=wait_time).text
-            res_json = json.loads(text[text.index('{'):-2])
-            res_data = res_json['data']
-            if not res_data:
-                break
-            res_data = res_data['diff']
-            for _ in res_data:
-                data.append({'fund_code': _['f12'], 'short_name': _['f14'], 'net_value': _['f2']})
-            curr_page += 1
-        result_df = pd.DataFrame(data=data, columns=self.__ETF_INFO_COLUMNS)
-        return result_df
-
-
-if __name__ == '__main__':
-    print(FundInfo().all_etf_exchange_traded_info())
+# -*- coding: utf-8 -*-
+"""
+@desc: 基金信息 etf
+
+http://quote.eastmoney.com/center/gridlist.html#fund_etf
+
+@author: 1nchaos
+@time: 2023/5/31
+@log: change log
+"""
+import json
+import math
+
+import pandas as pd
+
+from adata.common import requests
+from adata.common.base.base_ths import BaseThs
+from adata.common.exception.exception_msg import THS_IP_LIMIT_RES, THS_IP_LIMIT_MSG
+
+
+class FundInfo(BaseThs):
+    """
+    基金信息
+    """
+    __ETF_INFO_COLUMNS = ['fund_code', 'short_name', 'net_value']
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def all_etf_exchange_traded_info(self, wait_time=None):
+        """
+        获取所有etl（场内）的信息
+        :return: ['fund_code', 'short_name', 'net_value']
+        fund_code: 基金代码
+        short_name: 简称
+        net_value: 最新净值
+        """
+        return self.__all_etf_exchange_traded_info_east(wait_time=wait_time)
+
+    def __all_etf_exchange_traded_info_ths(self, wait_time):
+        """
+        http://www.iwencai.com/customized/chart/get-robot-data
+        """
+        wc_url = 'http://www.iwencai.com/customized/chart/get-robot-data'
+        # 1. url拼接页码等参数
+        data = []
+        total_pages = 1
+        curr_page = 1
+        while curr_page <= total_pages:
+            params = {'source': "Ths_iwencai_Xuangu", 'version': '2.0', 'query_area': '', 'block_list': '',
+                      'add_info': '{\"urp\":{\"scene\":1,\"company\":1,\"business\":1},\"contentType\":\"json\",\"searchInfo\":true}',
+                      'question': '基金市场类型包含ETF(场内)', 'perpage': 100, 'page': curr_page, 'secondary_intent': 'fund',
+                      'log_info': '{\"input_type\":\"typewrite\"}',
+                      'rsh': 'Ths_iwencai_Xuangu_kn63wc5it6hwdapiye6hplx8h86di15p'}
+
+            headers = {'Host': 'www.iwencai.com', 'Content-Type': 'application/json',
+                       'Origin': 'http://www.iwencai.com',
+                       'Accept': 'application/json, text/plain, */*', 'hexin-v': self.wencai_hexin_v()}
+            res = requests.request(method='post', url=wc_url, headers=headers, data=json.dumps(params),
+                                   wait_time=wait_time)
+            curr_page += 1
+            # 2. 判断请求是否成功
+            if res.status_code != 200:
+                continue
+            text = res.text.encode('utf-8').decode('unicode escape')
+            if THS_IP_LIMIT_RES in text:
+                return Exception(THS_IP_LIMIT_MSG)
+            if 'ETF(场内)' not in text:
+                break
+            res_json = res.json()
+            data_dic = res_json['answer']['components'][0]['data']
+            # 3 .获取总的页数
+            if total_pages == 1:
+                total_pages = math.ceil(data_dic['meta']['extra']['code_count'] / 100)
+            # 4. 解析数据
+            page_data = []
+            data_list = data_dic['datas']
+            for one in data_list:
+                if 'ETF(场内)' in one['基金@基金市场类型']:
+                    page_data.append({'fund_code': one['code'], 'short_name': one['基金简称'],
+                                      'net_value': one['基金@最新单位净值'], 'net_date': one['基金@最新净值日期'],
+                                      'exchange': one['基金代码'].split('.')[1]})
+            data.extend(page_data)
+            # 5. 封装数据
+            if not data:
+                return pd.DataFrame(data=data, columns=self.__ETF_INFO_COLUMNS)
+        result_df = pd.DataFrame(data=data, columns=self.__ETF_INFO_COLUMNS)
+        data.clear()
+        return result_df[self.__ETF_INFO_COLUMNS]
+
+    def __all_etf_exchange_traded_info_east(self, wait_time):
+        """
+        http://68.push2.eastmoney.com/api/qt/clist/get?cb=jQuery1124047482019788167995_1690884441114&pn=1&pz=500&po=1&np=1&ut=bd1d9ddb04089700cf9c27f6f7426281&fltt=2&invt=2&wbp2u=|0|0|0|web&fid=f3&fs=b:MK0021,b:MK0022,b:MK0023,b:MK0024&fields=f12,f14,f2&_=1690884441121
+        :param wait_time: 等待时间
+        :return:
+        """
+        curr_page = 1
+        data = []
+        while curr_page < 5:
+            url = f"http://68.push2.eastmoney.com/api/qt/clist/get?cb=jQuery1124047482019788167995_1690884441114" \
+                  f"&pn={curr_page}&pz=500&po=1&np=1&ut=bd1d9ddb04089700cf9c27f6f7426281&fltt=2&invt=2&wbp2u=|0|0|0|web" \
+                  f"&fid=f3&fs=b:MK0021,b:MK0022,b:MK0023,b:MK0024&fields=f12,f14,f2&_=1690884441121"
+            text = requests.request('get', url, headers={}, proxies={}, wait_time=wait_time).text
+            res_json = json.loads(text[text.index('{'):-2])
+            res_data = res_json['data']
+            if not res_data:
+                break
+            res_data = res_data['diff']
+            for _ in res_data:
+                data.append({'fund_code': _['f12'], 'short_name': _['f14'], 'net_value': _['f2']})
+            curr_page += 1
+        result_df = pd.DataFrame(data=data, columns=self.__ETF_INFO_COLUMNS)
+        return result_df
+
+
+if __name__ == '__main__':
+    print(FundInfo().all_etf_exchange_traded_info())
```

### Comparing `adata-1.2.4/adata/sentiment/north_flow.py` & `adata-2.0.0b0/adata/sentiment/north_flow.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-# -*- coding: utf-8 -*-
-"""
-@desc:
-北向资金
-来源：东方财富
-https://data.eastmoney.com/hsgt/index.html
-https://datacenter-web.eastmoney.com/api/data/v1/get?callback=jQuery112307442704592215257_1690813516314&sortColumns=TRADE_DATE&sortTypes=-1&pageSize=10&pageNumber=2&reportName=RPT_MUTUAL_DEAL_HISTORY&columns=ALL&source=WEB&client=WEB&filter=(MUTUAL_TYPE="001")
-同花顺
-https://data.hexin.cn/market/hsgtApi/method/hsgtData/
-
-@author: 1nchaos
-@time: 2023/7/28
-@log: change log
-"""
-import copy
-import datetime
-import json
-import math
-
-import pandas as pd
-
-from adata.common import requests
-from adata.common.base.base_ths import BaseThs
-from adata.common.exception.exception_msg import THS_IP_LIMIT_RES, THS_IP_LIMIT_MSG
-from adata.common.headers import ths_headers
-
-
-class NorthFlow(BaseThs):
-    __NORTH_FLOW_COLUMNS = ['trade_date', 'net_hgt', 'buy_hgt', 'sell_hgt', 'net_sgt', 'buy_sgt', 'sell_sgt',
-                            'net_tgt', 'buy_tgt', 'sell_tgt']
-
-    __NORTH_FLOW_MIN_COLUMNS = ['trade_time', 'net_hgt', 'net_sgt', 'net_tgt']
-    __NORTH_FLOW_CURRENT_COLUMNS = __NORTH_FLOW_MIN_COLUMNS
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def north_flow(self, start_date=None):
-        """
-        获取北向资金历史的数据，开始时间到最新的历史数据，
-        :param start_date: 开始时间，最早：1017-01-01
-        :return:
-        'trade_date'：交易日期
-        'net_hgt', ：沪港通净买入金额（元）
-        'buy_hgt', ：沪港通净买入金额（元）
-        'sell_hgt', ：沪港通净买入金额（元）
-        'net_sgt', ：深港通净买入金额（元）
-        'buy_sgt', ：深港通净买入金额（元）
-        'sell_sgt', ：深港通卖出金额（元）
-        'net_tgt', ：合计净买入金额（元）
-        'buy_tgt', ：合计买入金额（元）
-        'sell_tgt' ：合计卖出金额（元）
-        """
-
-        return self.__north_flow_east(start_date=start_date)
-
-    def __north_flow_east(self, start_date=None):
-        """
-        https://datacenter-web.eastmoney.com/api/data/v1/get?callback=jQuery112307442704592215257_1690813516314&sortColumns=TRADE_DATE&sortTypes=-1&pageSize=10&pageNumber=2&reportName=RPT_MUTUAL_DEAL_HISTORY&columns=ALL&source=WEB&client=WEB&filter=(MUTUAL_TYPE="001")
-        """
-        if start_date:
-            start_date = datetime.datetime.strptime(start_date, '%Y-%m-%d')
-            date_min = datetime.datetime.strptime('2017-01-01', '%Y-%m-%d')
-            if start_date < date_min:
-                start_date = date_min
-        curr_page = 1
-        data = []
-        while curr_page < 18:
-            url = f'https://datacenter-web.eastmoney.com/api/data/v1/get?callback=jQuery112307442704592215257_1690813516314' \
-                  f'&sortColumns=TRADE_DATE&sortTypes=-1&pageSize=1000&pageNumber={curr_page}&' \
-                  f'reportName=RPT_MUTUAL_DEAL_HISTORY&columns=ALL&source=WEB&client=WEB&'
-            sgt_url = f"""{url}filter=(MUTUAL_TYPE="001")"""
-            hgt_url = f"""{url}filter=(MUTUAL_TYPE="003")"""
-
-            sgt = requests.request('get', sgt_url, headers={}, proxies={}).text.replace('null', '0')
-            hgt = requests.request('get', hgt_url, headers={}, proxies={}).text.replace('null', '0')
-
-            # 2. 解析数据
-            sgt_json = json.loads(sgt[sgt.index('{'):-2])
-            hgt_json = json.loads(hgt[hgt.index('{'):-2])
-            sgt_data = sgt_json["result"]["data"]
-            hgt_data = hgt_json["result"]["data"]
-            if not sgt_data:
-                break
-            is_end = False
-            for i in range(len(sgt_data)):
-                if not start_date and i >= 30:
-                    is_end = True
-                    break
-                if start_date:
-                    date_min = datetime.datetime.strptime(hgt_data[i]['TRADE_DATE'], '%Y-%m-%d %H:%M:%S')
-                    if start_date > date_min:
-                        is_end = True
-                        break
-
-                data.append({
-                    'trade_date': hgt_data[i]['TRADE_DATE'],
-                    'net_hgt': math.ceil(hgt_data[i]['NET_DEAL_AMT'] * 1000000),
-                    'buy_hgt': math.ceil(hgt_data[i]['BUY_AMT'] * 1000000),
-                    'sell_hgt': math.ceil(hgt_data[i]['SELL_AMT'] * 1000000),
-
-                    'net_sgt': math.ceil(sgt_data[i]['NET_DEAL_AMT'] * 1000000),
-                    'buy_sgt': math.ceil(sgt_data[i]['BUY_AMT'] * 1000000),
-                    'sell_sgt': math.ceil(sgt_data[i]['SELL_AMT'] * 1000000),
-
-                    'net_tgt': math.ceil((hgt_data[i]['NET_DEAL_AMT'] + sgt_data[i]['NET_DEAL_AMT']) * 1000000),
-                    'buy_tgt': math.ceil((hgt_data[i]['BUY_AMT'] + sgt_data[i]['BUY_AMT']) * 1000000),
-                    'sell_tgt': math.ceil((hgt_data[i]['SELL_AMT'] + sgt_data[i]['SELL_AMT']) * 1000000)
-                })
-
-            if is_end:
-                break
-            curr_page += 1
-
-        # 3.封装数据
-        result_df = pd.DataFrame(data=data, columns=self.__NORTH_FLOW_COLUMNS)
-        result_df['trade_date'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d')
-
-        return result_df[self.__NORTH_FLOW_COLUMNS]
-
-    def north_flow_min(self):
-        """
-        获取北向的分时数据，最新交易日的
-        https://data.hexin.cn/market/hsgtApi/method/dayChart/
-        """
-        res = self.__north_flow_min_east()
-        # res = pd.DataFrame()
-        if res.empty:
-            res = self.__north_flow_min_ths()
-        return res
-
-    def north_flow_current(self):
-        """
-        获取北向的最新数据，最新交易日的
-        """
-        return self.north_flow_min().tail(1)
-
-    def __north_flow_min_ths(self):
-        # 1.接口 url
-        api_url = f" https://data.hexin.cn/market/hsgtApi/method/dayChart/"
-        headers = copy.deepcopy(ths_headers.json_headers)
-        headers['Host'] = 'data.hexin.cn'
-        res = requests.request('get', api_url, headers=headers, proxies={})
-        text = res.text
-        if THS_IP_LIMIT_RES in text:
-            return Exception(THS_IP_LIMIT_MSG)
-        if not text:
-            return pd.DataFrame(data=[], columns=self.__NORTH_FLOW_CURRENT_COLUMNS)
-        # 2. 解析数据
-        result_json = json.loads(text)
-        time_list = result_json['time']
-        hgt_list = result_json['hgt']
-        sgt_list = result_json['sgt']
-        data = []
-        for i in range(len(time_list)):
-            row = [time_list[i], math.ceil(hgt_list[i] * 100000000), math.ceil(sgt_list[i] * 100000000),
-                   math.ceil((hgt_list[i] + sgt_list[i]) * 100000000)]
-            data.append(row)
-        # 3. 封装数据
-        result_df = pd.DataFrame(data=data, columns=self.__NORTH_FLOW_MIN_COLUMNS)
-        import adata
-        trade_year = adata.stock.info.trade_calendar()
-        # 获取当前日期
-        today = datetime.datetime.today().date()
-        # 筛选出小于等于今天并且 trade_status=1 的记录
-        trade_year['trade_date'] = pd.to_datetime(trade_year['trade_date'])
-        filtered_df = trade_year[(trade_year['trade_date'].dt.date <= today) & (trade_year['trade_status'] == 1)]
-        max_date = filtered_df.loc[filtered_df['trade_date'].idxmax()]
-
-        result_df['trade_time'] = max_date['trade_date'].strftime('%Y-%m-%d') + ' ' + result_df['trade_time']
-
-        # 将 trade_time 字符串转换为日期时间类型
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_time'])
-        return result_df[self.__NORTH_FLOW_MIN_COLUMNS]
-
-    def __north_flow_min_east(self):
-        """
-        https://push2.eastmoney.com/api/qt/kamt.rtmin/get?fields1=f1,f3&fields2=f51,f52,f54,f56&ut=b2884a393a59ad64002292a3e90d46a5&cb=jQuery1123041654203412972746_1690859251791&_=1690859251792
-        :return:
-        """
-        # 1. 请求数据
-        url = "https://push2.eastmoney.com/api/qt/kamt.rtmin/get?fields1=f1,f3&fields2=f51,f52,f54,f56&ut=b2884a393a59ad64002292a3e90d46a5&cb=jQuery112308613678156517719_1690861908580&_=1690861908581"
-        data = []
-        try:
-            gt = requests.request('get', url, headers={}, proxies={}).text
-
-            # 2. 解析数据
-            gt_json = json.loads(gt[gt.index('{'):-2])
-            gt_date = gt_json["data"]["s2nDate"]
-            gt_data = gt_json["data"]["s2n"]
-            for _ in gt_data:
-                row = str(_).split(',')
-                if row[1] != '-':
-                    data.append([row[0], math.ceil(float(row[1]) * 10000),
-                                 math.ceil(float(row[2]) * 10000), math.ceil(float(row[3]) * 10000)])
-        except Exception as e:
-            print("north_flow_min_east is ERROR!!!")
-            return pd.DataFrame(data=data, columns=self.__NORTH_FLOW_MIN_COLUMNS)
-        result_df = pd.DataFrame(data=data, columns=self.__NORTH_FLOW_MIN_COLUMNS)
-
-        # 3. 封装数据
-        result_df['trade_time'] = str(datetime.datetime.now().year) + '-' + gt_date + ' ' + result_df['trade_time']
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_time'])
-        result_df = result_df.dropna()
-        return result_df[self.__NORTH_FLOW_MIN_COLUMNS]
-
-
-if __name__ == '__main__':
-    print(NorthFlow().north_flow_min())
-    print(NorthFlow().north_flow_current())
-    print(NorthFlow().north_flow(start_date='2000-11-01'))
+# -*- coding: utf-8 -*-
+"""
+@desc:
+北向资金
+来源：东方财富
+https://data.eastmoney.com/hsgt/index.html
+https://datacenter-web.eastmoney.com/api/data/v1/get?callback=jQuery112307442704592215257_1690813516314&sortColumns=TRADE_DATE&sortTypes=-1&pageSize=10&pageNumber=2&reportName=RPT_MUTUAL_DEAL_HISTORY&columns=ALL&source=WEB&client=WEB&filter=(MUTUAL_TYPE="001")
+同花顺
+https://data.hexin.cn/market/hsgtApi/method/hsgtData/
+
+@author: 1nchaos
+@time: 2023/7/28
+@log: change log
+"""
+import copy
+import datetime
+import json
+import math
+
+import pandas as pd
+
+from adata.common import requests
+from adata.common.base.base_ths import BaseThs
+from adata.common.exception.exception_msg import THS_IP_LIMIT_RES, THS_IP_LIMIT_MSG
+from adata.common.headers import ths_headers
+
+
+class NorthFlow(BaseThs):
+    __NORTH_FLOW_COLUMNS = ['trade_date', 'net_hgt', 'buy_hgt', 'sell_hgt', 'net_sgt', 'buy_sgt', 'sell_sgt',
+                            'net_tgt', 'buy_tgt', 'sell_tgt']
+
+    __NORTH_FLOW_MIN_COLUMNS = ['trade_time', 'net_hgt', 'net_sgt', 'net_tgt']
+    __NORTH_FLOW_CURRENT_COLUMNS = __NORTH_FLOW_MIN_COLUMNS
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def north_flow(self, start_date=None):
+        """
+        获取北向资金历史的数据，开始时间到最新的历史数据，
+        :param start_date: 开始时间，最早：1017-01-01
+        :return:
+        'trade_date'：交易日期
+        'net_hgt', ：沪港通净买入金额（元）
+        'buy_hgt', ：沪港通净买入金额（元）
+        'sell_hgt', ：沪港通净买入金额（元）
+        'net_sgt', ：深港通净买入金额（元）
+        'buy_sgt', ：深港通净买入金额（元）
+        'sell_sgt', ：深港通卖出金额（元）
+        'net_tgt', ：合计净买入金额（元）
+        'buy_tgt', ：合计买入金额（元）
+        'sell_tgt' ：合计卖出金额（元）
+        """
+
+        return self.__north_flow_east(start_date=start_date)
+
+    def __north_flow_east(self, start_date=None):
+        """
+        https://datacenter-web.eastmoney.com/api/data/v1/get?callback=jQuery112307442704592215257_1690813516314&sortColumns=TRADE_DATE&sortTypes=-1&pageSize=10&pageNumber=2&reportName=RPT_MUTUAL_DEAL_HISTORY&columns=ALL&source=WEB&client=WEB&filter=(MUTUAL_TYPE="001")
+        """
+        if start_date:
+            start_date = datetime.datetime.strptime(start_date, '%Y-%m-%d')
+            date_min = datetime.datetime.strptime('2017-01-01', '%Y-%m-%d')
+            if start_date < date_min:
+                start_date = date_min
+        curr_page = 1
+        data = []
+        while curr_page < 18:
+            url = f'https://datacenter-web.eastmoney.com/api/data/v1/get?callback=jQuery112307442704592215257_1690813516314' \
+                  f'&sortColumns=TRADE_DATE&sortTypes=-1&pageSize=1000&pageNumber={curr_page}&' \
+                  f'reportName=RPT_MUTUAL_DEAL_HISTORY&columns=ALL&source=WEB&client=WEB&'
+            sgt_url = f"""{url}filter=(MUTUAL_TYPE="001")"""
+            hgt_url = f"""{url}filter=(MUTUAL_TYPE="003")"""
+
+            sgt = requests.request('get', sgt_url, headers={}, proxies={}).text.replace('null', '0')
+            hgt = requests.request('get', hgt_url, headers={}, proxies={}).text.replace('null', '0')
+
+            # 2. 解析数据
+            sgt_json = json.loads(sgt[sgt.index('{'):-2])
+            hgt_json = json.loads(hgt[hgt.index('{'):-2])
+            sgt_data = sgt_json["result"]["data"]
+            hgt_data = hgt_json["result"]["data"]
+            if not sgt_data:
+                break
+            is_end = False
+            for i in range(len(sgt_data)):
+                if not start_date and i >= 30:
+                    is_end = True
+                    break
+                if start_date:
+                    date_min = datetime.datetime.strptime(hgt_data[i]['TRADE_DATE'], '%Y-%m-%d %H:%M:%S')
+                    if start_date > date_min:
+                        is_end = True
+                        break
+
+                data.append({
+                    'trade_date': hgt_data[i]['TRADE_DATE'],
+                    'net_hgt': math.ceil(hgt_data[i]['NET_DEAL_AMT'] * 1000000),
+                    'buy_hgt': math.ceil(hgt_data[i]['BUY_AMT'] * 1000000),
+                    'sell_hgt': math.ceil(hgt_data[i]['SELL_AMT'] * 1000000),
+
+                    'net_sgt': math.ceil(sgt_data[i]['NET_DEAL_AMT'] * 1000000),
+                    'buy_sgt': math.ceil(sgt_data[i]['BUY_AMT'] * 1000000),
+                    'sell_sgt': math.ceil(sgt_data[i]['SELL_AMT'] * 1000000),
+
+                    'net_tgt': math.ceil((hgt_data[i]['NET_DEAL_AMT'] + sgt_data[i]['NET_DEAL_AMT']) * 1000000),
+                    'buy_tgt': math.ceil((hgt_data[i]['BUY_AMT'] + sgt_data[i]['BUY_AMT']) * 1000000),
+                    'sell_tgt': math.ceil((hgt_data[i]['SELL_AMT'] + sgt_data[i]['SELL_AMT']) * 1000000)
+                })
+
+            if is_end:
+                break
+            curr_page += 1
+
+        # 3.封装数据
+        result_df = pd.DataFrame(data=data, columns=self.__NORTH_FLOW_COLUMNS)
+        result_df['trade_date'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d')
+
+        return result_df[self.__NORTH_FLOW_COLUMNS]
+
+    def north_flow_min(self):
+        """
+        获取北向的分时数据，最新交易日的
+        https://data.hexin.cn/market/hsgtApi/method/dayChart/
+        """
+        res = self.__north_flow_min_east()
+        # res = pd.DataFrame()
+        if res.empty:
+            res = self.__north_flow_min_ths()
+        return res
+
+    def north_flow_current(self):
+        """
+        获取北向的最新数据，最新交易日的
+        """
+        return self.north_flow_min().tail(1)
+
+    def __north_flow_min_ths(self):
+        # 1.接口 url
+        api_url = f" https://data.hexin.cn/market/hsgtApi/method/dayChart/"
+        headers = copy.deepcopy(ths_headers.json_headers)
+        headers['Host'] = 'data.hexin.cn'
+        res = requests.request('get', api_url, headers=headers, proxies={})
+        text = res.text
+        if THS_IP_LIMIT_RES in text:
+            return Exception(THS_IP_LIMIT_MSG)
+        if not text:
+            return pd.DataFrame(data=[], columns=self.__NORTH_FLOW_CURRENT_COLUMNS)
+        # 2. 解析数据
+        result_json = json.loads(text)
+        time_list = result_json['time']
+        hgt_list = result_json['hgt']
+        sgt_list = result_json['sgt']
+        data = []
+        for i in range(len(time_list)):
+            row = [time_list[i], math.ceil(hgt_list[i] * 100000000), math.ceil(sgt_list[i] * 100000000),
+                   math.ceil((hgt_list[i] + sgt_list[i]) * 100000000)]
+            data.append(row)
+        # 3. 封装数据
+        result_df = pd.DataFrame(data=data, columns=self.__NORTH_FLOW_MIN_COLUMNS)
+        import adata
+        trade_year = adata.stock.info.trade_calendar()
+        # 获取当前日期
+        today = datetime.datetime.today().date()
+        # 筛选出小于等于今天并且 trade_status=1 的记录
+        trade_year['trade_date'] = pd.to_datetime(trade_year['trade_date'])
+        filtered_df = trade_year[(trade_year['trade_date'].dt.date <= today) & (trade_year['trade_status'] == 1)]
+        max_date = filtered_df.loc[filtered_df['trade_date'].idxmax()]
+
+        result_df['trade_time'] = max_date['trade_date'].strftime('%Y-%m-%d') + ' ' + result_df['trade_time']
+
+        # 将 trade_time 字符串转换为日期时间类型
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_time'])
+        return result_df[self.__NORTH_FLOW_MIN_COLUMNS]
+
+    def __north_flow_min_east(self):
+        """
+        https://push2.eastmoney.com/api/qt/kamt.rtmin/get?fields1=f1,f3&fields2=f51,f52,f54,f56&ut=b2884a393a59ad64002292a3e90d46a5&cb=jQuery1123041654203412972746_1690859251791&_=1690859251792
+        :return:
+        """
+        # 1. 请求数据
+        url = "https://push2.eastmoney.com/api/qt/kamt.rtmin/get?fields1=f1,f3&fields2=f51,f52,f54,f56&ut=b2884a393a59ad64002292a3e90d46a5&cb=jQuery112308613678156517719_1690861908580&_=1690861908581"
+        data = []
+        try:
+            gt = requests.request('get', url, headers={}, proxies={}).text
+
+            # 2. 解析数据
+            gt_json = json.loads(gt[gt.index('{'):-2])
+            gt_date = gt_json["data"]["s2nDate"]
+            gt_data = gt_json["data"]["s2n"]
+            for _ in gt_data:
+                row = str(_).split(',')
+                if row[1] != '-':
+                    data.append([row[0], math.ceil(float(row[1]) * 10000),
+                                 math.ceil(float(row[2]) * 10000), math.ceil(float(row[3]) * 10000)])
+        except Exception as e:
+            print("north_flow_min_east is ERROR!!!")
+            return pd.DataFrame(data=data, columns=self.__NORTH_FLOW_MIN_COLUMNS)
+        result_df = pd.DataFrame(data=data, columns=self.__NORTH_FLOW_MIN_COLUMNS)
+
+        # 3. 封装数据
+        result_df['trade_time'] = str(datetime.datetime.now().year) + '-' + gt_date + ' ' + result_df['trade_time']
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_time'])
+        result_df = result_df.dropna()
+        return result_df[self.__NORTH_FLOW_MIN_COLUMNS]
+
+
+if __name__ == '__main__':
+    print(NorthFlow().north_flow_min())
+    print(NorthFlow().north_flow_current())
+    print(NorthFlow().north_flow(start_date='2000-11-01'))
```

### Comparing `adata-1.2.4/adata/sentiment/securities_margin.py` & `adata-2.0.0b0/adata/sentiment/securities_margin.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-# -*- coding: utf-8 -*-
-"""
-@desc:
-融资融券数据
-同花顺
-http://data.10jqka.com.cn/market/rzrq/
-http://data.10jqka.com.cn/market/rzrq/board/getRzrqPage/page/2/ajax/1/
-东方财富
-https://data.eastmoney.com/rzrq/total.html
-https://datacenter-web.eastmoney.com/api/data/v1/get?reportName=RPTA_RZRQ_LSHJ&columns=ALL&source=WEB&sortColumns=dim_date&sortTypes=-1&pageNumber=2&pageSize=50&filter=&pageNo=2&p=2&pageNum=2&_=1690176931022
-
-@author: 1nchaos
-@time: 2023/7/24
-@log: change log
-"""
-from datetime import datetime
-
-import pandas as pd
-
-from adata.common import requests
-from adata.common.headers import east_headers
-
-
-class SecuritiesMargin(object):
-    __SECURITIES_MARGIN_COLUMN = ['trade_date', 'rzye', 'rqye', 'rzrqye', 'rzrqyecz']
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def securities_margin(self, start_date=None):
-        """
-        查询开始时间到现在的融资融券余额数据，默认：查询最近一年的数据
-        :return:  ['trade_date', 'rzye', 'rqye', 'rzrqye', 'rzrqyecz']
-        trade_date: 交易日
-        rzye： 融资余额（元）
-        rqye： 融券余额（元）
-        rzrqye： 融资融券余额（元）
-        rzrqyecz： 融资融券余额差值（元）
-        """
-        return self.__securities_margin_east(start_date=start_date)
-
-    def __securities_margin_east(self, start_date=None):
-        """
-        https://datacenter-web.eastmoney.com/api/data/v1/get?reportName=RPTA_RZRQ_LSHJ&columns=ALL&source=WEB&sortColumns=dim_date&sortTypes=-1&pageNumber=1&pageSize=250&_=1690176931022
-        :param start_date: 开始时间
-        :return:
-        """
-        # 1. url拼接页码等参数
-        data = []
-        total_pages = 1
-        curr_page = 1
-        page_size = 250
-        start_date_str = start_date
-        if start_date:
-            start_date = datetime.strptime(start_date, '%Y-%m-%d')
-        while curr_page <= total_pages:
-            api_url = f"https://datacenter-web.eastmoney.com/api/data/v1/get?" \
-                      f"reportName=RPTA_RZRQ_LSHJ&columns=ALL&source=WEB&sortColumns=dim_date&sortTypes=-1&" \
-                      f"pageNumber={curr_page}&pageSize={page_size}&_=1690176931022"
-
-            res = requests.request(method='get', url=api_url, headers=east_headers.json_headers, proxies={})
-            # 2. 判断请求是否成功
-            if res.status_code != 200:
-                continue
-            res_json = res.json()
-            if not res_json['success']:
-                continue
-            if curr_page == 1:
-                total_pages = res_json['result']['pages']
-            res_json = res_json['result']['data']
-            # 2.1 日期范围判断
-            data.extend(res_json)
-            if not start_date:
-                break
-            if start_date:
-                date_min = datetime.strptime(res_json[-1]['DIM_DATE'], '%Y-%m-%d %H:%M:%S')
-                if start_date >= date_min:
-                    break
-            curr_page += 1
-
-        # 3. 解析数据
-        result_df = pd.DataFrame(data=data)
-        rename_columns = {'RZYE': 'rzye', 'RQYE': 'rqye', 'RZRQYE': 'rzrqye', 'RZRQYECZ': 'rzrqyecz',
-                          'DIM_DATE': 'trade_date'}
-        result_df = result_df.rename(columns=rename_columns)[self.__SECURITIES_MARGIN_COLUMN]
-
-        # 4. 数据清洗
-        result_df['trade_date'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d')
-        result_df = result_df[result_df['trade_date'] > start_date_str]
-        return result_df
-
-
-if __name__ == '__main__':
-    print(SecuritiesMargin().securities_margin('2022-01-01'))
+# -*- coding: utf-8 -*-
+"""
+@desc:
+融资融券数据
+同花顺
+http://data.10jqka.com.cn/market/rzrq/
+http://data.10jqka.com.cn/market/rzrq/board/getRzrqPage/page/2/ajax/1/
+东方财富
+https://data.eastmoney.com/rzrq/total.html
+https://datacenter-web.eastmoney.com/api/data/v1/get?reportName=RPTA_RZRQ_LSHJ&columns=ALL&source=WEB&sortColumns=dim_date&sortTypes=-1&pageNumber=2&pageSize=50&filter=&pageNo=2&p=2&pageNum=2&_=1690176931022
+
+@author: 1nchaos
+@time: 2023/7/24
+@log: change log
+"""
+from datetime import datetime
+
+import pandas as pd
+
+from adata.common import requests
+from adata.common.headers import east_headers
+
+
+class SecuritiesMargin(object):
+    __SECURITIES_MARGIN_COLUMN = ['trade_date', 'rzye', 'rqye', 'rzrqye', 'rzrqyecz']
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def securities_margin(self, start_date=None):
+        """
+        查询开始时间到现在的融资融券余额数据，默认：查询最近一年的数据
+        :return:  ['trade_date', 'rzye', 'rqye', 'rzrqye', 'rzrqyecz']
+        trade_date: 交易日
+        rzye： 融资余额（元）
+        rqye： 融券余额（元）
+        rzrqye： 融资融券余额（元）
+        rzrqyecz： 融资融券余额差值（元）
+        """
+        return self.__securities_margin_east(start_date=start_date)
+
+    def __securities_margin_east(self, start_date=None):
+        """
+        https://datacenter-web.eastmoney.com/api/data/v1/get?reportName=RPTA_RZRQ_LSHJ&columns=ALL&source=WEB&sortColumns=dim_date&sortTypes=-1&pageNumber=1&pageSize=250&_=1690176931022
+        :param start_date: 开始时间
+        :return:
+        """
+        # 1. url拼接页码等参数
+        data = []
+        total_pages = 1
+        curr_page = 1
+        page_size = 250
+        start_date_str = start_date
+        if start_date:
+            start_date = datetime.strptime(start_date, '%Y-%m-%d')
+        while curr_page <= total_pages:
+            api_url = f"https://datacenter-web.eastmoney.com/api/data/v1/get?" \
+                      f"reportName=RPTA_RZRQ_LSHJ&columns=ALL&source=WEB&sortColumns=dim_date&sortTypes=-1&" \
+                      f"pageNumber={curr_page}&pageSize={page_size}&_=1690176931022"
+
+            res = requests.request(method='get', url=api_url, headers=east_headers.json_headers, proxies={})
+            # 2. 判断请求是否成功
+            if res.status_code != 200:
+                continue
+            res_json = res.json()
+            if not res_json['success']:
+                continue
+            if curr_page == 1:
+                total_pages = res_json['result']['pages']
+            res_json = res_json['result']['data']
+            # 2.1 日期范围判断
+            data.extend(res_json)
+            if not start_date:
+                break
+            if start_date:
+                date_min = datetime.strptime(res_json[-1]['DIM_DATE'], '%Y-%m-%d %H:%M:%S')
+                if start_date >= date_min:
+                    break
+            curr_page += 1
+
+        # 3. 解析数据
+        result_df = pd.DataFrame(data=data)
+        rename_columns = {'RZYE': 'rzye', 'RQYE': 'rqye', 'RZRQYE': 'rzrqye', 'RZRQYECZ': 'rzrqyecz',
+                          'DIM_DATE': 'trade_date'}
+        result_df = result_df.rename(columns=rename_columns)[self.__SECURITIES_MARGIN_COLUMN]
+
+        # 4. 数据清洗
+        result_df['trade_date'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d')
+        result_df = result_df[result_df['trade_date'] > start_date_str]
+        return result_df
+
+
+if __name__ == '__main__':
+    print(SecuritiesMargin().securities_margin('2022-01-01'))
```

### Comparing `adata-1.2.4/adata/sentiment/stock_lifting.py` & `adata-2.0.0b0/adata/sentiment/stock_lifting.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-# -*- coding: utf-8 -*-
-"""
-@desc:
-股票解禁：大概率大额解禁的票房风险较大，可以加入短线交易的因子数据
-解禁数据：来源同花顺行情中心
-http://data.10jqka.com.cn/market/xsjj/field/enddate/order/desc/ajax/1/free/1/
-http://data.10jqka.com.cn/market/xsjj/field/enddate/order/desc/ajax/1/free/1/page/2/free/1/
-
-@author: 1nchaos
-@time: 2023/6/14
-@log: change log
-"""
-import copy
-
-import pandas as pd
-from bs4 import BeautifulSoup
-
-from adata.common import requests
-from adata.common.headers import ths_headers
-from adata.common.utils import cookie
-
-
-class StockLifting(object):
-    __STOCK_LIFTING_COLUMN = ['stock_code', 'short_name', 'lift_date', 'volume', 'amount', 'ratio', 'price']
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def stock_lifting_last_month(self):
-        """
-        查询最近一个月的股票解禁列表
-        http://data.10jqka.com.cn/market/xsjj/field/enddate/order/desc/ajax/1/free/1/
-        http://data.10jqka.com.cn/market/xsjj/field/enddate/order/desc/ajax/1/free/1/page/2/free/1/
-        :return:  ['stock_code', 'short_name', 'lift_date', 'volume', 'ratio', 'price', 'amount']
-        stock_code: 股票代码
-        short_name： 股票简称
-        lift_date： 解禁日期
-        volume： 解禁股数（股）
-        ratio： 占总股本比例（%）
-        price： 最新股价（元）
-        amount： 最新解禁金额（元）
-        """
-        # 1. url拼接页码等参数
-        data = []
-        total_pages = 1
-        curr_page = 1
-        while curr_page <= total_pages:
-            api_url = f"http://data.10jqka.com.cn/market/xsjj/field/enddate/order/desc/ajax/1/free/1/"
-            if curr_page > 1:
-                api_url = api_url + f"page/{curr_page}/free/1/"
-            headers = copy.deepcopy(ths_headers.text_headers)
-            headers['Host'] = 'data.10jqka.com.cn'
-            headers['Referer'] = None
-            headers['Cookie'] = cookie.ths_cookie()
-            res = requests.request(method='get', url=api_url, headers=headers, proxies={})
-            curr_page += 1
-            # 2. 判断请求是否成功
-            if res.status_code != 200:
-                continue
-            text = res.text
-            if not ('解禁日期' in text or '解禁股' in text):
-                break
-            soup = BeautifulSoup(text, 'html.parser')
-            # 3 .获取总的页数
-            if total_pages == 1:
-                page_info = soup.find('span', {'class': 'page_info'})
-                if page_info:
-                    total_pages = int(page_info.text.split("/")[1])
-            # 4. 解析数据
-            page_data = []
-            for idx, tr in enumerate(soup.find_all('tr')):
-                if idx != 0:
-                    tds = tr.find_all('td')
-                    page_data.append({'stock_code': tds[1].contents[0].text, 'short_name': tds[2].contents[0].text,
-                                      'lift_date': tds[3].contents[0].text, 'volume': tds[4].contents[0].text,
-                                      'ratio': tds[7].contents[0].text, 'price': tds[5].contents[0].text,
-                                      'amount': tds[6].contents[0].text})
-            data.extend(page_data)
-        # 5. 封装数据
-        if not data:
-            return pd.DataFrame(data=data, columns=self.__STOCK_LIFTING_COLUMN)
-        result_df = pd.DataFrame(data=data)
-        data.clear()
-        # 6. 单位换算
-        result_df['volume'] = result_df['volume'].apply(lambda x: str(float(x[:-1]) * 10000) if '万' in x else x)
-        result_df['volume'] = result_df['volume'].apply(
-            lambda x: round(float(x[:-1]) * 100000000) if '亿' in x else round(float(x)))
-
-        # convert amount to yuan
-        result_df['amount'] = result_df['amount'].apply(lambda x: str(float(x[:-1]) * 10000) if '万' in x else x)
-        result_df['amount'] = result_df['amount'].apply(
-            lambda x: round(float(x[:-1]) * 100000000) if '亿' in x else round(float(x)))
-        return result_df[self.__STOCK_LIFTING_COLUMN]
-
-
-if __name__ == '__main__':
-    print(StockLifting().stock_lifting_last_month())
+# -*- coding: utf-8 -*-
+"""
+@desc:
+股票解禁：大概率大额解禁的票房风险较大，可以加入短线交易的因子数据
+解禁数据：来源同花顺行情中心
+http://data.10jqka.com.cn/market/xsjj/field/enddate/order/desc/ajax/1/free/1/
+http://data.10jqka.com.cn/market/xsjj/field/enddate/order/desc/ajax/1/free/1/page/2/free/1/
+
+@author: 1nchaos
+@time: 2023/6/14
+@log: change log
+"""
+import copy
+
+import pandas as pd
+from bs4 import BeautifulSoup
+
+from adata.common import requests
+from adata.common.headers import ths_headers
+from adata.common.utils import cookie
+
+
+class StockLifting(object):
+    __STOCK_LIFTING_COLUMN = ['stock_code', 'short_name', 'lift_date', 'volume', 'amount', 'ratio', 'price']
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def stock_lifting_last_month(self):
+        """
+        查询最近一个月的股票解禁列表
+        http://data.10jqka.com.cn/market/xsjj/field/enddate/order/desc/ajax/1/free/1/
+        http://data.10jqka.com.cn/market/xsjj/field/enddate/order/desc/ajax/1/free/1/page/2/free/1/
+        :return:  ['stock_code', 'short_name', 'lift_date', 'volume', 'ratio', 'price', 'amount']
+        stock_code: 股票代码
+        short_name： 股票简称
+        lift_date： 解禁日期
+        volume： 解禁股数（股）
+        ratio： 占总股本比例（%）
+        price： 最新股价（元）
+        amount： 最新解禁金额（元）
+        """
+        # 1. url拼接页码等参数
+        data = []
+        total_pages = 1
+        curr_page = 1
+        while curr_page <= total_pages:
+            api_url = f"http://data.10jqka.com.cn/market/xsjj/field/enddate/order/desc/ajax/1/free/1/"
+            if curr_page > 1:
+                api_url = api_url + f"page/{curr_page}/free/1/"
+            headers = copy.deepcopy(ths_headers.text_headers)
+            headers['Host'] = 'data.10jqka.com.cn'
+            headers['Referer'] = None
+            headers['Cookie'] = cookie.ths_cookie()
+            res = requests.request(method='get', url=api_url, headers=headers, proxies={})
+            curr_page += 1
+            # 2. 判断请求是否成功
+            if res.status_code != 200:
+                continue
+            text = res.text
+            if not ('解禁日期' in text or '解禁股' in text):
+                break
+            soup = BeautifulSoup(text, 'html.parser')
+            # 3 .获取总的页数
+            if total_pages == 1:
+                page_info = soup.find('span', {'class': 'page_info'})
+                if page_info:
+                    total_pages = int(page_info.text.split("/")[1])
+            # 4. 解析数据
+            page_data = []
+            for idx, tr in enumerate(soup.find_all('tr')):
+                if idx != 0:
+                    tds = tr.find_all('td')
+                    page_data.append({'stock_code': tds[1].contents[0].text, 'short_name': tds[2].contents[0].text,
+                                      'lift_date': tds[3].contents[0].text, 'volume': tds[4].contents[0].text,
+                                      'ratio': tds[7].contents[0].text, 'price': tds[5].contents[0].text,
+                                      'amount': tds[6].contents[0].text})
+            data.extend(page_data)
+        # 5. 封装数据
+        if not data:
+            return pd.DataFrame(data=data, columns=self.__STOCK_LIFTING_COLUMN)
+        result_df = pd.DataFrame(data=data)
+        data.clear()
+        # 6. 单位换算
+        result_df['volume'] = result_df['volume'].apply(lambda x: str(float(x[:-1]) * 10000) if '万' in x else x)
+        result_df['volume'] = result_df['volume'].apply(
+            lambda x: round(float(x[:-1]) * 100000000) if '亿' in x else round(float(x)))
+
+        # convert amount to yuan
+        result_df['amount'] = result_df['amount'].apply(lambda x: str(float(x[:-1]) * 10000) if '万' in x else x)
+        result_df['amount'] = result_df['amount'].apply(
+            lambda x: round(float(x[:-1]) * 100000000) if '亿' in x else round(float(x)))
+        return result_df[self.__STOCK_LIFTING_COLUMN]
+
+
+if __name__ == '__main__':
+    print(StockLifting().stock_lifting_last_month())
```

### Comparing `adata-1.2.4/adata/stock/cache/calendar/2006.csv` & `adata-2.0.0b0/adata/stock/cache/calendar/2006.csv`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,366 +1,366 @@
-trade_date,trade_status,day_week
-2006-01-01,0,1
-2006-01-02,0,2
-2006-01-03,0,3
-2006-01-04,1,4
-2006-01-05,1,5
-2006-01-06,1,6
-2006-01-07,0,7
-2006-01-08,0,1
-2006-01-09,1,2
-2006-01-10,1,3
-2006-01-11,1,4
-2006-01-12,1,5
-2006-01-13,1,6
-2006-01-14,0,7
-2006-01-15,0,1
-2006-01-16,1,2
-2006-01-17,1,3
-2006-01-18,1,4
-2006-01-19,1,5
-2006-01-20,1,6
-2006-01-21,0,7
-2006-01-22,0,1
-2006-01-23,1,2
-2006-01-24,1,3
-2006-01-25,1,4
-2006-01-26,0,5
-2006-01-27,0,6
-2006-01-28,0,7
-2006-01-29,0,1
-2006-01-30,0,2
-2006-01-31,0,3
-2006-02-01,0,4
-2006-02-02,0,5
-2006-02-03,0,6
-2006-02-04,0,7
-2006-02-05,0,1
-2006-02-06,1,2
-2006-02-07,1,3
-2006-02-08,1,4
-2006-02-09,1,5
-2006-02-10,1,6
-2006-02-11,0,7
-2006-02-12,0,1
-2006-02-13,1,2
-2006-02-14,1,3
-2006-02-15,1,4
-2006-02-16,1,5
-2006-02-17,1,6
-2006-02-18,0,7
-2006-02-19,0,1
-2006-02-20,1,2
-2006-02-21,1,3
-2006-02-22,1,4
-2006-02-23,1,5
-2006-02-24,1,6
-2006-02-25,0,7
-2006-02-26,0,1
-2006-02-27,1,2
-2006-02-28,1,3
-2006-03-01,1,4
-2006-03-02,1,5
-2006-03-03,1,6
-2006-03-04,0,7
-2006-03-05,0,1
-2006-03-06,1,2
-2006-03-07,1,3
-2006-03-08,1,4
-2006-03-09,1,5
-2006-03-10,1,6
-2006-03-11,0,7
-2006-03-12,0,1
-2006-03-13,1,2
-2006-03-14,1,3
-2006-03-15,1,4
-2006-03-16,1,5
-2006-03-17,1,6
-2006-03-18,0,7
-2006-03-19,0,1
-2006-03-20,1,2
-2006-03-21,1,3
-2006-03-22,1,4
-2006-03-23,1,5
-2006-03-24,1,6
-2006-03-25,0,7
-2006-03-26,0,1
-2006-03-27,1,2
-2006-03-28,1,3
-2006-03-29,1,4
-2006-03-30,1,5
-2006-03-31,1,6
-2006-04-01,0,7
-2006-04-02,0,1
-2006-04-03,1,2
-2006-04-04,1,3
-2006-04-05,1,4
-2006-04-06,1,5
-2006-04-07,1,6
-2006-04-08,0,7
-2006-04-09,0,1
-2006-04-10,1,2
-2006-04-11,1,3
-2006-04-12,1,4
-2006-04-13,1,5
-2006-04-14,1,6
-2006-04-15,0,7
-2006-04-16,0,1
-2006-04-17,1,2
-2006-04-18,1,3
-2006-04-19,1,4
-2006-04-20,1,5
-2006-04-21,1,6
-2006-04-22,0,7
-2006-04-23,0,1
-2006-04-24,1,2
-2006-04-25,1,3
-2006-04-26,1,4
-2006-04-27,1,5
-2006-04-28,1,6
-2006-04-29,0,7
-2006-04-30,0,1
-2006-05-01,0,2
-2006-05-02,0,3
-2006-05-03,0,4
-2006-05-04,0,5
-2006-05-05,0,6
-2006-05-06,0,7
-2006-05-07,0,1
-2006-05-08,1,2
-2006-05-09,1,3
-2006-05-10,1,4
-2006-05-11,1,5
-2006-05-12,1,6
-2006-05-13,0,7
-2006-05-14,0,1
-2006-05-15,1,2
-2006-05-16,1,3
-2006-05-17,1,4
-2006-05-18,1,5
-2006-05-19,1,6
-2006-05-20,0,7
-2006-05-21,0,1
-2006-05-22,1,2
-2006-05-23,1,3
-2006-05-24,1,4
-2006-05-25,1,5
-2006-05-26,1,6
-2006-05-27,0,7
-2006-05-28,0,1
-2006-05-29,1,2
-2006-05-30,1,3
-2006-05-31,1,4
-2006-06-01,1,5
-2006-06-02,1,6
-2006-06-03,0,7
-2006-06-04,0,1
-2006-06-05,1,2
-2006-06-06,1,3
-2006-06-07,1,4
-2006-06-08,1,5
-2006-06-09,1,6
-2006-06-10,0,7
-2006-06-11,0,1
-2006-06-12,1,2
-2006-06-13,1,3
-2006-06-14,1,4
-2006-06-15,1,5
-2006-06-16,1,6
-2006-06-17,0,7
-2006-06-18,0,1
-2006-06-19,1,2
-2006-06-20,1,3
-2006-06-21,1,4
-2006-06-22,1,5
-2006-06-23,1,6
-2006-06-24,0,7
-2006-06-25,0,1
-2006-06-26,1,2
-2006-06-27,1,3
-2006-06-28,1,4
-2006-06-29,1,5
-2006-06-30,1,6
-2006-07-01,0,7
-2006-07-02,0,1
-2006-07-03,1,2
-2006-07-04,1,3
-2006-07-05,1,4
-2006-07-06,1,5
-2006-07-07,1,6
-2006-07-08,0,7
-2006-07-09,0,1
-2006-07-10,1,2
-2006-07-11,1,3
-2006-07-12,1,4
-2006-07-13,1,5
-2006-07-14,1,6
-2006-07-15,0,7
-2006-07-16,0,1
-2006-07-17,1,2
-2006-07-18,1,3
-2006-07-19,1,4
-2006-07-20,1,5
-2006-07-21,1,6
-2006-07-22,0,7
-2006-07-23,0,1
-2006-07-24,1,2
-2006-07-25,1,3
-2006-07-26,1,4
-2006-07-27,1,5
-2006-07-28,1,6
-2006-07-29,0,7
-2006-07-30,0,1
-2006-07-31,1,2
-2006-08-01,1,3
-2006-08-02,1,4
-2006-08-03,1,5
-2006-08-04,1,6
-2006-08-05,0,7
-2006-08-06,0,1
-2006-08-07,1,2
-2006-08-08,1,3
-2006-08-09,1,4
-2006-08-10,1,5
-2006-08-11,1,6
-2006-08-12,0,7
-2006-08-13,0,1
-2006-08-14,1,2
-2006-08-15,1,3
-2006-08-16,1,4
-2006-08-17,1,5
-2006-08-18,1,6
-2006-08-19,0,7
-2006-08-20,0,1
-2006-08-21,1,2
-2006-08-22,1,3
-2006-08-23,1,4
-2006-08-24,1,5
-2006-08-25,1,6
-2006-08-26,0,7
-2006-08-27,0,1
-2006-08-28,1,2
-2006-08-29,1,3
-2006-08-30,1,4
-2006-08-31,1,5
-2006-09-01,1,6
-2006-09-02,0,7
-2006-09-03,0,1
-2006-09-04,1,2
-2006-09-05,1,3
-2006-09-06,1,4
-2006-09-07,1,5
-2006-09-08,1,6
-2006-09-09,0,7
-2006-09-10,0,1
-2006-09-11,1,2
-2006-09-12,1,3
-2006-09-13,1,4
-2006-09-14,1,5
-2006-09-15,1,6
-2006-09-16,0,7
-2006-09-17,0,1
-2006-09-18,1,2
-2006-09-19,1,3
-2006-09-20,1,4
-2006-09-21,1,5
-2006-09-22,1,6
-2006-09-23,0,7
-2006-09-24,0,1
-2006-09-25,1,2
-2006-09-26,1,3
-2006-09-27,1,4
-2006-09-28,1,5
-2006-09-29,1,6
-2006-09-30,0,7
-2006-10-01,0,1
-2006-10-02,0,2
-2006-10-03,0,3
-2006-10-04,0,4
-2006-10-05,0,5
-2006-10-06,0,6
-2006-10-07,0,7
-2006-10-08,0,1
-2006-10-09,1,2
-2006-10-10,1,3
-2006-10-11,1,4
-2006-10-12,1,5
-2006-10-13,1,6
-2006-10-14,0,7
-2006-10-15,0,1
-2006-10-16,1,2
-2006-10-17,1,3
-2006-10-18,1,4
-2006-10-19,1,5
-2006-10-20,1,6
-2006-10-21,0,7
-2006-10-22,0,1
-2006-10-23,1,2
-2006-10-24,1,3
-2006-10-25,1,4
-2006-10-26,1,5
-2006-10-27,1,6
-2006-10-28,0,7
-2006-10-29,0,1
-2006-10-30,1,2
-2006-10-31,1,3
-2006-11-01,1,4
-2006-11-02,1,5
-2006-11-03,1,6
-2006-11-04,0,7
-2006-11-05,0,1
-2006-11-06,1,2
-2006-11-07,1,3
-2006-11-08,1,4
-2006-11-09,1,5
-2006-11-10,1,6
-2006-11-11,0,7
-2006-11-12,0,1
-2006-11-13,1,2
-2006-11-14,1,3
-2006-11-15,1,4
-2006-11-16,1,5
-2006-11-17,1,6
-2006-11-18,0,7
-2006-11-19,0,1
-2006-11-20,1,2
-2006-11-21,1,3
-2006-11-22,1,4
-2006-11-23,1,5
-2006-11-24,1,6
-2006-11-25,0,7
-2006-11-26,0,1
-2006-11-27,1,2
-2006-11-28,1,3
-2006-11-29,1,4
-2006-11-30,1,5
-2006-12-01,1,6
-2006-12-02,0,7
-2006-12-03,0,1
-2006-12-04,1,2
-2006-12-05,1,3
-2006-12-06,1,4
-2006-12-07,1,5
-2006-12-08,1,6
-2006-12-09,0,7
-2006-12-10,0,1
-2006-12-11,1,2
-2006-12-12,1,3
-2006-12-13,1,4
-2006-12-14,1,5
-2006-12-15,1,6
-2006-12-16,0,7
-2006-12-17,0,1
-2006-12-18,1,2
-2006-12-19,1,3
-2006-12-20,1,4
-2006-12-21,1,5
-2006-12-22,1,6
-2006-12-23,0,7
-2006-12-24,0,1
-2006-12-25,1,2
-2006-12-26,1,3
-2006-12-27,1,4
-2006-12-28,1,5
-2006-12-29,1,6
-2006-12-30,0,7
-2006-12-31,0,1
+trade_date,trade_status,day_week
+2006-01-01,0,1
+2006-01-02,0,2
+2006-01-03,0,3
+2006-01-04,1,4
+2006-01-05,1,5
+2006-01-06,1,6
+2006-01-07,0,7
+2006-01-08,0,1
+2006-01-09,1,2
+2006-01-10,1,3
+2006-01-11,1,4
+2006-01-12,1,5
+2006-01-13,1,6
+2006-01-14,0,7
+2006-01-15,0,1
+2006-01-16,1,2
+2006-01-17,1,3
+2006-01-18,1,4
+2006-01-19,1,5
+2006-01-20,1,6
+2006-01-21,0,7
+2006-01-22,0,1
+2006-01-23,1,2
+2006-01-24,1,3
+2006-01-25,1,4
+2006-01-26,0,5
+2006-01-27,0,6
+2006-01-28,0,7
+2006-01-29,0,1
+2006-01-30,0,2
+2006-01-31,0,3
+2006-02-01,0,4
+2006-02-02,0,5
+2006-02-03,0,6
+2006-02-04,0,7
+2006-02-05,0,1
+2006-02-06,1,2
+2006-02-07,1,3
+2006-02-08,1,4
+2006-02-09,1,5
+2006-02-10,1,6
+2006-02-11,0,7
+2006-02-12,0,1
+2006-02-13,1,2
+2006-02-14,1,3
+2006-02-15,1,4
+2006-02-16,1,5
+2006-02-17,1,6
+2006-02-18,0,7
+2006-02-19,0,1
+2006-02-20,1,2
+2006-02-21,1,3
+2006-02-22,1,4
+2006-02-23,1,5
+2006-02-24,1,6
+2006-02-25,0,7
+2006-02-26,0,1
+2006-02-27,1,2
+2006-02-28,1,3
+2006-03-01,1,4
+2006-03-02,1,5
+2006-03-03,1,6
+2006-03-04,0,7
+2006-03-05,0,1
+2006-03-06,1,2
+2006-03-07,1,3
+2006-03-08,1,4
+2006-03-09,1,5
+2006-03-10,1,6
+2006-03-11,0,7
+2006-03-12,0,1
+2006-03-13,1,2
+2006-03-14,1,3
+2006-03-15,1,4
+2006-03-16,1,5
+2006-03-17,1,6
+2006-03-18,0,7
+2006-03-19,0,1
+2006-03-20,1,2
+2006-03-21,1,3
+2006-03-22,1,4
+2006-03-23,1,5
+2006-03-24,1,6
+2006-03-25,0,7
+2006-03-26,0,1
+2006-03-27,1,2
+2006-03-28,1,3
+2006-03-29,1,4
+2006-03-30,1,5
+2006-03-31,1,6
+2006-04-01,0,7
+2006-04-02,0,1
+2006-04-03,1,2
+2006-04-04,1,3
+2006-04-05,1,4
+2006-04-06,1,5
+2006-04-07,1,6
+2006-04-08,0,7
+2006-04-09,0,1
+2006-04-10,1,2
+2006-04-11,1,3
+2006-04-12,1,4
+2006-04-13,1,5
+2006-04-14,1,6
+2006-04-15,0,7
+2006-04-16,0,1
+2006-04-17,1,2
+2006-04-18,1,3
+2006-04-19,1,4
+2006-04-20,1,5
+2006-04-21,1,6
+2006-04-22,0,7
+2006-04-23,0,1
+2006-04-24,1,2
+2006-04-25,1,3
+2006-04-26,1,4
+2006-04-27,1,5
+2006-04-28,1,6
+2006-04-29,0,7
+2006-04-30,0,1
+2006-05-01,0,2
+2006-05-02,0,3
+2006-05-03,0,4
+2006-05-04,0,5
+2006-05-05,0,6
+2006-05-06,0,7
+2006-05-07,0,1
+2006-05-08,1,2
+2006-05-09,1,3
+2006-05-10,1,4
+2006-05-11,1,5
+2006-05-12,1,6
+2006-05-13,0,7
+2006-05-14,0,1
+2006-05-15,1,2
+2006-05-16,1,3
+2006-05-17,1,4
+2006-05-18,1,5
+2006-05-19,1,6
+2006-05-20,0,7
+2006-05-21,0,1
+2006-05-22,1,2
+2006-05-23,1,3
+2006-05-24,1,4
+2006-05-25,1,5
+2006-05-26,1,6
+2006-05-27,0,7
+2006-05-28,0,1
+2006-05-29,1,2
+2006-05-30,1,3
+2006-05-31,1,4
+2006-06-01,1,5
+2006-06-02,1,6
+2006-06-03,0,7
+2006-06-04,0,1
+2006-06-05,1,2
+2006-06-06,1,3
+2006-06-07,1,4
+2006-06-08,1,5
+2006-06-09,1,6
+2006-06-10,0,7
+2006-06-11,0,1
+2006-06-12,1,2
+2006-06-13,1,3
+2006-06-14,1,4
+2006-06-15,1,5
+2006-06-16,1,6
+2006-06-17,0,7
+2006-06-18,0,1
+2006-06-19,1,2
+2006-06-20,1,3
+2006-06-21,1,4
+2006-06-22,1,5
+2006-06-23,1,6
+2006-06-24,0,7
+2006-06-25,0,1
+2006-06-26,1,2
+2006-06-27,1,3
+2006-06-28,1,4
+2006-06-29,1,5
+2006-06-30,1,6
+2006-07-01,0,7
+2006-07-02,0,1
+2006-07-03,1,2
+2006-07-04,1,3
+2006-07-05,1,4
+2006-07-06,1,5
+2006-07-07,1,6
+2006-07-08,0,7
+2006-07-09,0,1
+2006-07-10,1,2
+2006-07-11,1,3
+2006-07-12,1,4
+2006-07-13,1,5
+2006-07-14,1,6
+2006-07-15,0,7
+2006-07-16,0,1
+2006-07-17,1,2
+2006-07-18,1,3
+2006-07-19,1,4
+2006-07-20,1,5
+2006-07-21,1,6
+2006-07-22,0,7
+2006-07-23,0,1
+2006-07-24,1,2
+2006-07-25,1,3
+2006-07-26,1,4
+2006-07-27,1,5
+2006-07-28,1,6
+2006-07-29,0,7
+2006-07-30,0,1
+2006-07-31,1,2
+2006-08-01,1,3
+2006-08-02,1,4
+2006-08-03,1,5
+2006-08-04,1,6
+2006-08-05,0,7
+2006-08-06,0,1
+2006-08-07,1,2
+2006-08-08,1,3
+2006-08-09,1,4
+2006-08-10,1,5
+2006-08-11,1,6
+2006-08-12,0,7
+2006-08-13,0,1
+2006-08-14,1,2
+2006-08-15,1,3
+2006-08-16,1,4
+2006-08-17,1,5
+2006-08-18,1,6
+2006-08-19,0,7
+2006-08-20,0,1
+2006-08-21,1,2
+2006-08-22,1,3
+2006-08-23,1,4
+2006-08-24,1,5
+2006-08-25,1,6
+2006-08-26,0,7
+2006-08-27,0,1
+2006-08-28,1,2
+2006-08-29,1,3
+2006-08-30,1,4
+2006-08-31,1,5
+2006-09-01,1,6
+2006-09-02,0,7
+2006-09-03,0,1
+2006-09-04,1,2
+2006-09-05,1,3
+2006-09-06,1,4
+2006-09-07,1,5
+2006-09-08,1,6
+2006-09-09,0,7
+2006-09-10,0,1
+2006-09-11,1,2
+2006-09-12,1,3
+2006-09-13,1,4
+2006-09-14,1,5
+2006-09-15,1,6
+2006-09-16,0,7
+2006-09-17,0,1
+2006-09-18,1,2
+2006-09-19,1,3
+2006-09-20,1,4
+2006-09-21,1,5
+2006-09-22,1,6
+2006-09-23,0,7
+2006-09-24,0,1
+2006-09-25,1,2
+2006-09-26,1,3
+2006-09-27,1,4
+2006-09-28,1,5
+2006-09-29,1,6
+2006-09-30,0,7
+2006-10-01,0,1
+2006-10-02,0,2
+2006-10-03,0,3
+2006-10-04,0,4
+2006-10-05,0,5
+2006-10-06,0,6
+2006-10-07,0,7
+2006-10-08,0,1
+2006-10-09,1,2
+2006-10-10,1,3
+2006-10-11,1,4
+2006-10-12,1,5
+2006-10-13,1,6
+2006-10-14,0,7
+2006-10-15,0,1
+2006-10-16,1,2
+2006-10-17,1,3
+2006-10-18,1,4
+2006-10-19,1,5
+2006-10-20,1,6
+2006-10-21,0,7
+2006-10-22,0,1
+2006-10-23,1,2
+2006-10-24,1,3
+2006-10-25,1,4
+2006-10-26,1,5
+2006-10-27,1,6
+2006-10-28,0,7
+2006-10-29,0,1
+2006-10-30,1,2
+2006-10-31,1,3
+2006-11-01,1,4
+2006-11-02,1,5
+2006-11-03,1,6
+2006-11-04,0,7
+2006-11-05,0,1
+2006-11-06,1,2
+2006-11-07,1,3
+2006-11-08,1,4
+2006-11-09,1,5
+2006-11-10,1,6
+2006-11-11,0,7
+2006-11-12,0,1
+2006-11-13,1,2
+2006-11-14,1,3
+2006-11-15,1,4
+2006-11-16,1,5
+2006-11-17,1,6
+2006-11-18,0,7
+2006-11-19,0,1
+2006-11-20,1,2
+2006-11-21,1,3
+2006-11-22,1,4
+2006-11-23,1,5
+2006-11-24,1,6
+2006-11-25,0,7
+2006-11-26,0,1
+2006-11-27,1,2
+2006-11-28,1,3
+2006-11-29,1,4
+2006-11-30,1,5
+2006-12-01,1,6
+2006-12-02,0,7
+2006-12-03,0,1
+2006-12-04,1,2
+2006-12-05,1,3
+2006-12-06,1,4
+2006-12-07,1,5
+2006-12-08,1,6
+2006-12-09,0,7
+2006-12-10,0,1
+2006-12-11,1,2
+2006-12-12,1,3
+2006-12-13,1,4
+2006-12-14,1,5
+2006-12-15,1,6
+2006-12-16,0,7
+2006-12-17,0,1
+2006-12-18,1,2
+2006-12-19,1,3
+2006-12-20,1,4
+2006-12-21,1,5
+2006-12-22,1,6
+2006-12-23,0,7
+2006-12-24,0,1
+2006-12-25,1,2
+2006-12-26,1,3
+2006-12-27,1,4
+2006-12-28,1,5
+2006-12-29,1,6
+2006-12-30,0,7
+2006-12-31,0,1
```

### Comparing `adata-1.2.4/adata/stock/cache/calendar/2024.csv` & `adata-2.0.0b0/adata/stock/cache/calendar/2024.csv`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,367 +1,367 @@
-trade_date,trade_status,day_week
-2024-01-01,0,2
-2024-01-02,1,3
-2024-01-03,1,4
-2024-01-04,1,5
-2024-01-05,1,6
-2024-01-06,0,7
-2024-01-07,0,1
-2024-01-08,1,2
-2024-01-09,1,3
-2024-01-10,1,4
-2024-01-11,1,5
-2024-01-12,1,6
-2024-01-13,0,7
-2024-01-14,0,1
-2024-01-15,1,2
-2024-01-16,1,3
-2024-01-17,1,4
-2024-01-18,1,5
-2024-01-19,1,6
-2024-01-20,0,7
-2024-01-21,0,1
-2024-01-22,1,2
-2024-01-23,1,3
-2024-01-24,1,4
-2024-01-25,1,5
-2024-01-26,1,6
-2024-01-27,0,7
-2024-01-28,0,1
-2024-01-29,1,2
-2024-01-30,1,3
-2024-01-31,1,4
-2024-02-01,1,5
-2024-02-02,1,6
-2024-02-03,0,7
-2024-02-04,0,1
-2024-02-05,1,2
-2024-02-06,1,3
-2024-02-07,1,4
-2024-02-08,1,5
-2024-02-09,0,6
-2024-02-10,0,7
-2024-02-11,0,1
-2024-02-12,0,2
-2024-02-13,0,3
-2024-02-14,0,4
-2024-02-15,0,5
-2024-02-16,0,6
-2024-02-17,0,7
-2024-02-18,0,1
-2024-02-19,1,2
-2024-02-20,1,3
-2024-02-21,1,4
-2024-02-22,1,5
-2024-02-23,1,6
-2024-02-24,0,7
-2024-02-25,0,1
-2024-02-26,1,2
-2024-02-27,1,3
-2024-02-28,1,4
-2024-02-29,1,5
-2024-03-01,1,6
-2024-03-02,0,7
-2024-03-03,0,1
-2024-03-04,1,2
-2024-03-05,1,3
-2024-03-06,1,4
-2024-03-07,1,5
-2024-03-08,1,6
-2024-03-09,0,7
-2024-03-10,0,1
-2024-03-11,1,2
-2024-03-12,1,3
-2024-03-13,1,4
-2024-03-14,1,5
-2024-03-15,1,6
-2024-03-16,0,7
-2024-03-17,0,1
-2024-03-18,1,2
-2024-03-19,1,3
-2024-03-20,1,4
-2024-03-21,1,5
-2024-03-22,1,6
-2024-03-23,0,7
-2024-03-24,0,1
-2024-03-25,1,2
-2024-03-26,1,3
-2024-03-27,1,4
-2024-03-28,1,5
-2024-03-29,1,6
-2024-03-30,0,7
-2024-03-31,0,1
-2024-04-01,1,2
-2024-04-02,1,3
-2024-04-03,1,4
-2024-04-04,0,5
-2024-04-05,0,6
-2024-04-06,0,7
-2024-04-07,0,1
-2024-04-08,1,2
-2024-04-09,1,3
-2024-04-10,1,4
-2024-04-11,1,5
-2024-04-12,1,6
-2024-04-13,0,7
-2024-04-14,0,1
-2024-04-15,1,2
-2024-04-16,1,3
-2024-04-17,1,4
-2024-04-18,1,5
-2024-04-19,1,6
-2024-04-20,0,7
-2024-04-21,0,1
-2024-04-22,1,2
-2024-04-23,1,3
-2024-04-24,1,4
-2024-04-25,1,5
-2024-04-26,1,6
-2024-04-27,0,7
-2024-04-28,0,1
-2024-04-29,1,2
-2024-04-30,1,3
-2024-05-01,0,4
-2024-05-02,0,5
-2024-05-03,0,6
-2024-05-04,0,7
-2024-05-05,0,1
-2024-05-06,1,2
-2024-05-07,1,3
-2024-05-08,1,4
-2024-05-09,1,5
-2024-05-10,1,6
-2024-05-11,0,7
-2024-05-12,0,1
-2024-05-13,1,2
-2024-05-14,1,3
-2024-05-15,1,4
-2024-05-16,1,5
-2024-05-17,1,6
-2024-05-18,0,7
-2024-05-19,0,1
-2024-05-20,1,2
-2024-05-21,1,3
-2024-05-22,1,4
-2024-05-23,1,5
-2024-05-24,1,6
-2024-05-25,0,7
-2024-05-26,0,1
-2024-05-27,1,2
-2024-05-28,1,3
-2024-05-29,1,4
-2024-05-30,1,5
-2024-05-31,1,6
-2024-06-01,0,7
-2024-06-02,0,1
-2024-06-03,1,2
-2024-06-04,1,3
-2024-06-05,1,4
-2024-06-06,1,5
-2024-06-07,1,6
-2024-06-08,0,7
-2024-06-09,0,1
-2024-06-10,0,2
-2024-06-11,1,3
-2024-06-12,1,4
-2024-06-13,1,5
-2024-06-14,1,6
-2024-06-15,0,7
-2024-06-16,0,1
-2024-06-17,1,2
-2024-06-18,1,3
-2024-06-19,1,4
-2024-06-20,1,5
-2024-06-21,1,6
-2024-06-22,0,7
-2024-06-23,0,1
-2024-06-24,1,2
-2024-06-25,1,3
-2024-06-26,1,4
-2024-06-27,1,5
-2024-06-28,1,6
-2024-06-29,0,7
-2024-06-30,0,1
-2024-07-01,1,2
-2024-07-02,1,3
-2024-07-03,1,4
-2024-07-04,1,5
-2024-07-05,1,6
-2024-07-06,0,7
-2024-07-07,0,1
-2024-07-08,1,2
-2024-07-09,1,3
-2024-07-10,1,4
-2024-07-11,1,5
-2024-07-12,1,6
-2024-07-13,0,7
-2024-07-14,0,1
-2024-07-15,1,2
-2024-07-16,1,3
-2024-07-17,1,4
-2024-07-18,1,5
-2024-07-19,1,6
-2024-07-20,0,7
-2024-07-21,0,1
-2024-07-22,1,2
-2024-07-23,1,3
-2024-07-24,1,4
-2024-07-25,1,5
-2024-07-26,1,6
-2024-07-27,0,7
-2024-07-28,0,1
-2024-07-29,1,2
-2024-07-30,1,3
-2024-07-31,1,4
-2024-08-01,1,5
-2024-08-02,1,6
-2024-08-03,0,7
-2024-08-04,0,1
-2024-08-05,1,2
-2024-08-06,1,3
-2024-08-07,1,4
-2024-08-08,1,5
-2024-08-09,1,6
-2024-08-10,0,7
-2024-08-11,0,1
-2024-08-12,1,2
-2024-08-13,1,3
-2024-08-14,1,4
-2024-08-15,1,5
-2024-08-16,1,6
-2024-08-17,0,7
-2024-08-18,0,1
-2024-08-19,1,2
-2024-08-20,1,3
-2024-08-21,1,4
-2024-08-22,1,5
-2024-08-23,1,6
-2024-08-24,0,7
-2024-08-25,0,1
-2024-08-26,1,2
-2024-08-27,1,3
-2024-08-28,1,4
-2024-08-29,1,5
-2024-08-30,1,6
-2024-08-31,0,7
-2024-09-01,0,1
-2024-09-02,1,2
-2024-09-03,1,3
-2024-09-04,1,4
-2024-09-05,1,5
-2024-09-06,1,6
-2024-09-07,0,7
-2024-09-08,0,1
-2024-09-09,1,2
-2024-09-10,1,3
-2024-09-11,1,4
-2024-09-12,1,5
-2024-09-13,1,6
-2024-09-14,0,7
-2024-09-15,0,1
-2024-09-16,0,2
-2024-09-17,0,3
-2024-09-18,1,4
-2024-09-19,1,5
-2024-09-20,1,6
-2024-09-21,0,7
-2024-09-22,0,1
-2024-09-23,1,2
-2024-09-24,1,3
-2024-09-25,1,4
-2024-09-26,1,5
-2024-09-27,1,6
-2024-09-28,0,7
-2024-09-29,0,1
-2024-09-30,1,2
-2024-10-01,0,3
-2024-10-02,0,4
-2024-10-03,0,5
-2024-10-04,0,6
-2024-10-05,0,7
-2024-10-06,0,1
-2024-10-07,0,2
-2024-10-08,1,3
-2024-10-09,1,4
-2024-10-10,1,5
-2024-10-11,1,6
-2024-10-12,0,7
-2024-10-13,0,1
-2024-10-14,1,2
-2024-10-15,1,3
-2024-10-16,1,4
-2024-10-17,1,5
-2024-10-18,1,6
-2024-10-19,0,7
-2024-10-20,0,1
-2024-10-21,1,2
-2024-10-22,1,3
-2024-10-23,1,4
-2024-10-24,1,5
-2024-10-25,1,6
-2024-10-26,0,7
-2024-10-27,0,1
-2024-10-28,1,2
-2024-10-29,1,3
-2024-10-30,1,4
-2024-10-31,1,5
-2024-11-01,1,6
-2024-11-02,0,7
-2024-11-03,0,1
-2024-11-04,1,2
-2024-11-05,1,3
-2024-11-06,1,4
-2024-11-07,1,5
-2024-11-08,1,6
-2024-11-09,0,7
-2024-11-10,0,1
-2024-11-11,1,2
-2024-11-12,1,3
-2024-11-13,1,4
-2024-11-14,1,5
-2024-11-15,1,6
-2024-11-16,0,7
-2024-11-17,0,1
-2024-11-18,1,2
-2024-11-19,1,3
-2024-11-20,1,4
-2024-11-21,1,5
-2024-11-22,1,6
-2024-11-23,0,7
-2024-11-24,0,1
-2024-11-25,1,2
-2024-11-26,1,3
-2024-11-27,1,4
-2024-11-28,1,5
-2024-11-29,1,6
-2024-11-30,0,7
-2024-12-01,0,1
-2024-12-02,1,2
-2024-12-03,1,3
-2024-12-04,1,4
-2024-12-05,1,5
-2024-12-06,1,6
-2024-12-07,0,7
-2024-12-08,0,1
-2024-12-09,1,2
-2024-12-10,1,3
-2024-12-11,1,4
-2024-12-12,1,5
-2024-12-13,1,6
-2024-12-14,0,7
-2024-12-15,0,1
-2024-12-16,1,2
-2024-12-17,1,3
-2024-12-18,1,4
-2024-12-19,1,5
-2024-12-20,1,6
-2024-12-21,0,7
-2024-12-22,0,1
-2024-12-23,1,2
-2024-12-24,1,3
-2024-12-25,1,4
-2024-12-26,1,5
-2024-12-27,1,6
-2024-12-28,0,7
-2024-12-29,0,1
-2024-12-30,1,2
+trade_date,trade_status,day_week
+2024-01-01,0,2
+2024-01-02,1,3
+2024-01-03,1,4
+2024-01-04,1,5
+2024-01-05,1,6
+2024-01-06,0,7
+2024-01-07,0,1
+2024-01-08,1,2
+2024-01-09,1,3
+2024-01-10,1,4
+2024-01-11,1,5
+2024-01-12,1,6
+2024-01-13,0,7
+2024-01-14,0,1
+2024-01-15,1,2
+2024-01-16,1,3
+2024-01-17,1,4
+2024-01-18,1,5
+2024-01-19,1,6
+2024-01-20,0,7
+2024-01-21,0,1
+2024-01-22,1,2
+2024-01-23,1,3
+2024-01-24,1,4
+2024-01-25,1,5
+2024-01-26,1,6
+2024-01-27,0,7
+2024-01-28,0,1
+2024-01-29,1,2
+2024-01-30,1,3
+2024-01-31,1,4
+2024-02-01,1,5
+2024-02-02,1,6
+2024-02-03,0,7
+2024-02-04,0,1
+2024-02-05,1,2
+2024-02-06,1,3
+2024-02-07,1,4
+2024-02-08,1,5
+2024-02-09,0,6
+2024-02-10,0,7
+2024-02-11,0,1
+2024-02-12,0,2
+2024-02-13,0,3
+2024-02-14,0,4
+2024-02-15,0,5
+2024-02-16,0,6
+2024-02-17,0,7
+2024-02-18,0,1
+2024-02-19,1,2
+2024-02-20,1,3
+2024-02-21,1,4
+2024-02-22,1,5
+2024-02-23,1,6
+2024-02-24,0,7
+2024-02-25,0,1
+2024-02-26,1,2
+2024-02-27,1,3
+2024-02-28,1,4
+2024-02-29,1,5
+2024-03-01,1,6
+2024-03-02,0,7
+2024-03-03,0,1
+2024-03-04,1,2
+2024-03-05,1,3
+2024-03-06,1,4
+2024-03-07,1,5
+2024-03-08,1,6
+2024-03-09,0,7
+2024-03-10,0,1
+2024-03-11,1,2
+2024-03-12,1,3
+2024-03-13,1,4
+2024-03-14,1,5
+2024-03-15,1,6
+2024-03-16,0,7
+2024-03-17,0,1
+2024-03-18,1,2
+2024-03-19,1,3
+2024-03-20,1,4
+2024-03-21,1,5
+2024-03-22,1,6
+2024-03-23,0,7
+2024-03-24,0,1
+2024-03-25,1,2
+2024-03-26,1,3
+2024-03-27,1,4
+2024-03-28,1,5
+2024-03-29,1,6
+2024-03-30,0,7
+2024-03-31,0,1
+2024-04-01,1,2
+2024-04-02,1,3
+2024-04-03,1,4
+2024-04-04,0,5
+2024-04-05,0,6
+2024-04-06,0,7
+2024-04-07,0,1
+2024-04-08,1,2
+2024-04-09,1,3
+2024-04-10,1,4
+2024-04-11,1,5
+2024-04-12,1,6
+2024-04-13,0,7
+2024-04-14,0,1
+2024-04-15,1,2
+2024-04-16,1,3
+2024-04-17,1,4
+2024-04-18,1,5
+2024-04-19,1,6
+2024-04-20,0,7
+2024-04-21,0,1
+2024-04-22,1,2
+2024-04-23,1,3
+2024-04-24,1,4
+2024-04-25,1,5
+2024-04-26,1,6
+2024-04-27,0,7
+2024-04-28,0,1
+2024-04-29,1,2
+2024-04-30,1,3
+2024-05-01,0,4
+2024-05-02,0,5
+2024-05-03,0,6
+2024-05-04,0,7
+2024-05-05,0,1
+2024-05-06,1,2
+2024-05-07,1,3
+2024-05-08,1,4
+2024-05-09,1,5
+2024-05-10,1,6
+2024-05-11,0,7
+2024-05-12,0,1
+2024-05-13,1,2
+2024-05-14,1,3
+2024-05-15,1,4
+2024-05-16,1,5
+2024-05-17,1,6
+2024-05-18,0,7
+2024-05-19,0,1
+2024-05-20,1,2
+2024-05-21,1,3
+2024-05-22,1,4
+2024-05-23,1,5
+2024-05-24,1,6
+2024-05-25,0,7
+2024-05-26,0,1
+2024-05-27,1,2
+2024-05-28,1,3
+2024-05-29,1,4
+2024-05-30,1,5
+2024-05-31,1,6
+2024-06-01,0,7
+2024-06-02,0,1
+2024-06-03,1,2
+2024-06-04,1,3
+2024-06-05,1,4
+2024-06-06,1,5
+2024-06-07,1,6
+2024-06-08,0,7
+2024-06-09,0,1
+2024-06-10,0,2
+2024-06-11,1,3
+2024-06-12,1,4
+2024-06-13,1,5
+2024-06-14,1,6
+2024-06-15,0,7
+2024-06-16,0,1
+2024-06-17,1,2
+2024-06-18,1,3
+2024-06-19,1,4
+2024-06-20,1,5
+2024-06-21,1,6
+2024-06-22,0,7
+2024-06-23,0,1
+2024-06-24,1,2
+2024-06-25,1,3
+2024-06-26,1,4
+2024-06-27,1,5
+2024-06-28,1,6
+2024-06-29,0,7
+2024-06-30,0,1
+2024-07-01,1,2
+2024-07-02,1,3
+2024-07-03,1,4
+2024-07-04,1,5
+2024-07-05,1,6
+2024-07-06,0,7
+2024-07-07,0,1
+2024-07-08,1,2
+2024-07-09,1,3
+2024-07-10,1,4
+2024-07-11,1,5
+2024-07-12,1,6
+2024-07-13,0,7
+2024-07-14,0,1
+2024-07-15,1,2
+2024-07-16,1,3
+2024-07-17,1,4
+2024-07-18,1,5
+2024-07-19,1,6
+2024-07-20,0,7
+2024-07-21,0,1
+2024-07-22,1,2
+2024-07-23,1,3
+2024-07-24,1,4
+2024-07-25,1,5
+2024-07-26,1,6
+2024-07-27,0,7
+2024-07-28,0,1
+2024-07-29,1,2
+2024-07-30,1,3
+2024-07-31,1,4
+2024-08-01,1,5
+2024-08-02,1,6
+2024-08-03,0,7
+2024-08-04,0,1
+2024-08-05,1,2
+2024-08-06,1,3
+2024-08-07,1,4
+2024-08-08,1,5
+2024-08-09,1,6
+2024-08-10,0,7
+2024-08-11,0,1
+2024-08-12,1,2
+2024-08-13,1,3
+2024-08-14,1,4
+2024-08-15,1,5
+2024-08-16,1,6
+2024-08-17,0,7
+2024-08-18,0,1
+2024-08-19,1,2
+2024-08-20,1,3
+2024-08-21,1,4
+2024-08-22,1,5
+2024-08-23,1,6
+2024-08-24,0,7
+2024-08-25,0,1
+2024-08-26,1,2
+2024-08-27,1,3
+2024-08-28,1,4
+2024-08-29,1,5
+2024-08-30,1,6
+2024-08-31,0,7
+2024-09-01,0,1
+2024-09-02,1,2
+2024-09-03,1,3
+2024-09-04,1,4
+2024-09-05,1,5
+2024-09-06,1,6
+2024-09-07,0,7
+2024-09-08,0,1
+2024-09-09,1,2
+2024-09-10,1,3
+2024-09-11,1,4
+2024-09-12,1,5
+2024-09-13,1,6
+2024-09-14,0,7
+2024-09-15,0,1
+2024-09-16,0,2
+2024-09-17,0,3
+2024-09-18,1,4
+2024-09-19,1,5
+2024-09-20,1,6
+2024-09-21,0,7
+2024-09-22,0,1
+2024-09-23,1,2
+2024-09-24,1,3
+2024-09-25,1,4
+2024-09-26,1,5
+2024-09-27,1,6
+2024-09-28,0,7
+2024-09-29,0,1
+2024-09-30,1,2
+2024-10-01,0,3
+2024-10-02,0,4
+2024-10-03,0,5
+2024-10-04,0,6
+2024-10-05,0,7
+2024-10-06,0,1
+2024-10-07,0,2
+2024-10-08,1,3
+2024-10-09,1,4
+2024-10-10,1,5
+2024-10-11,1,6
+2024-10-12,0,7
+2024-10-13,0,1
+2024-10-14,1,2
+2024-10-15,1,3
+2024-10-16,1,4
+2024-10-17,1,5
+2024-10-18,1,6
+2024-10-19,0,7
+2024-10-20,0,1
+2024-10-21,1,2
+2024-10-22,1,3
+2024-10-23,1,4
+2024-10-24,1,5
+2024-10-25,1,6
+2024-10-26,0,7
+2024-10-27,0,1
+2024-10-28,1,2
+2024-10-29,1,3
+2024-10-30,1,4
+2024-10-31,1,5
+2024-11-01,1,6
+2024-11-02,0,7
+2024-11-03,0,1
+2024-11-04,1,2
+2024-11-05,1,3
+2024-11-06,1,4
+2024-11-07,1,5
+2024-11-08,1,6
+2024-11-09,0,7
+2024-11-10,0,1
+2024-11-11,1,2
+2024-11-12,1,3
+2024-11-13,1,4
+2024-11-14,1,5
+2024-11-15,1,6
+2024-11-16,0,7
+2024-11-17,0,1
+2024-11-18,1,2
+2024-11-19,1,3
+2024-11-20,1,4
+2024-11-21,1,5
+2024-11-22,1,6
+2024-11-23,0,7
+2024-11-24,0,1
+2024-11-25,1,2
+2024-11-26,1,3
+2024-11-27,1,4
+2024-11-28,1,5
+2024-11-29,1,6
+2024-11-30,0,7
+2024-12-01,0,1
+2024-12-02,1,2
+2024-12-03,1,3
+2024-12-04,1,4
+2024-12-05,1,5
+2024-12-06,1,6
+2024-12-07,0,7
+2024-12-08,0,1
+2024-12-09,1,2
+2024-12-10,1,3
+2024-12-11,1,4
+2024-12-12,1,5
+2024-12-13,1,6
+2024-12-14,0,7
+2024-12-15,0,1
+2024-12-16,1,2
+2024-12-17,1,3
+2024-12-18,1,4
+2024-12-19,1,5
+2024-12-20,1,6
+2024-12-21,0,7
+2024-12-22,0,1
+2024-12-23,1,2
+2024-12-24,1,3
+2024-12-25,1,4
+2024-12-26,1,5
+2024-12-27,1,6
+2024-12-28,0,7
+2024-12-29,0,1
+2024-12-30,1,2
 2024-12-31,1,3
```

### Comparing `adata-1.2.4/adata/stock/cache/code.csv` & `adata-2.0.0b0/adata/stock/cache/code.csv`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,5641 +1,5641 @@
-stock_code,short_name,list_date2
-000001,平安银行,1991-04-03
-000002,万  科Ａ,1991-01-29
-000003,PT金田A,
-000004,国华网安,1990-12-01
-000005,ST星源,1990-12-10
-000006,深振业Ａ,1992-04-27
-000007,*ST全新,1992-04-13
-000008,神州高铁,1992-05-07
-000009,中国宝安,1991-06-25
-000010,美丽生态,1995-10-27
-000011,深物业A,1992-03-30
-000012,南  玻Ａ,1992-02-28
-000013,*ST石化A,
-000014,沙河股份,1992-06-02
-000015,PT中浩A,
-000016,深康佳Ａ,1992-03-27
-000017,深中华A,1992-03-31
-000018,神城A退,
-000019,深粮控股,1992-10-12
-000020,深华发Ａ,1992-04-28
-000021,深科技,1994-02-02
-000023,ST深天,1993-04-29
-000024,招商地产,
-000025,特  力Ａ,1993-06-21
-000026,飞亚达,1993-06-03
-000027,深圳能源,1993-09-03
-000028,国药一致,1993-08-09
-000029,深深房Ａ,1993-09-15
-000030,富奥股份,1993-09-29
-000031,大悦城,1993-10-08
-000032,深桑达Ａ,1993-10-28
-000033,新都退,
-000034,神州数码,1994-05-09
-000035,中国天楹,1994-04-08
-000036,华联控股,1994-06-17
-000037,深南电A,1994-07-01
-000038,大通退,
-000039,中集集团,1994-04-08
-000040,东旭蓝天,1994-08-08
-000042,中洲控股,1994-09-21
-000045,深纺织Ａ,1994-08-15
-000046,*ST泛海,1994-09-12
-000047,ST中侨,
-000048,京基智农,1994-11-01
-000049,德赛电池,1995-03-20
-000050,深天马Ａ,1995-03-15
-000055,方大集团,1996-04-15
-000056,皇庭国际,1996-07-08
-000058,深 赛 格,1996-12-26
-000059,华锦股份,1997-01-30
-000060,中金岭南,1997-01-23
-000061,农 产 品,1997-01-10
-000062,深圳华强,1997-01-30
-000063,中兴通讯,1997-11-18
-000065,北方国际,1998-06-05
-000066,中国长城,1997-06-26
-000068,华控赛格,1997-06-11
-000069,华侨城Ａ,1997-09-10
-000070,特发信息,2000-05-11
-000078,海王生物,1998-12-18
-000088,盐 田 港,1997-07-28
-000089,深圳机场,1998-04-20
-000090,天健集团,1999-07-21
-000096,广聚能源,2000-07-24
-000099,中信海直,2000-07-31
-000100,TCL科技,2004-01-30
-000150,*ST宜康,
-000151,中成股份,2000-09-06
-000153,丰原药业,2000-09-20
-000155,川能动力,2000-09-26
-000156,华数传媒,2000-09-06
-000157,中联重科,2000-10-12
-000158,常山北明,2000-07-24
-000159,国际实业,2000-09-26
-000166,申万宏源,2015-01-26
-000301,东方盛虹,2000-05-29
-000333,美的集团,2013-09-18
-000338,潍柴动力,2007-04-30
-000400,许继电气,1997-04-18
-000401,冀东水泥,1996-06-14
-000402,金 融 街,1996-06-26
-000403,派林生物,1996-06-28
-000404,长虹华意,1996-06-19
-000405,ST鑫光,
-000406,石油大明,
-000407,胜利股份,1996-07-03
-000408,藏格矿业,1996-06-28
-000409,云鼎科技,1996-06-27
-000410,沈阳机床,1996-07-18
-000411,英特集团,1996-07-16
-000412,ST五环,
-000413,东旭光电,1996-09-25
-000415,渤海租赁,1996-07-16
-000416,*ST民控,1996-07-19
-000417,合肥百货,1996-08-12
-000418,小天鹅A,
-000419,通程控股,1996-08-16
-000420,吉林化纤,1996-08-02
-000421,南京公用,1996-08-06
-000422,湖北宜化,1996-08-15
-000423,东阿阿胶,1996-07-29
-000425,徐工机械,1996-08-28
-000426,兴业银锡,1996-08-28
-000428,华天酒店,1996-08-08
-000429,粤高速Ａ,1998-02-20
-000430,张家界,1996-08-29
-000488,晨鸣纸业,2000-11-20
-000498,山东路桥,1997-06-09
-000501,武商集团,1992-11-20
-000502,绿景退,
-000503,国新健康,1992-11-30
-000504,南华生物,1992-12-08
-000505,京粮控股,1992-12-21
-000506,中润资源,1993-03-12
-000507,珠海港,1993-03-26
-000508,琼民源A,
-000509,华塑控股,1993-05-07
-000510,新金路,1993-05-07
-000511,烯碳退,
-000513,丽珠集团,1993-10-28
-000514,渝 开 发,1993-07-12
-000515,攀渝钛业,
-000516,国际医学,1993-08-09
-000517,荣安地产,1993-08-06
-000518,四环生物,1993-09-08
-000519,中兵红箭,1993-10-08
-000520,凤凰航运,1993-10-25
-000521,长虹美菱,1993-10-18
-000522,白云山A,
-000523,广州浪奇,1993-11-08
-000524,岭南控股,1993-11-18
-000525,ST红太阳,1993-10-28
-000526,学大教育,1993-11-01
-000527,美的电器,
-000528,柳    工,1993-11-18
-000529,广弘控股,1993-11-18
-000530,冰山冷热,1993-12-08
-000531,穗恒运Ａ,1994-01-06
-000532,华金资本,1994-01-03
-000533,顺钠股份,1994-01-03
-000534,万泽股份,1994-01-10
-000535,*ST猴王,
-000536,华映科技,1993-11-26
-000537,广宇发展,1993-12-10
-000538,云南白药,1993-12-15
-000539,粤电力Ａ,1993-11-26
-000540,*ST中天,
-000541,佛山照明,1993-11-23
-000542,TCL通讯,
-000543,皖能电力,1993-12-20
-000544,中原环保,1993-12-08
-000545,金浦钛业,1993-12-15
-000546,ST金圆,1993-12-15
-000547,航天发展,1993-11-30
-000548,湖南投资,1993-12-20
-000549,S湘火炬,
-000550,江铃汽车,1993-12-01
-000551,创元科技,1994-01-06
-000552,甘肃能化,1994-01-06
-000553,安道麦A,1993-12-03
-000554,泰山石油,1993-12-15
-000555,神州信息,1994-04-08
-000556,PT南洋,
-000557,西部创业,1994-06-17
-000558,莱茵体育,1994-05-09
-000559,万向钱潮,1994-01-10
-000560,我爱我家,1994-02-02
-000561,烽火电子,1994-05-09
-000562,宏源证券,
-000563,陕国投Ａ,1994-01-10
-000564,ST大集,1994-01-10
-000565,渝三峡Ａ,1994-04-08
-000566,海南海药,1994-05-25
-000567,海德股份,1994-05-25
-000568,泸州老窖,1994-05-09
-000569,长城股份,
-000570,苏常柴Ａ,1994-07-01
-000571,新大洲A,1994-05-25
-000572,海马汽车,1994-08-08
-000573,粤宏远Ａ,1994-08-15
-000576,甘化科工,1994-09-07
-000578,盐湖集团,
-000581,威孚高科,1998-09-24
-000582,北部湾港,1995-11-02
-000583,S*ST托普,
-000584,ST工智,1995-11-28
-000585,东电退,
-000586,汇源通信,1995-12-20
-000587,*ST金洲,
-000588,PT粤金曼,
-000589,贵州轮胎,1996-03-08
-000590,启迪药业,1996-01-19
-000591,太阳能,1996-02-08
-000592,平潭发展,1996-03-27
-000593,德龙汇能,1996-03-12
-000594,国恒退,
-000595,宝塔实业,1996-04-19
-000596,古井贡酒,1996-09-27
-000597,东北制药,1996-05-23
-000598,兴蓉环境,1996-05-29
-000599,青岛双星,1996-04-30
-000600,建投能源,1996-06-06
-000601,韶能股份,1996-08-30
-000602,金马集团,
-000603,盛达资源,1996-08-23
-000605,渤海股份,1996-09-13
-000606,顺利退,
-000607,华媒控股,1996-08-30
-000608,阳光股份,1996-09-19
-000609,中迪投资,1996-10-10
-000610,西安旅游,1996-09-26
-000611,天首退,
-000612,焦作万方,1996-09-26
-000613,东海A退,
-000615,*ST美谷,1996-10-16
-000616,*ST海投,
-000617,中油资本,1996-10-22
-000618,吉林化工,
-000619,海螺新材,1996-10-23
-000620,*ST新联,1996-10-29
-000621,*ST比特,
-000622,恒立实业,1996-11-07
-000623,吉林敖东,1996-10-28
-000625,长安汽车,1997-06-10
-000626,远大控股,1996-11-28
-000627,天茂集团,1996-11-12
-000628,高新发展,1996-11-18
-000629,钒钛股份,1996-11-15
-000630,铜陵有色,1996-11-20
-000631,顺发恒业,1996-11-22
-000632,三木集团,1996-11-21
-000633,合金投资,1996-11-12
-000635,英 力 特,1996-11-20
-000636,风华高科,1996-11-29
-000637,ST实华,1996-11-14
-000638,万方发展,1996-11-26
-000639,西王食品,1996-11-26
-000650,仁和药业,1996-12-10
-000651,格力电器,1996-11-18
-000652,泰达股份,1996-11-28
-000653,ST九州,
-000655,金岭矿业,1996-11-28
-000656,金科股份,1996-11-28
-000657,中钨高新,1996-12-05
-000658,ST海洋,
-000659,珠海中富,1996-12-03
-000660,*ST南华,
-000661,长春高新,1996-12-18
-000662,天夏退,
-000663,永安林业,1996-12-06
-000665,湖北广电,1996-12-10
-000666,经纬纺机,1996-12-10
-000667,ST美置,
-000668,荣丰控股,1996-12-10
-000669,ST金鸿,1996-12-10
-000670,盈方微,1996-12-17
-000671,ST阳光城,
-000672,上峰水泥,1996-12-18
-000673,当代退,
-000675,ST银山,
-000676,智度股份,1996-12-24
-000677,恒天海龙,1996-12-26
-000678,襄阳轴承,1997-01-06
-000679,大连友谊,1997-01-24
-000680,山推股份,1997-01-22
-000681,视觉中国,1997-01-21
-000682,东方电子,1997-01-21
-000683,远兴能源,1997-01-31
-000685,中山公用,1997-01-23
-000686,东北证券,1997-02-27
-000687,华讯退,
-000688,国城矿业,1997-01-20
-000689,ST宏业,
-000690,宝新能源,1997-01-28
-000691,亚太实业,1997-02-28
-000692,*ST惠天,1997-02-27
-000693,华泽退,
-000695,滨海能源,1997-02-18
-000697,*ST炼石,1997-03-25
-000698,沈阳化工,1997-02-20
-000699,S*ST佳纸,
-000700,模塑科技,1997-02-28
-000701,厦门信达,1997-02-26
-000702,正虹科技,1997-03-18
-000703,恒逸石化,1997-03-28
-000705,浙江震元,1997-04-10
-000707,双环科技,1997-04-15
-000708,中信特钢,1997-03-26
-000709,河钢股份,1997-04-16
-000710,贝瑞基因,1997-04-22
-000711,*ST京蓝,1997-04-11
-000712,锦龙股份,1997-04-15
-000713,丰乐种业,1997-04-22
-000715,中兴商业,1997-05-08
-000716,黑芝麻,1997-04-18
-000717,中南股份,1997-05-08
-000718,苏宁环球,1997-04-08
-000719,中原传媒,1997-03-31
-000720,新能泰山,1997-05-09
-000721,西安饮食,1997-04-30
-000722,湖南发展,1997-05-22
-000723,美锦能源,1997-05-15
-000725,京东方Ａ,2001-01-12
-000726,鲁  泰Ａ,2000-12-25
-000727,冠捷科技,1997-05-20
-000728,国元证券,1997-06-16
-000729,燕京啤酒,1997-07-16
-000730,*ST环保,
-000731,四川美丰,1997-06-17
-000732,ST泰禾,
-000733,振华科技,1997-07-03
-000735,罗 牛 山,1997-06-11
-000736,中交地产,1997-04-25
-000737,北方铜业,1997-04-28
-000738,航发控制,1997-06-26
-000739,普洛药业,1997-05-09
-000748,长城信息,
-000750,国海证券,1997-07-09
-000751,锌业股份,1997-06-26
-000752,*ST西发,1997-06-25
-000753,漳州发展,1997-06-26
-000755,山西路桥,1997-06-27
-000756,新华制药,1997-08-06
-000757,浩物股份,1997-06-27
-000758,中色股份,1997-04-16
-000759,中百集团,1997-05-19
-000760,斯太退,
-000761,本钢板材,1998-01-15
-000762,西藏矿业,1997-07-08
-000763,锦州石化,
-000765,*ST华信,
-000766,通化金马,1997-04-30
-000767,晋控电力,1997-06-09
-000768,中航西飞,1997-06-26
-000769,*ST大菲,
-000776,广发证券,1997-06-11
-000777,中核科技,1997-07-10
-000778,新兴铸管,1997-06-06
-000779,甘咨询,1997-05-28
-000780,ST平能,
-000782,美达股份,1997-06-19
-000783,长江证券,1997-07-31
-000785,居然之家,1997-07-11
-000786,北新建材,1997-06-06
-000787,*ST创智,
-000788,北大医药,1997-06-16
-000789,万年青,1997-09-23
-000790,华神科技,1998-03-27
-000791,甘肃能源,1997-10-14
-000792,盐湖股份,1997-09-04
-000793,华闻集团,1997-07-29
-000795,英洛华,1997-08-08
-000796,*ST凯撒,1997-07-03
-000797,中国武夷,1997-07-15
-000798,中水渔业,1998-02-12
-000799,酒鬼酒,1997-07-18
-000800,一汽解放,1997-06-18
-000801,四川九洲,1998-05-06
-000802,北京文化,1998-01-08
-000803,山高环能,1998-03-03
-000805,*ST炎黄,
-000806,银河退,
-000807,云铝股份,1998-04-08
-000809,铁岭新城,1998-06-16
-000810,创维数字,1998-06-02
-000811,冰轮环境,1998-05-28
-000812,陕西金叶,1998-06-23
-000813,德展健康,1998-05-19
-000815,美利云,1998-06-09
-000816,智慧农业,1997-08-18
-000817,辽河油田,
-000818,航锦科技,1997-10-17
-000819,岳阳兴长,1997-06-25
-000820,神雾节能,1998-06-30
-000821,京山轻机,1998-06-26
-000822,山东海化,1998-07-03
-000823,超声电子,1997-10-08
-000825,太钢不锈,1998-10-21
-000826,启迪环境,1998-02-25
-000827,*ST长兴,
-000828,东莞控股,1997-06-17
-000829,天音控股,1997-12-02
-000830,鲁西化工,1998-08-07
-000831,中国稀土,1998-09-11
-000832,*ST龙涤,
-000833,粤桂股份,1998-11-11
-000835,长动退,
-000836,富通信息,1997-09-29
-000837,秦川机床,1998-09-28
-000838,财信发展,1997-06-26
-000839,ST国安,1997-10-31
-000848,承德露露,1997-11-13
-000850,华茂股份,1998-10-07
-000851,高鸿股份,1998-06-09
-000852,石化机械,1998-11-26
-000856,冀东装备,1998-08-13
-000858,五 粮 液,1998-04-27
-000859,国风新材,1998-11-19
-000860,顺鑫农业,1998-11-04
-000861,海印股份,1998-10-28
-000862,银星能源,1998-09-15
-000863,三湘印象,1997-09-25
-000866,扬子石化,
-000868,安凯客车,1997-07-25
-000869,张  裕Ａ,2000-10-26
-000875,吉电股份,2002-09-26
-000876,新 希 望,1998-03-11
-000877,天山股份,1999-01-07
-000878,云南铜业,1998-06-02
-000880,潍柴重机,1998-04-02
-000881,中广核技,1998-09-02
-000882,华联股份,1998-06-16
-000883,湖北能源,1998-05-19
-000885,城发环境,1999-03-19
-000886,海南高速,1998-01-23
-000887,中鼎股份,1998-12-03
-000888,峨眉山Ａ,1997-10-21
-000889,ST中嘉,1997-12-18
-000890,法尔胜,1999-01-19
-000892,欢瑞世纪,1999-01-15
-000893,亚钾国际,1998-12-24
-000895,双汇发展,1998-12-10
-000897,津滨发展,1999-04-22
-000898,鞍钢股份,1997-12-25
-000899,赣能股份,1997-11-26
-000900,现代投资,1999-01-28
-000901,航天科技,1999-04-01
-000902,新洋丰,1999-04-08
-000903,云内动力,1999-04-15
-000905,厦门港务,1999-04-29
-000906,浙商中拓,1999-07-07
-000908,景峰医药,1999-02-03
-000909,ST数源,1999-05-07
-000910,大亚圣象,1999-06-30
-000911,南宁糖业,1999-05-27
-000912,泸天化,1999-06-03
-000913,钱江摩托,1999-05-14
-000915,华特达因,1999-06-09
-000916,华北高速,
-000917,电广传媒,1999-03-25
-000918,*ST嘉凯,
-000919,金陵药业,1999-11-18
-000920,沃顿科技,1999-06-16
-000921,海信家电,1999-07-13
-000922,佳电股份,1999-06-18
-000923,河钢资源,1999-07-14
-000925,众合科技,1999-06-11
-000926,福星股份,1999-06-18
-000927,中国铁物,1999-07-27
-000928,中钢国际,1999-03-12
-000929,兰州黄河,1999-06-23
-000930,中粮科技,1999-07-12
-000931,中 关 村,1999-07-12
-000932,华菱钢铁,1999-08-03
-000933,神火股份,1999-08-31
-000935,四川双马,1999-08-24
-000936,华西股份,1999-08-10
-000937,冀中能源,1999-09-09
-000938,紫光股份,1999-11-04
-000939,凯迪退,
-000948,南天信息,1999-10-14
-000949,新乡化纤,1999-10-21
-000950,重药控股,1999-09-16
-000951,中国重汽,1999-11-25
-000952,广济药业,1999-11-12
-000953,河化股份,1999-12-02
-000955,欣龙控股,1999-12-09
-000956,中原油气,
-000957,中通客车,2000-01-13
-000958,电投产融,1999-12-23
-000959,首钢股份,1999-12-16
-000960,锡业股份,2000-02-21
-000961,中南建设,2000-03-01
-000962,东方钽业,2000-01-20
-000963,华东医药,2000-01-27
-000965,天保基建,2000-04-06
-000966,长源电力,2000-03-16
-000967,盈峰环境,2000-03-30
-000968,蓝焰控股,2000-06-22
-000969,安泰科技,2000-05-29
-000970,中科三环,2000-04-20
-000971,ST高升,2000-04-27
-000972,中基健康,2000-09-26
-000973,佛塑科技,2000-05-25
-000975,银泰黄金,2000-06-08
-000976,ST华铁,2000-06-01
-000977,浪潮信息,2000-06-08
-000978,桂林旅游,2000-05-18
-000979,中弘退,
-000980,众泰汽车,2000-06-16
-000981,山子股份,2000-06-22
-000982,中银绒业,2000-07-06
-000983,山西焦煤,2000-07-26
-000985,大庆华科,2000-07-26
-000987,越秀资本,2000-07-18
-000988,华工科技,2000-06-08
-000989,九 芝 堂,2000-06-28
-000990,诚志股份,2000-07-06
-000993,闽东电力,2000-07-31
-000995,皇台酒业,2000-08-07
-000996,*ST中期,2000-07-18
-000997,新 大 陆,2000-08-07
-000998,隆平高科,2000-12-11
-000999,华润三九,2000-03-09
-001201,东瑞股份,2021-04-28
-001202,炬申股份,2021-04-29
-001203,大中矿业,2021-05-10
-001205,盛航股份,2021-05-13
-001206,依依股份,2021-05-18
-001207,联科科技,2021-06-23
-001208,华菱线缆,2021-06-24
-001209,洪兴股份,2021-07-23
-001210,金房能源,2021-07-29
-001211,双枪科技,2021-08-05
-001212,中旗新材,2021-08-23
-001213,中铁特货,2021-09-08
-001215,千味央厨,2021-09-06
-001216,华瓷股份,2021-10-19
-001217,华尔泰,2021-09-29
-001218,丽臣实业,2021-10-15
-001219,青岛食品,2021-10-21
-001222,源飞宠物,2022-08-18
-001223,欧克科技,2022-12-12
-001225,和泰机电,2023-02-22
-001226,拓山重工,2022-06-22
-001227,兰州银行,2022-01-17
-001228,永泰运,2022-04-29
-001229,魅视科技,2022-08-08
-001230,劲旅环境,2022-07-15
-001231,农心科技,2022-08-19
-001234,泰慕士,2022-01-11
-001236,弘业期货,2022-08-05
-001238,浙江正特,2022-09-19
-001255,博菲电气,2022-09-30
-001256,炜冈科技,2022-12-05
-001258,立新能源,2022-07-27
-001259,利仁科技,2022-08-31
-001260,坤泰股份,2023-02-16
-001266,宏英智能,2022-02-28
-001267,汇绿生态,2021-11-17
-001268,联合精密,2022-06-30
-001269,欧晶科技,2022-09-30
-001270,铖昌科技,2022-06-06
-001278,一彬科技,2023-03-08
-001282,三联锻造,2023-05-24
-001283,豪鹏科技,2022-09-05
-001286,陕西能源,2023-04-10
-001287,中电港,2023-04-10
-001288,运机集团,2021-11-01
-001289,龙源电力,2022-01-24
-001296,长江材料,2021-12-24
-001298,好上好,2022-10-31
-001299,美能能源,2022-10-31
-001300,三柏硕,2022-10-19
-001301,尚太科技,2022-12-28
-001308,康冠科技,2022-03-18
-001309,德明利,2022-07-01
-001311,多利科技,2023-02-27
-001313,粤海饲料,2022-02-16
-001314,亿道信息,2023-02-14
-001316,润贝航科,2022-06-24
-001317,三羊马,2021-11-30
-001318,阳光乳业,2022-05-20
-001319,铭科精技,2022-05-12
-001322,箭牌家居,2022-10-26
-001323,慕思股份,2022-06-23
-001324,长青科技,2023-05-22
-001328,登康口腔,2023-04-10
-001330,博纳影业,2022-08-18
-001331,胜通能源,2022-09-08
-001332,锡装股份,2022-09-20
-001333,光华股份,2022-12-08
-001336,楚环科技,2022-07-25
-001337,四川黄金,2023-03-03
-001338,永顺泰,2022-11-16
-001339,智微智能,2022-08-15
-001360,南矿集团,2023-04-10
-001366,播恩集团,2023-03-07
-001367,海森药业,2023-04-10
-001368,通达创智,2023-03-13
-001373,翔腾新材,2023-06-01
-001380,华纬科技,2023-05-16
-001696,宗申动力,1997-03-06
-001872,招商港口,1993-05-05
-001896,豫能控股,1998-01-22
-001914,招商积余,1994-09-28
-001965,招商公路,2017-12-25
-001979,招商蛇口,2015-12-30
-002001,新 和 成,2004-06-25
-002002,ST鸿达,2004-06-25
-002003,伟星股份,2004-06-25
-002004,华邦健康,2004-06-25
-002005,ST德豪,2004-06-25
-002006,精工科技,2004-06-25
-002007,华兰生物,2004-06-25
-002008,大族激光,2004-06-25
-002009,天奇股份,2004-06-29
-002010,传化智联,2004-06-29
-002011,盾安环境,2004-07-05
-002012,凯恩股份,2004-07-05
-002013,中航机电,
-002014,永新股份,2004-07-08
-002015,协鑫能科,2004-07-08
-002016,世荣兆业,2004-07-08
-002017,东信和平,2004-07-13
-002018,华信退,
-002019,亿帆医药,2004-07-13
-002020,京新药业,2004-07-15
-002021,*ST中捷,2004-07-15
-002022,科华生物,2004-07-21
-002023,海特高新,2004-07-21
-002024,ST易购,2004-07-21
-002025,航天电器,2004-07-26
-002026,山东威达,2004-07-27
-002027,分众传媒,2004-08-04
-002028,思源电气,2004-08-05
-002029,七 匹 狼,2004-08-06
-002030,达安基因,2004-08-09
-002031,巨轮智能,2004-08-16
-002032,苏 泊 尔,2004-08-17
-002033,丽江股份,2004-08-25
-002034,旺能环境,2004-08-26
-002035,华帝股份,2004-09-01
-002036,联创电子,2004-09-03
-002037,保利联合,2004-09-08
-002038,双鹭药业,2004-09-09
-002039,黔源电力,2005-03-03
-002040,南 京 港,2005-03-25
-002041,登海种业,2005-04-18
-002042,华孚时尚,2005-04-27
-002043,兔 宝 宝,2005-05-10
-002044,美年健康,2005-05-18
-002045,国光电器,2005-05-23
-002046,国机精工,2005-05-26
-002047,宝鹰股份,2005-05-31
-002048,宁波华翔,2005-06-03
-002049,紫光国微,2005-06-06
-002050,三花智控,2005-06-07
-002051,中工国际,2006-06-19
-002052,ST同洲,2006-06-27
-002053,云南能投,2006-06-27
-002054,德美化工,2006-07-25
-002055,得润电子,2006-07-25
-002056,横店东磁,2006-08-02
-002057,中钢天源,2006-08-02
-002058,威尔泰,2006-08-02
-002059,云南旅游,2006-08-10
-002060,粤 水 电,2006-08-10
-002061,浙江交科,2006-08-16
-002062,宏润建设,2006-08-16
-002063,远光软件,2006-08-23
-002064,华峰化学,2006-08-23
-002065,东华软件,2006-08-23
-002066,瑞泰科技,2006-08-23
-002067,景兴纸业,2006-09-15
-002068,黑猫股份,2006-09-15
-002069,獐子岛,2006-09-28
-002070,众和退,
-002071,长城退,
-002072,凯瑞德,2006-10-18
-002073,软控股份,2006-10-18
-002074,国轩高科,2006-10-18
-002075,沙钢股份,2006-10-25
-002076,星光股份,2006-10-25
-002077,大港股份,2006-11-16
-002078,太阳纸业,2006-11-16
-002079,苏州固锝,2006-11-16
-002080,中材科技,2006-11-20
-002081,金 螳 螂,2006-11-20
-002082,万邦德,2006-11-20
-002083,孚日股份,2006-11-24
-002084,海鸥住工,2006-11-24
-002085,万丰奥威,2006-11-28
-002086,*ST东洋,2006-11-28
-002087,*ST新纺,2006-11-30
-002088,鲁阳节能,2006-11-30
-002089,*ST新海,2006-11-30
-002090,金智科技,2006-12-08
-002091,江苏国泰,2006-12-08
-002092,中泰化学,2006-12-08
-002093,国脉科技,2006-12-15
-002094,青岛金王,2006-12-15
-002095,生 意 宝,2006-12-15
-002096,易普力,2006-12-22
-002097,山河智能,2006-12-22
-002098,浔兴股份,2006-12-22
-002099,海翔药业,2006-12-26
-002100,天康生物,2006-12-26
-002101,广东鸿图,2006-12-29
-002102,冠福股份,2006-12-29
-002103,广博股份,2007-01-10
-002104,恒宝股份,2007-01-10
-002105,信隆健康,2007-01-12
-002106,莱宝高科,2007-01-12
-002107,沃华医药,2007-01-24
-002108,沧州明珠,2007-01-24
-002109,兴化股份,2007-01-26
-002110,三钢闽光,2007-01-26
-002111,威海广泰,2007-01-26
-002112,三变科技,2007-02-08
-002113,*ST天润,
-002114,罗平锌电,2007-02-15
-002115,三维通信,2007-02-15
-002116,中国海诚,2007-02-15
-002117,东港股份,2007-03-02
-002118,*ST紫鑫,
-002119,康强电子,2007-03-02
-002120,韵达股份,2007-03-06
-002121,科陆电子,2007-03-06
-002122,汇洲智能,2007-03-28
-002123,梦网科技,2007-03-28
-002124,天邦食品,2007-04-03
-002125,湘潭电化,2007-04-03
-002126,银轮股份,2007-04-18
-002127,南极电商,2007-04-18
-002128,电投能源,2007-04-18
-002129,TCL中环,2007-04-20
-002130,沃尔核材,2007-04-20
-002131,利欧股份,2007-04-27
-002132,恒星科技,2007-04-27
-002133,广宇集团,2007-04-27
-002134,天津普林,2007-05-16
-002135,东南网架,2007-05-30
-002136,安 纳 达,2007-05-30
-002137,实益达,2007-06-13
-002138,顺络电子,2007-06-13
-002139,拓邦股份,2007-06-29
-002140,东华科技,2007-07-12
-002141,贤丰控股,2007-07-20
-002142,宁波银行,2007-07-19
-002143,印纪退,
-002144,宏达高科,2007-08-03
-002145,中核钛白,2007-08-03
-002146,荣盛发展,2007-08-08
-002147,新光退,
-002148,北纬科技,2007-08-10
-002149,西部材料,2007-08-10
-002150,通润装备,2007-08-10
-002151,北斗星通,2007-08-13
-002152,广电运通,2007-08-13
-002153,石基信息,2007-08-13
-002154,报 喜 鸟,2007-08-16
-002155,湖南黄金,2007-08-16
-002156,通富微电,2007-08-16
-002157,*ST 正邦,2007-08-17
-002158,汉钟精机,2007-08-17
-002159,三特索道,2007-08-17
-002160,常铝股份,2007-08-21
-002161,远 望 谷,2007-08-21
-002162,悦心健康,2007-08-23
-002163,海南发展,2007-08-23
-002164,宁波东力,2007-08-23
-002165,红 宝 丽,2007-09-13
-002166,莱茵生物,2007-09-13
-002167,东方锆业,2007-09-13
-002168,惠程科技,2007-09-19
-002169,智光电气,2007-09-19
-002170,芭田股份,2007-09-19
-002171,楚江新材,2007-09-21
-002172,澳洋健康,2007-09-21
-002173,创新医疗,2007-09-25
-002174,游族网络,2007-09-25
-002175,东方智造,2007-10-12
-002176,江特电机,2007-10-12
-002177,御银股份,2007-11-01
-002178,延华智能,2007-11-01
-002179,中航光电,2007-11-01
-002180,纳思达,2007-11-13
-002181,粤 传 媒,2007-11-16
-002182,宝武镁业,2007-11-13
-002183,怡 亚 通,2007-11-13
-002184,海得控制,2007-11-16
-002185,华天科技,2007-11-20
-002186,全 聚 德,2007-11-20
-002187,广百股份,2007-11-22
-002188,中天服务,2007-11-22
-002189,中光学,2007-12-03
-002190,成飞集成,2007-12-03
-002191,劲嘉股份,2007-12-05
-002192,融捷股份,2007-12-05
-002193,如意集团,2007-12-07
-002194,武汉凡谷,2007-12-07
-002195,岩山科技,2007-12-12
-002196,方正电机,2007-12-12
-002197,证通电子,2007-12-18
-002198,嘉应制药,2007-12-18
-002199,东晶电子,2007-12-21
-002200,ST交投,2007-12-21
-002201,正威新材,2007-12-26
-002202,金风科技,2007-12-26
-002203,海亮股份,2008-01-16
-002204,大连重工,2008-01-16
-002205,国统股份,2008-01-23
-002206,海 利 得,2008-01-23
-002207,准油股份,2008-01-28
-002208,合肥城建,2008-01-28
-002209,达 意 隆,2008-01-30
-002210,飞马国际,2008-01-30
-002211,宏达新材,2008-02-01
-002212,天融信,2008-02-01
-002213,大为股份,2008-02-01
-002214,大立科技,2008-02-18
-002215,诺 普 信,2008-02-18
-002216,三全食品,2008-02-20
-002217,合力泰,2008-02-20
-002218,拓日新能,2008-02-28
-002219,新里程,2008-03-06
-002220,天宝退,
-002221,东华能源,2008-03-06
-002222,福晶科技,2008-03-19
-002223,鱼跃医疗,2008-04-18
-002224,三 力 士,2008-04-25
-002225,濮耐股份,2008-04-25
-002226,江南化工,2008-05-06
-002227,奥 特 迅,2008-05-06
-002228,合兴包装,2008-05-08
-002229,鸿博股份,2008-05-08
-002230,科大讯飞,2008-05-12
-002231,奥维通信,2008-05-12
-002232,启明信息,2008-05-09
-002233,塔牌集团,2008-05-16
-002234,民和股份,2008-05-16
-002235,安妮股份,2008-05-16
-002236,大华股份,2008-05-20
-002237,恒邦股份,2008-05-20
-002238,天威视讯,2008-05-26
-002239,奥特佳,2008-05-22
-002240,盛新锂能,2008-05-23
-002241,歌尔股份,2008-05-22
-002242,九阳股份,2008-05-28
-002243,力合科创,2008-05-28
-002244,滨江集团,2008-05-29
-002245,蔚蓝锂芯,2008-06-05
-002246,北化股份,2008-06-05
-002247,聚力文化,2008-06-12
-002248,华东数控,2008-06-12
-002249,大洋电机,2008-06-19
-002250,联化科技,2008-06-19
-002251,步 步 高,2008-06-19
-002252,上海莱士,2008-06-23
-002253,川大智胜,2008-06-23
-002254,泰和新材,2008-06-25
-002255,海陆重工,2008-06-25
-002256,兆新股份,2008-06-25
-002258,利尔化学,2008-07-08
-002259,ST升达,2008-07-16
-002260,德奥退,
-002261,拓维信息,2008-07-23
-002262,恩华药业,2008-07-23
-002263,大东南,2008-07-28
-002264,新 华 都,2008-07-31
-002265,建设工业,2008-08-06
-002266,浙富控股,2008-08-06
-002267,陕天然气,2008-08-13
-002268,电科网安,2008-08-11
-002269,美邦服饰,2008-08-28
-002270,华明装备,2008-09-05
-002271,东方雨虹,2008-09-10
-002272,川润股份,2008-09-19
-002273,水晶光电,2008-09-19
-002274,华昌化工,2008-09-25
-002275,桂林三金,2009-07-10
-002276,万马股份,2009-07-10
-002277,友阿股份,2009-07-17
-002278,神开股份,2009-08-11
-002279,久其软件,2009-08-11
-002280,联络互动,2009-08-21
-002281,光迅科技,2009-08-21
-002282,博深股份,2009-08-21
-002283,天润工业,2009-08-21
-002284,亚太股份,2009-08-28
-002285,世联行,2009-08-28
-002286,保龄宝,2009-08-28
-002287,奇正藏药,2009-08-28
-002288,超华科技,2009-09-03
-002289,ST宇顺,2009-09-03
-002290,禾盛新材,2009-09-03
-002291,遥望科技,2009-09-03
-002292,奥飞娱乐,2009-09-10
-002293,罗莱生活,2009-09-10
-002294,信立泰,2009-09-10
-002295,精艺股份,2009-09-29
-002296,辉煌科技,2009-09-29
-002297,博云新材,2009-09-29
-002298,中电兴发,2009-09-29
-002299,圣农发展,2009-10-21
-002300,太阳电缆,2009-10-21
-002301,齐心集团,2009-10-21
-002302,西部建设,2009-11-03
-002303,美盈森,2009-11-03
-002304,洋河股份,2009-11-06
-002305,南国置业,2009-11-06
-002306,中科云网,2009-11-11
-002307,北新路桥,2009-11-11
-002308,威创股份,2009-11-27
-002309,ST中利,2009-11-27
-002310,东方园林,2009-11-27
-002311,海大集团,2009-11-27
-002312,川发龙蟒,2009-12-03
-002313,*ST日海,2009-12-03
-002314,南山控股,2009-12-03
-002315,焦点科技,2009-12-09
-002316,亚联发展,2009-12-09
-002317,众生药业,2009-12-11
-002318,久立特材,2009-12-11
-002319,乐通股份,2009-12-11
-002320,海峡股份,2009-12-16
-002321,华英农业,2009-12-16
-002322,理工能科,2009-12-18
-002323,雅博股份,2009-12-18
-002324,普利特,2009-12-18
-002325,洪涛股份,2009-12-22
-002326,永太科技,2009-12-22
-002327,富安娜,2009-12-30
-002328,新朋股份,2009-12-30
-002329,皇氏集团,2010-01-06
-002330,得利斯,2010-01-06
-002331,皖通科技,2010-01-06
-002332,仙琚制药,2010-01-12
-002333,罗普斯金,2010-01-12
-002334,英威腾,2010-01-13
-002335,科华数据,2010-01-13
-002336,人人乐,2010-01-13
-002337,赛象科技,2010-01-15
-002338,奥普光电,2010-01-15
-002339,积成电子,2010-01-22
-002340,格林美,2010-01-22
-002341,新纶新材,2010-01-22
-002342,巨力索具,2010-01-26
-002343,慈文传媒,2010-01-26
-002344,海宁皮城,2010-01-26
-002345,潮宏基,2010-01-28
-002346,柘中股份,2010-01-28
-002347,泰尔股份,2010-01-28
-002348,高乐股份,2010-02-03
-002349,精华制药,2010-02-03
-002350,北京科锐,2010-02-03
-002351,漫步者,2010-02-05
-002352,顺丰控股,2010-02-05
-002353,杰瑞股份,2010-02-05
-002354,天娱数科,2010-02-09
-002355,兴民智通,2010-02-09
-002356,赫美集团,2010-02-09
-002357,富临运业,2010-02-10
-002358,森源电气,2010-02-10
-002359,北讯退,
-002360,同德化工,2010-03-03
-002361,神剑股份,2010-03-03
-002362,汉王科技,2010-03-03
-002363,隆基机械,2010-03-05
-002364,中恒电气,2010-03-05
-002365,永安药业,2010-03-05
-002366,融发核电,2010-03-12
-002367,康力电梯,2010-03-12
-002368,太极股份,2010-03-12
-002369,卓翼科技,2010-03-16
-002370,亚太药业,2010-03-16
-002371,北方华创,2010-03-16
-002372,伟星新材,2010-03-18
-002373,千方科技,2010-03-18
-002374,中锐股份,2010-03-18
-002375,亚厦股份,2010-03-23
-002376,新北洋,2010-03-23
-002377,国创高新,2010-03-23
-002378,章源钨业,2010-03-31
-002379,宏创控股,2010-03-31
-002380,科远智慧,2010-03-31
-002381,双箭股份,2010-04-02
-002382,蓝帆医疗,2010-04-02
-002383,合众思壮,2010-04-02
-002384,东山精密,2010-04-09
-002385,大北农,2010-04-09
-002386,天原股份,2010-04-09
-002387,维信诺,2010-04-13
-002388,新亚制程,2010-04-13
-002389,航天彩虹,2010-04-13
-002390,信邦制药,2010-04-16
-002391,长青股份,2010-04-16
-002392,北京利尔,2010-04-23
-002393,力生制药,2010-04-23
-002394,联发股份,2010-04-23
-002395,双象股份,2010-04-29
-002396,星网锐捷,2010-06-23
-002397,梦洁股份,2010-04-29
-002398,垒知集团,2010-05-06
-002399,海普瑞,2010-05-06
-002400,省广集团,2010-05-06
-002401,中远海科,2010-05-06
-002402,和而泰,2010-05-11
-002403,爱仕达,2010-05-11
-002404,嘉欣丝绸,2010-05-11
-002405,四维图新,2010-05-18
-002406,远东传动,2010-05-18
-002407,多氟多,2010-05-18
-002408,齐翔腾达,2010-05-18
-002409,雅克科技,2010-05-25
-002410,广联达,2010-05-25
-002411,必康退,
-002412,汉森制药,2010-05-25
-002413,雷科防务,2010-05-28
-002414,高德红外,2010-07-16
-002415,海康威视,2010-05-28
-002416,爱施德,2010-05-28
-002417,深南退,
-002418,康盛股份,2010-06-01
-002419,天虹股份,2010-06-01
-002420,毅昌科技,2010-06-01
-002421,达实智能,2010-06-03
-002422,科伦药业,2010-06-03
-002423,中粮资本,2010-06-03
-002424,贵州百灵,2010-06-03
-002425,凯撒文化,2010-06-08
-002426,胜利精密,2010-06-08
-002427,尤夫股份,2010-06-08
-002428,云南锗业,2010-06-08
-002429,兆驰股份,2010-06-10
-002430,杭氧股份,2010-06-10
-002431,棕榈股份,2010-06-10
-002432,九安医疗,2010-06-10
-002433,*ST太安,2010-06-18
-002434,万里扬,2010-06-18
-002435,长江健康,2010-06-18
-002436,兴森科技,2010-06-18
-002437,誉衡药业,2010-06-23
-002438,江苏神通,2010-06-23
-002439,启明星辰,2010-06-23
-002440,闰土股份,2010-07-06
-002441,众业达,2010-07-06
-002442,龙星化工,2010-07-06
-002443,金洲管道,2010-07-06
-002444,巨星科技,2010-07-13
-002445,中南文化,2010-07-13
-002446,盛路通信,2010-07-13
-002447,晨鑫退,
-002448,中原内配,2010-07-16
-002449,国星光电,2010-07-16
-002450,康得退,
-002451,摩恩电气,2010-07-20
-002452,长高电新,2010-07-20
-002453,华软科技,2010-07-20
-002454,松芝股份,2010-07-20
-002455,百川股份,2010-08-03
-002456,欧菲光,2010-08-03
-002457,青龙管业,2010-08-03
-002458,益生股份,2010-08-10
-002459,晶澳科技,2010-08-10
-002460,赣锋锂业,2010-08-10
-002461,珠江啤酒,2010-08-18
-002462,嘉事堂,2010-08-18
-002463,沪电股份,2010-08-18
-002464,众应退,
-002465,海格通信,2010-08-31
-002466,天齐锂业,2010-08-31
-002467,二六三,2010-09-08
-002468,申通快递,2010-09-08
-002469,三维化学,2010-09-08
-002470,金正大,2010-09-08
-002471,中超控股,2010-09-10
-002472,双环传动,2010-09-10
-002473,圣莱退,
-002474,榕基软件,2010-09-15
-002475,立讯精密,2010-09-15
-002476,宝莫股份,2010-09-15
-002477,雏鹰退,
-002478,常宝股份,2010-09-21
-002479,富春环保,2010-09-21
-002480,新筑股份,2010-09-21
-002481,双塔食品,2010-09-21
-002482,*ST广田,2010-09-29
-002483,润邦股份,2010-09-29
-002484,江海股份,2010-09-29
-002485,*ST雪发,2010-10-15
-002486,嘉麟杰,2010-10-15
-002487,大金重工,2010-10-15
-002488,金固股份,2010-10-21
-002489,浙江永强,2010-10-21
-002490,山东墨龙,2010-10-21
-002491,通鼎互联,2010-10-21
-002492,恒基达鑫,2010-11-02
-002493,荣盛石化,2010-11-02
-002494,华斯股份,2010-11-02
-002495,佳隆股份,2010-11-02
-002496,辉丰股份,2010-11-09
-002497,雅化集团,2010-11-09
-002498,汉缆股份,2010-11-09
-002499,科林退,
-002500,山西证券,2010-11-15
-002501,利源股份,2010-11-17
-002502,ST鼎龙,2010-11-17
-002503,*ST搜特,
-002504,*ST弘高,
-002505,鹏都农牧,2010-11-18
-002506,协鑫集成,2010-11-18
-002507,涪陵榨菜,2010-11-23
-002508,老板电器,2010-11-23
-002509,天茂退,
-002510,天汽模,2010-11-25
-002511,中顺洁柔,2010-11-25
-002512,达华智能,2010-12-03
-002513,蓝丰生化,2010-12-03
-002514,宝馨科技,2010-12-03
-002515,金字火腿,2010-12-03
-002516,旷达科技,2010-12-07
-002517,恺英网络,2010-12-07
-002518,科士达,2010-12-07
-002519,银河电子,2010-12-07
-002520,日发精机,2010-12-10
-002521,齐峰新材,2010-12-10
-002522,浙江众成,2010-12-10
-002523,天桥起重,2010-12-10
-002524,光正眼科,2010-12-17
-002526,山东矿机,2010-12-17
-002527,新时达,2010-12-24
-002528,英飞拓,2010-12-24
-002529,海源复材,2010-12-24
-002530,金财互联,2010-12-31
-002531,天顺风能,2010-12-31
-002532,天山铝业,2010-12-31
-002533,金杯电工,2010-12-31
-002534,西子洁能,2011-01-10
-002535,林州重机,2011-01-11
-002536,飞龙股份,2011-01-11
-002537,海联金汇,2011-01-10
-002538,司尔特,2011-01-18
-002539,云图控股,2011-01-18
-002540,亚太科技,2011-01-18
-002541,鸿路钢构,2011-01-18
-002542,中化岩土,2011-01-28
-002543,万和电气,2011-01-28
-002544,普天科技,2011-01-28
-002545,东方铁塔,2011-02-11
-002546,新联电子,2011-02-11
-002547,春兴精工,2011-02-18
-002548,金新农,2011-02-18
-002549,凯美特气,2011-02-18
-002550,千红制药,2011-02-18
-002551,尚荣医疗,2011-02-25
-002552,宝鼎科技,2011-02-25
-002553,南方精工,2011-02-25
-002554,惠博普,2011-02-25
-002555,三七互娱,2011-03-02
-002556,辉隆股份,2011-03-02
-002557,洽洽食品,2011-03-02
-002558,巨人网络,2011-03-02
-002559,亚威股份,2011-03-03
-002560,通达股份,2011-03-03
-002561,徐家汇,2011-03-03
-002562,兄弟科技,2011-03-10
-002563,森马服饰,2011-03-11
-002564,*ST天沃,2011-03-10
-002565,顺灏股份,2011-03-18
-002566,益盛药业,2011-03-18
-002567,唐人神,2011-03-25
-002568,百润股份,2011-03-25
-002569,ST步森,2011-04-12
-002570,贝因美,2011-04-12
-002571,德力股份,2011-04-12
-002572,索菲亚,2011-04-12
-002573,清新环境,2011-04-22
-002574,明牌珠宝,2011-04-22
-002575,群兴玩具,2011-04-22
-002576,通达动力,2011-04-28
-002577,雷柏科技,2011-04-28
-002578,闽发铝业,2011-04-28
-002579,中京电子,2011-05-06
-002580,圣阳股份,2011-05-06
-002581,未名医药,2011-05-20
-002582,好想你,2011-05-20
-002583,海能达,2011-05-27
-002584,西陇科学,2011-06-02
-002585,双星新材,2011-06-02
-002586,*ST围海,2011-06-02
-002587,奥拓电子,2011-06-10
-002588,史丹利,2011-06-10
-002589,瑞康医药,2011-06-10
-002590,万安科技,2011-06-10
-002591,恒大高新,2011-06-21
-002592,ST八菱,2011-11-11
-002593,日上集团,2011-06-28
-002594,比亚迪,2011-06-30
-002595,豪迈科技,2011-06-28
-002596,海南瑞泽,2011-07-07
-002597,金禾实业,2011-07-07
-002598,山东章鼓,2011-07-07
-002599,盛通股份,2011-07-15
-002600,领益智造,2011-07-15
-002601,龙佰集团,2011-07-15
-002602,世纪华通,2011-07-28
-002603,以岭药业,2011-07-28
-002604,龙力退,
-002605,姚记科技,2011-08-05
-002606,大连电瓷,2011-08-05
-002607,中公教育,2011-08-10
-002608,江苏国信,2011-08-10
-002609,捷顺科技,2011-08-15
-002610,爱康科技,2011-08-15
-002611,东方精工,2011-08-30
-002612,朗姿股份,2011-08-30
-002613,北玻股份,2011-08-30
-002614,奥佳华,2011-09-09
-002615,哈尔斯,2011-09-09
-002616,长青集团,2011-09-20
-002617,露笑科技,2011-09-20
-002618,丹邦退,
-002619,*ST艾格,
-002620,瑞和股份,2011-09-29
-002621,美吉姆,2011-09-29
-002622,皓宸医疗,2011-10-18
-002623,亚玛顿,2011-10-13
-002624,完美世界,2011-10-28
-002625,光启技术,2011-11-03
-002626,金达威,2011-10-28
-002627,三峡旅游,2011-11-03
-002628,成都路桥,2011-11-03
-002629,仁智股份,2011-11-03
-002630,华西能源,2011-11-11
-002631,德尔未来,2011-11-11
-002632,道明光学,2011-11-22
-002633,申科股份,2011-11-22
-002634,棒杰股份,2011-12-05
-002635,安洁科技,2011-11-25
-002636,金安国纪,2011-11-25
-002637,赞宇科技,2011-11-25
-002638,勤上股份,2011-11-25
-002639,雪人股份,2011-12-05
-002640,跨境通,2011-12-08
-002641,公元股份,2011-12-08
-002642,荣联科技,2011-12-20
-002643,万润股份,2011-12-20
-002644,佛慈制药,2011-12-22
-002645,华宏科技,2011-12-20
-002646,天佑德酒,2011-12-22
-002647,仁东控股,2011-12-28
-002648,卫星化学,2011-12-28
-002649,博彦科技,2012-01-06
-002650,加加食品,2012-01-06
-002651,利君股份,2012-01-06
-002652,扬子新材,2012-01-19
-002653,海思科,2012-01-17
-002654,万润科技,2012-02-17
-002655,共达电声,2012-02-17
-002656,ST摩登,2012-02-28
-002657,中科金财,2012-02-28
-002658,雪迪龙,2012-03-09
-002659,凯文教育,2012-03-09
-002660,茂硕电源,2012-03-16
-002661,克明食品,2012-03-16
-002662,京威股份,2012-03-09
-002663,普邦股份,2012-03-16
-002664,信质集团,2012-03-16
-002665,首航高科,2012-03-27
-002666,德联集团,2012-03-27
-002667,威领股份,2012-03-29
-002668,奥马电器,2012-04-16
-002669,康达新材,2012-04-16
-002670,国盛金控,2012-04-16
-002671,龙泉股份,2012-04-26
-002672,东江环保,2012-04-26
-002673,西部证券,2012-05-03
-002674,兴业科技,2012-05-07
-002675,东诚药业,2012-05-25
-002676,顺威股份,2012-05-25
-002677,浙江美大,2012-05-25
-002678,珠江钢琴,2012-05-30
-002679,福建金森,2012-06-05
-002680,长生退,
-002681,奋达科技,2012-06-05
-002682,龙洲股份,2012-06-12
-002683,广东宏大,2012-06-12
-002684,猛狮退,
-002685,华东重机,2012-06-12
-002686,亿利达,2012-07-03
-002687,乔治白,2012-07-13
-002688,金河生物,2012-07-13
-002689,远大智能,2012-07-17
-002690,美亚光电,2012-07-31
-002691,冀凯股份,2012-07-31
-002692,ST远程,2012-08-08
-002693,双成药业,2012-08-08
-002694,顾地科技,2012-08-16
-002695,煌上煌,2012-09-05
-002696,百洋股份,2012-09-05
-002697,红旗连锁,2012-09-05
-002698,博实股份,2012-09-11
-002699,*ST美盛,2012-09-11
-002700,ST浩源,2012-09-21
-002701,奥瑞金,2012-10-11
-002702,海欣食品,2012-10-11
-002703,浙江世宝,2012-11-02
-002705,新宝股份,2014-01-21
-002706,良信股份,2014-01-21
-002707,众信旅游,2014-01-23
-002708,光洋股份,2014-01-21
-002709,天赐材料,2014-01-23
-002711,欧浦退,
-002712,思美传媒,2014-01-23
-002713,东易日盛,2014-02-19
-002714,牧原股份,2014-01-28
-002715,登云股份,2014-02-19
-002716,金贵银业,2014-01-28
-002717,岭南股份,2014-02-19
-002718,友邦吊顶,2014-01-28
-002719,麦趣尔,2014-01-28
-002721,*ST金一,2014-01-27
-002722,物产金轮,2014-01-28
-002723,小崧股份,2014-01-29
-002724,海洋王,2014-11-04
-002725,跃岭股份,2014-01-29
-002726,龙大美食,2014-06-26
-002727,一心堂,2014-07-02
-002728,特一药业,2014-07-31
-002729,好利科技,2014-09-12
-002730,电光科技,2014-10-09
-002731,萃华珠宝,2014-11-04
-002732,燕塘乳业,2014-12-05
-002733,雄韬股份,2014-12-03
-002734,利民股份,2015-01-27
-002735,王子新材,2014-12-03
-002736,国信证券,2014-12-29
-002737,葵花药业,2014-12-30
-002738,中矿资源,2014-12-30
-002739,万达电影,2015-01-22
-002740,*ST爱迪,2015-01-22
-002741,光华科技,2015-02-16
-002742,ST三圣,2015-02-17
-002743,富煌钢构,2015-02-17
-002745,木林森,2015-02-17
-002746,仙坛股份,2015-02-16
-002747,埃斯顿,2015-03-20
-002748,世龙实业,2015-03-19
-002749,国光股份,2015-03-20
-002750,龙津药业,2015-03-24
-002751,易尚退,
-002752,昇兴股份,2015-04-22
-002753,永东股份,2015-05-19
-002755,奥赛康,2015-05-15
-002756,永兴材料,2015-05-15
-002757,南兴股份,2015-05-27
-002758,浙农股份,2015-05-27
-002759,天际股份,2015-05-28
-002760,凤形股份,2015-06-11
-002761,浙江建投,2015-06-10
-002762,金发拉比,2015-06-10
-002763,汇洁股份,2015-06-10
-002765,蓝黛科技,2015-06-12
-002766,索菱股份,2015-06-11
-002767,先锋电子,2015-06-12
-002768,国恩股份,2015-06-30
-002769,普路通,2015-06-29
-002770,科迪退,
-002771,真视通,2015-06-29
-002772,众兴菌业,2015-06-26
-002773,康弘药业,2015-06-26
-002774,快意电梯,2017-03-24
-002775,文科园林,2015-06-29
-002776,*ST柏龙,2015-06-26
-002777,久远银海,2015-12-31
-002778,中晟高科,2016-01-06
-002779,中坚科技,2015-12-09
-002780,三夫户外,2015-12-09
-002781,奇信退,
-002782,可立克,2015-12-22
-002783,凯龙股份,2015-12-09
-002785,万里石,2015-12-23
-002786,银宝山新,2015-12-23
-002787,华源控股,2015-12-31
-002788,鹭燕医药,2016-02-18
-002789,建艺集团,2016-03-11
-002790,瑞尔特,2016-03-08
-002791,坚朗五金,2016-03-29
-002792,通宇通讯,2016-03-28
-002793,罗欣药业,2016-04-15
-002795,永和智控,2016-04-28
-002796,世嘉科技,2016-05-10
-002797,第一创业,2016-05-11
-002798,帝欧家居,2016-05-25
-002799,环球印务,2016-06-08
-002800,ST天顺,2016-05-30
-002801,微光股份,2016-06-22
-002802,洪汇新材,2016-06-29
-002803,吉宏股份,2016-07-12
-002805,丰元股份,2016-07-07
-002806,华锋股份,2016-07-26
-002807,江阴银行,2016-09-02
-002808,ST恒久,2016-08-12
-002809,红墙股份,2016-08-23
-002810,山东赫达,2016-08-26
-002811,郑中设计,2016-09-08
-002812,恩捷股份,2016-09-14
-002813,路畅科技,2016-10-12
-002815,崇达技术,2016-10-12
-002816,*ST和科,2016-10-25
-002817,黄山胶囊,2016-10-25
-002818,富森美,2016-11-09
-002819,东方中科,2016-11-11
-002820,桂发祥,2016-11-18
-002821,凯莱英,2016-11-18
-002822,中装建设,2016-11-29
-002823,凯中精密,2016-11-24
-002824,和胜股份,2017-01-12
-002825,纳尔股份,2016-11-29
-002826,易明医药,2016-12-09
-002827,高争民爆,2016-12-09
-002828,贝肯能源,2016-12-08
-002829,星网宇达,2016-12-13
-002830,名雕股份,2016-12-13
-002831,裕同科技,2016-12-16
-002832,比音勒芬,2016-12-23
-002833,弘亚数控,2016-12-28
-002835,同为股份,2016-12-28
-002836,新宏泽,2016-12-29
-002837,英维克,2016-12-29
-002838,道恩股份,2017-01-06
-002839,张家港行,2017-01-24
-002840,华统股份,2017-01-10
-002841,视源股份,2017-01-19
-002842,翔鹭钨业,2017-01-19
-002843,泰嘉股份,2017-01-20
-002845,同兴达,2017-01-25
-002846,英联股份,2017-02-07
-002847,盐津铺子,2017-02-08
-002848,高斯贝尔,2017-02-13
-002849,威星智能,2017-02-17
-002850,科达利,2017-03-02
-002851,麦格米特,2017-03-06
-002852,道道全,2017-03-10
-002853,皮阿诺,2017-03-10
-002855,捷荣技术,2017-03-21
-002856,美芝股份,2017-03-20
-002857,三晖电气,2017-03-23
-002858,力盛体育,2017-03-24
-002859,洁美科技,2017-04-07
-002860,星帅尔,2017-04-12
-002861,瀛通通讯,2017-04-13
-002862,实丰文化,2017-04-11
-002863,今飞凯达,2017-04-18
-002864,盘龙药业,2017-11-16
-002865,钧达股份,2017-04-25
-002866,传艺科技,2017-04-26
-002867,周大生,2017-04-27
-002868,绿康生化,2017-05-03
-002869,金溢科技,2017-05-15
-002870,香山股份,2017-05-15
-002871,伟隆股份,2017-05-11
-002872,ST天圣,2017-05-19
-002873,新天药业,2017-05-19
-002875,安奈儿,2017-06-01
-002876,三利谱,2017-05-25
-002877,智能自控,2017-06-05
-002878,元隆雅图,2017-06-06
-002879,长缆科技,2017-07-07
-002880,卫光生物,2017-06-16
-002881,美格智能,2017-06-22
-002882,金龙羽,2017-07-17
-002883,中设股份,2017-06-20
-002884,凌霄泵业,2017-07-11
-002885,京泉华,2017-06-27
-002886,沃特股份,2017-06-27
-002887,绿茵生态,2017-08-01
-002888,惠威科技,2017-07-21
-002889,东方嘉盛,2017-07-31
-002890,弘宇股份,2017-08-02
-002891,中宠股份,2017-08-21
-002892,科力尔,2017-08-17
-002893,京能热力,2017-09-15
-002895,川恒股份,2017-08-25
-002896,中大力德,2017-08-29
-002897,意华股份,2017-09-07
-002898,赛隆药业,2017-09-12
-002899,英派斯,2017-09-15
-002900,哈三联,2017-09-22
-002901,大博医疗,2017-09-22
-002902,铭普光磁,2017-09-29
-002903,宇环数控,2017-10-13
-002905,金逸影视,2017-10-16
-002906,华阳集团,2017-10-13
-002907,华森制药,2017-10-20
-002908,德生科技,2017-10-20
-002909,集泰股份,2017-10-26
-002910,庄园牧场,2017-10-31
-002911,佛燃能源,2017-11-22
-002912,中新赛克,2017-11-21
-002913,奥士康,2017-12-01
-002915,中欣氟材,2017-12-05
-002916,深南电路,2017-12-13
-002917,金奥博,2017-12-08
-002918,蒙娜丽莎,2017-12-19
-002919,名臣健康,2017-12-18
-002920,德赛西威,2017-12-26
-002921,联诚精密,2017-12-27
-002922,伊戈尔,2017-12-29
-002923,润都股份,2018-01-05
-002925,盈趣科技,2018-01-15
-002926,华西证券,2018-02-05
-002927,泰永长征,2018-02-23
-002928,华夏航空,2018-03-02
-002929,润建股份,2018-03-01
-002930,宏川智慧,2018-03-28
-002931,锋龙股份,2018-04-03
-002932,明德生物,2018-07-10
-002933,新兴装备,2018-08-28
-002935,天奥电子,2018-09-03
-002936,郑州银行,2018-09-19
-002937,兴瑞科技,2018-09-26
-002938,鹏鼎控股,2018-09-18
-002939,长城证券,2018-10-26
-002940,昂利康,2018-10-23
-002941,新疆交建,2018-11-28
-002942,新农股份,2018-12-05
-002943,宇晶股份,2018-11-29
-002945,华林证券,2019-01-17
-002946,新乳业,2019-01-25
-002947,恒铭达,2019-02-01
-002948,青岛银行,2019-01-16
-002949,华阳国际,2019-02-26
-002950,奥美医疗,2019-03-11
-002951,ST金时,2019-03-15
-002952,亚世光电,2019-03-28
-002953,日丰股份,2019-05-09
-002955,鸿合科技,2019-05-23
-002956,西麦食品,2019-06-19
-002957,科瑞技术,2019-07-26
-002958,青农商行,2019-03-26
-002959,小熊电器,2019-08-23
-002960,青鸟消防,2019-08-09
-002961,瑞达期货,2019-09-05
-002962,五方光电,2019-09-17
-002963,豪尔赛,2019-10-28
-002965,祥鑫科技,2019-10-25
-002966,苏州银行,2019-08-02
-002967,广电计量,2019-11-08
-002968,新大正,2019-12-03
-002969,嘉美包装,2019-12-02
-002970,锐明技术,2019-12-17
-002971,和远气体,2020-01-13
-002972,科安达,2019-12-27
-002973,侨银股份,2020-01-06
-002975,博杰股份,2020-02-05
-002976,瑞玛精密,2020-03-06
-002977,天箭科技,2020-03-17
-002978,安宁股份,2020-04-17
-002979,雷赛智能,2020-04-08
-002980,华盛昌,2020-04-15
-002981,朝阳科技,2020-04-17
-002982,湘佳股份,2020-04-24
-002983,芯瑞达,2020-04-28
-002984,森麒麟,2020-09-11
-002985,北摩高科,2020-04-29
-002986,宇新股份,2020-06-02
-002987,京北方,2020-05-07
-002988,豪美新材,2020-05-18
-002989,中天精装,2020-06-10
-002990,盛视科技,2020-05-25
-002991,甘源食品,2020-07-31
-002992,宝明科技,2020-08-03
-002993,奥海科技,2020-08-17
-002995,天地在线,2020-08-05
-002996,顺博合金,2020-08-28
-002997,瑞鹄模具,2020-09-03
-002998,优彩资源,2020-09-25
-002999,天禾股份,2020-09-03
-003000,劲仔食品,2020-09-14
-003001,中岩大地,2020-10-13
-003002,壶化股份,2020-09-22
-003003,天元股份,2020-09-21
-003004,声迅股份,2020-11-26
-003005,竞业达,2020-09-22
-003006,百亚股份,2020-09-21
-003007,直真科技,2020-09-23
-003008,开普检测,2020-09-23
-003009,中天火箭,2020-09-25
-003010,若羽臣,2020-09-25
-003011,海象新材,2020-09-30
-003012,东鹏控股,2020-10-19
-003013,地铁设计,2020-10-22
-003015,日久光电,2020-10-21
-003016,欣贺股份,2020-10-26
-003017,大洋生物,2020-10-26
-003018,金富科技,2020-11-06
-003019,宸展光电,2020-11-17
-003020,立方制药,2020-12-15
-003021,兆威机电,2020-12-04
-003022,联泓新科,2020-12-08
-003023,彩虹集团,2020-12-11
-003025,思进智能,2020-12-11
-003026,中晶科技,2020-12-18
-003027,同兴环保,2020-12-18
-003028,振邦智能,2020-12-28
-003029,吉大正元,2020-12-24
-003030,祖名股份,2021-01-06
-003031,中瓷电子,2021-01-04
-003032,传智教育,2021-01-12
-003033,征和工业,2021-01-11
-003035,南网能源,2021-01-19
-003036,泰坦股份,2021-01-28
-003037,三和管桩,2021-02-04
-003038,鑫铂股份,2021-02-10
-003039,顺控发展,2021-03-08
-003040,楚天龙,2021-03-22
-003041,真爱美家,2021-04-06
-003042,中农联合,2021-04-06
-003043,华亚智能,2021-04-06
-003816,中国广核,2019-08-26
-200002,万科B,
-200003,PT金田B,
-200011,深物业B,
-200012,南  玻Ｂ,
-200013,*ST石化B,
-200015,PT中浩B,
-200016,深康佳Ｂ,
-200017,深中华B,
-200018,神城B退,
-200019,深粮B,
-200020,深华发Ｂ,
-200024,招商局B,
-200025,特  力Ｂ,
-200026,飞亚达Ｂ,
-200028,一致Ｂ,
-200029,深深房Ｂ,
-200030,富奥B,
-200037,深南电B,
-200039,中集B,
-200041,*ST本实B,
-200045,深纺织Ｂ,
-200053,深基地B,
-200054,建车B,
-200055,方大Ｂ,
-200056,皇庭B,
-200057,*ST大洋B,
-200058,深赛格B,
-200152,山航B退,
-200160,东沣B退,
-200168,*ST舜喆B,
-200413,东旭B,
-200418,小天鹅B,
-200429,粤高速Ｂ,
-200468,宁通信B,
-200488,晨  鸣Ｂ,
-200505,京粮B,
-200512,闽灿坤Ｂ,
-200513,丽珠B,
-200521,虹美菱B,
-200530,冰山B,
-200539,粤电力Ｂ,
-200541,粤照明Ｂ,
-200550,江  铃Ｂ,
-200553,安道麦B,
-200570,苏常柴Ｂ,
-200581,苏威孚Ｂ,
-200596,古井贡Ｂ,
-200613,东海B退,
-200625,长  安Ｂ,
-200706,瓦轴B,
-200725,京东方Ｂ,
-200726,鲁  泰Ｂ,
-200761,本钢板Ｂ,
-200770,武锅B退,
-200771,杭汽轮Ｂ,
-200869,张  裕Ｂ,
-200986,粤华包B,
-200992,中  鲁Ｂ,
-201872,招港B,
-300001,特锐德,2009-10-30
-300002,神州泰岳,2009-10-30
-300003,乐普医疗,2009-10-30
-300004,南风股份,2009-10-30
-300005,探路者,2009-10-30
-300006,莱美药业,2009-10-30
-300007,汉威科技,2009-10-30
-300008,天海防务,2009-10-30
-300009,安科生物,2009-10-30
-300010,*ST豆神,2009-10-30
-300011,鼎汉技术,2009-10-30
-300012,华测检测,2009-10-30
-300013,新宁物流,2009-10-30
-300014,亿纬锂能,2009-10-30
-300015,爱尔眼科,2009-10-30
-300016,北陆药业,2009-10-30
-300017,网宿科技,2009-10-30
-300018,中元股份,2009-10-30
-300019,硅宝科技,2009-10-30
-300020,银江技术,2009-10-30
-300021,大禹节水,2009-10-30
-300022,吉峰科技,2009-10-30
-300023,宝德退,
-300024,机器人,2009-10-30
-300025,华星创业,2009-10-30
-300026,红日药业,2009-10-30
-300027,华谊兄弟,2009-10-30
-300028,金亚退,
-300029,ST天龙,2009-12-25
-300030,阳普医疗,2009-12-25
-300031,宝通科技,2009-12-25
-300032,金龙机电,2009-12-25
-300033,同花顺,2009-12-25
-300034,钢研高纳,2009-12-25
-300035,中科电气,2009-12-25
-300036,超图软件,2009-12-25
-300037,新宙邦,2010-01-08
-300038,数知退,
-300039,上海凯宝,2010-01-08
-300040,九洲集团,2010-01-08
-300041,回天新材,2010-01-08
-300042,朗科科技,2010-01-08
-300043,星辉娱乐,2010-01-20
-300044,赛为智能,2010-01-20
-300045,华力创通,2010-01-20
-300046,台基股份,2010-01-20
-300047,天源迪科,2010-01-20
-300048,合康新能,2010-01-20
-300049,福瑞股份,2010-01-20
-300050,世纪鼎利,2010-01-20
-300051,琏升科技,2010-02-11
-300052,中青宝,2010-02-11
-300053,航宇微,2010-02-11
-300054,鼎龙股份,2010-02-11
-300055,万邦达,2010-02-26
-300056,中创环保,2010-02-26
-300057,万顺新材,2010-02-26
-300058,蓝色光标,2010-02-26
-300059,东方财富,2010-03-19
-300061,旗天科技,2010-03-19
-300062,中能电气,2010-03-19
-300063,天龙集团,2010-03-26
-300064,金刚退,
-300065,海兰信,2010-03-26
-300066,三川智慧,2010-03-26
-300067,安诺其,2010-04-21
-300068,南都电源,2010-04-21
-300069,金利华电,2010-04-21
-300070,碧水源,2010-04-21
-300071,福石控股,2010-04-21
-300072,海新能科,2010-04-27
-300073,当升科技,2010-04-27
-300074,华平股份,2010-04-27
-300075,数字政通,2010-04-27
-300076,GQY视讯,2010-04-30
-300077,国民技术,2010-04-30
-300078,思创医惠,2010-04-30
-300079,数码视讯,2010-04-30
-300080,易成新能,2010-06-25
-300081,恒信东方,2010-05-20
-300082,奥克股份,2010-05-20
-300083,创世纪,2010-05-20
-300084,海默科技,2010-05-20
-300085,银之杰,2010-05-26
-300086,康芝药业,2010-05-26
-300087,荃银高科,2010-05-26
-300088,长信科技,2010-05-26
-300089,文化退,
-300090,盛运退,
-300091,金通灵,2010-06-25
-300092,科新机电,2010-07-08
-300093,金刚光伏,2010-07-08
-300094,国联水产,2010-07-08
-300095,华伍股份,2010-07-28
-300096,易联众,2010-07-28
-300097,智云股份,2010-07-28
-300098,高新兴,2010-07-28
-300099,精准信息,2010-08-06
-300100,双林股份,2010-08-06
-300101,振芯科技,2010-08-06
-300102,乾照光电,2010-08-12
-300103,达刚控股,2010-08-12
-300104,乐视退,
-300105,龙源技术,2010-08-20
-300106,西部牧业,2010-08-20
-300107,建新股份,2010-08-20
-300108,*ST吉药,2010-08-25
-300109,新开源,2010-08-25
-300110,华仁药业,2010-08-25
-300111,向日葵,2010-08-27
-300112,万讯自控,2010-08-27
-300113,顺网科技,2010-08-27
-300114,中航电测,2010-08-27
-300115,长盈精密,2010-09-02
-300116,保力新,2010-09-02
-300117,嘉寓股份,2010-09-02
-300118,东方日升,2010-09-02
-300119,瑞普生物,2010-09-17
-300120,经纬辉开,2010-09-17
-300121,阳谷华泰,2010-09-17
-300122,智飞生物,2010-09-28
-300123,亚光科技,2010-09-28
-300124,汇川技术,2010-09-28
-300125,聆达股份,2010-10-13
-300126,锐奇股份,2010-10-13
-300127,银河磁体,2010-10-13
-300128,锦富技术,2010-10-13
-300129,泰胜风能,2010-10-19
-300130,新国都,2010-10-19
-300131,英唐智控,2010-10-19
-300132,青松股份,2010-10-26
-300133,华策影视,2010-10-26
-300134,大富科技,2010-10-26
-300135,宝利国际,2010-10-26
-300136,信维通信,2010-11-05
-300137,先河环保,2010-11-05
-300138,晨光生物,2010-11-05
-300139,晓程科技,2010-11-12
-300140,节能环境,2010-11-12
-300141,和顺电气,2010-11-12
-300142,沃森生物,2010-11-12
-300143,盈康生命,2010-12-09
-300144,宋城演艺,2010-12-09
-300145,中金环境,2010-12-09
-300146,汤臣倍健,2010-12-15
-300147,香雪制药,2010-12-15
-300148,天舟文化,2010-12-15
-300149,睿智医药,2010-12-22
-300150,世纪瑞尔,2010-12-22
-300151,昌红科技,2010-12-22
-300152,新动力,2010-12-29
-300153,科泰电源,2010-12-29
-300154,瑞凌股份,2010-12-29
-300155,安居宝,2011-01-07
-300156,神雾退,
-300157,新锦动力,2011-01-07
-300158,振东制药,2011-01-07
-300159,新研股份,2011-01-07
-300160,秀强股份,2011-01-13
-300161,华中数控,2011-01-13
-300162,雷曼光电,2011-01-13
-300163,先锋新材,2011-01-13
-300164,通源石油,2011-01-13
-300165,天瑞仪器,2011-01-25
-300166,东方国信,2011-01-25
-300167,ST迪威迅,2011-01-25
-300168,万达信息,2011-01-25
-300169,天晟新材,2011-01-25
-300170,汉得信息,2011-02-01
-300171,东富龙,2011-02-01
-300172,中电环保,2011-02-01
-300173,福能东方,2011-02-01
-300174,元力股份,2011-02-01
-300175,朗源股份,2011-02-15
-300176,派生科技,2011-02-15
-300177,中海达,2011-02-15
-300178,腾邦退,
-300179,四方达,2011-02-15
-300180,华峰超纤,2011-02-22
-300181,佐力药业,2011-02-22
-300182,捷成股份,2011-02-22
-300183,东软载波,2011-02-22
-300184,力源信息,2011-02-22
-300185,通裕重工,2011-03-08
-300186,大华农,
-300187,永清环保,2011-03-08
-300188,美亚柏科,2011-03-16
-300189,神农科技,2011-03-16
-300190,维尔利,2011-03-16
-300191,潜能恒信,2011-03-16
-300192,科德教育,2011-03-22
-300193,佳士科技,2011-03-22
-300194,福安药业,2011-03-22
-300195,长荣股份,2011-03-29
-300196,长海股份,2011-03-29
-300197,节能铁汉,2011-03-29
-300198,纳川股份,2011-04-07
-300199,翰宇药业,2011-04-07
-300200,高盟新材,2011-04-07
-300201,海伦哲,2011-04-07
-300202,聚龙退,
-300203,聚光科技,2011-04-15
-300204,舒泰神,2011-04-15
-300205,天喻信息,2011-04-21
-300206,理邦仪器,2011-04-21
-300207,欣旺达,2011-04-21
-300208,青岛中程,2011-04-26
-300209,ST有棵树,2011-04-26
-300210,森远股份,2011-04-26
-300211,亿通科技,2011-05-05
-300212,易华录,2011-05-05
-300213,佳讯飞鸿,2011-05-05
-300214,日科化学,2011-05-11
-300215,电科院,2011-05-11
-300216,千山退,
-300217,东方电热,2011-05-18
-300218,安利股份,2011-05-18
-300219,鸿利智汇,2011-05-18
-300220,ST金运,2011-05-25
-300221,银禧科技,2011-05-25
-300222,科大智能,2011-05-25
-300223,北京君正,2011-05-31
-300224,正海磁材,2011-05-31
-300225,金力泰,2011-05-31
-300226,上海钢联,2011-06-08
-300227,光韵达,2011-06-08
-300228,富瑞特装,2011-06-08
-300229,拓尔思,2011-06-15
-300230,永利股份,2011-06-15
-300231,银信科技,2011-06-15
-300232,洲明科技,2011-06-22
-300233,金城医药,2011-06-22
-300234,开尔新材,2011-06-22
-300235,方直科技,2011-06-29
-300236,上海新阳,2011-06-29
-300237,美晨生态,2011-06-29
-300238,冠昊生物,2011-07-06
-300239,东宝生物,2011-07-06
-300240,飞力达,2011-07-06
-300241,瑞丰光电,2011-07-12
-300242,佳云科技,2011-07-12
-300243,瑞丰高材,2011-07-12
-300244,迪安诊断,2011-07-19
-300245,天玑科技,2011-07-19
-300246,宝莱特,2011-07-19
-300247,融捷健康,2011-07-29
-300248,新开普,2011-07-29
-300249,依米康,2011-08-03
-300250,初灵信息,2011-08-03
-300251,光线传媒,2011-08-03
-300252,金信诺,2011-08-18
-300253,卫宁健康,2011-08-18
-300254,仟源医药,2011-08-19
-300255,常山药业,2011-08-19
-300256,星星科技,2011-08-19
-300257,开山股份,2011-08-19
-300258,精锻科技,2011-08-26
-300259,新天科技,2011-08-31
-300260,新莱应材,2011-09-06
-300261,雅本化学,2011-09-06
-300262,巴安水务,2011-09-16
-300263,隆华科技,2011-09-16
-300264,佳创视讯,2011-09-16
-300265,通光线缆,2011-09-16
-300266,兴源环境,2011-09-27
-300267,尔康制药,2011-09-27
-300268,*ST佳沃,2011-09-27
-300269,联建光电,2011-10-12
-300270,中威电子,2011-10-12
-300271,华宇软件,2011-10-26
-300272,开能健康,2011-11-02
-300273,和佳退,
-300274,阳光电源,2011-11-02
-300275,梅安森,2011-11-02
-300276,三丰智能,2011-11-15
-300277,海联讯,2011-11-23
-300278,华昌达,2011-12-16
-300279,和晶科技,2011-12-29
-300280,紫天科技,2011-12-29
-300281,金明精机,2011-12-29
-300282,*ST三盛,2011-12-29
-300283,温州宏丰,2012-01-10
-300284,苏交科,2012-01-10
-300285,国瓷材料,2012-01-13
-300286,安科瑞,2012-01-13
-300287,飞利信,2012-02-01
-300288,朗玛信息,2012-02-16
-300289,利德曼,2012-02-16
-300290,荣科科技,2012-02-16
-300291,百纳千成,2012-02-09
-300292,吴通控股,2012-02-29
-300293,蓝英装备,2012-03-08
-300294,博雅生物,2012-03-08
-300295,三六五网,2012-03-15
-300296,利亚德,2012-03-15
-300297,蓝盾退,
-300298,三诺生物,2012-03-19
-300299,富春股份,2012-03-19
-300300,海峡创新,2012-03-19
-300301,*ST长方,2012-03-21
-300302,同有科技,2012-03-21
-300303,聚飞光电,2012-03-19
-300304,云意电气,2012-03-21
-300305,裕兴股份,2012-03-29
-300306,远方信息,2012-03-29
-300307,慈星股份,2012-03-29
-300308,中际旭创,2012-04-10
-300309,吉艾退,
-300310,宜通世纪,2012-04-25
-300311,任子行,2012-04-25
-300312,邦讯退,
-300313,*ST天山,2012-04-25
-300314,戴维医疗,2012-05-08
-300315,掌趣科技,2012-05-11
-300316,晶盛机电,2012-05-11
-300317,珈伟新能,2012-05-11
-300318,博晖创新,2012-05-23
-300319,麦捷科技,2012-05-23
-300320,海达股份,2012-06-01
-300321,同大股份,2012-05-23
-300322,硕贝德,2012-06-08
-300323,华灿光电,2012-06-01
-300324,旋极信息,2012-06-08
-300325,德威退,
-300326,凯利泰,2012-06-13
-300327,中颖电子,2012-06-13
-300328,宜安科技,2012-06-19
-300329,海伦钢琴,2012-06-19
-300330,计通退,
-300331,苏大维格,2012-06-28
-300332,天壕能源,2012-06-28
-300333,兆日科技,2012-06-28
-300334,津膜科技,2012-07-05
-300335,迪森股份,2012-07-10
-300336,新文退,
-300337,银邦股份,2012-07-18
-300338,开元教育,2012-07-26
-300339,润和软件,2012-07-18
-300340,科恒股份,2012-07-26
-300341,麦克奥迪,2012-07-26
-300342,天银机电,2012-07-26
-300343,联创股份,2012-08-01
-300344,立方数科,2012-08-01
-300345,华民股份,2012-08-01
-300346,南大光电,2012-08-07
-300347,泰格医药,2012-08-17
-300348,长亮科技,2012-08-17
-300349,金卡智能,2012-08-17
-300350,华鹏飞,2012-08-21
-300351,永贵电器,2012-09-20
-300352,北信源,2012-09-12
-300353,东土科技,2012-09-27
-300354,东华测试,2012-09-20
-300355,蒙草生态,2012-09-27
-300356,光一退,
-300357,我武生物,2014-01-21
-300358,楚天科技,2014-01-21
-300359,全通教育,2014-01-21
-300360,炬华科技,2014-01-21
-300362,天翔退,
-300363,博腾股份,2014-01-29
-300364,中文在线,2015-01-21
-300365,恒华科技,2014-01-23
-300366,创意信息,2014-01-27
-300367,网力退,
-300368,汇金股份,2014-01-23
-300369,绿盟科技,2014-01-29
-300370,安控科技,2014-01-23
-300371,汇中股份,2014-01-23
-300372,欣泰退,
-300373,扬杰科技,2014-01-23
-300374,中铁装配,2015-03-19
-300375,鹏翎股份,2014-01-27
-300376,易事特,2014-01-27
-300377,赢时胜,2014-01-27
-300378,鼎捷软件,2014-01-27
-300379,东方通,2014-01-28
-300380,安硕信息,2014-01-28
-300381,溢多利,2014-01-28
-300382,斯莱克,2014-01-29
-300383,光环新网,2014-01-29
-300384,三联虹普,2014-08-01
-300385,雪浪环境,2014-06-26
-300386,飞天诚信,2014-06-26
-300387,富邦股份,2014-07-02
-300388,节能国祯,2014-08-01
-300389,艾比森,2014-08-01
-300390,天华新能,2014-07-31
-300391,长药控股,2014-08-01
-300392,腾信退,
-300393,中来股份,2014-09-12
-300394,天孚通信,2015-02-17
-300395,菲利华,2014-09-10
-300396,迪瑞医疗,2014-09-10
-300397,天和防务,2014-09-10
-300398,飞凯材料,2014-10-09
-300399,天利科技,2014-10-09
-300400,劲拓股份,2014-10-10
-300401,花园生物,2014-10-09
-300402,宝色股份,2014-10-10
-300403,汉宇集团,2014-10-30
-300404,博济医药,2015-04-24
-300405,科隆股份,2014-10-30
-300406,九强生物,2014-10-30
-300407,凯发电气,2014-12-03
-300408,三环集团,2014-12-03
-300409,道氏技术,2014-12-03
-300410,正业科技,2014-12-31
-300411,金盾股份,2014-12-31
-300412,迦南科技,2014-12-31
-300413,芒果超媒,2015-01-21
-300414,中光防雷,2015-05-13
-300415,伊之密,2015-01-23
-300416,苏试试验,2015-01-22
-300417,南华仪器,2015-01-23
-300418,昆仑万维,2015-01-21
-300419,浩丰科技,2015-01-22
-300420,五洋停车,2015-02-17
-300421,力星股份,2015-02-17
-300422,博世科,2015-02-17
-300423,昇辉科技,2015-02-17
-300424,航新科技,2015-04-22
-300425,中建环能,2015-02-16
-300426,唐德影视,2015-02-17
-300427,*ST红相,2015-02-17
-300428,立中集团,2015-03-19
-300429,强力新材,2015-03-24
-300430,诚益通,2015-03-19
-300431,暴风退,
-300432,富临精工,2015-03-19
-300433,蓝思科技,2015-03-18
-300434,金石亚药,2015-04-24
-300435,中泰股份,2015-03-26
-300436,广生堂,2015-04-22
-300437,清水源,2015-04-23
-300438,鹏辉能源,2015-04-24
-300439,美康生物,2015-04-22
-300440,运达科技,2015-04-23
-300441,鲍斯股份,2015-04-23
-300442,润泽科技,2015-04-24
-300443,金雷股份,2015-04-22
-300444,双杰电气,2015-04-23
-300445,康斯特,2015-04-24
-300446,乐凯新材,2015-04-23
-300447,全信股份,2015-04-22
-300448,浩云科技,2015-04-24
-300449,汉邦高科,2015-04-22
-300450,先导智能,2015-05-18
-300451,创业慧康,2015-05-14
-300452,山河药辅,2015-05-15
-300453,三鑫医疗,2015-05-15
-300454,深信服,2018-05-16
-300455,航天智装,2015-05-15
-300456,赛微电子,2015-05-14
-300457,赢合科技,2015-05-14
-300458,全志科技,2015-05-15
-300459,汤姆猫,2015-05-15
-300460,惠伦晶体,2015-05-15
-300461,田中精机,2015-05-19
-300462,华铭智能,2015-05-27
-300463,迈克生物,2015-05-28
-300464,星徽股份,2015-06-10
-300465,高伟达,2015-05-28
-300466,赛摩智能,2015-05-28
-300467,迅游科技,2015-05-27
-300468,四方精创,2015-05-27
-300469,信息发展,2015-06-11
-300470,中密控股,2015-06-12
-300471,厚普股份,2015-06-11
-300472,新元科技,2015-06-11
-300473,德尔股份,2015-06-12
-300474,景嘉微,2016-03-31
-300475,香农芯创,2015-06-10
-300476,胜宏科技,2015-06-11
-300477,合纵科技,2015-06-10
-300478,杭州高新,2015-06-10
-300479,神思电子,2015-06-12
-300480,光力科技,2015-07-02
-300481,濮阳惠成,2015-06-30
-300482,万孚生物,2015-06-30
-300483,首华燃气,2015-06-30
-300484,蓝海华腾,2016-03-22
-300485,赛升药业,2015-06-26
-300486,东杰智能,2015-06-30
-300487,蓝晓科技,2015-07-02
-300488,恒锋工具,2015-07-01
-300489,光智科技,2015-07-01
-300490,华自科技,2015-12-31
-300491,通合科技,2015-12-31
-300492,华图山鼎,2015-12-23
-300493,润欣科技,2015-12-10
-300494,盛天网络,2015-12-31
-300495,*ST美尚,2015-12-22
-300496,中科创达,2015-12-10
-300497,富祥药业,2015-12-22
-300498,温氏股份,2015-11-02
-300499,高澜股份,2016-02-02
-300500,启迪设计,2016-02-04
-300501,海顺新材,2016-02-04
-300502,新易盛,2016-03-03
-300503,昊志机电,2016-03-09
-300504,天邑股份,2018-03-30
-300505,川金诺,2016-03-15
-300506,名家汇,2016-03-24
-300507,苏奥传感,2016-04-29
-300508,维宏股份,2016-04-19
-300509,新美星,2016-04-25
-300510,金冠股份,2016-05-06
-300511,雪榕生物,2016-05-04
-300512,中亚股份,2016-05-26
-300513,恒实科技,2016-05-30
-300514,友讯达,2017-04-26
-300515,三德科技,2016-06-08
-300516,久之洋,2016-06-02
-300517,海波重科,2016-07-19
-300518,盛讯达,2016-06-24
-300519,新光药业,2016-06-24
-300520,科大国创,2016-07-08
-300521,爱司凯,2016-07-05
-300522,世名科技,2016-07-05
-300523,辰安科技,2016-07-26
-300525,博思软件,2016-07-26
-300526,中潜退,
-300527,中船应急,2016-08-05
-300528,幸福蓝海,2016-08-08
-300529,健帆生物,2016-08-02
-300530,领湃科技,2016-08-09
-300531,优博讯,2016-08-09
-300532,今天国际,2016-08-18
-300533,冰川网络,2016-08-18
-300534,陇神戎发,2016-09-13
-300535,达威股份,2016-08-12
-300536,农尚环境,2016-09-20
-300537,广信材料,2016-08-30
-300538,同益股份,2016-08-26
-300539,横河精密,2016-08-30
-300540,蜀道装备,2016-08-23
-300541,先进数通,2016-09-13
-300542,新晨科技,2016-09-20
-300543,朗科智能,2016-09-08
-300545,联得装备,2016-09-28
-300546,雄帝科技,2016-09-28
-300547,川环科技,2016-09-30
-300548,博创科技,2016-10-12
-300549,优德精密,2016-09-30
-300550,和仁科技,2016-10-18
-300551,古鳌科技,2016-10-18
-300552,万集科技,2016-10-21
-300553,集智股份,2016-10-21
-300554,三超新材,2017-04-21
-300555,ST路通,2016-10-18
-300556,丝路视觉,2016-11-04
-300557,理工光科,2016-11-01
-300558,贝达药业,2016-11-07
-300559,佳发教育,2016-11-01
-300560,中富通,2016-11-01
-300561,汇金科技,2016-11-17
-300562,乐心医疗,2016-11-16
-300563,神宇股份,2016-11-14
-300564,筑博设计,2019-11-08
-300565,科信技术,2016-11-22
-300566,激智科技,2016-11-15
-300567,精测电子,2016-11-22
-300568,星源材质,2016-12-01
-300569,天能重工,2016-11-25
-300570,太辰光,2016-12-06
-300571,平治信息,2016-12-13
-300572,安车检测,2016-12-06
-300573,兴齐眼药,2016-12-08
-300575,中旗股份,2016-12-20
-300576,容大感光,2016-12-20
-300577,开润股份,2016-12-21
-300578,会畅通讯,2017-01-25
-300579,数字认证,2016-12-23
-300580,贝斯特,2017-01-11
-300581,晨曦航空,2016-12-20
-300582,英飞特,2016-12-28
-300583,赛托生物,2017-01-06
-300584,海辰药业,2017-01-12
-300585,奥联电子,2016-12-29
-300586,美联新材,2017-01-04
-300587,天铁股份,2017-01-05
-300588,熙菱信息,2017-01-05
-300589,江龙船艇,2017-01-13
-300590,移为通信,2017-01-11
-300591,万里马,2017-01-10
-300592,华凯易佰,2017-01-20
-300593,新雷能,2017-01-13
-300594,朗进科技,2019-06-21
-300595,欧普康视,2017-01-17
-300596,利安隆,2017-01-19
-300597,吉大通信,2017-01-23
-300598,诚迈科技,2017-01-20
-300599,雄塑科技,2017-01-23
-300600,国瑞科技,2017-01-25
-300601,康泰生物,2017-02-07
-300602,飞荣达,2017-01-26
-300603,立昂技术,2017-01-26
-300604,长川科技,2017-04-17
-300605,恒锋信息,2017-02-08
-300606,金太阳,2017-02-08
-300607,拓斯达,2017-02-09
-300608,思特奇,2017-02-13
-300609,汇纳科技,2017-02-15
-300610,晨化股份,2017-02-13
-300611,美力科技,2017-02-20
-300612,宣亚国际,2017-02-15
-300613,富瀚微,2017-02-20
-300614,百川畅银,2021-05-25
-300615,欣天科技,2017-02-15
-300616,尚品宅配,2017-03-07
-300617,安靠智电,2017-02-28
-300618,寒锐钴业,2017-03-06
-300619,金银河,2017-03-01
-300620,光库科技,2017-03-10
-300621,维业股份,2017-03-16
-300622,博士眼镜,2017-03-15
-300623,捷捷微电,2017-03-14
-300624,万兴科技,2018-01-18
-300625,三雄极光,2017-03-17
-300626,华瑞股份,2017-03-20
-300627,华测导航,2017-03-21
-300628,亿联网络,2017-03-17
-300629,新劲刚,2017-03-24
-300630,普利制药,2017-03-28
-300631,久吾高科,2017-03-23
-300632,光莆股份,2017-04-06
-300633,开立医疗,2017-04-06
-300634,彩讯股份,2018-03-23
-300635,中达安,2017-03-31
-300636,同和药业,2017-03-31
-300637,扬帆新材,2017-04-12
-300638,广和通,2017-04-13
-300639,凯普生物,2017-04-12
-300640,德艺文创,2017-04-17
-300641,正丹股份,2017-04-18
-300642,透景生命,2017-04-21
-300643,万通智控,2017-05-05
-300644,南京聚隆,2018-02-06
-300645,正元智慧,2017-04-21
-300647,超频三,2017-05-03
-300648,星云股份,2017-04-25
-300649,杭州园林,2017-05-05
-300650,太龙股份,2017-05-03
-300651,金陵体育,2017-05-09
-300652,雷迪克,2017-05-16
-300653,正海生物,2017-05-16
-300654,世纪天鸿,2017-09-26
-300655,晶瑞电材,2017-05-23
-300656,民德电子,2017-05-19
-300657,弘信电子,2017-05-23
-300658,延江股份,2017-06-02
-300659,中孚信息,2017-05-26
-300660,江苏雷利,2017-06-02
-300661,圣邦股份,2017-06-06
-300662,科锐国际,2017-06-08
-300663,科蓝软件,2017-06-08
-300664,鹏鹞环保,2018-01-05
-300665,飞鹿股份,2017-06-13
-300666,江丰电子,2017-06-15
-300667,必创科技,2017-06-19
-300668,杰恩设计,2017-06-19
-300669,沪宁股份,2017-06-29
-300670,大烨智能,2017-07-03
-300671,富满微,2017-07-05
-300672,国科微,2017-07-12
-300673,佩蒂股份,2017-07-11
-300674,宇信科技,2018-11-07
-300675,建科院,2017-07-19
-300676,华大基因,2017-07-14
-300677,英科医疗,2017-07-21
-300678,中科信息,2017-07-28
-300679,电连技术,2017-07-31
-300680,隆盛科技,2017-07-25
-300681,英搏尔,2017-07-25
-300682,朗新科技,2017-08-01
-300683,海特生物,2017-08-08
-300684,中石科技,2017-12-27
-300685,艾德生物,2017-08-02
-300686,智动力,2017-08-04
-300687,赛意信息,2017-08-03
-300688,创业黑马,2017-08-10
-300689,澄天伟业,2017-08-09
-300690,双一科技,2017-08-08
-300691,联合光电,2017-08-11
-300692,中环环保,2017-08-21
-300693,盛弘股份,2017-08-22
-300694,蠡湖股份,2018-10-15
-300695,兆丰股份,2017-09-08
-300696,爱乐达,2017-08-22
-300697,电工合金,2017-09-07
-300698,万马科技,2017-08-31
-300699,光威复材,2017-09-01
-300700,岱勒新材,2017-09-12
-300701,森霸传感,2017-09-15
-300702,天宇股份,2017-09-19
-300703,创源股份,2017-09-19
-300705,九典制药,2017-10-10
-300706,阿石创,2017-09-26
-300707,威唐工业,2017-10-10
-300708,聚灿光电,2017-10-16
-300709,精研科技,2017-10-19
-300710,万隆光电,2017-10-19
-300711,广哈通信,2017-11-01
-300712,永福股份,2017-10-31
-300713,英可瑞,2017-11-01
-300715,凯伦股份,2017-10-26
-300716,泉为科技,2017-11-09
-300717,华信新材,2017-11-06
-300718,长盛轴承,2017-11-06
-300719,安达维尔,2017-11-09
-300720,海川智能,2017-11-06
-300721,怡达股份,2017-11-15
-300722,新余国科,2017-11-10
-300723,一品红,2017-11-16
-300724,捷佳伟创,2018-08-10
-300725,药石科技,2017-11-10
-300726,宏达电子,2017-11-21
-300727,润禾材料,2017-11-27
-300729,乐歌股份,2017-12-01
-300730,科创信息,2017-12-05
-300731,科创新源,2017-12-08
-300732,设研院,2017-12-12
-300733,西菱动力,2018-01-16
-300735,光弘科技,2017-12-29
-300736,百邦科技,2018-01-09
-300737,科顺股份,2018-01-25
-300738,奥飞数据,2018-01-19
-300739,明阳电路,2018-02-01
-300740,水羊股份,2018-02-08
-300741,华宝股份,2018-03-01
-300742,*ST越博,2018-05-08
-300743,天地数码,2018-04-27
-300745,欣锐科技,2018-05-23
-300746,汉嘉设计,2018-05-25
-300747,锐科激光,2018-06-25
-300748,金力永磁,2018-09-21
-300749,顶固集创,2018-09-25
-300750,宁德时代,2018-06-11
-300751,迈为股份,2018-11-09
-300752,隆利科技,2018-11-30
-300753,爱朋医疗,2018-12-13
-300755,华致酒行,2019-01-29
-300756,金马游乐,2018-12-28
-300757,罗博特科,2019-01-08
-300758,七彩化学,2019-02-22
-300759,康龙化成,2019-01-28
-300760,迈瑞医疗,2018-10-16
-300761,立华股份,2019-02-18
-300762,上海瀚讯,2019-03-14
-300763,锦浪科技,2019-03-19
-300765,新诺威,2019-03-22
-300766,每日互动,2019-03-25
-300767,震安科技,2019-03-29
-300768,迪普科技,2019-04-12
-300769,德方纳米,2019-04-15
-300770,新媒股份,2019-04-19
-300771,智莱科技,2019-04-22
-300772,运达股份,2019-04-26
-300773,拉卡拉,2019-04-25
-300774,倍杰特,2021-08-04
-300775,三角防务,2019-05-21
-300776,帝尔激光,2019-05-17
-300777,中简科技,2019-05-16
-300778,新城市,2019-05-10
-300779,惠城环保,2019-05-22
-300780,德恩精工,2019-05-31
-300781,因赛集团,2019-06-06
-300782,卓胜微,2019-06-18
-300783,三只松鼠,2019-07-12
-300785,值得买,2019-07-15
-300786,国林科技,2019-07-23
-300787,海能实业,2019-08-15
-300788,中信出版,2019-07-05
-300789,唐源电气,2019-08-28
-300790,宇瞳光学,2019-09-20
-300791,仙乐健康,2019-09-25
-300792,壹网壹创,2019-09-27
-300793,佳禾智能,2019-10-18
-300795,米奥会展,2019-10-22
-300796,贝斯美,2019-11-15
-300797,钢研纳克,2019-11-01
-300798,锦鸡股份,2019-11-22
-300799,*ST左江,2019-10-29
-300800,力合科技,2019-11-06
-300801,泰和科技,2019-11-28
-300802,矩子科技,2019-11-14
-300803,指南针,2019-11-18
-300804,广康生化,2023-06-27
-300805,电声股份,2019-11-21
-300806,斯迪克,2019-11-25
-300807,天迈科技,2019-12-19
-300808,久量股份,2019-11-29
-300809,华辰装备,2019-12-04
-300810,中科海讯,2019-12-06
-300811,铂科新材,2019-12-30
-300812,易天股份,2020-01-09
-300813,泰林生物,2020-01-14
-300814,中富电路,2021-08-12
-300815,玉禾田,2020-01-23
-300816,艾可蓝,2020-02-10
-300817,双飞股份,2020-02-18
-300818,耐普矿机,2020-02-12
-300819,聚杰微纤,2020-03-12
-300820,英杰电气,2020-02-13
-300821,东岳硅材,2020-03-12
-300822,贝仕达克,2020-03-13
-300823,建科机械,2020-03-19
-300824,北鼎股份,2020-06-19
-300825,阿尔特,2020-03-27
-300826,测绘股份,2020-04-03
-300827,上能电气,2020-04-10
-300828,锐新科技,2020-04-21
-300829,金丹科技,2020-04-22
-300830,金现代,2020-05-06
-300831,派瑞股份,2020-05-07
-300832,新产业,2020-05-12
-300833,浩洋股份,2020-05-20
-300834,星辉环材,2022-01-13
-300835,龙磁科技,2020-05-25
-300836,佰奥智能,2020-05-28
-300837,浙矿股份,2020-06-05
-300838,浙江力诺,2020-06-08
-300839,博汇股份,2020-06-30
-300840,酷特智能,2020-07-08
-300841,康华生物,2020-06-16
-300842,帝科股份,2020-06-18
-300843,胜蓝股份,2020-07-02
-300844,山水比德,2021-08-13
-300845,捷安高科,2020-07-03
-300846,首都在线,2020-07-01
-300847,中船汉光,2020-07-09
-300848,美瑞新材,2020-07-20
-300849,锦盛新材,2020-07-10
-300850,新强联,2020-07-13
-300851,交大思诺,2020-07-17
-300852,四会富仕,2020-07-13
-300853,申昊科技,2020-07-24
-300854,中兰环保,2021-09-16
-300855,图南股份,2020-07-23
-300856,科思股份,2020-07-22
-300857,协创数据,2020-07-27
-300858,科拓生物,2020-07-27
-300859,*ST西域,2020-08-06
-300860,锋尚文化,2020-08-24
-300861,美畅股份,2020-08-24
-300862,蓝盾光电,2020-08-24
-300863,卡倍亿,2020-08-24
-300864,南大环境,2020-08-24
-300865,大宏立,2020-08-24
-300866,安克创新,2020-08-24
-300867,圣元环保,2020-08-24
-300868,杰美特,2020-08-24
-300869,康泰医学,2020-08-24
-300870,欧陆通,2020-08-24
-300871,回盛生物,2020-08-24
-300872,天阳科技,2020-08-24
-300873,海晨股份,2020-08-24
-300875,捷强装备,2020-08-24
-300876,蒙泰高新,2020-08-24
-300877,金春股份,2020-08-24
-300878,维康药业,2020-08-24
-300879,大叶股份,2020-09-01
-300880,迦南智能,2020-09-01
-300881,盛德鑫泰,2020-09-01
-300882,万胜智能,2020-09-10
-300883,龙利得,2020-09-10
-300884,狄耐克,2020-11-12
-300885,海昌新材,2020-09-10
-300886,华业香料,2020-09-16
-300887,谱尼测试,2020-09-16
-300888,稳健医疗,2020-09-17
-300889,爱克股份,2020-09-16
-300890,翔丰华,2020-09-17
-300891,惠云钛业,2020-09-17
-300892,品渥食品,2020-09-24
-300893,松原股份,2020-09-24
-300894,火星人,2020-12-31
-300895,铜牛信息,2020-09-24
-300896,爱美客,2020-09-28
-300897,山科智能,2020-09-28
-300898,熊猫乳品,2020-10-16
-300899,上海凯鑫,2020-10-16
-300900,广联航空,2020-10-29
-300901,中胤时尚,2020-10-29
-300902,国安达,2020-10-29
-300903,科翔股份,2020-11-05
-300904,威力传动,2023-08-09
-300905,宝丽迪,2020-11-05
-300906,日月明,2020-11-05
-300907,康平科技,2020-11-18
-300908,仲景食品,2020-11-23
-300909,汇创达,2020-11-18
-300910,瑞丰新材,2020-11-27
-300911,亿田智能,2020-12-03
-300912,凯龙高科,2020-12-07
-300913,兆龙互连,2020-12-07
-300915,海融科技,2020-12-02
-300916,朗特智能,2020-12-02
-300917,特发服务,2020-12-21
-300918,南山智尚,2020-12-22
-300919,中伟股份,2020-12-23
-300920,润阳科技,2020-12-25
-300921,南凌科技,2020-12-22
-300922,天秦装备,2020-12-25
-300923,研奥股份,2020-12-24
-300925,法本信息,2020-12-30
-300926,博俊科技,2021-01-07
-300927,江天化学,2021-01-07
-300928,华安鑫创,2021-01-06
-300929,华骐环保,2021-01-20
-300930,屹通新材,2021-01-21
-300931,通用电梯,2021-01-21
-300932,三友联众,2021-01-22
-300933,中辰股份,2021-01-22
-300935,盈建科,2021-01-20
-300936,中英科技,2021-01-26
-300937,药易购,2021-01-27
-300938,信测标准,2021-01-27
-300939,秋田微,2021-01-28
-300940,南极光,2021-02-03
-300941,创识科技,2021-02-09
-300942,易瑞生物,2021-02-09
-300943,春晖智控,2021-02-10
-300945,曼卡龙,2021-02-10
-300946,恒而达,2021-02-08
-300947,德必集团,2021-02-10
-300948,冠中生态,2021-02-25
-300949,奥雅股份,2021-02-26
-300950,德固特,2021-03-03
-300951,博硕科技,2021-02-26
-300952,恒辉安防,2021-03-11
-300953,震裕科技,2021-03-18
-300955,嘉亨家化,2021-03-24
-300956,英力股份,2021-03-26
-300957,贝泰妮,2021-03-25
-300958,建工修复,2021-03-29
-300959,线上线下,2021-03-22
-300960,通业科技,2021-03-29
-300961,深水海纳,2021-03-30
-300962,中金辐照,2021-04-09
-300963,中洲特材,2021-04-09
-300964,本川智能,2021-08-05
-300965,恒宇信通,2021-04-02
-300966,共同药业,2021-04-09
-300967,晓鸣股份,2021-04-13
-300968,格林精密,2021-04-15
-300969,恒帅股份,2021-04-12
-300970,华绿生物,2021-04-12
-300971,博亚精工,2021-04-15
-300972,万辰集团,2021-04-19
-300973,立高食品,2021-04-15
-300975,商络电子,2021-04-21
-300976,达瑞电子,2021-04-19
-300977,深圳瑞捷,2021-04-20
-300978,东箭科技,2021-04-26
-300979,华利集团,2021-04-26
-300980,祥源新材,2021-04-21
-300981,中红医疗,2021-04-27
-300982,苏文电能,2021-04-27
-300983,尤安设计,2021-04-20
-300984,金沃股份,2021-06-18
-300985,致远新能,2021-04-29
-300986,志特新材,2021-04-30
-300987,川网传媒,2021-05-11
-300988,津荣天宇,2021-05-12
-300989,蕾奥规划,2021-05-07
-300990,同飞股份,2021-05-12
-300991,创益通,2021-05-20
-300992,泰福泵业,2021-05-25
-300993,玉马遮阳,2021-05-24
-300994,久祺股份,2021-08-12
-300995,奇德新材,2021-05-26
-300996,普联软件,2021-06-03
-300997,欢乐家,2021-06-02
-300998,宁波方正,2021-06-02
-300999,金龙鱼,2020-10-15
-301000,肇民科技,2021-05-28
-301001,凯淳股份,2021-05-28
-301002,崧盛股份,2021-06-07
-301003,江苏博云,2021-06-01
-301004,嘉益股份,2021-06-25
-301005,超捷股份,2021-06-01
-301006,迈拓股份,2021-06-07
-301007,德迈仕,2021-06-16
-301008,宏昌科技,2021-06-11
-301009,可靠股份,2021-06-17
-301010,晶雪节能,2021-06-18
-301011,华立科技,2021-06-17
-301012,扬电科技,2021-06-22
-301013,利和兴,2021-06-29
-301015,百洋医药,2021-06-30
-301016,雷尔伟,2021-06-30
-301017,漱玉平民,2021-07-05
-301018,申菱环境,2021-07-07
-301019,宁波色母,2021-06-28
-301020,密封科技,2021-07-06
-301021,英诺激光,2021-07-06
-301022,海泰科,2021-07-02
-301023,江南奕帆,2021-07-07
-301024,霍普股份,2021-07-28
-301025,读客文化,2021-07-19
-301026,浩通科技,2021-07-16
-301027,华蓝集团,2021-07-15
-301028,东亚机械,2021-07-20
-301029,怡合达,2021-07-23
-301030,仕净科技,2021-07-22
-301031,中熔电气,2021-07-15
-301032,新柴股份,2021-07-22
-301033,迈普医学,2021-07-26
-301035,润丰股份,2021-07-28
-301036,双乐股份,2021-07-29
-301037,保立佳,2021-07-30
-301038,深水规院,2021-08-04
-301039,中集车辆,2021-07-08
-301040,中环海陆,2021-08-03
-301041,金百泽,2021-08-11
-301042,安联锐视,2021-08-05
-301043,绿岛风,2021-08-11
-301045,天禄科技,2021-08-13
-301046,能辉科技,2021-08-17
-301047,义翘神州,2021-08-16
-301048,金鹰重工,2021-08-18
-301049,超越科技,2021-08-24
-301050,雷电微力,2021-08-24
-301051,信濠光电,2021-08-27
-301052,果麦文化,2021-08-30
-301053,远信工业,2021-09-01
-301055,张小泉,2021-09-06
-301056,森赫股份,2021-09-07
-301057,汇隆新材,2021-09-09
-301058,中粮科工,2021-09-09
-301059,金三江,2021-09-13
-301060,兰卫医学,2021-09-13
-301061,匠心家居,2021-09-13
-301062,上海艾录,2021-09-14
-301063,海锅股份,2021-09-24
-301065,本立科技,2021-09-14
-301066,万事利,2021-09-22
-301067,显盈科技,2021-09-22
-301068,大地海洋,2021-09-28
-301069,凯盛新材,2021-09-27
-301070,开勒股份,2021-09-23
-301071,力量钻石,2021-09-24
-301072,中捷精工,2021-09-29
-301073,君亭酒店,2021-09-30
-301075,多瑞医药,2021-09-29
-301076,新瀚新材,2021-10-11
-301077,星华新材,2021-09-30
-301078,孩子王,2021-10-14
-301079,邵阳液压,2021-10-19
-301080,百普赛斯,2021-10-18
-301081,严牌股份,2021-10-20
-301082,久盛电气,2021-10-27
-301083,百胜智能,2021-10-21
-301085,亚康股份,2021-10-18
-301086,鸿富瀚,2021-10-20
-301087,可孚医疗,2021-10-25
-301088,戎美股份,2021-10-28
-301089,拓新药业,2021-10-27
-301090,华润材料,2021-10-26
-301091,深城交,2021-10-29
-301092,争光股份,2021-11-02
-301093,华兰股份,2021-11-01
-301095,广立微,2022-08-05
-301096,百诚医药,2021-12-20
-301097,天益医疗,2022-04-07
-301098,金埔园林,2021-11-12
-301099,雅创电子,2021-11-22
-301100,风光股份,2021-12-17
-301101,明月镜片,2021-12-16
-301102,兆讯传媒,2022-03-28
-301103,何氏眼科,2022-03-22
-301105,鸿铭股份,2022-12-30
-301106,骏成科技,2022-01-28
-301107,瑜欣电子,2022-05-24
-301108,洁雅股份,2021-12-03
-301109,军信股份,2022-04-13
-301110,青木股份,2022-03-11
-301111,粤万年青,2021-12-07
-301112,信邦智能,2022-06-29
-301113,雅艺科技,2021-12-22
-301115,建科股份,2022-08-31
-301116,益客食品,2022-01-18
-301117,佳缘科技,2022-01-17
-301118,恒光股份,2021-11-18
-301119,正强股份,2021-11-22
-301120,新特电气,2022-04-19
-301121,紫建电子,2022-08-08
-301122,采纳股份,2022-01-26
-301123,奕东电子,2022-01-25
-301125,腾亚精工,2022-06-08
-301126,达嘉维康,2021-12-07
-301127,天源环保,2021-12-30
-301128,强瑞技术,2021-11-10
-301129,瑞纳智能,2021-11-02
-301130,西点药业,2022-02-23
-301131,聚赛龙,2022-03-14
-301132,满坤科技,2022-08-10
-301133,金钟股份,2021-11-26
-301135,瑞德智能,2022-04-12
-301136,招标股份,2022-01-11
-301137,哈焊华通,2022-03-22
-301138,华研精机,2021-12-15
-301139,元道通信,2022-07-08
-301141,中科磁业,2023-04-03
-301148,嘉戎技术,2022-04-21
-301149,隆华新材,2021-11-10
-301150,中一科技,2022-04-21
-301151,冠龙节能,2022-04-11
-301152,天力锂能,2022-08-29
-301153,中科江南,2022-05-18
-301155,海力风电,2021-11-24
-301156,美农生物,2022-06-17
-301157,华塑科技,2023-03-09
-301158,德石股份,2022-01-17
-301159,三维天地,2022-01-07
-301160,翔楼新材,2022-06-06
-301161,唯万密封,2022-09-14
-301162,国能日新,2022-04-29
-301163,宏德股份,2022-04-19
-301165,锐捷网络,2022-11-21
-301166,优宁维,2021-12-28
-301167,建研设计,2021-12-06
-301168,通灵股份,2021-12-10
-301169,零点有数,2021-11-03
-301170,锡南科技,2023-06-27
-301171,易点天下,2022-08-19
-301172,君逸数码,2023-07-26
-301175,中科环保,2022-07-08
-301176,逸豪新材,2022-09-28
-301177,迪阿股份,2021-12-15
-301178,天亿马,2021-11-12
-301179,泽宇智能,2021-12-08
-301180,万祥科技,2021-11-16
-301181,标榜股份,2022-02-21
-301182,凯旺科技,2021-12-23
-301183,东田微,2022-05-24
-301185,鸥玛软件,2021-11-19
-301186,超达装备,2021-12-23
-301187,欧圣电气,2022-04-22
-301188,力诺特玻,2021-11-11
-301189,奥尼电子,2021-12-28
-301190,善水科技,2021-12-24
-301191,菲菱科思,2022-05-26
-301192,泰祥股份,2022-08-11
-301193,家联科技,2021-12-09
-301195,北路智控,2022-08-01
-301196,唯科科技,2022-01-11
-301197,工大科雅,2022-08-08
-301198,喜悦智行,2021-12-02
-301199,迈赫股份,2021-12-07
-301200,大族数控,2022-02-28
-301201,诚达药业,2022-01-20
-301202,朗威股份,2023-07-05
-301203,国泰环保,2023-04-04
-301205,联特科技,2022-09-13
-301206,三元生物,2022-02-10
-301207,华兰疫苗,2022-02-18
-301208,中亦科技,2022-07-07
-301209,联合化学,2022-08-25
-301210,金杨股份,2023-06-30
-301211,亨迪药业,2021-12-22
-301212,联盛化学,2022-04-19
-301213,观想科技,2021-12-06
-301215,中汽股份,2022-03-08
-301216,万凯新材,2022-03-29
-301217,铜冠铜箔,2022-01-27
-301218,华是科技,2022-03-07
-301219,腾远钴业,2022-03-17
-301220,亚香股份,2022-06-22
-301221,光庭信息,2021-12-22
-301222,浙江恒威,2022-03-09
-301223,中荣股份,2022-10-26
-301225,恒勃股份,2023-06-16
-301226,祥明智能,2022-03-25
-301227,森鹰窗业,2022-09-26
-301228,实朴检测,2022-01-28
-301229,纽泰格,2022-02-22
-301230,泓博医药,2022-11-01
-301231,荣信文化,2022-09-08
-301232,飞沃科技,2023-06-15
-301233,盛帮股份,2022-07-06
-301234,五洲医疗,2022-07-05
-301235,华康医疗,2022-01-28
-301236,软通动力,2022-03-15
-301237,和顺科技,2022-03-23
-301238,瑞泰新材,2022-06-17
-301239,普瑞眼科,2022-07-05
-301246,宏源药业,2023-03-20
-301248,杰创智能,2022-04-20
-301251,威尔高,2023-09-06
-301252,同星科技,2023-05-25
-301255,通力科技,2022-12-27
-301256,华融化学,2022-03-22
-301257,普蕊斯,2022-05-17
-301258,富士莱,2022-03-29
-301259,艾布鲁,2022-04-26
-301260,格力博,2023-02-08
-301261,恒工精密,2023-07-10
-301262,海看股份,2023-06-20
-301263,泰恩康,2022-03-29
-301265,华新环保,2022-12-16
-301266,宇邦新材,2022-06-08
-301267,华厦眼科,2022-11-07
-301268,铭利达,2022-04-07
-301269,华大九天,2022-07-29
-301270,汉仪股份,2022-08-31
-301272,英华特,2023-07-13
-301273,瑞晨环保,2022-10-25
-301276,嘉曼服饰,2022-09-09
-301277,新天地,2022-11-16
-301278,快可电子,2022-08-04
-301279,金道科技,2022-04-13
-301280,珠城科技,2022-12-26
-301281,科源制药,2023-04-04
-301282,金禄电子,2022-08-26
-301283,聚胶股份,2022-09-02
-301285,鸿日达,2022-09-28
-301286,侨源股份,2022-06-14
-301287,康力源,2023-06-14
-301288,清研环境,2022-04-22
-301289,国缆检测,2022-06-22
-301290,东星医疗,2022-11-30
-301291,明阳电气,2023-06-30
-301292,海科新源,2023-07-07
-301293,三博脑科,2023-05-05
-301295,美硕科技,2023-06-28
-301296,新巨丰,2022-09-02
-301297,富乐德,2022-12-30
-301298,东利机械,2022-06-06
-301299,卓创资讯,2022-10-19
-301300,远翔新材,2022-08-19
-301301,川宁生物,2022-12-27
-301302,华如科技,2022-06-23
-301303,真兰仪表,2023-02-20
-301305,朗坤环境,2023-05-23
-301306,西测测试,2022-07-26
-301307,美利信,2023-04-24
-301308,江波龙,2022-08-05
-301309,万得凯,2022-09-19
-301310,鑫宏业,2023-06-02
-301311,昆船智能,2022-11-30
-301312,智立方,2022-07-11
-301313,凡拓数创,2022-09-30
-301314,科瑞思,2023-03-28
-301315,威士顿,2023-06-21
-301316,慧博云通,2022-10-13
-301317,鑫磊股份,2023-01-19
-301318,维海德,2022-08-10
-301319,唯特偶,2022-09-29
-301320,豪江智能,2023-06-09
-301321,翰博高新,2022-08-18
-301322,绿通科技,2023-03-06
-301323,新莱福,2023-06-06
-301325,曼恩斯特,2023-05-12
-301326,捷邦科技,2022-09-21
-301327,华宝新能,2022-09-19
-301328,维峰电子,2022-09-08
-301329,信音电子,2023-07-17
-301330,熵基科技,2022-08-17
-301331,恩威医药,2022-09-21
-301332,德尔玛,2023-05-18
-301333,诺思格,2022-08-02
-301335,天元宠物,2022-11-18
-301336,趣睡科技,2022-08-12
-301337,亚华电子,2023-05-26
-301338,凯格精机,2022-08-16
-301339,通行宝,2022-09-09
-301345,涛涛车业,2023-03-21
-301348,蓝箭电子,2023-08-10
-301349,信德新材,2022-09-09
-301353,普莱得,2023-05-30
-301355,南王科技,2023-06-12
-301356,天振股份,2022-11-14
-301357,北方长龙,2023-04-18
-301358,湖南裕能,2023-02-09
-301359,东南电子,2022-11-09
-301360,荣旗科技,2023-04-25
-301361,众智科技,2022-11-16
-301362,民爆光电,2023-08-04
-301363,美好医疗,2022-10-12
-301365,矩阵股份,2022-11-22
-301366,一博科技,2022-09-26
-301367,怡和嘉业,2022-11-01
-301368,丰立智能,2022-12-15
-301369,联动科技,2022-09-22
-301370,国科恒泰,2023-07-12
-301371,敷尔佳,2023-08-01
-301372,科净源,2023-08-11
-301373,凌玮科技,2023-02-08
-301376,致欧科技,2023-06-21
-301377,鼎泰高科,2022-11-22
-301378,通达海,2023-03-20
-301379,天山电子,2022-11-01
-301380,挖金客,2022-10-25
-301381,赛维时代,2023-07-12
-301382,蜂助手,2023-05-17
-301383,天键股份,2023-06-09
-301386,未来电器,2023-03-29
-301387,光大同创,2023-04-18
-301388,欣灵电气,2022-11-09
-301389,隆扬电子,2022-10-31
-301390,经纬股份,2023-05-08
-301391,卡莱特,2022-12-01
-301393,昊帆生物,2023-07-12
-301395,仁信新材,2023-07-03
-301396,宏景科技,2022-11-11
-301397,溯联股份,2023-06-28
-301398,星源卓镁,2022-12-15
-301399,英特科技,2023-05-23
-301408,华人健康,2023-03-01
-301418,协昌科技,2023-08-21
-301419,阿莱德,2023-02-09
-301421,波长光电,2023-08-23
-301428,世纪恒通,2023-05-19
-301429,森泰股份,2023-04-17
-301439,泓淋电力,2023-03-17
-301446,福事特,2023-07-25
-301448,开创电气,2023-06-19
-301456,盘古智能,2023-07-14
-301468,博盈特焊,2023-07-24
-301469,恒达新材,2023-08-22
-301486,致尚科技,2023-07-07
-301487,盟固利,2023-08-09
-301488,豪恩汽电,2023-07-04
-301498,乖宝宠物,2023-08-16
-301499,维科精密,2023-07-21
-301500,飞南资源,2023-09-21
-301503,智迪科技,2023-07-17
-301505,苏州规划,2023-07-19
-301507,民生健康,2023-09-05
-301509,金凯生科,2023-08-03
-301510,固高科技,2023-08-15
-301511,德福科技,2023-08-17
-301512,智信精密,2023-07-20
-301515,港通医疗,2023-07-25
-301517,陕西华达,2023-10-17
-301518,长华化学,2023-08-03
-301519,舜禹股份,2023-07-27
-301520,万邦医药,2023-09-25
-301525,儒竞科技,2023-08-30
-301528,多浦乐,2023-08-28
-301529,福赛科技,2023-09-11
-301533,威马农机,2023-08-18
-301548,崇德科技,2023-09-20
-301550,斯菱股份,2023-09-15
-301558,三态股份,2023-09-28
-301559,中集环科,2023-10-11
-430017,星昊医药,2023-05-31
-430047,诺思兰德,2020-11-24
-430090,同辉信息,2021-08-09
-430139,华岭股份,2022-10-28
-430198,微创光电,2020-07-27
-430300,辰光医疗,2022-12-07
-430418,苏轴股份,2020-07-27
-430425,乐创技术,2023-01-30
-430476,海能技术,2022-10-14
-430478,峆一药业,2023-02-23
-430489,佳先股份,2020-07-27
-430510,丰光精密,2020-12-28
-430556,雅达股份,2023-03-17
-430564,天润科技,2022-06-17
-430685,新芝生物,2022-10-10
-430718,合肥高科,2022-12-22
-600000,浦发银行,1999-11-10
-600001,邯郸钢铁,
-600002,齐鲁石化,
-600003,ST东北高,
-600004,白云机场,2003-04-28
-600005,武钢股份,
-600006,东风汽车,1999-07-27
-600007,中国国贸,1999-03-12
-600008,首创环保,2000-04-27
-600009,上海机场,1998-02-18
-600010,包钢股份,2001-03-09
-600011,华能国际,2001-12-06
-600012,皖通高速,2003-01-07
-600015,华夏银行,2003-09-12
-600016,民生银行,2000-12-19
-600017,日照港  ,2006-10-17
-600018,上港集团,2000-07-19
-600019,宝钢股份,2000-12-12
-600020,中原高速,2003-08-08
-600021,上海电力,2003-10-29
-600022,山东钢铁,2004-06-29
-600023,浙能电力,2013-12-19
-600025,华能水电,2017-12-15
-600026,中远海能,2002-05-23
-600027,华电国际,2005-02-03
-600028,中国石化,2001-08-08
-600029,南方航空,2003-07-25
-600030,中信证券,2003-01-06
-600031,三一重工,2003-07-03
-600032,浙江新能,2021-05-25
-600033,福建高速,2001-02-09
-600035,楚天高速,2004-03-10
-600036,招商银行,2002-04-09
-600037,歌华有线,2001-02-08
-600038,中直股份,2000-12-18
-600039,四川路桥,2003-03-25
-600048,保利发展,2006-07-31
-600050,中国联通,2002-10-09
-600051,宁波联合,1997-04-10
-600052,东望时代,1997-04-15
-600053,九鼎投资,1997-04-18
-600054,黄山旅游,1997-05-06
-600055,万东医疗,1997-05-19
-600056,中国医药,1997-05-15
-600057,厦门象屿,1997-06-04
-600058,五矿发展,1997-05-28
-600059,古越龙山,1997-05-16
-600060,海信视像,1997-04-22
-600061,国投资本,1997-05-19
-600062,华润双鹤,1997-05-22
-600063,皖维高新,1997-05-28
-600064,南京高科,1997-05-06
-600065,*ST联谊,
-600066,宇通客车,1997-05-08
-600067,冠城大通,1997-05-08
-600068,葛洲坝,
-600069,退市银鸽,
-600070,ST富润  ,1997-06-04
-600071,凤凰光学,1997-05-28
-600072,中船科技,1997-06-03
-600073,上海梅林,1997-07-04
-600074,退市保千,
-600075,新疆天业,1997-06-17
-600076,康欣新材,1997-05-26
-600077,*ST宋都,
-600078,ST澄星  ,1997-06-27
-600079,人福医药,1997-06-06
-600080,金花股份,1997-06-12
-600081,东风科技,1997-07-03
-600082,海泰发展,1997-06-20
-600083,博信股份,1997-06-06
-600084,中葡股份,1997-07-11
-600085,同仁堂  ,1997-06-25
-600086,退市金钰,
-600087,退市长油,
-600088,中视传媒,1997-06-16
-600089,特变电工,1997-06-18
-600090,退市济堂,
-600091,退市明科,
-600092,S*ST精密,
-600093,退市易见,
-600094,大名城  ,1997-07-03
-600095,湘财股份,1997-07-08
-600096,云天化  ,1997-07-09
-600097,开创国际,1997-06-19
-600098,广州发展,1997-07-18
-600099,林海股份,1997-07-04
-600100,同方股份,1997-06-27
-600101,明星电力,1997-06-27
-600102,莱钢股份,
-600103,青山纸业,1997-07-03
-600104,上汽集团,1997-11-25
-600105,永鼎股份,1997-09-29
-600106,重庆路桥,1997-06-18
-600107,美尔雅  ,1997-11-06
-600108,亚盛集团,1997-08-18
-600109,国金证券,1997-08-07
-600110,诺德股份,1997-10-07
-600111,北方稀土,1997-09-24
-600112,ST天成  ,1997-11-27
-600113,浙江东日,1997-10-21
-600114,东睦股份,2004-05-11
-600115,中国东航,1997-11-05
-600116,三峡水利,1997-08-04
-600117,*ST西钢 ,1997-10-15
-600118,中国卫星,1997-09-08
-600119,长江投资,1998-01-15
-600120,浙江东方,1997-12-01
-600121,郑州煤电,1998-01-07
-600122,*ST宏图,
-600123,兰花科创,1998-12-17
-600125,铁龙物流,1998-05-11
-600126,杭钢股份,1998-03-11
-600127,金健米业,1998-05-06
-600128,苏豪弘业,1997-09-01
-600129,太极集团,1997-11-18
-600130,波导股份,2000-07-06
-600131,国网信通,1998-04-02
-600132,重庆啤酒,1997-10-30
-600133,东湖高新,1998-02-12
-600135,乐凯胶片,1998-01-22
-600136,*ST明诚 ,1998-03-03
-600137,浪莎股份,1998-04-16
-600138,中青旅  ,1997-12-03
-600139,*ST西源,
-600141,兴发集团,1999-06-16
-600143,金发科技,2004-06-23
-600145,退市新亿,
-600146,退市环球,
-600148,长春一东,1998-05-20
-600149,廊坊发展,1999-10-14
-600150,中国船舶,1998-05-20
-600151,航天机电,1998-06-05
-600152,维科技术,1998-06-09
-600153,建发股份,1998-06-16
-600155,华创云信,1998-09-18
-600156,华升股份,1998-05-27
-600157,永泰能源,1998-05-13
-600158,中体产业,1998-03-27
-600159,大龙地产,1998-05-26
-600160,巨化股份,1998-06-26
-600161,天坛生物,1998-06-16
-600162,香江控股,1998-06-09
-600163,中闽能源,1998-06-02
-600165,宁科生物,1998-05-29
-600166,福田汽车,1998-06-02
-600167,联美控股,1999-01-28
-600168,武汉控股,1998-04-27
-600169,太原重工,1998-09-04
-600170,上海建工,1998-06-23
-600171,上海贝岭,1998-09-24
-600172,黄河旋风,1998-11-26
-600173,卧龙地产,1999-04-15
-600175,退市美都,
-600176,中国巨石,1999-04-22
-600177,雅戈尔  ,1998-11-19
-600178,东安动力,1998-10-14
-600179,安通控股,1998-11-04
-600180,瑞茂通  ,1998-07-03
-600181,S*ST云大,
-600182,S佳通   ,1999-05-07
-600183,生益科技,1998-10-28
-600184,光电股份,2003-11-06
-600185,格力地产,1999-06-11
-600186,莲花健康,1998-08-25
-600187,国中水务,1998-11-11
-600188,兖矿能源,1998-07-01
-600189,泉阳泉  ,1998-10-07
-600190,锦州港  ,1999-06-09
-600191,华资实业,1998-12-10
-600192,长城电工,1998-12-24
-600193,创兴资源,1999-05-27
-600195,中牧股份,1999-01-07
-600196,复星医药,1998-08-07
-600197,伊力特  ,1999-09-16
-600198,大唐电信,1998-10-21
-600199,金种子酒,1998-08-12
-600200,江苏吴中,1999-04-01
-600201,生物股份,1999-01-15
-600202,哈空调  ,1999-06-03
-600203,福日电子,1999-05-14
-600205,S山东铝,
-600206,有研新材,1999-03-19
-600207,安彩高科,1999-07-14
-600208,新湖中宝,1999-06-23
-600209,退市罗顿,
-600210,紫江企业,1999-08-24
-600211,西藏药业,1999-07-21
-600212,绿能慧充,1999-08-17
-600213,亚星客车,1999-08-31
-600215,派斯林  ,1999-09-09
-600216,浙江医药,1999-10-21
-600217,中再资环,1999-12-16
-600218,全柴动力,1998-12-03
-600219,南山铝业,1999-12-23
-600220,江苏阳光,1999-09-27
-600221,海航控股,1999-11-25
-600222,太龙药业,1999-11-05
-600223,福瑞达  ,2000-01-13
-600225,卓朗科技,2000-01-27
-600226,瀚叶股份,1999-11-16
-600227,赤天化  ,2000-02-21
-600228,返利科技,1999-01-19
-600229,城市传媒,2000-03-09
-600230,沧州大化,2000-04-06
-600231,凌钢股份,2000-05-11
-600232,金鹰股份,2000-06-02
-600233,圆通速递,2000-06-08
-600234,科新发展,2000-06-15
-600235,民丰特纸,2000-06-15
-600236,桂冠电力,2000-03-23
-600237,铜峰电子,2000-06-09
-600238,海南椰岛,2000-01-20
-600239,云南城投,1999-12-02
-600240,退市华业,
-600241,时代万恒,2000-11-28
-600242,退市中昌,
-600243,青海华鼎,2000-11-20
-600246,万通发展,2000-09-22
-600247,*ST成城,
-600248,陕建股份,2000-06-22
-600249,两面针  ,2004-01-30
-600250,南纺股份,2001-03-06
-600251,冠农股份,2003-06-09
-600252,中恒集团,2000-11-30
-600253,天方药业,
-600255,鑫科材料,2000-11-22
-600256,广汇能源,2000-05-26
-600257,大湖股份,2000-06-12
-600258,首旅酒店,2000-06-01
-600259,广晟有色,2000-05-25
-600260,*ST凯乐,
-600261,阳光照明,2000-07-20
-600262,北方股份,2000-06-30
-600263,路桥建设,
-600265,ST景谷  ,2000-08-25
-600266,城建发展,1999-02-03
-600267,海正药业,2000-07-25
-600268,国电南自,1999-11-18
-600269,赣粤高速,2000-05-18
-600270,外运发展,
-600271,航天信息,2003-07-11
-600272,开开实业,2001-02-28
-600273,嘉化能源,2003-06-27
-600275,退市昌鱼,
-600276,恒瑞医药,2000-10-18
-600277,亿利洁能,2000-07-25
-600278,东方创业,2000-07-12
-600279,重庆港  ,2000-07-31
-600280,中央商场,2000-09-26
-600281,华阳新材,2000-11-09
-600282,南钢股份,2000-09-19
-600283,钱江水利,2000-10-18
-600284,浦东建设,2004-03-16
-600285,羚锐制药,2000-10-18
-600286,S*ST国瓷,
-600287,江苏舜天,2000-09-01
-600288,大恒科技,2000-11-29
-600289,ST信通  ,2000-07-20
-600290,*ST华仪 ,2000-11-06
-600291,退市西水,
-600292,远达环保,2000-11-01
-600293,三峡新材,2000-09-19
-600295,鄂尔多斯,2001-04-26
-600296,S兰铝,
-600297,广汇汽车,2000-11-16
-600298,安琪酵母,2000-08-18
-600299,安迪苏  ,2000-04-20
-600300,维维股份,2000-06-30
-600301,华锡有色,2000-07-12
-600302,标准股份,2000-12-13
-600303,ST曙光  ,2000-12-26
-600305,恒顺醋业,2001-02-06
-600306,*ST商城 ,2000-12-26
-600307,酒钢宏兴,2000-12-20
-600308,华泰股份,2000-09-28
-600309,万华化学,2001-01-05
-600310,广西能源,2001-02-28
-600311,*ST荣华,
-600312,平高电气,2001-02-21
-600313,农发种业,2001-01-19
-600315,上海家化,2001-03-15
-600316,洪都航空,2000-12-15
-600317,营口港,
-600318,新力金融,2000-12-08
-600319,亚星化学,2001-03-26
-600320,振华重工,2000-12-21
-600321,正源股份,2001-05-24
-600322,津投城开,2001-09-10
-600323,瀚蓝环境,2000-12-25
-600325,华发股份,2004-02-25
-600326,西藏天路,2001-01-16
-600327,大东方  ,2002-06-25
-600328,中盐化工,2000-12-22
-600329,达仁堂  ,2001-06-06
-600330,天通股份,2001-01-18
-600331,宏达股份,2001-12-20
-600332,白云山  ,2001-02-06
-600333,长春燃气,2000-12-11
-600335,国机汽车,2001-03-05
-600336,澳柯玛  ,2000-12-29
-600337,美克家居,2000-11-27
-600338,西藏珠峰,2000-12-27
-600339,中油工程,2000-12-25
-600340,华夏幸福,2003-12-30
-600343,航天动力,2003-04-08
-600345,长江通信,2000-12-22
-600346,恒力石化,2001-08-20
-600348,华阳股份,2003-08-21
-600350,山东高速,2002-03-18
-600351,亚宝药业,2002-09-26
-600352,浙江龙盛,2003-08-01
-600353,旭光电子,2002-11-20
-600354,敦煌种业,2004-01-15
-600355,精伦电子,2002-06-13
-600356,恒丰纸业,2001-04-19
-600357,承德钒钛,
-600358,国旅联合,2000-09-22
-600359,新农开发,1999-04-29
-600360,华微电子,2001-03-16
-600361,创新新材,2001-11-29
-600362,江西铜业,2002-01-11
-600363,联创光电,2001-03-29
-600365,ST通葡  ,2001-01-15
-600366,宁波韵升,2000-10-30
-600367,红星发展,2001-03-20
-600368,五洲交通,2000-12-21
-600369,西南证券,2001-01-09
-600370,三房巷  ,2003-03-06
-600371,万向德农,2002-09-16
-600372,中航机载,2001-07-06
-600373,中文传媒,2002-03-04
-600375,汉马科技,2003-04-01
-600376,首开股份,2001-03-12
-600377,宁沪高速,2001-01-16
-600378,昊华科技,2001-01-11
-600379,宝光股份,2002-01-16
-600380,健康元  ,2001-06-08
-600381,青海春天,2001-05-08
-600382,广东明珠,2001-01-18
-600383,金地集团,2001-04-12
-600385,退市金泰,
-600386,北巴传媒,2001-02-16
-600387,ST海越  ,2004-02-18
-600388,龙净环保,2000-12-29
-600389,江山股份,2001-01-10
-600390,五矿资本,2001-01-15
-600391,航发科技,2001-12-12
-600392,盛和资源,2003-05-29
-600393,ST粤泰,
-600395,盘江股份,2001-05-31
-600396,*ST金山 ,2001-03-28
-600397,安源煤业,2002-07-02
-600398,海澜之家,2000-12-28
-600399,抚顺特钢,2000-12-29
-600400,红豆股份,2001-01-08
-600401,退市海润,
-600403,大有能源,2003-10-09
-600405,动力源  ,2004-04-01
-600406,国电南瑞,2003-10-16
-600408,安泰集团,2003-02-12
-600409,三友化工,2003-06-18
-600410,华胜天成,2004-04-27
-600415,小商品城,2002-05-09
-600416,湘电股份,2002-07-18
-600418,江淮汽车,2001-08-24
-600419,天润乳业,2001-06-28
-600420,国药现代,2004-06-16
-600421,华嵘控股,2004-06-07
-600422,昆药集团,2000-12-06
-600423,柳化股份,2003-07-17
-600425,青松建化,2003-07-24
-600426,华鲁恒升,2002-06-20
-600428,中远海特,2002-04-18
-600429,三元股份,2003-09-15
-600432,退市吉恩,
-600433,冠豪高新,2003-06-19
-600435,北方导航,2003-07-04
-600436,片仔癀  ,2003-06-16
-600438,通威股份,2004-03-02
-600439,瑞贝卡  ,2003-07-10
-600444,国机通用,2004-02-19
-600446,金证股份,2003-12-24
-600448,华纺股份,2001-09-03
-600449,宁夏建材,2003-08-29
-600452,涪陵电力,2004-03-03
-600455,博通股份,2004-03-29
-600456,宝钛股份,2002-04-12
-600458,时代新材,2002-12-19
-600459,贵研铂业,2003-05-16
-600460,士兰微  ,2003-03-11
-600461,洪城环境,2004-06-01
-600462,ST九有  ,2003-09-03
-600463,空港股份,2004-03-18
-600466,*ST蓝光,
-600467,好当家  ,2004-04-05
-600468,百利电气,2001-06-15
-600469,风神股份,2003-10-21
-600470,六国化工,2004-03-05
-600472,包头铝业,
-600475,华光环能,2003-07-21
-600476,湘邮科技,2003-12-10
-600477,杭萧钢构,2003-11-10
-600478,科力远  ,2003-09-18
-600479,千金药业,2004-03-12
-600480,凌云股份,2003-08-15
-600481,双良节能,2003-04-22
-600482,中国动力,2004-07-14
-600483,福能股份,2004-05-31
-600485,*ST信威,
-600486,扬农化工,2002-04-25
-600487,亨通光电,2003-08-22
-600488,津药药业,2001-06-18
-600489,中金黄金,2003-08-14
-600490,鹏欣资源,2003-06-26
-600491,龙元建设,2004-05-24
-600493,凤竹纺织,2004-04-21
-600495,晋西车轴,2004-05-26
-600496,精工钢构,2002-06-05
-600497,驰宏锌锗,2004-04-20
-600498,烽火通信,2001-08-23
-600499,科达制造,2002-10-10
-600500,中化国际,2000-03-01
-600501,航天晨光,2001-06-15
-600502,安徽建工,2003-04-15
-600503,华丽家族,2002-07-09
-600505,西昌电力,2002-05-30
-600506,统一股份,2001-12-26
-600507,方大特钢,2003-09-30
-600508,上海能源,2001-08-29
-600509,天富能源,2002-02-28
-600510,黑牡丹  ,2002-06-18
-600511,国药股份,2002-11-27
-600512,腾达建设,2002-12-26
-600513,联环药业,2003-03-19
-600515,海南机场,2002-08-06
-600516,方大炭素,2002-08-30
-600517,国网英大,2003-10-10
-600518,ST康美  ,2001-03-19
-600519,贵州茅台,2001-08-27
-600520,文一科技,2002-01-08
-600521,华海药业,2003-03-04
-600522,中天科技,2002-10-24
-600523,贵航股份,2001-12-27
-600525,长园集团,2002-12-02
-600526,菲达环保,2002-07-22
-600527,江南高纤,2003-11-27
-600528,中铁工业,2001-05-28
-600529,山东药玻,2002-06-03
-600530,ST交昂  ,2001-07-02
-600531,豫光金铅,2002-07-30
-600532,退市未来,
-600533,栖霞建设,2002-03-28
-600535,天士力  ,2002-08-23
-600536,中国软件,2002-05-17
-600537,亿晶光电,2003-01-23
-600538,国发股份,2003-01-14
-600539,狮头股份,2001-08-24
-600540,新赛股份,2004-01-07
-600543,*ST莫高 ,2004-03-24
-600545,卓郎智能,2003-12-03
-600546,山煤国际,2003-07-31
-600547,山东黄金,2003-08-28
-600548,深高速  ,2001-12-25
-600549,厦门钨业,2002-11-07
-600550,保变电气,2001-02-28
-600551,时代出版,2002-09-05
-600552,凯盛科技,2002-11-08
-600553,太行水泥,
-600555,退市海创,
-600556,天下秀  ,2001-08-07
-600557,康缘药业,2002-09-18
-600558,大西洋  ,2001-02-27
-600559,老白干酒,2002-10-29
-600560,金自天正,2002-09-19
-600561,江西长运,2002-07-16
-600562,国睿科技,2003-01-28
-600563,法拉电子,2002-12-10
-600565,迪马股份,2002-07-23
-600566,济川药业,2001-08-22
-600567,山鹰国际,2001-12-18
-600568,ST中珠  ,2001-05-18
-600569,安阳钢铁,2001-08-20
-600570,恒生电子,2003-12-16
-600571,信雅达  ,2002-11-01
-600572,康恩贝  ,2004-04-12
-600573,惠泉啤酒,2003-02-26
-600575,淮河能源,2003-03-28
-600576,祥源文旅,2003-02-20
-600577,精达股份,2002-09-11
-600578,京能电力,2002-05-10
-600579,克劳斯  ,2002-08-09
-600580,卧龙电驱,2002-06-06
-600581,八一钢铁,2002-08-16
-600582,天地科技,2002-05-15
-600583,海油工程,2002-02-05
-600584,长电科技,2003-06-03
-600585,海螺水泥,2002-02-07
-600586,金晶科技,2002-08-15
-600587,新华医疗,2002-09-27
-600588,用友网络,2001-05-18
-600589,*ST榕泰 ,2001-06-12
-600590,泰豪科技,2002-07-03
-600591,*ST上航,
-600592,龙溪股份,2002-08-05
-600593,大连圣亚,2002-07-11
-600594,益佰制药,2004-03-23
-600595,中孚实业,2002-06-26
-600596,新安股份,2001-09-06
-600597,光明乳业,2002-08-28
-600598,北大荒  ,2002-03-29
-600599,ST熊猫  ,2001-08-28
-600600,青岛啤酒,1993-08-27
-600601,方正科技,1990-12-19
-600602,云赛智联,1990-12-19
-600603,广汇物流,1992-01-13
-600604,市北高新,1992-03-27
-600605,汇通能源,1992-03-27
-600606,绿地控股,1992-03-27
-600607,上实医药,
-600608,ST沪科  ,1992-03-27
-600609,金杯汽车,1992-07-24
-600610,中毅达  ,1992-08-05
-600611,大众交通,1992-08-07
-600612,老凤祥  ,1992-08-14
-600613,神奇制药,1992-08-20
-600614,退市鹏起,
-600615,丰华股份,1992-09-10
-600616,金枫酒业,1992-09-29
-600617,国新能源,1992-10-13
-600618,氯碱化工,1992-11-13
-600619,海立股份,1992-11-16
-600620,天宸股份,1992-11-17
-600621,华鑫股份,1992-12-02
-600622,光大嘉宝,1992-12-03
-600623,华谊集团,1992-12-04
-600624,复旦复华,1993-01-05
-600625,PT水仙,
-600626,申达股份,1993-01-07
-600627,上电股份,
-600628,新世界  ,1993-01-19
-600629,华建集团,1993-02-09
-600630,龙头股份,1993-02-09
-600631,百联股份(已合并),
-600632,华联商厦,
-600633,浙数文化,1993-03-04
-600634,退市富控,
-600635,大众公用,1993-03-04
-600636,国新文化,1993-03-16
-600637,东方明珠,1993-03-16
-600638,新黄浦  ,1993-03-26
-600639,浦东金桥,1993-03-26
-600640,国脉文化,1993-04-07
-600641,万业企业,1993-04-07
-600642,申能股份,1993-04-16
-600643,爱建集团,1993-04-26
-600644,乐山电力,1993-04-26
-600645,中源协和,1993-05-04
-600646,ST国嘉,
-600647,*ST同达 ,1993-05-04
-600648,外高桥  ,1993-05-04
-600649,城投控股,1993-05-18
-600650,锦江在线,1993-06-07
-600651,飞乐音响,1990-12-19
-600652,退市游久,
-600653,申华控股,1990-12-19
-600654,ST中安  ,1990-12-19
-600655,豫园股份,1992-09-02
-600656,退市博元,
-600657,信达地产,1993-05-24
-600658,电子城  ,1993-05-24
-600659,*ST花雕,
-600660,福耀玻璃,1993-06-10
-600661,昂立教育,1993-06-14
-600662,外服控股,1993-06-14
-600663,陆家嘴  ,1993-06-28
-600664,哈药股份,1993-06-29
-600665,天地源  ,1993-07-09
-600666,ST瑞德  ,1993-07-12
-600667,太极实业,1993-07-28
-600668,尖峰集团,1993-07-28
-600669,*ST鞍成,
-600670,*ST斯达,
-600671,*ST目药 ,1993-08-23
-600672,*ST华圣,
-600673,东阳光  ,1993-09-17
-600674,川投能源,1993-09-24
-600675,中华企业,1993-09-24
-600676,交运股份,1993-09-28
-600677,*ST航通,
-600678,四川金顶,1993-10-08
-600679,上海凤凰,1993-10-08
-600680,*ST上普,
-600681,百川能源,1993-10-18
-600682,南京新百,1993-10-18
-600683,京投发展,1993-10-25
-600684,珠江股份,1993-10-28
-600685,中船防务,1993-10-28
-600686,金龙汽车,1993-11-08
-600687,退市刚泰,
-600688,上海石化,1993-11-08
-600689,上海三毛,1993-11-08
-600690,海尔智家,1993-11-19
-600691,阳煤化工,1993-11-19
-600692,亚通股份,1993-11-19
-600693,东百集团,1993-11-22
-600694,大商股份,1993-11-22
-600695,退市绿庭,
-600696,岩石股份,1993-12-06
-600697,欧亚集团,1993-12-06
-600698,湖南天雁,1993-12-06
-600699,均胜电子,1993-12-06
-600700,*ST数码,
-600701,退市工新,
-600702,舍得酒业,1996-05-24
-600703,三安光电,1996-05-28
-600704,物产中大,1996-06-06
-600705,中航产融,1996-05-16
-600706,曲江文旅,1996-05-16
-600707,彩虹股份,1996-05-20
-600708,光明地产,1996-06-06
-600709,ST生态,
-600710,苏美达  ,1996-07-01
-600711,盛屯矿业,1996-05-31
-600712,南宁百货,1996-06-26
-600713,南京医药,1996-07-01
-600714,金瑞矿业,1996-06-06
-600715,文投控股,1996-07-01
-600716,凤凰股份,1996-07-02
-600717,天津港  ,1996-06-14
-600718,东软集团,1996-06-18
-600719,大连热电,1996-07-16
-600720,祁连山  ,1996-07-16
-600721,百花医药,1996-06-26
-600722,金牛化工,1996-06-26
-600723,首商股份,
-600724,宁波富达,1996-07-16
-600725,云维股份,1996-07-02
-600726,华电能源,1996-07-01
-600727,鲁北化工,1996-07-02
-600728,佳都科技,1996-07-16
-600729,重庆百货,1996-07-02
-600730,中国高科,1996-07-26
-600731,湖南海利,1996-08-02
-600732,爱旭股份,1996-08-16
-600733,北汽蓝谷,1996-08-16
-600734,ST实达  ,1996-08-08
-600735,新华锦  ,1996-07-26
-600736,苏州高新,1996-08-15
-600737,中粮糖业,1996-07-31
-600738,丽尚国潮,1996-08-02
-600739,辽宁成大,1996-08-19
-600740,山西焦化,1996-08-08
-600741,华域汽车,1996-08-26
-600742,一汽富维,1996-08-26
-600743,华远地产,1996-09-09
-600744,华银电力,1996-09-05
-600745,闻泰科技,1996-08-28
-600746,江苏索普,1996-09-18
-600747,退市大控,
-600748,上实发展,1996-09-25
-600749,西藏旅游,1996-10-15
-600750,江中药业,1996-09-23
-600751,海航科技,1996-09-09
-600752,*ST哈慈,
-600753,庚星股份,1996-09-27
-600754,锦江酒店,1996-10-11
-600755,厦门国贸,1996-10-03
-600756,浪潮软件,1996-09-23
-600757,长江传媒,1996-10-03
-600758,辽宁能源,1996-10-29
-600759,*ST洲际 ,1996-10-08
-600760,中航沈飞,1996-10-11
-600761,安徽合力,1996-10-09
-600762,S*ST金荔,
-600763,通策医疗,1996-10-30
-600764,中国海防,1996-11-04
-600765,中航重机,1996-11-06
-600766,*ST园城 ,1996-10-28
-600767,退市运盛,
-600768,宁波富邦,1996-11-11
-600769,祥龙电业,1996-11-01
-600770,综艺股份,1996-11-20
-600771,广誉远  ,1996-11-05
-600772,S*ST龙昌,
-600773,西藏城投,1996-11-08
-600774,汉商集团,1996-11-08
-600775,南京熊猫,1996-11-18
-600776,东方通信,1996-11-26
-600777,新潮能源,1996-11-21
-600778,友好集团,1996-12-03
-600779,水井坊  ,1996-12-06
-600780,通宝能源,1996-12-05
-600781,退市辅仁,
-600782,新钢股份,1996-12-25
-600783,鲁信创投,1996-12-25
-600784,鲁银投资,1996-12-25
-600785,新华百货,1997-01-08
-600786,东方锅炉,
-600787,中储股份,1997-01-21
-600788,*ST达曼,
-600789,鲁抗医药,1997-02-26
-600790,轻纺城  ,1997-02-28
-600791,京能置业,1997-01-30
-600792,云煤能源,1997-01-23
-600793,宜宾纸业,1997-02-20
-600794,保税科技,1997-03-06
-600795,国电电力,1997-03-18
-600796,钱江生化,1997-04-08
-600797,浙大网新,1997-04-18
-600798,宁波海运,1997-04-23
-600799,*ST龙科,
-600800,渤海化学,1993-12-06
-600801,华新水泥,1994-01-03
-600802,福建水泥,1994-01-03
-600803,新奥股份,1994-01-03
-600804,ST鹏博士,1994-01-03
-600805,悦达投资,1994-01-03
-600806,退市昆机,
-600807,济南高新,1994-01-03
-600808,马钢股份,1994-01-06
-600809,山西汾酒,1994-01-06
-600810,神马股份,1994-01-06
-600811,东方集团,1994-01-06
-600812,华北制药,1994-01-14
-600813,ST鞍一工,
-600814,杭州解百,1994-01-14
-600815,厦工股份,1994-01-28
-600816,ST建元  ,1994-01-28
-600817,宇通重工,1994-01-28
-600818,中路股份,1994-01-28
-600819,耀皮玻璃,1994-01-28
-600820,隧道股份,1994-01-28
-600821,金开新能,1994-01-28
-600822,上海物贸,1994-02-04
-600823,ST世茂  ,1994-02-04
-600824,益民集团,1994-02-04
-600825,新华传媒,1994-02-04
-600826,兰生股份,1994-02-04
-600827,百联股份,1994-02-04
-600828,茂业商业,1994-02-24
-600829,人民同泰,1994-02-24
-600830,香溢融通,1994-02-24
-600831,广电网络,1994-02-24
-600832,东方明珠,
-600833,第一医药,1994-02-24
-600834,申通地铁,1994-02-24
-600835,上海机电,1994-02-24
-600836,上海易连,1994-02-24
-600837,海通证券,1994-02-24
-600838,上海九百,1994-02-24
-600839,四川长虹,1994-03-11
-600840,新湖创业,
-600841,动力新科,1994-03-11
-600842,中西药业,
-600843,上工申贝,1994-03-11
-600844,丹化科技,1994-03-11
-600845,宝信软件,1994-03-11
-600846,同济科技,1994-03-11
-600847,万里股份,1994-03-24
-600848,上海临港,1994-03-24
-600850,电科数字,1994-03-24
-600851,海欣股份,1994-04-04
-600852,*ST中川,
-600853,龙建股份,1994-04-04
-600854,春兰股份,1994-04-25
-600855,航天长峰,1994-04-25
-600856,退市中天,
-600857,宁波中百,1994-04-25
-600858,银座股份,1994-05-06
-600859,王府井  ,1994-05-06
-600860,京城股份,1994-05-06
-600861,北京人力,1994-05-20
-600862,中航高科,1994-05-20
-600863,内蒙华电,1994-05-20
-600864,哈投股份,1994-08-09
-600865,百大集团,1994-08-09
-600866,星湖科技,1994-08-18
-600867,通化东宝,1994-08-24
-600868,梅雁吉祥,1994-09-12
-600869,远东股份,1995-02-06
-600870,退市厦华,
-600871,石化油服,1995-04-11
-600872,中炬高新,1995-01-24
-600873,梅花生物,1995-02-17
-600874,创业环保,1995-06-30
-600875,东方电气,1995-10-10
-600876,凯盛新能,1995-10-31
-600877,电科芯片,1995-10-13
-600878,*ST北科,
-600879,航天电子,1995-11-15
-600880,博瑞传播,1995-11-15
-600881,亚泰集团,1995-11-15
-600882,妙可蓝多,1995-12-06
-600883,博闻科技,1995-12-08
-600884,杉杉股份,1996-01-30
-600885,宏发股份,1996-02-05
-600886,国投电力,1996-01-18
-600887,伊利股份,1996-03-12
-600888,新疆众和,1996-02-15
-600889,南京化纤,1996-03-08
-600890,退市中房,
-600891,退市秋林,
-600892,大晟文化,1996-03-15
-600893,航发动力,1996-04-08
-600894,广日股份,1996-03-28
-600895,张江高科,1996-04-22
-600896,退市海医,
-600897,厦门空港,1996-05-31
-600898,ST美讯  ,1996-04-18
-600899,*ST信联,
-600900,长江电力,2003-11-18
-600901,江苏金租,2018-03-01
-600903,贵州燃气,2017-11-07
-600905,三峡能源,2021-06-10
-600906,财达证券,2021-05-07
-600908,无锡银行,2016-09-23
-600909,华安证券,2016-12-06
-600916,中国黄金,2021-02-05
-600917,重庆燃气,2014-09-30
-600918,中泰证券,2020-06-03
-600919,江苏银行,2016-08-02
-600925,苏能股份,2023-03-29
-600926,杭州银行,2016-10-27
-600927,永安期货,2021-12-23
-600928,西安银行,2019-03-01
-600929,雪天盐业,2018-03-26
-600933,爱柯迪  ,2017-11-17
-600935,华塑股份,2021-11-26
-600936,广西广电,2016-08-15
-600938,中国海油,2022-04-21
-600939,重庆建工,2017-02-21
-600941,中国移动,2022-01-05
-600955,维远股份,2021-09-15
-600956,新天绿能,2020-06-29
-600958,东方证券,2015-03-23
-600959,江苏有线,2015-04-28
-600960,渤海汽车,2004-04-07
-600961,株冶集团,2004-08-30
-600962,国投中鲁,2004-06-22
-600963,岳阳林纸,2004-05-25
-600965,福成股份,2004-07-13
-600966,博汇纸业,2004-06-08
-600967,内蒙一机,2004-05-18
-600968,海油发展,2019-06-26
-600969,郴电国际,2004-04-08
-600970,中材国际,2005-04-12
-600971,恒源煤电,2004-08-17
-600973,宝胜股份,2004-08-02
-600975,新五丰  ,2004-06-09
-600976,健民集团,2004-04-19
-600977,中国电影,2016-08-09
-600978,*ST宜生,
-600979,广安爱众,2004-09-06
-600980,北矿科技,2004-05-12
-600981,汇鸿集团,2004-06-30
-600982,宁波能源,2004-07-06
-600983,惠而浦  ,2004-07-27
-600984,建设机械,2004-07-07
-600985,淮北矿业,2004-04-28
-600986,浙文互联,2004-04-26
-600987,航民股份,2004-08-09
-600988,赤峰黄金,2004-04-14
-600989,宝丰能源,2019-05-16
-600990,四创电子,2004-05-10
-600991,广汽长丰,
-600992,贵绳股份,2004-05-14
-600993,马应龙  ,2004-05-17
-600995,南网储能,2004-06-15
-600996,贵广网络,2016-12-26
-600997,开滦股份,2004-06-02
-600998,九州通  ,2010-11-02
-600999,招商证券,2009-11-17
-601000,唐山港  ,2010-07-05
-601001,晋控煤业,2006-06-23
-601002,晋亿实业,2007-01-26
-601003,柳钢股份,2007-02-27
-601005,重庆钢铁,2007-02-28
-601006,大秦铁路,2006-08-01
-601007,金陵饭店,2007-04-06
-601008,连云港  ,2007-04-26
-601009,南京银行,2007-07-19
-601010,文峰股份,2011-06-03
-601011,宝泰隆  ,2011-03-09
-601012,隆基绿能,2012-04-11
-601015,陕西黑猫,2014-11-05
-601016,节能风电,2014-09-29
-601018,宁波港  ,2010-09-28
-601019,山东出版,2017-11-22
-601020,华钰矿业,2016-03-16
-601021,春秋航空,2015-01-21
-601022,宁波远洋,2022-12-08
-601028,玉龙股份,2011-11-07
-601038,一拖股份,2012-08-08
-601058,赛轮轮胎,2011-06-30
-601059,信达证券,2023-02-01
-601061,中信金属,2023-04-10
-601065,江盐集团,2023-04-10
-601066,中信建投,2018-06-20
-601068,中铝国际,2018-08-31
-601069,西部黄金,2015-01-22
-601077,渝农商行,2019-10-29
-601086,国芳集团,2017-09-29
-601088,中国神华,2007-10-09
-601089,福元医药,2022-06-30
-601098,中南传媒,2010-10-28
-601099,太平洋  ,2007-12-28
-601100,恒立液压,2011-10-28
-601101,昊华能源,2010-03-31
-601106,中国一重,2010-02-09
-601107,四川成渝,2009-07-27
-601108,财通证券,2017-10-24
-601111,中国国航,2006-08-18
-601113,华鼎股份,2011-05-09
-601116,三江购物,2011-03-02
-601117,中国化学,2010-01-07
-601118,海南橡胶,2011-01-07
-601121,宝地矿业,2023-03-10
-601126,四方股份,2010-12-31
-601127,赛力斯  ,2016-06-15
-601128,常熟银行,2016-09-30
-601133,柏诚股份,2023-04-10
-601136,首创证券,2022-12-22
-601137,博威合金,2011-01-27
-601138,工业富联,2018-06-08
-601139,深圳燃气,2009-12-25
-601155,新城控股,2015-12-04
-601156,东航物流,2021-06-09
-601158,重庆水务,2010-03-29
-601162,天风证券,2018-10-19
-601163,三角轮胎,2016-09-09
-601166,兴业银行,2007-02-05
-601168,西部矿业,2007-07-12
-601169,北京银行,2007-09-19
-601177,杭齿前进,2010-10-11
-601179,中国西电,2010-01-28
-601186,中国铁建,2008-03-10
-601187,厦门银行,2020-10-27
-601188,龙江交通,2010-03-19
-601198,东兴证券,2015-02-26
-601199,江南水务,2011-03-17
-601200,上海环境,2017-03-31
-601208,东材科技,2011-05-20
-601211,国泰君安,2015-06-26
-601212,白银有色,2017-02-15
-601216,君正集团,2011-02-22
-601218,吉鑫科技,2011-05-06
-601222,林洋能源,2011-08-08
-601225,陕西煤业,2014-01-28
-601226,华电重工,2014-12-11
-601228,广州港  ,2017-03-29
-601229,上海银行,2016-11-16
-601231,环旭电子,2012-02-20
-601233,桐昆股份,2011-05-18
-601236,红塔证券,2019-07-05
-601238,广汽集团,2012-03-29
-601258,*ST庞大,
-601268,*ST二重,
-601279,英利汽车,2021-04-15
-601288,农业银行,2010-07-15
-601298,青岛港  ,2019-01-21
-601299,中国北车,
-601311,骆驼股份,2011-06-02
-601318,中国平安,2007-03-01
-601319,中国人保,2018-11-16
-601326,秦港股份,2017-08-16
-601328,交通银行,2007-05-15
-601330,绿色动力,2018-06-11
-601333,广深铁路,2006-12-22
-601336,新华保险,2011-12-16
-601339,百隆东方,2012-06-12
-601360,三六零  ,2012-01-16
-601366,利群股份,2017-04-12
-601368,绿城水务,2015-06-12
-601369,陕鼓动力,2010-04-28
-601375,中原证券,2017-01-03
-601377,兴业证券,2010-10-13
-601388,怡球资源,2012-04-23
-601390,中国中铁,2007-12-03
-601398,工商银行,2006-10-27
-601399,国机重装,2020-06-08
-601456,国联证券,2020-07-31
-601500,通用股份,2016-09-19
-601512,中新集团,2019-12-20
-601515,东风股份,2012-02-16
-601518,吉林高速,2010-03-19
-601519,大智慧  ,2011-01-28
-601528,瑞丰银行,2021-06-25
-601555,东吴证券,2011-12-12
-601558,退市锐电,
-601566,九牧王  ,2011-05-30
-601567,三星医疗,2011-06-15
-601568,北元集团,2020-10-20
-601577,长沙银行,2018-09-26
-601579,会稽山  ,2014-08-25
-601588,北辰实业,2006-10-16
-601595,上海电影,2016-08-17
-601598,中国外运,2019-01-18
-601599,浙文影业,2011-05-27
-601600,中国铝业,2007-04-30
-601601,中国太保,2007-12-25
-601606,长城军工,2018-08-06
-601607,上海医药,1994-03-24
-601608,中信重工,2012-07-06
-601609,金田股份,2020-04-22
-601611,中国核建,2016-06-06
-601615,明阳智能,2019-01-23
-601616,广电电气,2011-02-01
-601618,中国中冶,2009-09-21
-601619,嘉泽新能,2017-07-20
-601628,中国人寿,2007-01-09
-601633,长城汽车,2011-09-28
-601636,旗滨集团,2011-08-12
-601658,邮储银行,2019-12-10
-601665,齐鲁银行,2021-06-18
-601666,平煤股份,2006-11-23
-601668,中国建筑,2009-07-29
-601669,中国电建,2011-10-18
-601677,明泰铝业,2011-09-19
-601678,滨化股份,2010-02-23
-601686,友发集团,2020-12-04
-601688,华泰证券,2010-02-26
-601689,拓普集团,2015-03-19
-601696,中银证券,2020-02-26
-601698,中国卫通,2019-06-28
-601699,潞安环能,2006-09-22
-601700,风范股份,2011-01-18
-601702,华峰铝业,2020-09-07
-601717,郑煤机  ,2010-08-03
-601718,际华集团,2010-08-16
-601727,上海电气,2008-12-05
-601728,中国电信,2021-08-20
-601766,中国中车,2008-08-18
-601777,力帆科技,2010-11-25
-601778,晶科科技,2020-05-19
-601788,光大证券,2009-08-18
-601789,宁波建工,2011-08-16
-601798,蓝科高新,2011-06-22
-601799,星宇股份,2011-02-01
-601800,中国交建,2012-03-09
-601801,皖新传媒,2010-01-18
-601808,中海油服,2007-09-28
-601811,新华文轩,2016-08-08
-601816,京沪高铁,2020-01-16
-601818,光大银行,2010-08-18
-601825,沪农商行,2021-08-19
-601827,三峰环境,2020-06-05
-601828,美凯龙  ,2018-01-17
-601838,成都银行,2018-01-31
-601857,中国石油,2007-11-05
-601858,中国科传,2017-01-18
-601860,紫金银行,2019-01-03
-601865,福莱特  ,2019-02-15
-601866,中远海发,2007-12-12
-601868,中国能建,2021-09-28
-601869,长飞光纤,2018-07-20
-601872,招商轮船,2006-12-01
-601877,正泰电器,2010-01-21
-601878,浙商证券,2017-06-26
-601880,辽港股份,2010-12-06
-601881,中国银河,2017-01-23
-601882,海天精工,2016-11-07
-601886,江河集团,2011-08-18
-601888,中国中免,2009-10-15
-601890,亚星锚链,2010-12-28
-601898,中煤能源,2008-02-01
-601899,紫金矿业,2008-04-25
-601900,南方传媒,2016-02-15
-601901,方正证券,2011-08-10
-601908,京运通  ,2011-09-08
-601916,浙商银行,2019-11-26
-601918,新集能源,2007-12-19
-601919,中远海控,2007-06-26
-601921,浙版传媒,2021-07-23
-601928,凤凰传媒,2011-11-30
-601929,吉视传媒,2012-02-23
-601933,永辉超市,2010-12-15
-601939,建设银行,2007-09-25
-601949,中国出版,2017-08-21
-601952,苏垦农发,2017-05-15
-601956,东贝集团,2020-12-25
-601958,金钼股份,2008-04-17
-601963,重庆银行,2021-02-05
-601965,中国汽研,2012-06-11
-601966,玲珑轮胎,2016-07-06
-601968,宝钢包装,2015-06-11
-601969,海南矿业,2014-12-09
-601975,招商南油,2019-01-08
-601985,中国核电,2015-06-10
-601988,中国银行,2006-07-05
-601989,中国重工,2009-12-16
-601990,南京证券,2018-06-13
-601991,大唐发电,2006-12-20
-601992,金隅集团,2011-03-01
-601995,中金公司,2020-11-02
-601996,丰林集团,2011-09-29
-601997,贵阳银行,2016-08-16
-601998,中信银行,2007-04-27
-601999,出版传媒,2007-12-21
-603000,人民网  ,2012-04-27
-603001,ST奥康  ,2012-04-26
-603002,宏昌电子,2012-05-18
-603003,龙宇股份,2012-08-17
-603005,晶方科技,2014-02-10
-603006,联明股份,2014-06-30
-603007,ST花王  ,2016-08-26
-603008,喜临门  ,2012-07-17
-603009,北特科技,2014-07-18
-603010,万盛股份,2014-10-10
-603011,合锻智能,2014-11-07
-603012,创力集团,2015-03-20
-603013,亚普股份,2018-05-09
-603015,弘讯科技,2015-03-03
-603016,新宏泰  ,2016-07-01
-603017,XD中衡设,2014-12-31
-603018,华设集团,2014-10-13
-603019,中科曙光,2014-11-06
-603020,爱普股份,2015-03-25
-603021,山东华鹏,2015-04-23
-603022,新通联  ,2015-05-18
-603023,威帝股份,2015-05-27
-603025,大豪科技,2015-04-22
-603026,胜华新材,2015-05-29
-603027,千禾味业,2016-03-07
-603028,赛福天  ,2016-03-31
-603029,天鹅股份,2016-04-27
-603030,*ST全筑 ,2015-03-20
-603031,安孚科技,2016-08-22
-603032,德新科技,2017-01-05
-603033,三维股份,2016-12-07
-603035,常熟汽饰,2017-01-05
-603036,如通股份,2016-12-09
-603037,凯众股份,2017-01-20
-603038,华立股份,2017-01-16
-603039,泛微网络,2017-01-13
-603040,新坐标  ,2017-02-09
-603041,美思德  ,2017-03-30
-603042,华脉科技,2017-06-02
-603043,广州酒家,2017-06-27
-603045,福达合金,2018-05-17
-603048,浙江黎明,2021-11-16
-603050,科林电气,2017-04-14
-603051,鹿山新材,2022-03-25
-603052,可川科技,2022-10-11
-603053,成都燃气,2019-12-17
-603055,台华新材,2017-09-21
-603056,德邦股份,2018-01-16
-603057,紫燕食品,2022-09-26
-603058,永吉股份,2016-12-23
-603059,倍加洁  ,2018-03-02
-603060,国检集团,2016-11-09
-603061,金海通,2023-03-03
-603063,禾望电气,2017-07-28
-603065,宿迁联盛,2023-03-21
-603066,音飞储存,2015-06-11
-603067,振华股份,2016-09-13
-603068,博通集成,2019-04-15
-603069,海汽集团,2016-07-12
-603070,万控智造,2022-03-10
-603071,物产环能,2021-12-16
-603073,彩蝶实业,2023-03-16
-603075,热威股份,2023-09-11
-603076,乐惠国际,2017-11-13
-603077,和邦生物,2012-07-31
-603078,江化微  ,2017-04-10
-603079,圣达生物,2017-08-23
-603080,新疆火炬,2018-01-03
-603081,大丰实业,2017-04-20
-603083,剑桥科技,2017-11-10
-603085,天成自控,2015-06-30
-603086,先达股份,2017-05-11
-603087,甘李药业,2020-06-29
-603088,宁波精达,2014-11-11
-603089,正裕工业,2017-01-26
-603090,宏盛股份,2016-08-31
-603093,南华期货,2019-08-30
-603095,越剑智能,2020-04-15
-603096,新经典  ,2017-04-25
-603097,江苏华辰,2022-05-12
-603098,森特股份,2016-12-16
-603099,长白山  ,2014-08-22
-603100,川仪股份,2014-08-05
-603101,汇嘉时代,2016-05-06
-603102,百合股份,2022-01-25
-603103,横店影视,2017-10-12
-603105,芯能科技,2018-07-09
-603106,恒银科技,2017-09-20
-603108,润达医疗,2015-05-27
-603109,神驰机电,2019-12-31
-603110,东方材料,2017-10-13
-603111,康尼机电,2014-08-01
-603112,华翔股份,2020-09-17
-603113,金能科技,2017-05-11
-603115,海星股份,2019-08-09
-603116,红蜻蜓  ,2015-06-29
-603117,ST万林  ,2015-06-29
-603118,共进股份,2015-02-25
-603119,浙江荣泰,2023-08-01
-603121,华培动力,2019-01-11
-603122,合富中国,2022-02-16
-603123,翠微股份,2012-05-03
-603125,常青科技,2023-04-10
-603126,中材节能,2014-07-31
-603127,昭衍新药,2017-08-25
-603128,华贸物流,2012-05-29
-603129,春风动力,2017-08-18
-603130,云中马,2022-11-18
-603131,上海沪工,2016-06-07
-603132,金徽股份,2022-02-22
-603133,*ST碳元 ,2017-03-20
-603135,中重科技,2023-04-10
-603136,天目湖  ,2017-09-27
-603137,恒尚节能,2023-04-19
-603138,海量数据,2017-03-06
-603139,康惠制药,2017-04-21
-603150,万朗磁塑,2022-01-24
-603151,邦基科技,2022-10-19
-603153,上海建科,2023-03-13
-603155,新亚强,2020-09-01
-603156,养元饮品,2018-02-12
-603157,退市拉夏,
-603158,腾龙股份,2015-03-20
-603159,上海亚虹,2016-08-12
-603160,汇顶科技,2016-10-17
-603161,科华控股,2018-01-05
-603162,海通发展,2023-03-29
-603163,圣晖集成,2022-10-13
-603165,荣晟环保,2017-01-17
-603166,福达股份,2014-11-27
-603167,渤海轮渡,2012-09-06
-603168,莎普爱思,2014-07-02
-603169,兰石重装,2014-10-09
-603170,宝立食品,2022-07-15
-603171,税友股份,2021-06-30
-603172,万丰股份,2023-05-10
-603173,福斯达,2023-01-30
-603176,汇通集团,2021-12-31
-603177,德创环保,2017-02-07
-603178,圣龙股份,2017-03-28
-603179,新泉股份,2017-03-17
-603180,金牌厨柜,2017-05-12
-603181,皇马科技,2017-08-24
-603182,嘉华股份,2022-09-09
-603183,建研院  ,2017-09-05
-603185,弘元绿能,2018-12-28
-603186,华正新材,2017-01-03
-603187,海容冷链,2018-11-29
-603188,亚邦股份,2014-09-09
-603189,网达软件,2016-09-14
-603190,亚通精工,2023-02-17
-603191,望变电气,2022-04-28
-603192,汇得科技,2018-08-28
-603193,润本股份,2023-10-17
-603195,公牛集团,2020-02-06
-603196,日播时尚,2017-05-31
-603197,保隆科技,2017-05-19
-603198,迎驾贡酒,2015-05-28
-603199,九华旅游,2015-03-26
-603200,上海洗霸,2017-06-01
-603201,常润股份,2022-07-29
-603203,快克智能,2016-11-08
-603206,嘉环科技,2022-05-06
-603208,江山欧派,2017-02-10
-603209,兴通股份,2022-03-24
-603211,晋拓股份,2022-07-25
-603212,赛伍技术,2020-04-30
-603213,镇洋发展,2021-11-11
-603214,爱婴室  ,2018-03-30
-603215,比依股份,2022-02-18
-603216,梦天家居,2021-12-15
-603217,元利科技,2019-06-20
-603218,日月股份,2016-12-28
-603219,富佳股份,2021-11-22
-603220,中贝通信,2018-11-15
-603221,爱丽家居,2020-03-23
-603222,济民医疗,2015-02-17
-603223,恒通股份,2015-06-30
-603225,新凤鸣  ,2017-04-18
-603226,菲林格尔,2017-06-15
-603227,雪峰科技,2015-05-15
-603228,景旺电子,2017-01-06
-603229,奥翔药业,2017-05-09
-603230,内蒙新华,2021-12-24
-603232,格尔软件,2017-04-21
-603233,大参林  ,2017-07-31
-603235,天新药业,2022-07-12
-603236,移远通信,2019-07-16
-603237,五芳斋,2022-08-31
-603238,诺邦股份,2017-02-22
-603239,浙江仙通,2016-12-30
-603255,鼎际得,2022-08-18
-603256,宏和科技,2019-07-19
-603258,电魂网络,2016-10-26
-603259,药明康德,2018-05-08
-603260,合盛硅业,2017-10-30
-603261,立航科技,2022-03-15
-603266,天龙股份,2017-01-10
-603267,鸿远电子,2019-05-15
-603268,松发股份,2015-03-19
-603269,海鸥股份,2017-05-17
-603270,金帝股份,2023-09-01
-603272,联翔股份,2022-05-20
-603275,众辰科技,2023-08-23
-603276,恒兴新材,2023-09-25
-603277,银都股份,2017-09-11
-603278,大业股份,2017-11-13
-603279,景津装备,2019-07-29
-603280,南方路机,2022-11-08
-603281,江瀚新材,2023-01-31
-603282,亚光股份,2023-03-15
-603283,赛腾股份,2017-12-25
-603286,日盈电子,2017-06-27
-603288,海天味业,2014-02-11
-603289,泰瑞机器,2017-10-31
-603290,斯达半导,2020-02-04
-603291,联合水务,2023-03-27
-603296,华勤技术,2023-08-08
-603297,永新光学,2018-09-10
-603298,杭叉集团,2016-12-27
-603299,苏盐井神,2015-12-31
-603300,华铁应急,2015-05-29
-603301,振德医疗,2018-04-12
-603303,得邦照明,2017-03-30
-603305,旭升集团,2017-07-10
-603306,华懋科技,2014-09-26
-603307,扬州金泉,2023-02-16
-603308,应流股份,2014-01-22
-603309,维力医疗,2015-03-02
-603311,金海高科,2015-05-18
-603313,梦百合  ,2016-10-13
-603315,福鞍股份,2015-04-24
-603316,诚邦股份,2017-06-19
-603317,天味食品,2019-04-16
-603318,水发燃气,2015-04-24
-603319,湘油泵  ,2016-11-30
-603320,迪贝电气,2017-05-02
-603321,梅轮电梯,2017-09-15
-603322,超讯通信,2016-07-28
-603323,苏农银行,2016-11-29
-603324,盛剑环境,2021-04-07
-603326,我乐家居,2017-06-16
-603327,福蓉科技,2019-05-23
-603328,依顿电子,2014-07-01
-603329,上海雅仕,2017-12-29
-603330,天洋新材,2017-02-13
-603331,百达精工,2017-07-05
-603332,苏州龙杰,2019-01-17
-603333,尚纬股份,2012-05-07
-603335,迪生力  ,2017-06-20
-603336,宏辉果蔬,2016-11-24
-603337,杰克股份,2017-01-19
-603338,浙江鼎力,2015-03-25
-603339,四方科技,2016-05-19
-603345,安井食品,2017-02-22
-603348,文灿股份,2018-04-26
-603351,威尔药业,2019-01-30
-603353,和顺石油,2020-04-07
-603355,莱克电气,2015-05-13
-603356,华菱精工,2018-01-24
-603357,设计总院,2017-08-01
-603358,华达科技,2017-01-25
-603359,东珠生态,2017-09-01
-603360,百傲化学,2017-02-06
-603363,傲农生物,2017-09-26
-603365,水星家纺,2017-11-20
-603366,日出东方,2012-05-21
-603367,辰欣药业,2017-09-29
-603368,柳药集团,2014-12-04
-603369,今世缘  ,2014-07-03
-603377,东方时尚,2016-02-05
-603378,亚士创能,2017-09-28
-603379,三美股份,2019-04-02
-603380,易德龙  ,2017-06-22
-603383,顶点软件,2017-05-22
-603385,惠达卫浴,2017-04-05
-603386,骏亚科技,2017-09-12
-603387,基蛋生物,2017-07-17
-603388,元成股份,2017-03-24
-603389,亚振家居,2016-12-15
-603390,通达电气,2019-11-25
-603392,万泰生物,2020-04-29
-603393,新天然气,2016-09-12
-603396,金辰股份,2017-10-18
-603398,沐邦高科,2015-12-09
-603399,吉翔股份,2012-08-24
-603408,建霖家居,2020-07-30
-603416,信捷电气,2016-12-21
-603421,鼎信通讯,2016-10-11
-603429,集友股份,2017-01-24
-603439,贵州三力,2020-04-28
-603444,吉比特  ,2017-01-04
-603456,九洲药业,2014-10-10
-603458,勘设股份,2017-08-09
-603466,风语筑  ,2017-10-20
-603477,巨星农牧,2017-12-18
-603486,科沃斯  ,2018-05-28
-603488,展鹏科技,2017-05-16
-603489,八方股份,2019-11-11
-603496,恒为科技,2017-06-07
-603499,翔港科技,2017-10-16
-603500,祥和实业,2017-09-04
-603501,韦尔股份,2017-05-04
-603505,金石资源,2017-05-03
-603506,南都物业,2018-02-01
-603507,振江股份,2017-11-06
-603508,思维列控,2015-12-24
-603511,爱慕股份,2021-05-31
-603515,欧普照明,2016-08-19
-603516,淳中科技,2018-02-02
-603517,绝味食品,2017-03-17
-603518,锦泓集团,2014-12-03
-603519,立霸股份,2015-03-19
-603520,司太立  ,2016-03-09
-603527,众源新材,2017-09-07
-603528,多伦科技,2016-05-03
-603529,爱玛科技,2021-06-15
-603530,神马电力,2019-08-05
-603533,掌阅科技,2017-09-21
-603535,嘉诚国际,2017-08-08
-603536,惠发食品,2017-06-13
-603538,美诺华  ,2017-04-07
-603551,奥普家居,2020-01-15
-603555,ST贵人  ,2014-01-24
-603556,海兴电力,2016-11-10
-603557,ST起步  ,2017-08-18
-603558,健盛集团,2015-01-27
-603559,ST通脉  ,2016-12-02
-603565,中谷物流,2020-09-25
-603566,普莱柯  ,2015-05-18
-603567,珍宝岛  ,2015-04-24
-603568,伟明环保,2015-05-28
-603569,长久物流,2016-08-10
-603577,汇金通  ,2016-12-22
-603578,三星新材,2017-03-06
-603579,荣泰健康,2017-01-11
-603580,艾艾精工,2017-05-25
-603583,捷昌驱动,2018-09-21
-603585,苏利股份,2016-12-14
-603586,金麒麟  ,2017-04-06
-603587,地素时尚,2018-06-22
-603588,高能环境,2014-12-29
-603589,口子窖  ,2015-06-29
-603590,康辰药业,2018-08-27
-603595,东尼电子,2017-07-12
-603596,伯特利  ,2018-04-27
-603598,引力传媒,2015-05-27
-603599,广信股份,2015-05-13
-603600,永艺股份,2015-01-23
-603601,再升科技,2015-01-22
-603602,纵横通信,2017-08-10
-603603,*ST博天 ,2017-02-17
-603605,珀莱雅  ,2017-11-15
-603606,东方电缆,2014-10-15
-603607,京华激光,2017-10-25
-603608,天创时尚,2016-02-18
-603609,禾丰股份,2014-08-08
-603610,麒盛科技,2019-10-29
-603611,诺力股份,2015-01-28
-603612,索通发展,2017-07-18
-603613,国联股份,2019-07-30
-603615,茶花股份,2017-02-13
-603616,韩建河山,2015-06-11
-603617,君禾股份,2017-07-03
-603618,杭电股份,2015-02-17
-603619,中曼石油,2017-11-17
-603626,科森科技,2017-02-09
-603628,清源股份,2017-01-12
-603629,利通电子,2018-12-24
-603630,拉芳家化,2017-03-13
-603633,徕木股份,2016-11-17
-603636,南威软件,2014-12-30
-603637,镇海股份,2017-02-08
-603638,艾迪精密,2017-01-20
-603639,海利尔  ,2017-01-12
-603648,畅联股份,2017-09-13
-603650,彤程新材,2018-06-27
-603655,朗博科技,2017-12-29
-603656,泰禾智能,2017-03-21
-603657,春光科技,2018-07-30
-603658,安图生物,2016-09-01
-603659,璞泰来  ,2017-11-03
-603660,苏州科达,2016-12-01
-603661,恒林股份,2017-11-21
-603662,柯力传感,2019-08-06
-603663,三祥新材,2016-08-01
-603665,康隆达  ,2017-03-13
-603666,亿嘉和  ,2018-06-12
-603667,五洲新春,2016-10-25
-603668,天马科技,2017-01-17
-603669,灵康药业,2015-05-28
-603676,卫信康  ,2017-07-21
-603677,奇精机械,2017-02-06
-603678,火炬电子,2015-01-26
-603679,华体科技,2017-06-21
-603680,今创集团,2018-02-27
-603681,永冠新材,2019-03-26
-603682,锦和商管,2020-04-21
-603683,晶华新材,2017-10-20
-603685,晨丰科技,2017-11-27
-603686,福龙马  ,2015-01-26
-603687,大胜达  ,2019-07-26
-603688,石英股份,2014-10-31
-603689,皖天然气,2017-01-10
-603690,至纯科技,2017-01-13
-603693,江苏新能,2018-07-03
-603696,安记食品,2015-12-09
-603697,有友食品,2019-05-08
-603698,航天工程,2015-01-28
-603699,纽威股份,2014-01-17
-603700,宁水集团,2019-01-22
-603701,德宏股份,2016-04-12
-603703,盛洋科技,2015-04-23
-603706,东方环宇,2018-07-09
-603707,健友股份,2017-07-19
-603708,家家悦  ,2016-12-13
-603709,中源家居,2018-02-08
-603711,香飘飘  ,2017-11-30
-603712,七一二  ,2018-02-26
-603713,密尔克卫,2018-07-13
-603716,塞力医疗,2016-10-31
-603717,天域生态,2017-03-27
-603718,海利生物,2015-05-15
-603719,良品铺子,2020-02-24
-603721,中广天择,2017-08-11
-603722,阿科力  ,2017-10-25
-603725,天安新材,2017-09-06
-603726,朗迪集团,2016-04-21
-603727,博迈科  ,2016-11-22
-603728,鸣志电器,2017-05-09
-603729,龙韵股份,2015-03-24
-603730,岱美股份,2017-07-28
-603733,仙鹤股份,2018-04-20
-603737,三棵树  ,2016-06-03
-603738,泰晶科技,2016-09-28
-603739,蔚蓝生物,2019-01-16
-603755,日辰股份,2019-08-28
-603757,大元泵业,2017-07-11
-603758,秦安股份,2017-05-17
-603759,海天股份,2021-03-26
-603766,隆鑫通用,2012-08-10
-603767,中马传动,2017-06-13
-603768,常青股份,2017-03-24
-603773,沃格光电,2018-04-17
-603776,永安行  ,2017-08-17
-603777,来伊份  ,2016-10-12
-603778,乾景园林,2015-12-31
-603779,威龙股份,2016-05-16
-603786,科博达  ,2019-10-15
-603787,新日股份,2017-04-27
-603788,宁波高发,2015-01-20
-603789,星光农机,2015-04-27
-603790,雅运股份,2018-09-12
-603797,联泰环保,2017-04-13
-603798,康普顿  ,2016-04-06
-603799,华友钴业,2015-01-29
-603800,道森股份,2015-12-10
-603801,志邦家居,2017-06-30
-603803,瑞斯康达,2017-04-20
-603806,福斯特  ,2014-09-05
-603808,歌力思  ,2015-04-22
-603809,豪能股份,2017-11-28
-603810,丰山集团,2018-09-17
-603811,诚意药业,2017-03-15
-603813,原尚股份,2017-09-18
-603815,交建股份,2019-10-21
-603816,顾家家居,2016-10-14
-603817,海峡环保,2017-02-20
-603818,曲美家居,2015-04-22
-603819,神力股份,2016-11-25
-603822,嘉澳环保,2016-04-28
-603823,百合花  ,2016-12-20
-603825,华扬联众,2017-08-02
-603826,坤彩科技,2017-04-14
-603828,柯利达  ,2015-02-26
-603829,洛凯股份,2017-10-17
-603833,欧派家居,2017-03-28
-603836,海程邦达,2021-05-26
-603838,四通股份,2015-07-01
-603839,安正时尚,2017-02-14
-603843,正平股份,2016-09-05
-603848,好太太  ,2017-12-01
-603855,华荣股份,2017-05-24
-603856,东宏股份,2017-11-06
-603858,步长制药,2016-11-18
-603859,能科科技,2016-10-21
-603860,中公高科,2017-08-02
-603861,白云电器,2016-03-22
-603863,松炀资源,2019-06-21
-603866,桃李面包,2015-12-22
-603867,新化股份,2019-06-27
-603868,飞科电器,2016-04-18
-603869,新智认知,2015-03-26
-603871,嘉友国际,2018-02-06
-603876,鼎胜新材,2018-04-18
-603877,太平鸟  ,2017-01-09
-603878,武进不锈,2016-12-19
-603879,永悦科技,2017-06-14
-603880,ST南卫  ,2017-08-07
-603881,数据港  ,2017-02-08
-603882,金域医学,2017-09-08
-603883,老百姓  ,2015-04-23
-603885,吉祥航空,2015-05-27
-603886,元祖股份,2016-12-28
-603887,城地香江,2016-10-10
-603888,新华网  ,2016-10-28
-603889,新澳股份,2014-12-31
-603890,春秋电子,2017-12-12
-603893,瑞芯微,2020-02-07
-603895,天永智能,2018-01-22
-603896,寿仙谷  ,2017-05-10
-603897,长城科技,2018-04-10
-603898,好莱客  ,2015-02-17
-603899,晨光股份,2015-01-27
-603900,莱绅通灵,2016-11-23
-603901,永创智能,2015-05-29
-603903,中持股份,2017-03-14
-603906,龙蟠科技,2017-04-10
-603908,牧高笛  ,2017-03-07
-603909,建发合诚,2016-06-28
-603912,佳力图  ,2017-11-01
-603915,国茂股份,2019-06-14
-603916,苏博特  ,2017-11-10
-603917,合力科技,2017-12-04
-603918,金桥信息,2015-05-28
-603919,金徽酒  ,2016-03-10
-603920,世运电路,2017-04-26
-603922,金鸿顺  ,2017-10-23
-603926,铁流股份,2017-05-10
-603927,中科软  ,2019-09-09
-603928,兴业股份,2016-12-12
-603929,亚翔集成,2016-12-30
-603931,格林达,2020-08-19
-603933,睿能科技,2017-07-06
-603936,博敏电子,2015-12-09
-603937,丽岛新材,2017-11-02
-603938,三孚股份,2017-06-28
-603939,益丰药房,2015-02-17
-603948,建业股份,2020-03-02
-603949,雪龙集团,2020-03-10
-603950,长源东谷,2020-05-26
-603955,大千生态,2017-03-10
-603956,威派格  ,2019-02-22
-603958,哈森股份,2016-06-29
-603959,百利科技,2016-05-17
-603960,克来机电,2017-03-14
-603963,大理药业,2017-09-22
-603966,法兰泰克,2017-01-25
-603967,中创物流,2019-04-29
-603968,醋化股份,2015-05-18
-603969,银龙股份,2015-02-27
-603970,中农立华,2017-11-16
-603976,正川股份,2017-08-22
-603977,国泰集团,2016-11-11
-603978,深圳新星,2017-08-07
-603979,金诚信  ,2015-06-30
-603980,吉华集团,2017-06-15
-603982,泉峰汽车,2019-05-22
-603983,丸美股份,2019-07-25
-603985,恒润股份,2017-05-05
-603986,兆易创新,2016-08-18
-603987,康德莱  ,2016-11-21
-603988,中电电机,2014-11-04
-603989,艾华集团,2015-05-15
-603990,麦迪科技,2016-12-08
-603991,至正股份,2017-03-08
-603992,松霖科技,2019-08-26
-603993,洛阳钼业,2012-10-09
-603995,甬金股份,2019-12-24
-603996,退市中新,
-603997,继峰股份,2015-03-02
-603998,方盛制药,2014-12-05
-603999,读者传媒,2015-12-10
-605001,威奥股份,2020-05-22
-605003,众望布艺,2020-09-08
-605005,合兴股份,2021-01-19
-605006,山东玻纤,2020-09-03
-605007,五洲特纸,2020-11-10
-605008,长鸿高科,2020-08-21
-605009,豪悦护理,2020-09-11
-605011,杭州热电,2021-06-30
-605016,百龙创园,2021-04-21
-605018,长华集团,2020-09-29
-605020,永和股份,2021-07-09
-605028,世茂能源,2021-07-12
-605033,美邦股份,2021-09-16
-605050,福然德,2020-09-24
-605055,迎丰股份,2021-01-29
-605056,咸亨国际,2021-07-20
-605058,澳弘电子,2020-10-21
-605060,联德股份,2021-03-01
-605066,天正电气,2020-08-07
-605068,明新旭腾,2020-11-23
-605069,正和生态,2021-08-16
-605077,华康股份,2021-02-09
-605080,浙江自然,2021-05-06
-605081,太和水,2021-02-09
-605086,龙高股份,2021-04-16
-605088,冠盛股份,2020-08-17
-605089,味知香,2021-04-27
-605090,九丰能源,2021-05-25
-605098,行动教育,2021-04-21
-605099,共创草坪,2020-09-30
-605100,华丰股份,2020-08-11
-605108,同庆楼,2020-07-16
-605111,新洁能,2020-09-28
-605116,奥锐特,2020-09-21
-605117,德业股份,2021-04-20
-605118,力鼎光电,2020-07-30
-605122,四方新材,2021-03-10
-605123,派克新材,2020-08-25
-605128,上海沿浦,2020-09-15
-605133,嵘泰股份,2021-02-24
-605136,丽人丽妆,2020-09-29
-605138,盛泰集团,2021-10-27
-605151,西上海,2020-12-15
-605155,西大门,2020-12-31
-605158,华达新材,2020-08-05
-605162,新中港,2021-07-07
-605166,聚合顺,2020-06-18
-605167,利柏特,2021-07-26
-605168,三人行,2020-05-28
-605169,洪通燃气,2020-10-30
-605177,东亚药业,2020-11-25
-605178,时空科技,2020-08-21
-605179,一鸣食品,2020-12-28
-605180,华生科技,2021-04-30
-605183,确成股份,2020-12-07
-605186,健麾信息,2020-12-22
-605188,国光连锁,2020-07-28
-605189,富春染织,2021-05-28
-605196,华通线缆,2021-05-11
-605198,安德利,2020-09-18
-605199,葫芦娃,2020-07-10
-605208,永茂泰,2021-03-08
-605218,伟时电子,2020-09-28
-605222,起帆电缆,2020-07-31
-605228,神通科技,2021-01-20
-605255,天普股份,2020-08-25
-605258,协和电子,2020-12-03
-605259,绿田机械,2021-06-15
-605266,健之佳,2020-12-01
-605268,王力安防,2021-02-24
-605277,新亚电子,2021-01-06
-605286,同力日升,2021-03-22
-605287,德才股份,2021-07-06
-605288,凯迪股份,2020-06-01
-605289,罗曼股份,2021-04-26
-605296,神农集团,2021-05-28
-605298,必得科技,2021-03-01
-605299,舒华体育,2020-12-15
-605300,佳禾食品,2021-04-30
-605303,园林股份,2021-03-01
-605305,中际联合,2021-05-06
-605318,法狮龙,2020-08-03
-605319,无锡振华,2021-06-07
-605333,沪光股份,2020-08-18
-605336,帅丰电器,2020-10-19
-605337,李子园,2021-02-08
-605338,巴比食品,2020-10-12
-605339,南侨食品,2021-05-18
-605358,立昂微,2020-09-11
-605365,立达信,2021-07-20
-605366,宏柏新材,2020-08-12
-605368,蓝天燃气,2021-01-29
-605369,拱东医疗,2020-09-16
-605376,博迁新材,2020-12-08
-605377,华旺科技,2020-12-28
-605378,野马电池,2021-04-12
-605388,均瑶健康,2020-08-18
-605389,长龄液压,2021-03-22
-605398,新炬网络,2021-01-21
-605399,晨光新材,2020-08-04
-605488,福莱新材,2021-05-13
-605499,东鹏饮料,2021-05-27
-605500,森林包装,2020-12-22
-605507,国邦医药,2021-08-02
-605555,德昌股份,2021-10-21
-605566,福莱蒽特,2021-10-25
-605567,春雪食品,2021-10-13
-605577,龙版传媒,2021-08-24
-605580,恒盛能源,2021-08-19
-605588,冠石科技,2021-08-12
-605589,圣泉集团,2021-08-10
-605598,上海港湾,2021-09-17
-605599,菜百股份,2021-09-09
-688001,华兴源创,2019-07-22
-688002,睿创微纳,2019-07-22
-688003,天准科技,2019-07-22
-688004,博汇科技,2020-06-12
-688005,容百科技,2019-07-22
-688006,杭可科技,2019-07-22
-688007,光峰科技,2019-07-22
-688008,澜起科技,2019-07-22
-688009,中国通号,2019-07-22
-688010,福光股份,2019-07-22
-688011,新光光电,2019-07-22
-688012,中微公司,2019-07-22
-688013,天臣医疗,2020-09-28
-688015,交控科技,2019-07-22
-688016,心脉医疗,2019-07-22
-688017,绿的谐波,2020-08-28
-688018,乐鑫科技,2019-07-22
-688019,安集科技,2019-07-22
-688020,方邦股份,2019-07-22
-688021,奥福环保,2019-11-06
-688022,瀚川智能,2019-07-22
-688023,安恒信息,2019-11-05
-688025,杰普特  ,2019-10-31
-688026,洁特生物,2020-01-22
-688027,国盾量子,2020-07-09
-688028,沃尔德  ,2019-07-22
-688029,南微医学,2019-07-22
-688030,山石网科,2019-09-30
-688031,星环科技,2022-10-18
-688032,禾迈股份,2021-12-20
-688033,天宜上佳,2019-07-22
-688035,德邦科技,2022-09-19
-688036,传音控股,2019-09-30
-688037,芯源微,2019-12-16
-688038,中科通达,2021-07-13
-688039,当虹科技,2019-12-11
-688041,海光信息,2022-08-12
-688045,必易微,2022-05-26
-688046,药康生物,2022-04-25
-688047,龙芯中科,2022-06-24
-688048,长光华芯,2022-04-01
-688049,炬芯科技,2021-11-29
-688050,爱博医疗,2020-07-29
-688051,佳华科技,2020-03-20
-688052,纳芯微,2022-04-22
-688053,思科瑞,2022-07-08
-688055,龙腾光电,2020-08-17
-688056,莱伯泰科,2020-09-02
-688057,金达莱,2020-11-11
-688058,宝兰德  ,2019-11-01
-688059,华锐精密,2021-02-08
-688060,云涌科技,2020-07-10
-688061,灿瑞科技,2022-10-18
-688062,迈威生物,2022-01-18
-688063,派能科技,2020-12-30
-688065,凯赛生物,2020-08-12
-688066,航天宏图,2019-07-22
-688067,爱威科技,2021-06-16
-688068,热景生物,2019-09-30
-688069,德林海,2020-07-22
-688070,纵横股份,2021-02-10
-688071,华依科技,2021-07-29
-688072,拓荆科技,2022-04-20
-688073,毕得医药,2022-10-11
-688075,安旭生物,2021-11-18
-688076,诺泰生物,2021-05-20
-688077,大地熊,2020-07-22
-688078,龙软科技,2019-12-30
-688079,美迪凯,2021-03-02
-688080,映翰通,2020-02-12
-688081,兴图新科,2020-01-06
-688082,盛美上海,2021-11-18
-688083,中望软件,2021-03-11
-688084,晶品特装,2022-12-08
-688085,三友医疗,2020-04-09
-688087,英科再生,2021-07-09
-688088,虹软科技,2019-07-22
-688089,嘉必优,2019-12-19
-688090,瑞松科技,2020-02-17
-688091,上海谊众,2021-09-09
-688092,爱科科技,2021-03-19
-688093,世华科技,2020-09-30
-688095,福昕软件,2020-09-08
-688096,京源环保,2020-04-09
-688097,博众精工,2021-05-12
-688098,申联生物,2019-10-28
-688099,晶晨股份,2019-08-08
-688100,威胜信息,2020-01-21
-688101,三达膜,2019-11-15
-688102,斯瑞新材,2022-03-16
-688103,国力股份,2021-09-10
-688105,诺唯赞,2021-11-15
-688106,金宏气体,2020-06-16
-688107,安路科技,2021-11-12
-688108,赛诺医疗,2019-10-30
-688109,品茗科技,2021-03-30
-688110,东芯股份,2021-12-10
-688111,金山办公,2019-11-18
-688112,鼎阳科技,2021-12-01
-688113,联测科技,2021-05-06
-688114,华大智造,2022-09-09
-688115,思林杰,2022-03-14
-688116,天奈科技,2019-09-25
-688117,圣诺生物,2021-06-03
-688118,普元信息,2019-12-04
-688119,中钢洛耐,2022-06-06
-688120,华海清科,2022-06-08
-688121,卓然股份,2021-09-06
-688122,西部超导,2019-07-22
-688123,聚辰股份,2019-12-23
-688125,安达智能,2022-04-15
-688126,沪硅产业,2020-04-20
-688127,蓝特光学,2020-09-21
-688128,中国电研,2019-11-05
-688129,东来技术,2020-10-23
-688130,晶华微,2022-07-29
-688131,皓元医药,2021-06-08
-688132,邦彦技术,2022-09-23
-688133,泰坦科技,2020-10-30
-688135,利扬芯片,2020-11-11
-688136,科兴制药,2020-12-14
-688137,近岸蛋白,2022-09-29
-688138,清溢光电,2019-11-20
-688139,海尔生物,2019-10-25
-688141,杰华特,2022-12-23
-688143,长盈通,2022-12-12
-688146,中船特气,2023-04-21
-688147,微导纳米,2022-12-23
-688148,芳源股份,2021-08-06
-688150,莱特光电,2022-03-18
-688151,华强科技,2021-12-06
-688152,麒麟信安,2022-10-28
-688153,唯捷创芯,2022-04-12
-688155,先惠技术,2020-08-11
-688156,路德环境,2020-09-22
-688157,松井股份,2020-06-09
-688158,优刻得,2020-01-20
-688159,有方科技,2020-01-23
-688160,步科股份,2020-11-12
-688161,威高骨科,2021-06-30
-688162,巨一科技,2021-11-10
-688163,赛伦生物,2022-03-11
-688165,埃夫特,2020-07-15
-688166,博瑞医药,2019-11-08
-688167,炬光科技,2021-12-24
-688168,安博通  ,2019-09-06
-688169,石头科技,2020-02-21
-688170,德龙激光,2022-04-29
-688171,纬德信息,2022-01-27
-688172,燕东微,2022-12-16
-688173,希荻微,2022-01-21
-688175,高凌信息,2022-03-15
-688176,亚虹医药,2022-01-07
-688177,百奥泰,2020-02-21
-688178,万德斯,2020-01-14
-688179,阿拉丁,2020-10-26
-688180,君实生物,2020-07-15
-688181,八亿时空,2020-01-06
-688182,灿勤科技,2021-11-16
-688183,生益电子,2021-02-25
-688184,帕瓦股份,2022-09-19
-688185,康希诺,2020-08-13
-688186,广大特材,2020-02-11
-688187,时代电气,2021-09-07
-688188,柏楚电子,2019-08-08
-688189,南新制药,2020-03-26
-688190,云路股份,2021-11-26
-688191,智洋创新,2021-04-08
-688192,迪哲医药,2021-12-10
-688193,仁度生物,2022-03-30
-688195,腾景科技,2021-03-26
-688196,卓越新能,2019-11-21
-688197,首药控股,2022-03-23
-688198,佰仁医疗,2019-12-09
-688199,久日新材,2019-11-05
-688200,华峰测控,2020-02-18
-688201,信安世纪,2021-04-21
-688202,美迪西  ,2019-11-05
-688203,海正生材,2022-08-16
-688205,德科立,2022-08-09
-688206,概伦电子,2021-12-28
-688207,格灵深瞳,2022-03-17
-688208,道通科技,2020-02-13
-688209,英集芯,2022-04-19
-688210,统联精密,2021-12-27
-688211,中科微至,2021-10-26
-688212,澳华内镜,2021-11-15
-688213,思特威,2022-05-20
-688215,瑞晟智能,2020-08-28
-688216,气派科技,2021-06-23
-688217,睿昂基因,2021-05-17
-688218,江苏北人,2019-12-11
-688219,会通股份,2020-11-18
-688220,翱捷科技,2022-01-14
-688221,前沿生物,2020-10-28
-688222,成都先导,2020-04-16
-688223,晶科能源,2022-01-26
-688225,亚信安全,2022-02-09
-688226,威腾电气,2021-07-07
-688227,品高股份,2021-12-30
-688228,开普云,2020-03-27
-688229,博睿数据,2020-08-17
-688230,芯导科技,2021-12-01
-688231,隆达股份,2022-07-22
-688232,新点软件,2021-11-17
-688233,神工股份,2020-02-21
-688234,天岳先进,2022-01-12
-688235,百济神州,2021-12-15
-688236,春立医疗,2021-12-30
-688237,超卓航科,2022-07-01
-688238,和元生物,2022-03-22
-688239,航宇科技,2021-07-05
-688244,永信至诚,2022-10-19
-688246,嘉和美康,2021-12-14
-688247,宣泰医药,2022-08-25
-688248,南网科技,2021-12-22
-688249,晶合集成,2023-05-05
-688251,井松智能,2022-06-06
-688252,天德钰,2022-09-27
-688253,英诺特,2022-07-28
-688255,凯尔达,2021-10-25
-688256,寒武纪,2020-07-20
-688257,新锐股份,2021-10-27
-688258,卓易信息,2019-12-09
-688259,创耀科技,2022-01-12
-688260,昀冢科技,2021-04-06
-688261,东微半导,2022-02-10
-688262,国芯科技,2022-01-06
-688265,南模生物,2021-12-28
-688266,泽璟制药,2020-01-23
-688267,中触媒,2022-02-16
-688268,华特气体,2019-12-26
-688269,凯立新材,2021-06-09
-688270,臻镭科技,2022-01-27
-688271,联影医疗,2022-08-22
-688272,*ST富吉,2021-10-18
-688273,麦澜德,2022-08-11
-688275,万润新能,2022-09-29
-688276,百克生物,2021-06-25
-688277,天智航,2020-07-07
-688278,特宝生物,2020-01-17
-688279,峰岹科技,2022-04-20
-688280,精进电动,2021-10-27
-688281,华秦科技,2022-03-07
-688282,理工导航,2022-03-18
-688283,坤恒顺维,2022-02-15
-688285,高铁电气,2021-10-20
-688286,敏芯股份,2020-08-10
-688287,观典防务,2022-05-25
-688288,鸿泉物联,2019-11-06
-688289,圣湘生物,2020-08-28
-688290,景业智能,2022-04-29
-688291,金橙子,2022-10-26
-688292,浩瀚深度,2022-08-18
-688293,奥浦迈,2022-09-02
-688295,中复神鹰,2022-04-06
-688296,和达科技,2021-07-27
-688297,中无人机,2022-06-29
-688298,东方生物,2020-02-05
-688299,长阳科技,2019-11-06
-688300,联瑞新材,2019-11-15
-688301,奕瑞科技,2020-09-18
-688302,海创药业,2022-04-12
-688303,大全能源,2021-07-22
-688305,科德数控,2021-07-09
-688306,均普智能,2022-03-22
-688307,中润光学,2023-02-16
-688308,欧科亿,2020-12-10
-688309,恒誉环保,2020-07-14
-688310,迈得医疗,2019-12-03
-688311,盟升电子,2020-07-31
-688312,燕麦科技,2020-06-08
-688313,仕佳光子,2020-08-12
-688314,康拓医疗,2021-05-18
-688315,诺禾致源,2021-04-13
-688316,青云科技,2021-03-16
-688317,之江生物,2021-01-18
-688318,财富趋势,2020-04-27
-688319,欧林生物,2021-06-08
-688320,禾川科技,2022-04-28
-688321,微芯生物,2019-08-12
-688322,奥比中光,2022-07-07
-688323,瑞华泰,2021-04-28
-688325,赛微微电,2022-04-22
-688326,经纬恒润,2022-04-19
-688327,云从科技,2022-05-27
-688328,深科达,2021-03-09
-688329,艾隆科技,2021-03-29
-688330,宏力达,2020-10-15
-688331,荣昌生物,2022-03-31
-688332,中科蓝讯,2022-07-15
-688333,铂力特  ,2019-07-22
-688334,西高院,2023-06-19
-688335,复洁环保,2020-08-17
-688336,三生国健,2020-07-22
-688337,普源精电,2022-04-08
-688338,赛科希德,2020-08-06
-688339,亿华通,2020-08-10
-688343,云天励飞,2023-04-04
-688345,博力威,2021-06-11
-688347,华虹公司,2023-08-07
-688348,昱能科技,2022-06-08
-688349,三一重能,2022-06-22
-688350,富淼科技,2021-01-28
-688351,微电生理,2022-08-31
-688352,颀中科技,2023-04-20
-688353,华盛锂电,2022-07-13
-688355,明志科技,2021-05-12
-688356,键凯科技,2020-08-26
-688357,建龙微纳,2019-12-04
-688358,祥生医疗,2019-12-03
-688359,三孚新科,2021-05-21
-688360,德马科技,2020-06-02
-688361,中科飞测,2023-05-19
-688362,甬矽电子,2022-11-16
-688363,华熙生物,2019-11-06
-688365,光云科技,2020-04-29
-688366,昊海生科,2019-10-30
-688367,工大高科,2021-06-28
-688368,晶丰明源,2019-10-14
-688369,致远互联,2019-10-31
-688370,丛麟科技,2022-08-25
-688371,菲沃泰,2022-08-02
-688372,伟测科技,2022-10-26
-688373,盟科药业,2022-08-05
-688375,国博电子,2022-07-22
-688376,美埃科技,2022-11-18
-688377,迪威尔,2020-07-08
-688378,奥来德,2020-09-03
-688379,华光新材,2020-08-19
-688380,中微半导,2022-08-05
-688381,帝奥微,2022-08-23
-688382,益方生物,2022-07-25
-688383,新益昌,2021-04-28
-688385,复旦微电,2021-08-04
-688386,泛亚微透,2020-10-16
-688387,信科移动,2022-09-26
-688388,嘉元科技,2019-07-22
-688389,普门科技,2019-11-05
-688390,固德威,2020-09-04
-688391,钜泉科技,2022-09-13
-688392,骄成超声,2022-09-27
-688393,安必平,2020-08-20
-688395,正弦电气,2021-04-29
-688396,华润微,2020-02-27
-688398,赛特新材,2020-02-11
-688399,硕世生物,2019-12-05
-688400,凌云光,2022-07-06
-688401,路维光电,2022-08-17
-688403,汇成股份,2022-08-18
-688408,中信博,2020-08-28
-688409,富创精密,2022-10-10
-688410,山外山,2022-12-26
-688416,恒烁股份,2022-08-29
-688418,震有科技,2020-07-22
-688419,耐科装备,2022-11-07
-688420,美腾科技,2022-12-09
-688425,铁建重工,2021-06-22
-688426,康为世纪,2022-10-25
-688428,诺诚健华,2022-09-21
-688429,时创能源,2023-06-29
-688432,有研硅,2022-11-10
-688433,华曙高科,2023-04-17
-688435,英方软件,2023-01-19
-688439,振华风光,2022-08-26
-688443,智翔金泰,2023-06-20
-688448,磁谷科技,2022-09-21
-688450,光格科技,2023-07-24
-688455,科捷智能,2022-09-15
-688456,有研粉材,2021-03-17
-688458,美芯晟,2023-05-22
-688459,哈铁科技,2022-10-12
-688466,金科环境,2020-05-08
-688468,科美诊断,2021-04-09
-688469,中芯集成,2023-05-10
-688472,阿特斯,2023-06-09
-688475,萤石网络,2022-12-28
-688478,晶升股份,2023-04-24
-688479,友车科技,2023-05-11
-688480,赛恩斯,2022-11-25
-688484,南芯科技,2023-04-07
-688485,九州一轨,2023-01-18
-688486,龙迅股份,2023-02-21
-688488,艾迪药业,2020-07-20
-688489,三未信安,2022-12-02
-688496,清越科技,2022-12-28
-688498,源杰科技,2022-12-21
-688499,利元亨,2021-07-01
-688500,*ST慧辰,2020-07-16
-688501,青达环保,2021-07-16
-688502,茂莱光学,2023-03-09
-688503,聚和材料,2022-12-09
-688505,复旦张江,2020-06-19
-688506,百利天恒,2023-01-06
-688507,索辰科技,2023-04-18
-688508,芯朋微,2020-07-22
-688509,正元地信,2021-07-30
-688510,航亚科技,2020-12-16
-688511,天微电子,2021-07-30
-688512,慧智微,2023-05-16
-688513,苑东生物,2020-09-02
-688515,裕太微,2023-02-10
-688516,奥特维,2020-05-21
-688517,金冠电气,2021-06-18
-688518,联赢激光,2020-06-22
-688519,南亚新材,2020-08-18
-688520,神州细胞,2020-06-22
-688521,芯原股份,2020-08-18
-688522,纳睿雷达,2023-03-01
-688523,航天环宇,2023-06-02
-688525,佰维存储,2022-12-30
-688526,科前生物,2020-09-22
-688528,秦川物联,2020-07-01
-688529,豪森股份,2020-11-09
-688531,日联科技,2023-03-31
-688533,上声电子,2021-04-19
-688535,华海诚科,2023-04-04
-688536,思瑞浦,2020-09-21
-688538,和辉光电,2021-05-28
-688539,高华科技,2023-04-18
-688543,国科军工,2023-06-21
-688548,广钢气体,2023-08-15
-688549,中巨芯,2023-09-08
-688550,瑞联新材,2020-09-02
-688551,科威尔,2020-09-10
-688552,航天南湖,2023-05-18
-688553,汇宇制药,2021-10-26
-688556,高测股份,2020-08-07
-688557,兰剑智能,2020-12-02
-688558,国盛智科,2020-06-30
-688559,海目星,2020-09-09
-688560,明冠新材,2020-12-24
-688561,奇安信,2020-07-22
-688562,航天软件,2023-05-24
-688563,航材股份,2023-07-19
-688565,力源科技,2021-05-13
-688566,吉贝尔,2020-05-18
-688567,孚能科技,2020-07-17
-688568,中科星图,2020-07-08
-688569,铁科轨道,2020-08-31
-688570,天玛智控,2023-06-05
-688571,杭华股份,2020-12-11
-688573,信宇人,2023-08-17
-688575,亚辉龙,2021-05-17
-688576,西山科技,2023-06-06
-688577,浙海德曼,2020-09-16
-688578,艾力斯,2020-12-02
-688579,山大地纬,2020-07-17
-688580,伟思医疗,2020-07-21
-688581,安杰思,2023-05-19
-688582,芯动联科,2023-06-30
-688585,上纬新材,2020-09-28
-688586,江航装备,2020-07-31
-688588,凌志软件,2020-05-11
-688589,力合微,2020-07-22
-688590,新致软件,2020-12-07
-688591,泰凌微,2023-08-25
-688592,司南导航,2023-08-16
-688593,新相微,2023-06-01
-688595,芯海科技,2020-09-28
-688596,正帆科技,2020-08-20
-688597,煜邦电力,2021-06-17
-688598,金博股份,2020-05-18
-688599,天合光能,2020-06-10
-688600,皖仪科技,2020-07-03
-688601,力芯微,2021-06-28
-688602,康鹏科技,2023-07-20
-688603,天承科技,2023-07-10
-688606,奥泰生物,2021-03-25
-688607,康众医疗,2021-02-01
-688608,恒玄科技,2020-12-16
-688609,九联科技,2021-03-23
-688610,埃科光电,2023-07-19
-688611,杭州柯林,2021-04-12
-688612,威迈斯,2023-07-26
-688613,奥精医疗,2021-05-21
-688616,西力科技,2021-03-18
-688617,惠泰医疗,2021-01-07
-688618,三旺通信,2020-12-30
-688619,罗普特,2021-02-23
-688620,安凯微,2023-06-27
-688621,阳光诺和,2021-06-21
-688622,禾信仪器,2021-09-13
-688623,双元科技,2023-06-08
-688625,呈和科技,2021-06-07
-688626,翔宇医疗,2021-03-31
-688627,精智达,2023-07-18
-688628,优利德,2021-02-01
-688629,华丰科技,2023-06-27
-688630,芯碁微装,2021-04-01
-688631,莱斯信息,2023-06-28
-688633,星球石墨,2021-03-24
-688636,智明达,2021-04-08
-688638,誉辰智能,2023-07-12
-688639,华恒生物,2021-04-22
-688646,逸飞激光,2023-07-28
-688651,盛邦安全,2023-07-26
-688655,迅捷兴,2021-05-11
-688656,浩欧博,2021-01-13
-688657,浩辰软件,2023-10-10
-688658,悦康药业,2020-12-24
-688659,元琛科技,2021-03-31
-688660,电气风电,2021-05-19
-688661,和林微纳,2021-03-29
-688662,富信科技,2021-04-01
-688663,新风光,2021-04-13
-688665,四方光电,2021-02-09
-688667,菱电电控,2021-03-12
-688668,鼎通科技,2020-12-21
-688669,聚石化学,2021-01-25
-688670,金迪克,2021-08-02
-688671,碧兴物联,2023-08-09
-688676,金盘科技,2021-03-09
-688677,海泰新光,2021-02-26
-688678,福立旺,2020-12-23
-688679,通源环境,2020-12-25
-688680,海优新材,2021-01-22
-688681,科汇股份,2021-06-16
-688682,霍莱沃,2021-04-20
-688683,莱尔科技,2021-04-12
-688685,迈信林,2021-05-13
-688686,奥普特,2020-12-31
-688687,凯因科技,2021-02-08
-688689,银河微电,2021-01-27
-688690,纳微科技,2021-06-23
-688693,锴威特,2023-08-18
-688696,极米科技,2021-03-03
-688697,纽威数控,2021-09-17
-688698,伟创电气,2020-12-29
-688699,明微电子,2020-12-18
-688700,东威科技,2021-06-15
-688701,卓锦股份,2021-09-16
-688702,盛科通信,2023-09-14
-688707,振华新材,2021-09-14
-688711,宏微科技,2021-09-01
-688716,中研股份,2023-09-20
-688718,唯赛勃,2021-07-28
-688719,爱科赛博,2023-09-28
-688722,同益中,2021-10-19
-688728,格科微,2021-08-18
-688733,壹石通,2021-08-17
-688737,中自科技,2021-10-22
-688739,成大生物,2021-10-28
-688766,普冉股份,2021-08-23
-688767,博拓生物,2021-09-08
-688768,容知日新,2021-07-26
-688772,珠海冠宇,2021-10-15
-688776,国光电气,2021-08-31
-688777,中控技术,2020-11-24
-688778,厦钨新能,2021-08-05
-688779,长远锂科,2021-08-11
-688786,悦安新材,2021-08-26
-688787,海天瑞声,2021-08-13
-688788,科思科技,2020-10-22
-688789,宏华数科,2021-07-08
-688793,倍轻松,2021-07-15
-688798,艾为电子,2021-08-16
-688799,华纳药厂,2021-07-13
-688800,瑞可达,2021-07-22
-688819,天能股份,2021-01-18
-688981,中芯国际,2020-07-16
-689009,九号公司,2020-10-29
-830779,武汉蓝电,2023-06-01
-830799,艾融软件,2020-07-27
-830809,安达科技,2023-03-23
-830832,齐鲁华信,2021-02-23
-830839,万通液压,2020-11-09
-830879,基康仪器,2022-12-20
-830896,旺成科技,2023-04-19
-830946,森萱医药,2020-07-27
-830964,润农节水,2020-07-27
-830974,凯大催化,2023-03-08
-831010,凯添燃气,2020-07-27
-831039,国义招标,2021-08-18
-831087,秋乐种业,2022-12-07
-831152,昆工科技,2022-09-01
-831167,鑫汇科,2022-05-27
-831195,三祥科技,2022-12-30
-831278,泰德股份,2022-06-20
-831304,迪尔化工,2023-04-18
-831305,海希通讯,2021-11-05
-831370,新安洁,2020-07-27
-831445,龙竹科技,2020-07-27
-831526,凯华材料,2022-12-22
-831627,力王股份,2023-09-07
-831641,格利尔,2022-12-02
-831689,克莱特,2022-03-21
-831726,朱老六,2021-05-27
-831768,拾比佰,2021-06-28
-831832,科达自控,2021-11-15
-831834,三维股份,2022-08-22
-831855,浙江大农,2022-12-29
-831856,浩淼科技,2020-12-25
-831906,舜宇精工,2023-02-22
-831961,创远信科,2020-07-27
-832000,安徽凤凰,2020-12-23
-832023,田野股份,2023-02-02
-832089,禾昌聚合,2021-11-09
-832110,雷特科技,2022-12-06
-832145,恒合股份,2021-11-15
-832149,利尔达,2023-02-17
-832171,志晟信息,2021-11-15
-832175,东方碳素,2023-06-30
-832225,利通科技,2021-02-25
-832278,鹿得医疗,2020-07-27
-832317,观典防务,2020-07-27
-832419,路斯股份,2022-03-11
-832469,富恒新材,2023-09-18
-832471,美邦科技,2023-05-25
-832491,奥迪威,2022-06-14
-832566,梓橦宫,2021-08-13
-832651,天罡股份,2023-06-27
-832662,方盛股份,2022-11-28
-832735,德源药业,2021-02-19
-832786,骑士乳业,2023-10-13
-832802,保丽洁,2023-02-06
-832876,慧为智能,2022-11-09
-832885,星辰科技,2021-07-08
-832978,开特股份,2023-09-28
-832982,锦波生物,2023-07-20
-833075,柏星龙,2022-12-14
-833171,国航远洋,2022-12-15
-833230,欧康医药,2022-12-09
-833266,生物谷,2020-07-27
-833346,威贸电子,2022-02-23
-833394,民士达,2023-04-25
-833427,华维设计,2021-02-05
-833429,康比特,2022-12-15
-833454,同心传动,2021-11-15
-833455,汇隆活塞,2023-06-21
-833509,同惠电子,2021-01-11
-833523,德瑞锂电,2021-06-03
-833533,骏创科技,2022-05-24
-833575,康乐卫士,2023-03-15
-833580,科创新材,2022-05-13
-833751,惠同新材,2023-07-17
-833781,瑞奇智造,2022-12-26
-833819,颖泰生物,2020-07-27
-833873,中设咨询,2021-11-15
-833874,泰祥股份,2020-07-27
-833914,远航精密,2022-11-11
-833943,优机股份,2022-06-24
-833994,翰博高新,2020-07-27
-834014,特瑞斯,2022-12-13
-834021,流金科技,2020-07-27
-834033,康普化学,2022-12-21
-834058,华洋赛车,2023-08-10
-834062,科润智控,2022-07-13
-834261,一诺威,2023-04-03
-834407,驰诚股份,2023-02-16
-834415,恒拓开源,2020-07-27
-834475,三友科技,2020-07-27
-834599,同力股份,2021-02-22
-834639,晨光电缆,2022-07-12
-834682,球冠电缆,2020-07-27
-834765,美之高,2021-07-05
-834770,艾能聚,2023-02-28
-834950,迅安科技,2023-01-11
-835174,五新隧装,2021-08-20
-835179,凯德石英,2022-03-04
-835184,国源科技,2020-07-27
-835185,贝特瑞,2020-07-27
-835207,众诚科技,2022-09-23
-835237,力佳科技,2022-11-25
-835305,云创数据,2021-08-26
-835368,连城数控,2020-07-27
-835508,殷图网联,2020-07-27
-835640,富士达,2020-07-27
-835670,数字人,2020-12-08
-835857,百甲科技,2023-03-14
-835892,中科美菱,2022-10-18
-835985,海泰新能,2022-08-08
-836077,吉林碳谷,2021-08-31
-836149,旭杰科技,2020-07-27
-836208,青矩技术,2023-06-29
-836221,易实精密,2023-06-08
-836239,长虹能源,2021-02-09
-836247,华密新材,2022-12-23
-836260,中寰股份,2021-11-15
-836263,中航泰达,2020-07-27
-836270,天铭科技,2022-09-02
-836395,朗鸿科技,2022-09-01
-836414,欧普泰,2022-12-12
-836419,万德股份,2023-09-15
-836422,润普食品,2023-03-01
-836433,大唐药业,2020-07-27
-836504,博迅生物,2023-08-17
-836675,秉扬科技,2020-12-28
-836699,海达尔,2023-05-09
-836717,瑞星股份,2023-07-03
-836720,吉冈精密,2021-11-24
-836807,奔朗新材,2022-12-20
-836826,盖世食品,2021-01-12
-836871,派特尔,2022-07-22
-836892,广咨国际,2021-10-28
-836942,恒立钻具,2022-12-08
-836957,汉维科技,2022-12-14
-837006,晟楠科技,2023-05-18
-837046,亿能电力,2022-10-13
-837092,汉鑫科技,2021-11-15
-837174,宏裕包材,2023-08-18
-837212,智新电子,2021-06-08
-837242,建邦科技,2020-07-27
-837344,三元基因,2021-01-08
-837592,华信永道,2023-07-10
-837663,明阳科技,2023-03-15
-837748,路桥信息,2023-08-16
-837821,则成电子,2022-07-06
-838030,德众汽车,2020-11-27
-838163,方大新材,2020-07-27
-838171,邦德股份,2022-06-02
-838227,美登科技,2022-12-28
-838262,太湖雪,2022-12-30
-838275,驱动力,2021-01-25
-838402,硅烷科技,2022-09-28
-838670,恒进感应,2022-07-05
-838701,豪声电子,2023-07-19
-838810,春光药装,2022-12-16
-838837,华原股份,2023-05-15
-838924,广脉科技,2021-11-03
-838971,天马新材,2022-09-27
-839167,同享科技,2020-07-27
-839273,一致魔芋,2023-02-21
-839371,欧福蛋业,2023-01-18
-839680,广道数字,2021-11-15
-839719,宁新新材,2023-05-26
-839725,惠丰钻石,2022-07-18
-839729,永顺生物,2020-07-27
-839790,联迪信息,2022-09-02
-839792,东和新材,2023-03-30
-839946,华阳变速,2021-07-20
-870199,倍益康,2022-12-01
-870204,沪江材料,2022-01-18
-870299,灿能电力,2022-06-10
-870357,雅葆轩,2022-11-18
-870436,大地电气,2021-11-15
-870508,丰安股份,2022-12-16
-870726,鸿智科技,2023-08-08
-870866,绿亨科技,2022-12-09
-870976,视声智能,2023-09-01
-871245,威博液压,2022-01-06
-871396,常辅股份,2020-11-18
-871478,巨能股份,2023-05-12
-871553,凯腾精工,2021-08-06
-871634,新威凌,2022-11-24
-871642,通易航天,2021-08-16
-871694,中裕科技,2023-04-24
-871753,天纺标,2022-10-31
-871857,泓禧科技,2022-02-28
-871970,大禹生物,2022-05-18
-871981,晶赛科技,2021-11-15
-872190,雷神科技,2022-12-23
-872351,华光源海,2022-12-29
-872374,云里物里,2022-11-29
-872392,佳合科技,2022-12-30
-872541,铁大科技,2023-03-10
-872808,曙光数创,2022-11-18
-872895,花溪科技,2023-04-06
-872925,锦好医疗,2021-10-25
-872953,国子软件,2023-08-23
-873001,纬达光电,2022-12-27
-873122,中纺标,2022-09-27
-873152,天宏锂电,2023-01-19
-873167,新赣江,2023-02-09
-873169,七丰精工,2022-04-15
-873223,荣亿精密,2022-06-09
-873305,九菱科技,2022-12-21
-873339,恒太照明,2022-11-17
-873527,夜光明,2022-10-27
-873576,天力复合,2023-07-12
-873593,鼎智科技,2023-04-13
-873665,科强股份,2023-09-26
-873726,卓兆点胶,2023-10-19
-900901,云赛Ｂ股,1992-02-21
-900902,市北B股 ,1992-07-01
-900903,大众Ｂ股,1992-07-22
-900904,神奇B股 ,1992-07-22
-900905,老凤祥Ｂ,1992-07-28
-900906,中毅达B ,1992-07-28
-900907,退市鹏B,
-900908,氯碱Ｂ股,1992-08-20
-900909,华谊B股 ,1992-08-28
-900910,海立Ｂ股,1993-01-18
-900911,金桥Ｂ股,1993-05-31
-900912,外高Ｂ股,1993-07-26
-900913,国新B股 ,1993-09-28
-900914,锦在线B ,1993-10-18
-900915,中路Ｂ股,1993-11-15
-900916,凤凰B股 ,1993-11-19
-900917,海欣Ｂ股,1993-12-08
-900918,耀皮Ｂ股,1993-12-10
-900919,退市庭B,
-900920,动力Ｂ股,1993-12-28
-900921,丹科B股 ,1993-12-28
-900922,三毛B股 ,1993-12-31
-900923,百联Ｂ股,1994-01-05
-900924,上工Ｂ股,1994-01-18
-900925,机电Ｂ股,1994-01-31
-900926,宝信Ｂ  ,1994-03-15
-900927,物贸Ｂ股,1994-03-30
-900928,临港B股 ,1994-04-29
-900929,锦旅Ｂ股,1994-09-28
-900930,*ST沪普B,
-900931,PT水仙B,
-900932,陆家Ｂ股,1994-11-22
-900933,华新B股,
-900934,锦江Ｂ股,1994-12-15
-900935,阳晨B股,
-900936,鄂资Ｂ股,1995-10-20
-900937,华电B股 ,1996-04-22
-900938,海科B   ,1996-04-30
-900939,汇丽B   ,1996-06-28
-900940,大名城B ,1996-07-26
-900941,东信Ｂ股,1996-08-09
-900942,黄山Ｂ股,1996-11-22
-900943,开开Ｂ股,1997-01-08
-900945,海控B股 ,1997-06-26
-900946,天雁B股 ,1997-06-17
-900947,振华Ｂ股,1997-08-05
-900948,伊泰Ｂ股,1997-08-08
-900949,东电B股,
-900950,新城B股,
-900951,退市大化,
-900952,锦港Ｂ股,1998-05-19
-900953,凯马Ｂ  ,1998-06-24
-900955,退市海B,
-900956,东贝B股,
-900957,凌云Ｂ股,2000-07-28
+stock_code,short_name,list_date2
+000001,平安银行,1991-04-03
+000002,万  科Ａ,1991-01-29
+000003,PT金田A,
+000004,国华网安,1990-12-01
+000005,ST星源,1990-12-10
+000006,深振业Ａ,1992-04-27
+000007,*ST全新,1992-04-13
+000008,神州高铁,1992-05-07
+000009,中国宝安,1991-06-25
+000010,美丽生态,1995-10-27
+000011,深物业A,1992-03-30
+000012,南  玻Ａ,1992-02-28
+000013,*ST石化A,
+000014,沙河股份,1992-06-02
+000015,PT中浩A,
+000016,深康佳Ａ,1992-03-27
+000017,深中华A,1992-03-31
+000018,神城A退,
+000019,深粮控股,1992-10-12
+000020,深华发Ａ,1992-04-28
+000021,深科技,1994-02-02
+000023,ST深天,1993-04-29
+000024,招商地产,
+000025,特  力Ａ,1993-06-21
+000026,飞亚达,1993-06-03
+000027,深圳能源,1993-09-03
+000028,国药一致,1993-08-09
+000029,深深房Ａ,1993-09-15
+000030,富奥股份,1993-09-29
+000031,大悦城,1993-10-08
+000032,深桑达Ａ,1993-10-28
+000033,新都退,
+000034,神州数码,1994-05-09
+000035,中国天楹,1994-04-08
+000036,华联控股,1994-06-17
+000037,深南电A,1994-07-01
+000038,大通退,
+000039,中集集团,1994-04-08
+000040,东旭蓝天,1994-08-08
+000042,中洲控股,1994-09-21
+000045,深纺织Ａ,1994-08-15
+000046,*ST泛海,1994-09-12
+000047,ST中侨,
+000048,京基智农,1994-11-01
+000049,德赛电池,1995-03-20
+000050,深天马Ａ,1995-03-15
+000055,方大集团,1996-04-15
+000056,皇庭国际,1996-07-08
+000058,深 赛 格,1996-12-26
+000059,华锦股份,1997-01-30
+000060,中金岭南,1997-01-23
+000061,农 产 品,1997-01-10
+000062,深圳华强,1997-01-30
+000063,中兴通讯,1997-11-18
+000065,北方国际,1998-06-05
+000066,中国长城,1997-06-26
+000068,华控赛格,1997-06-11
+000069,华侨城Ａ,1997-09-10
+000070,特发信息,2000-05-11
+000078,海王生物,1998-12-18
+000088,盐 田 港,1997-07-28
+000089,深圳机场,1998-04-20
+000090,天健集团,1999-07-21
+000096,广聚能源,2000-07-24
+000099,中信海直,2000-07-31
+000100,TCL科技,2004-01-30
+000150,*ST宜康,
+000151,中成股份,2000-09-06
+000153,丰原药业,2000-09-20
+000155,川能动力,2000-09-26
+000156,华数传媒,2000-09-06
+000157,中联重科,2000-10-12
+000158,常山北明,2000-07-24
+000159,国际实业,2000-09-26
+000166,申万宏源,2015-01-26
+000301,东方盛虹,2000-05-29
+000333,美的集团,2013-09-18
+000338,潍柴动力,2007-04-30
+000400,许继电气,1997-04-18
+000401,冀东水泥,1996-06-14
+000402,金 融 街,1996-06-26
+000403,派林生物,1996-06-28
+000404,长虹华意,1996-06-19
+000405,ST鑫光,
+000406,石油大明,
+000407,胜利股份,1996-07-03
+000408,藏格矿业,1996-06-28
+000409,云鼎科技,1996-06-27
+000410,沈阳机床,1996-07-18
+000411,英特集团,1996-07-16
+000412,ST五环,
+000413,东旭光电,1996-09-25
+000415,渤海租赁,1996-07-16
+000416,*ST民控,1996-07-19
+000417,合肥百货,1996-08-12
+000418,小天鹅A,
+000419,通程控股,1996-08-16
+000420,吉林化纤,1996-08-02
+000421,南京公用,1996-08-06
+000422,湖北宜化,1996-08-15
+000423,东阿阿胶,1996-07-29
+000425,徐工机械,1996-08-28
+000426,兴业银锡,1996-08-28
+000428,华天酒店,1996-08-08
+000429,粤高速Ａ,1998-02-20
+000430,张家界,1996-08-29
+000488,晨鸣纸业,2000-11-20
+000498,山东路桥,1997-06-09
+000501,武商集团,1992-11-20
+000502,绿景退,
+000503,国新健康,1992-11-30
+000504,南华生物,1992-12-08
+000505,京粮控股,1992-12-21
+000506,中润资源,1993-03-12
+000507,珠海港,1993-03-26
+000508,琼民源A,
+000509,华塑控股,1993-05-07
+000510,新金路,1993-05-07
+000511,烯碳退,
+000513,丽珠集团,1993-10-28
+000514,渝 开 发,1993-07-12
+000515,攀渝钛业,
+000516,国际医学,1993-08-09
+000517,荣安地产,1993-08-06
+000518,四环生物,1993-09-08
+000519,中兵红箭,1993-10-08
+000520,凤凰航运,1993-10-25
+000521,长虹美菱,1993-10-18
+000522,白云山A,
+000523,广州浪奇,1993-11-08
+000524,岭南控股,1993-11-18
+000525,ST红太阳,1993-10-28
+000526,学大教育,1993-11-01
+000527,美的电器,
+000528,柳    工,1993-11-18
+000529,广弘控股,1993-11-18
+000530,冰山冷热,1993-12-08
+000531,穗恒运Ａ,1994-01-06
+000532,华金资本,1994-01-03
+000533,顺钠股份,1994-01-03
+000534,万泽股份,1994-01-10
+000535,*ST猴王,
+000536,华映科技,1993-11-26
+000537,广宇发展,1993-12-10
+000538,云南白药,1993-12-15
+000539,粤电力Ａ,1993-11-26
+000540,*ST中天,
+000541,佛山照明,1993-11-23
+000542,TCL通讯,
+000543,皖能电力,1993-12-20
+000544,中原环保,1993-12-08
+000545,金浦钛业,1993-12-15
+000546,ST金圆,1993-12-15
+000547,航天发展,1993-11-30
+000548,湖南投资,1993-12-20
+000549,S湘火炬,
+000550,江铃汽车,1993-12-01
+000551,创元科技,1994-01-06
+000552,甘肃能化,1994-01-06
+000553,安道麦A,1993-12-03
+000554,泰山石油,1993-12-15
+000555,神州信息,1994-04-08
+000556,PT南洋,
+000557,西部创业,1994-06-17
+000558,莱茵体育,1994-05-09
+000559,万向钱潮,1994-01-10
+000560,我爱我家,1994-02-02
+000561,烽火电子,1994-05-09
+000562,宏源证券,
+000563,陕国投Ａ,1994-01-10
+000564,ST大集,1994-01-10
+000565,渝三峡Ａ,1994-04-08
+000566,海南海药,1994-05-25
+000567,海德股份,1994-05-25
+000568,泸州老窖,1994-05-09
+000569,长城股份,
+000570,苏常柴Ａ,1994-07-01
+000571,新大洲A,1994-05-25
+000572,海马汽车,1994-08-08
+000573,粤宏远Ａ,1994-08-15
+000576,甘化科工,1994-09-07
+000578,盐湖集团,
+000581,威孚高科,1998-09-24
+000582,北部湾港,1995-11-02
+000583,S*ST托普,
+000584,ST工智,1995-11-28
+000585,东电退,
+000586,汇源通信,1995-12-20
+000587,*ST金洲,
+000588,PT粤金曼,
+000589,贵州轮胎,1996-03-08
+000590,启迪药业,1996-01-19
+000591,太阳能,1996-02-08
+000592,平潭发展,1996-03-27
+000593,德龙汇能,1996-03-12
+000594,国恒退,
+000595,宝塔实业,1996-04-19
+000596,古井贡酒,1996-09-27
+000597,东北制药,1996-05-23
+000598,兴蓉环境,1996-05-29
+000599,青岛双星,1996-04-30
+000600,建投能源,1996-06-06
+000601,韶能股份,1996-08-30
+000602,金马集团,
+000603,盛达资源,1996-08-23
+000605,渤海股份,1996-09-13
+000606,顺利退,
+000607,华媒控股,1996-08-30
+000608,阳光股份,1996-09-19
+000609,中迪投资,1996-10-10
+000610,西安旅游,1996-09-26
+000611,天首退,
+000612,焦作万方,1996-09-26
+000613,东海A退,
+000615,*ST美谷,1996-10-16
+000616,*ST海投,
+000617,中油资本,1996-10-22
+000618,吉林化工,
+000619,海螺新材,1996-10-23
+000620,*ST新联,1996-10-29
+000621,*ST比特,
+000622,恒立实业,1996-11-07
+000623,吉林敖东,1996-10-28
+000625,长安汽车,1997-06-10
+000626,远大控股,1996-11-28
+000627,天茂集团,1996-11-12
+000628,高新发展,1996-11-18
+000629,钒钛股份,1996-11-15
+000630,铜陵有色,1996-11-20
+000631,顺发恒业,1996-11-22
+000632,三木集团,1996-11-21
+000633,合金投资,1996-11-12
+000635,英 力 特,1996-11-20
+000636,风华高科,1996-11-29
+000637,ST实华,1996-11-14
+000638,万方发展,1996-11-26
+000639,西王食品,1996-11-26
+000650,仁和药业,1996-12-10
+000651,格力电器,1996-11-18
+000652,泰达股份,1996-11-28
+000653,ST九州,
+000655,金岭矿业,1996-11-28
+000656,金科股份,1996-11-28
+000657,中钨高新,1996-12-05
+000658,ST海洋,
+000659,珠海中富,1996-12-03
+000660,*ST南华,
+000661,长春高新,1996-12-18
+000662,天夏退,
+000663,永安林业,1996-12-06
+000665,湖北广电,1996-12-10
+000666,经纬纺机,1996-12-10
+000667,ST美置,
+000668,荣丰控股,1996-12-10
+000669,ST金鸿,1996-12-10
+000670,盈方微,1996-12-17
+000671,ST阳光城,
+000672,上峰水泥,1996-12-18
+000673,当代退,
+000675,ST银山,
+000676,智度股份,1996-12-24
+000677,恒天海龙,1996-12-26
+000678,襄阳轴承,1997-01-06
+000679,大连友谊,1997-01-24
+000680,山推股份,1997-01-22
+000681,视觉中国,1997-01-21
+000682,东方电子,1997-01-21
+000683,远兴能源,1997-01-31
+000685,中山公用,1997-01-23
+000686,东北证券,1997-02-27
+000687,华讯退,
+000688,国城矿业,1997-01-20
+000689,ST宏业,
+000690,宝新能源,1997-01-28
+000691,亚太实业,1997-02-28
+000692,*ST惠天,1997-02-27
+000693,华泽退,
+000695,滨海能源,1997-02-18
+000697,*ST炼石,1997-03-25
+000698,沈阳化工,1997-02-20
+000699,S*ST佳纸,
+000700,模塑科技,1997-02-28
+000701,厦门信达,1997-02-26
+000702,正虹科技,1997-03-18
+000703,恒逸石化,1997-03-28
+000705,浙江震元,1997-04-10
+000707,双环科技,1997-04-15
+000708,中信特钢,1997-03-26
+000709,河钢股份,1997-04-16
+000710,贝瑞基因,1997-04-22
+000711,*ST京蓝,1997-04-11
+000712,锦龙股份,1997-04-15
+000713,丰乐种业,1997-04-22
+000715,中兴商业,1997-05-08
+000716,黑芝麻,1997-04-18
+000717,中南股份,1997-05-08
+000718,苏宁环球,1997-04-08
+000719,中原传媒,1997-03-31
+000720,新能泰山,1997-05-09
+000721,西安饮食,1997-04-30
+000722,湖南发展,1997-05-22
+000723,美锦能源,1997-05-15
+000725,京东方Ａ,2001-01-12
+000726,鲁  泰Ａ,2000-12-25
+000727,冠捷科技,1997-05-20
+000728,国元证券,1997-06-16
+000729,燕京啤酒,1997-07-16
+000730,*ST环保,
+000731,四川美丰,1997-06-17
+000732,ST泰禾,
+000733,振华科技,1997-07-03
+000735,罗 牛 山,1997-06-11
+000736,中交地产,1997-04-25
+000737,北方铜业,1997-04-28
+000738,航发控制,1997-06-26
+000739,普洛药业,1997-05-09
+000748,长城信息,
+000750,国海证券,1997-07-09
+000751,锌业股份,1997-06-26
+000752,*ST西发,1997-06-25
+000753,漳州发展,1997-06-26
+000755,山西路桥,1997-06-27
+000756,新华制药,1997-08-06
+000757,浩物股份,1997-06-27
+000758,中色股份,1997-04-16
+000759,中百集团,1997-05-19
+000760,斯太退,
+000761,本钢板材,1998-01-15
+000762,西藏矿业,1997-07-08
+000763,锦州石化,
+000765,*ST华信,
+000766,通化金马,1997-04-30
+000767,晋控电力,1997-06-09
+000768,中航西飞,1997-06-26
+000769,*ST大菲,
+000776,广发证券,1997-06-11
+000777,中核科技,1997-07-10
+000778,新兴铸管,1997-06-06
+000779,甘咨询,1997-05-28
+000780,ST平能,
+000782,美达股份,1997-06-19
+000783,长江证券,1997-07-31
+000785,居然之家,1997-07-11
+000786,北新建材,1997-06-06
+000787,*ST创智,
+000788,北大医药,1997-06-16
+000789,万年青,1997-09-23
+000790,华神科技,1998-03-27
+000791,甘肃能源,1997-10-14
+000792,盐湖股份,1997-09-04
+000793,华闻集团,1997-07-29
+000795,英洛华,1997-08-08
+000796,*ST凯撒,1997-07-03
+000797,中国武夷,1997-07-15
+000798,中水渔业,1998-02-12
+000799,酒鬼酒,1997-07-18
+000800,一汽解放,1997-06-18
+000801,四川九洲,1998-05-06
+000802,北京文化,1998-01-08
+000803,山高环能,1998-03-03
+000805,*ST炎黄,
+000806,银河退,
+000807,云铝股份,1998-04-08
+000809,铁岭新城,1998-06-16
+000810,创维数字,1998-06-02
+000811,冰轮环境,1998-05-28
+000812,陕西金叶,1998-06-23
+000813,德展健康,1998-05-19
+000815,美利云,1998-06-09
+000816,智慧农业,1997-08-18
+000817,辽河油田,
+000818,航锦科技,1997-10-17
+000819,岳阳兴长,1997-06-25
+000820,神雾节能,1998-06-30
+000821,京山轻机,1998-06-26
+000822,山东海化,1998-07-03
+000823,超声电子,1997-10-08
+000825,太钢不锈,1998-10-21
+000826,启迪环境,1998-02-25
+000827,*ST长兴,
+000828,东莞控股,1997-06-17
+000829,天音控股,1997-12-02
+000830,鲁西化工,1998-08-07
+000831,中国稀土,1998-09-11
+000832,*ST龙涤,
+000833,粤桂股份,1998-11-11
+000835,长动退,
+000836,富通信息,1997-09-29
+000837,秦川机床,1998-09-28
+000838,财信发展,1997-06-26
+000839,ST国安,1997-10-31
+000848,承德露露,1997-11-13
+000850,华茂股份,1998-10-07
+000851,高鸿股份,1998-06-09
+000852,石化机械,1998-11-26
+000856,冀东装备,1998-08-13
+000858,五 粮 液,1998-04-27
+000859,国风新材,1998-11-19
+000860,顺鑫农业,1998-11-04
+000861,海印股份,1998-10-28
+000862,银星能源,1998-09-15
+000863,三湘印象,1997-09-25
+000866,扬子石化,
+000868,安凯客车,1997-07-25
+000869,张  裕Ａ,2000-10-26
+000875,吉电股份,2002-09-26
+000876,新 希 望,1998-03-11
+000877,天山股份,1999-01-07
+000878,云南铜业,1998-06-02
+000880,潍柴重机,1998-04-02
+000881,中广核技,1998-09-02
+000882,华联股份,1998-06-16
+000883,湖北能源,1998-05-19
+000885,城发环境,1999-03-19
+000886,海南高速,1998-01-23
+000887,中鼎股份,1998-12-03
+000888,峨眉山Ａ,1997-10-21
+000889,ST中嘉,1997-12-18
+000890,法尔胜,1999-01-19
+000892,欢瑞世纪,1999-01-15
+000893,亚钾国际,1998-12-24
+000895,双汇发展,1998-12-10
+000897,津滨发展,1999-04-22
+000898,鞍钢股份,1997-12-25
+000899,赣能股份,1997-11-26
+000900,现代投资,1999-01-28
+000901,航天科技,1999-04-01
+000902,新洋丰,1999-04-08
+000903,云内动力,1999-04-15
+000905,厦门港务,1999-04-29
+000906,浙商中拓,1999-07-07
+000908,景峰医药,1999-02-03
+000909,ST数源,1999-05-07
+000910,大亚圣象,1999-06-30
+000911,南宁糖业,1999-05-27
+000912,泸天化,1999-06-03
+000913,钱江摩托,1999-05-14
+000915,华特达因,1999-06-09
+000916,华北高速,
+000917,电广传媒,1999-03-25
+000918,*ST嘉凯,
+000919,金陵药业,1999-11-18
+000920,沃顿科技,1999-06-16
+000921,海信家电,1999-07-13
+000922,佳电股份,1999-06-18
+000923,河钢资源,1999-07-14
+000925,众合科技,1999-06-11
+000926,福星股份,1999-06-18
+000927,中国铁物,1999-07-27
+000928,中钢国际,1999-03-12
+000929,兰州黄河,1999-06-23
+000930,中粮科技,1999-07-12
+000931,中 关 村,1999-07-12
+000932,华菱钢铁,1999-08-03
+000933,神火股份,1999-08-31
+000935,四川双马,1999-08-24
+000936,华西股份,1999-08-10
+000937,冀中能源,1999-09-09
+000938,紫光股份,1999-11-04
+000939,凯迪退,
+000948,南天信息,1999-10-14
+000949,新乡化纤,1999-10-21
+000950,重药控股,1999-09-16
+000951,中国重汽,1999-11-25
+000952,广济药业,1999-11-12
+000953,河化股份,1999-12-02
+000955,欣龙控股,1999-12-09
+000956,中原油气,
+000957,中通客车,2000-01-13
+000958,电投产融,1999-12-23
+000959,首钢股份,1999-12-16
+000960,锡业股份,2000-02-21
+000961,中南建设,2000-03-01
+000962,东方钽业,2000-01-20
+000963,华东医药,2000-01-27
+000965,天保基建,2000-04-06
+000966,长源电力,2000-03-16
+000967,盈峰环境,2000-03-30
+000968,蓝焰控股,2000-06-22
+000969,安泰科技,2000-05-29
+000970,中科三环,2000-04-20
+000971,ST高升,2000-04-27
+000972,中基健康,2000-09-26
+000973,佛塑科技,2000-05-25
+000975,银泰黄金,2000-06-08
+000976,ST华铁,2000-06-01
+000977,浪潮信息,2000-06-08
+000978,桂林旅游,2000-05-18
+000979,中弘退,
+000980,众泰汽车,2000-06-16
+000981,山子股份,2000-06-22
+000982,中银绒业,2000-07-06
+000983,山西焦煤,2000-07-26
+000985,大庆华科,2000-07-26
+000987,越秀资本,2000-07-18
+000988,华工科技,2000-06-08
+000989,九 芝 堂,2000-06-28
+000990,诚志股份,2000-07-06
+000993,闽东电力,2000-07-31
+000995,皇台酒业,2000-08-07
+000996,*ST中期,2000-07-18
+000997,新 大 陆,2000-08-07
+000998,隆平高科,2000-12-11
+000999,华润三九,2000-03-09
+001201,东瑞股份,2021-04-28
+001202,炬申股份,2021-04-29
+001203,大中矿业,2021-05-10
+001205,盛航股份,2021-05-13
+001206,依依股份,2021-05-18
+001207,联科科技,2021-06-23
+001208,华菱线缆,2021-06-24
+001209,洪兴股份,2021-07-23
+001210,金房能源,2021-07-29
+001211,双枪科技,2021-08-05
+001212,中旗新材,2021-08-23
+001213,中铁特货,2021-09-08
+001215,千味央厨,2021-09-06
+001216,华瓷股份,2021-10-19
+001217,华尔泰,2021-09-29
+001218,丽臣实业,2021-10-15
+001219,青岛食品,2021-10-21
+001222,源飞宠物,2022-08-18
+001223,欧克科技,2022-12-12
+001225,和泰机电,2023-02-22
+001226,拓山重工,2022-06-22
+001227,兰州银行,2022-01-17
+001228,永泰运,2022-04-29
+001229,魅视科技,2022-08-08
+001230,劲旅环境,2022-07-15
+001231,农心科技,2022-08-19
+001234,泰慕士,2022-01-11
+001236,弘业期货,2022-08-05
+001238,浙江正特,2022-09-19
+001255,博菲电气,2022-09-30
+001256,炜冈科技,2022-12-05
+001258,立新能源,2022-07-27
+001259,利仁科技,2022-08-31
+001260,坤泰股份,2023-02-16
+001266,宏英智能,2022-02-28
+001267,汇绿生态,2021-11-17
+001268,联合精密,2022-06-30
+001269,欧晶科技,2022-09-30
+001270,铖昌科技,2022-06-06
+001278,一彬科技,2023-03-08
+001282,三联锻造,2023-05-24
+001283,豪鹏科技,2022-09-05
+001286,陕西能源,2023-04-10
+001287,中电港,2023-04-10
+001288,运机集团,2021-11-01
+001289,龙源电力,2022-01-24
+001296,长江材料,2021-12-24
+001298,好上好,2022-10-31
+001299,美能能源,2022-10-31
+001300,三柏硕,2022-10-19
+001301,尚太科技,2022-12-28
+001308,康冠科技,2022-03-18
+001309,德明利,2022-07-01
+001311,多利科技,2023-02-27
+001313,粤海饲料,2022-02-16
+001314,亿道信息,2023-02-14
+001316,润贝航科,2022-06-24
+001317,三羊马,2021-11-30
+001318,阳光乳业,2022-05-20
+001319,铭科精技,2022-05-12
+001322,箭牌家居,2022-10-26
+001323,慕思股份,2022-06-23
+001324,长青科技,2023-05-22
+001328,登康口腔,2023-04-10
+001330,博纳影业,2022-08-18
+001331,胜通能源,2022-09-08
+001332,锡装股份,2022-09-20
+001333,光华股份,2022-12-08
+001336,楚环科技,2022-07-25
+001337,四川黄金,2023-03-03
+001338,永顺泰,2022-11-16
+001339,智微智能,2022-08-15
+001360,南矿集团,2023-04-10
+001366,播恩集团,2023-03-07
+001367,海森药业,2023-04-10
+001368,通达创智,2023-03-13
+001373,翔腾新材,2023-06-01
+001380,华纬科技,2023-05-16
+001696,宗申动力,1997-03-06
+001872,招商港口,1993-05-05
+001896,豫能控股,1998-01-22
+001914,招商积余,1994-09-28
+001965,招商公路,2017-12-25
+001979,招商蛇口,2015-12-30
+002001,新 和 成,2004-06-25
+002002,ST鸿达,2004-06-25
+002003,伟星股份,2004-06-25
+002004,华邦健康,2004-06-25
+002005,ST德豪,2004-06-25
+002006,精工科技,2004-06-25
+002007,华兰生物,2004-06-25
+002008,大族激光,2004-06-25
+002009,天奇股份,2004-06-29
+002010,传化智联,2004-06-29
+002011,盾安环境,2004-07-05
+002012,凯恩股份,2004-07-05
+002013,中航机电,
+002014,永新股份,2004-07-08
+002015,协鑫能科,2004-07-08
+002016,世荣兆业,2004-07-08
+002017,东信和平,2004-07-13
+002018,华信退,
+002019,亿帆医药,2004-07-13
+002020,京新药业,2004-07-15
+002021,*ST中捷,2004-07-15
+002022,科华生物,2004-07-21
+002023,海特高新,2004-07-21
+002024,ST易购,2004-07-21
+002025,航天电器,2004-07-26
+002026,山东威达,2004-07-27
+002027,分众传媒,2004-08-04
+002028,思源电气,2004-08-05
+002029,七 匹 狼,2004-08-06
+002030,达安基因,2004-08-09
+002031,巨轮智能,2004-08-16
+002032,苏 泊 尔,2004-08-17
+002033,丽江股份,2004-08-25
+002034,旺能环境,2004-08-26
+002035,华帝股份,2004-09-01
+002036,联创电子,2004-09-03
+002037,保利联合,2004-09-08
+002038,双鹭药业,2004-09-09
+002039,黔源电力,2005-03-03
+002040,南 京 港,2005-03-25
+002041,登海种业,2005-04-18
+002042,华孚时尚,2005-04-27
+002043,兔 宝 宝,2005-05-10
+002044,美年健康,2005-05-18
+002045,国光电器,2005-05-23
+002046,国机精工,2005-05-26
+002047,宝鹰股份,2005-05-31
+002048,宁波华翔,2005-06-03
+002049,紫光国微,2005-06-06
+002050,三花智控,2005-06-07
+002051,中工国际,2006-06-19
+002052,ST同洲,2006-06-27
+002053,云南能投,2006-06-27
+002054,德美化工,2006-07-25
+002055,得润电子,2006-07-25
+002056,横店东磁,2006-08-02
+002057,中钢天源,2006-08-02
+002058,威尔泰,2006-08-02
+002059,云南旅游,2006-08-10
+002060,粤 水 电,2006-08-10
+002061,浙江交科,2006-08-16
+002062,宏润建设,2006-08-16
+002063,远光软件,2006-08-23
+002064,华峰化学,2006-08-23
+002065,东华软件,2006-08-23
+002066,瑞泰科技,2006-08-23
+002067,景兴纸业,2006-09-15
+002068,黑猫股份,2006-09-15
+002069,獐子岛,2006-09-28
+002070,众和退,
+002071,长城退,
+002072,凯瑞德,2006-10-18
+002073,软控股份,2006-10-18
+002074,国轩高科,2006-10-18
+002075,沙钢股份,2006-10-25
+002076,星光股份,2006-10-25
+002077,大港股份,2006-11-16
+002078,太阳纸业,2006-11-16
+002079,苏州固锝,2006-11-16
+002080,中材科技,2006-11-20
+002081,金 螳 螂,2006-11-20
+002082,万邦德,2006-11-20
+002083,孚日股份,2006-11-24
+002084,海鸥住工,2006-11-24
+002085,万丰奥威,2006-11-28
+002086,*ST东洋,2006-11-28
+002087,*ST新纺,2006-11-30
+002088,鲁阳节能,2006-11-30
+002089,*ST新海,2006-11-30
+002090,金智科技,2006-12-08
+002091,江苏国泰,2006-12-08
+002092,中泰化学,2006-12-08
+002093,国脉科技,2006-12-15
+002094,青岛金王,2006-12-15
+002095,生 意 宝,2006-12-15
+002096,易普力,2006-12-22
+002097,山河智能,2006-12-22
+002098,浔兴股份,2006-12-22
+002099,海翔药业,2006-12-26
+002100,天康生物,2006-12-26
+002101,广东鸿图,2006-12-29
+002102,冠福股份,2006-12-29
+002103,广博股份,2007-01-10
+002104,恒宝股份,2007-01-10
+002105,信隆健康,2007-01-12
+002106,莱宝高科,2007-01-12
+002107,沃华医药,2007-01-24
+002108,沧州明珠,2007-01-24
+002109,兴化股份,2007-01-26
+002110,三钢闽光,2007-01-26
+002111,威海广泰,2007-01-26
+002112,三变科技,2007-02-08
+002113,*ST天润,
+002114,罗平锌电,2007-02-15
+002115,三维通信,2007-02-15
+002116,中国海诚,2007-02-15
+002117,东港股份,2007-03-02
+002118,*ST紫鑫,
+002119,康强电子,2007-03-02
+002120,韵达股份,2007-03-06
+002121,科陆电子,2007-03-06
+002122,汇洲智能,2007-03-28
+002123,梦网科技,2007-03-28
+002124,天邦食品,2007-04-03
+002125,湘潭电化,2007-04-03
+002126,银轮股份,2007-04-18
+002127,南极电商,2007-04-18
+002128,电投能源,2007-04-18
+002129,TCL中环,2007-04-20
+002130,沃尔核材,2007-04-20
+002131,利欧股份,2007-04-27
+002132,恒星科技,2007-04-27
+002133,广宇集团,2007-04-27
+002134,天津普林,2007-05-16
+002135,东南网架,2007-05-30
+002136,安 纳 达,2007-05-30
+002137,实益达,2007-06-13
+002138,顺络电子,2007-06-13
+002139,拓邦股份,2007-06-29
+002140,东华科技,2007-07-12
+002141,贤丰控股,2007-07-20
+002142,宁波银行,2007-07-19
+002143,印纪退,
+002144,宏达高科,2007-08-03
+002145,中核钛白,2007-08-03
+002146,荣盛发展,2007-08-08
+002147,新光退,
+002148,北纬科技,2007-08-10
+002149,西部材料,2007-08-10
+002150,通润装备,2007-08-10
+002151,北斗星通,2007-08-13
+002152,广电运通,2007-08-13
+002153,石基信息,2007-08-13
+002154,报 喜 鸟,2007-08-16
+002155,湖南黄金,2007-08-16
+002156,通富微电,2007-08-16
+002157,*ST 正邦,2007-08-17
+002158,汉钟精机,2007-08-17
+002159,三特索道,2007-08-17
+002160,常铝股份,2007-08-21
+002161,远 望 谷,2007-08-21
+002162,悦心健康,2007-08-23
+002163,海南发展,2007-08-23
+002164,宁波东力,2007-08-23
+002165,红 宝 丽,2007-09-13
+002166,莱茵生物,2007-09-13
+002167,东方锆业,2007-09-13
+002168,惠程科技,2007-09-19
+002169,智光电气,2007-09-19
+002170,芭田股份,2007-09-19
+002171,楚江新材,2007-09-21
+002172,澳洋健康,2007-09-21
+002173,创新医疗,2007-09-25
+002174,游族网络,2007-09-25
+002175,东方智造,2007-10-12
+002176,江特电机,2007-10-12
+002177,御银股份,2007-11-01
+002178,延华智能,2007-11-01
+002179,中航光电,2007-11-01
+002180,纳思达,2007-11-13
+002181,粤 传 媒,2007-11-16
+002182,宝武镁业,2007-11-13
+002183,怡 亚 通,2007-11-13
+002184,海得控制,2007-11-16
+002185,华天科技,2007-11-20
+002186,全 聚 德,2007-11-20
+002187,广百股份,2007-11-22
+002188,中天服务,2007-11-22
+002189,中光学,2007-12-03
+002190,成飞集成,2007-12-03
+002191,劲嘉股份,2007-12-05
+002192,融捷股份,2007-12-05
+002193,如意集团,2007-12-07
+002194,武汉凡谷,2007-12-07
+002195,岩山科技,2007-12-12
+002196,方正电机,2007-12-12
+002197,证通电子,2007-12-18
+002198,嘉应制药,2007-12-18
+002199,东晶电子,2007-12-21
+002200,ST交投,2007-12-21
+002201,正威新材,2007-12-26
+002202,金风科技,2007-12-26
+002203,海亮股份,2008-01-16
+002204,大连重工,2008-01-16
+002205,国统股份,2008-01-23
+002206,海 利 得,2008-01-23
+002207,准油股份,2008-01-28
+002208,合肥城建,2008-01-28
+002209,达 意 隆,2008-01-30
+002210,飞马国际,2008-01-30
+002211,宏达新材,2008-02-01
+002212,天融信,2008-02-01
+002213,大为股份,2008-02-01
+002214,大立科技,2008-02-18
+002215,诺 普 信,2008-02-18
+002216,三全食品,2008-02-20
+002217,合力泰,2008-02-20
+002218,拓日新能,2008-02-28
+002219,新里程,2008-03-06
+002220,天宝退,
+002221,东华能源,2008-03-06
+002222,福晶科技,2008-03-19
+002223,鱼跃医疗,2008-04-18
+002224,三 力 士,2008-04-25
+002225,濮耐股份,2008-04-25
+002226,江南化工,2008-05-06
+002227,奥 特 迅,2008-05-06
+002228,合兴包装,2008-05-08
+002229,鸿博股份,2008-05-08
+002230,科大讯飞,2008-05-12
+002231,奥维通信,2008-05-12
+002232,启明信息,2008-05-09
+002233,塔牌集团,2008-05-16
+002234,民和股份,2008-05-16
+002235,安妮股份,2008-05-16
+002236,大华股份,2008-05-20
+002237,恒邦股份,2008-05-20
+002238,天威视讯,2008-05-26
+002239,奥特佳,2008-05-22
+002240,盛新锂能,2008-05-23
+002241,歌尔股份,2008-05-22
+002242,九阳股份,2008-05-28
+002243,力合科创,2008-05-28
+002244,滨江集团,2008-05-29
+002245,蔚蓝锂芯,2008-06-05
+002246,北化股份,2008-06-05
+002247,聚力文化,2008-06-12
+002248,华东数控,2008-06-12
+002249,大洋电机,2008-06-19
+002250,联化科技,2008-06-19
+002251,步 步 高,2008-06-19
+002252,上海莱士,2008-06-23
+002253,川大智胜,2008-06-23
+002254,泰和新材,2008-06-25
+002255,海陆重工,2008-06-25
+002256,兆新股份,2008-06-25
+002258,利尔化学,2008-07-08
+002259,ST升达,2008-07-16
+002260,德奥退,
+002261,拓维信息,2008-07-23
+002262,恩华药业,2008-07-23
+002263,大东南,2008-07-28
+002264,新 华 都,2008-07-31
+002265,建设工业,2008-08-06
+002266,浙富控股,2008-08-06
+002267,陕天然气,2008-08-13
+002268,电科网安,2008-08-11
+002269,美邦服饰,2008-08-28
+002270,华明装备,2008-09-05
+002271,东方雨虹,2008-09-10
+002272,川润股份,2008-09-19
+002273,水晶光电,2008-09-19
+002274,华昌化工,2008-09-25
+002275,桂林三金,2009-07-10
+002276,万马股份,2009-07-10
+002277,友阿股份,2009-07-17
+002278,神开股份,2009-08-11
+002279,久其软件,2009-08-11
+002280,联络互动,2009-08-21
+002281,光迅科技,2009-08-21
+002282,博深股份,2009-08-21
+002283,天润工业,2009-08-21
+002284,亚太股份,2009-08-28
+002285,世联行,2009-08-28
+002286,保龄宝,2009-08-28
+002287,奇正藏药,2009-08-28
+002288,超华科技,2009-09-03
+002289,ST宇顺,2009-09-03
+002290,禾盛新材,2009-09-03
+002291,遥望科技,2009-09-03
+002292,奥飞娱乐,2009-09-10
+002293,罗莱生活,2009-09-10
+002294,信立泰,2009-09-10
+002295,精艺股份,2009-09-29
+002296,辉煌科技,2009-09-29
+002297,博云新材,2009-09-29
+002298,中电兴发,2009-09-29
+002299,圣农发展,2009-10-21
+002300,太阳电缆,2009-10-21
+002301,齐心集团,2009-10-21
+002302,西部建设,2009-11-03
+002303,美盈森,2009-11-03
+002304,洋河股份,2009-11-06
+002305,南国置业,2009-11-06
+002306,中科云网,2009-11-11
+002307,北新路桥,2009-11-11
+002308,威创股份,2009-11-27
+002309,ST中利,2009-11-27
+002310,东方园林,2009-11-27
+002311,海大集团,2009-11-27
+002312,川发龙蟒,2009-12-03
+002313,*ST日海,2009-12-03
+002314,南山控股,2009-12-03
+002315,焦点科技,2009-12-09
+002316,亚联发展,2009-12-09
+002317,众生药业,2009-12-11
+002318,久立特材,2009-12-11
+002319,乐通股份,2009-12-11
+002320,海峡股份,2009-12-16
+002321,华英农业,2009-12-16
+002322,理工能科,2009-12-18
+002323,雅博股份,2009-12-18
+002324,普利特,2009-12-18
+002325,洪涛股份,2009-12-22
+002326,永太科技,2009-12-22
+002327,富安娜,2009-12-30
+002328,新朋股份,2009-12-30
+002329,皇氏集团,2010-01-06
+002330,得利斯,2010-01-06
+002331,皖通科技,2010-01-06
+002332,仙琚制药,2010-01-12
+002333,罗普斯金,2010-01-12
+002334,英威腾,2010-01-13
+002335,科华数据,2010-01-13
+002336,人人乐,2010-01-13
+002337,赛象科技,2010-01-15
+002338,奥普光电,2010-01-15
+002339,积成电子,2010-01-22
+002340,格林美,2010-01-22
+002341,新纶新材,2010-01-22
+002342,巨力索具,2010-01-26
+002343,慈文传媒,2010-01-26
+002344,海宁皮城,2010-01-26
+002345,潮宏基,2010-01-28
+002346,柘中股份,2010-01-28
+002347,泰尔股份,2010-01-28
+002348,高乐股份,2010-02-03
+002349,精华制药,2010-02-03
+002350,北京科锐,2010-02-03
+002351,漫步者,2010-02-05
+002352,顺丰控股,2010-02-05
+002353,杰瑞股份,2010-02-05
+002354,天娱数科,2010-02-09
+002355,兴民智通,2010-02-09
+002356,赫美集团,2010-02-09
+002357,富临运业,2010-02-10
+002358,森源电气,2010-02-10
+002359,北讯退,
+002360,同德化工,2010-03-03
+002361,神剑股份,2010-03-03
+002362,汉王科技,2010-03-03
+002363,隆基机械,2010-03-05
+002364,中恒电气,2010-03-05
+002365,永安药业,2010-03-05
+002366,融发核电,2010-03-12
+002367,康力电梯,2010-03-12
+002368,太极股份,2010-03-12
+002369,卓翼科技,2010-03-16
+002370,亚太药业,2010-03-16
+002371,北方华创,2010-03-16
+002372,伟星新材,2010-03-18
+002373,千方科技,2010-03-18
+002374,中锐股份,2010-03-18
+002375,亚厦股份,2010-03-23
+002376,新北洋,2010-03-23
+002377,国创高新,2010-03-23
+002378,章源钨业,2010-03-31
+002379,宏创控股,2010-03-31
+002380,科远智慧,2010-03-31
+002381,双箭股份,2010-04-02
+002382,蓝帆医疗,2010-04-02
+002383,合众思壮,2010-04-02
+002384,东山精密,2010-04-09
+002385,大北农,2010-04-09
+002386,天原股份,2010-04-09
+002387,维信诺,2010-04-13
+002388,新亚制程,2010-04-13
+002389,航天彩虹,2010-04-13
+002390,信邦制药,2010-04-16
+002391,长青股份,2010-04-16
+002392,北京利尔,2010-04-23
+002393,力生制药,2010-04-23
+002394,联发股份,2010-04-23
+002395,双象股份,2010-04-29
+002396,星网锐捷,2010-06-23
+002397,梦洁股份,2010-04-29
+002398,垒知集团,2010-05-06
+002399,海普瑞,2010-05-06
+002400,省广集团,2010-05-06
+002401,中远海科,2010-05-06
+002402,和而泰,2010-05-11
+002403,爱仕达,2010-05-11
+002404,嘉欣丝绸,2010-05-11
+002405,四维图新,2010-05-18
+002406,远东传动,2010-05-18
+002407,多氟多,2010-05-18
+002408,齐翔腾达,2010-05-18
+002409,雅克科技,2010-05-25
+002410,广联达,2010-05-25
+002411,必康退,
+002412,汉森制药,2010-05-25
+002413,雷科防务,2010-05-28
+002414,高德红外,2010-07-16
+002415,海康威视,2010-05-28
+002416,爱施德,2010-05-28
+002417,深南退,
+002418,康盛股份,2010-06-01
+002419,天虹股份,2010-06-01
+002420,毅昌科技,2010-06-01
+002421,达实智能,2010-06-03
+002422,科伦药业,2010-06-03
+002423,中粮资本,2010-06-03
+002424,贵州百灵,2010-06-03
+002425,凯撒文化,2010-06-08
+002426,胜利精密,2010-06-08
+002427,尤夫股份,2010-06-08
+002428,云南锗业,2010-06-08
+002429,兆驰股份,2010-06-10
+002430,杭氧股份,2010-06-10
+002431,棕榈股份,2010-06-10
+002432,九安医疗,2010-06-10
+002433,*ST太安,2010-06-18
+002434,万里扬,2010-06-18
+002435,长江健康,2010-06-18
+002436,兴森科技,2010-06-18
+002437,誉衡药业,2010-06-23
+002438,江苏神通,2010-06-23
+002439,启明星辰,2010-06-23
+002440,闰土股份,2010-07-06
+002441,众业达,2010-07-06
+002442,龙星化工,2010-07-06
+002443,金洲管道,2010-07-06
+002444,巨星科技,2010-07-13
+002445,中南文化,2010-07-13
+002446,盛路通信,2010-07-13
+002447,晨鑫退,
+002448,中原内配,2010-07-16
+002449,国星光电,2010-07-16
+002450,康得退,
+002451,摩恩电气,2010-07-20
+002452,长高电新,2010-07-20
+002453,华软科技,2010-07-20
+002454,松芝股份,2010-07-20
+002455,百川股份,2010-08-03
+002456,欧菲光,2010-08-03
+002457,青龙管业,2010-08-03
+002458,益生股份,2010-08-10
+002459,晶澳科技,2010-08-10
+002460,赣锋锂业,2010-08-10
+002461,珠江啤酒,2010-08-18
+002462,嘉事堂,2010-08-18
+002463,沪电股份,2010-08-18
+002464,众应退,
+002465,海格通信,2010-08-31
+002466,天齐锂业,2010-08-31
+002467,二六三,2010-09-08
+002468,申通快递,2010-09-08
+002469,三维化学,2010-09-08
+002470,金正大,2010-09-08
+002471,中超控股,2010-09-10
+002472,双环传动,2010-09-10
+002473,圣莱退,
+002474,榕基软件,2010-09-15
+002475,立讯精密,2010-09-15
+002476,宝莫股份,2010-09-15
+002477,雏鹰退,
+002478,常宝股份,2010-09-21
+002479,富春环保,2010-09-21
+002480,新筑股份,2010-09-21
+002481,双塔食品,2010-09-21
+002482,*ST广田,2010-09-29
+002483,润邦股份,2010-09-29
+002484,江海股份,2010-09-29
+002485,*ST雪发,2010-10-15
+002486,嘉麟杰,2010-10-15
+002487,大金重工,2010-10-15
+002488,金固股份,2010-10-21
+002489,浙江永强,2010-10-21
+002490,山东墨龙,2010-10-21
+002491,通鼎互联,2010-10-21
+002492,恒基达鑫,2010-11-02
+002493,荣盛石化,2010-11-02
+002494,华斯股份,2010-11-02
+002495,佳隆股份,2010-11-02
+002496,辉丰股份,2010-11-09
+002497,雅化集团,2010-11-09
+002498,汉缆股份,2010-11-09
+002499,科林退,
+002500,山西证券,2010-11-15
+002501,利源股份,2010-11-17
+002502,ST鼎龙,2010-11-17
+002503,*ST搜特,
+002504,*ST弘高,
+002505,鹏都农牧,2010-11-18
+002506,协鑫集成,2010-11-18
+002507,涪陵榨菜,2010-11-23
+002508,老板电器,2010-11-23
+002509,天茂退,
+002510,天汽模,2010-11-25
+002511,中顺洁柔,2010-11-25
+002512,达华智能,2010-12-03
+002513,蓝丰生化,2010-12-03
+002514,宝馨科技,2010-12-03
+002515,金字火腿,2010-12-03
+002516,旷达科技,2010-12-07
+002517,恺英网络,2010-12-07
+002518,科士达,2010-12-07
+002519,银河电子,2010-12-07
+002520,日发精机,2010-12-10
+002521,齐峰新材,2010-12-10
+002522,浙江众成,2010-12-10
+002523,天桥起重,2010-12-10
+002524,光正眼科,2010-12-17
+002526,山东矿机,2010-12-17
+002527,新时达,2010-12-24
+002528,英飞拓,2010-12-24
+002529,海源复材,2010-12-24
+002530,金财互联,2010-12-31
+002531,天顺风能,2010-12-31
+002532,天山铝业,2010-12-31
+002533,金杯电工,2010-12-31
+002534,西子洁能,2011-01-10
+002535,林州重机,2011-01-11
+002536,飞龙股份,2011-01-11
+002537,海联金汇,2011-01-10
+002538,司尔特,2011-01-18
+002539,云图控股,2011-01-18
+002540,亚太科技,2011-01-18
+002541,鸿路钢构,2011-01-18
+002542,中化岩土,2011-01-28
+002543,万和电气,2011-01-28
+002544,普天科技,2011-01-28
+002545,东方铁塔,2011-02-11
+002546,新联电子,2011-02-11
+002547,春兴精工,2011-02-18
+002548,金新农,2011-02-18
+002549,凯美特气,2011-02-18
+002550,千红制药,2011-02-18
+002551,尚荣医疗,2011-02-25
+002552,宝鼎科技,2011-02-25
+002553,南方精工,2011-02-25
+002554,惠博普,2011-02-25
+002555,三七互娱,2011-03-02
+002556,辉隆股份,2011-03-02
+002557,洽洽食品,2011-03-02
+002558,巨人网络,2011-03-02
+002559,亚威股份,2011-03-03
+002560,通达股份,2011-03-03
+002561,徐家汇,2011-03-03
+002562,兄弟科技,2011-03-10
+002563,森马服饰,2011-03-11
+002564,*ST天沃,2011-03-10
+002565,顺灏股份,2011-03-18
+002566,益盛药业,2011-03-18
+002567,唐人神,2011-03-25
+002568,百润股份,2011-03-25
+002569,ST步森,2011-04-12
+002570,贝因美,2011-04-12
+002571,德力股份,2011-04-12
+002572,索菲亚,2011-04-12
+002573,清新环境,2011-04-22
+002574,明牌珠宝,2011-04-22
+002575,群兴玩具,2011-04-22
+002576,通达动力,2011-04-28
+002577,雷柏科技,2011-04-28
+002578,闽发铝业,2011-04-28
+002579,中京电子,2011-05-06
+002580,圣阳股份,2011-05-06
+002581,未名医药,2011-05-20
+002582,好想你,2011-05-20
+002583,海能达,2011-05-27
+002584,西陇科学,2011-06-02
+002585,双星新材,2011-06-02
+002586,*ST围海,2011-06-02
+002587,奥拓电子,2011-06-10
+002588,史丹利,2011-06-10
+002589,瑞康医药,2011-06-10
+002590,万安科技,2011-06-10
+002591,恒大高新,2011-06-21
+002592,ST八菱,2011-11-11
+002593,日上集团,2011-06-28
+002594,比亚迪,2011-06-30
+002595,豪迈科技,2011-06-28
+002596,海南瑞泽,2011-07-07
+002597,金禾实业,2011-07-07
+002598,山东章鼓,2011-07-07
+002599,盛通股份,2011-07-15
+002600,领益智造,2011-07-15
+002601,龙佰集团,2011-07-15
+002602,世纪华通,2011-07-28
+002603,以岭药业,2011-07-28
+002604,龙力退,
+002605,姚记科技,2011-08-05
+002606,大连电瓷,2011-08-05
+002607,中公教育,2011-08-10
+002608,江苏国信,2011-08-10
+002609,捷顺科技,2011-08-15
+002610,爱康科技,2011-08-15
+002611,东方精工,2011-08-30
+002612,朗姿股份,2011-08-30
+002613,北玻股份,2011-08-30
+002614,奥佳华,2011-09-09
+002615,哈尔斯,2011-09-09
+002616,长青集团,2011-09-20
+002617,露笑科技,2011-09-20
+002618,丹邦退,
+002619,*ST艾格,
+002620,瑞和股份,2011-09-29
+002621,美吉姆,2011-09-29
+002622,皓宸医疗,2011-10-18
+002623,亚玛顿,2011-10-13
+002624,完美世界,2011-10-28
+002625,光启技术,2011-11-03
+002626,金达威,2011-10-28
+002627,三峡旅游,2011-11-03
+002628,成都路桥,2011-11-03
+002629,仁智股份,2011-11-03
+002630,华西能源,2011-11-11
+002631,德尔未来,2011-11-11
+002632,道明光学,2011-11-22
+002633,申科股份,2011-11-22
+002634,棒杰股份,2011-12-05
+002635,安洁科技,2011-11-25
+002636,金安国纪,2011-11-25
+002637,赞宇科技,2011-11-25
+002638,勤上股份,2011-11-25
+002639,雪人股份,2011-12-05
+002640,跨境通,2011-12-08
+002641,公元股份,2011-12-08
+002642,荣联科技,2011-12-20
+002643,万润股份,2011-12-20
+002644,佛慈制药,2011-12-22
+002645,华宏科技,2011-12-20
+002646,天佑德酒,2011-12-22
+002647,仁东控股,2011-12-28
+002648,卫星化学,2011-12-28
+002649,博彦科技,2012-01-06
+002650,加加食品,2012-01-06
+002651,利君股份,2012-01-06
+002652,扬子新材,2012-01-19
+002653,海思科,2012-01-17
+002654,万润科技,2012-02-17
+002655,共达电声,2012-02-17
+002656,ST摩登,2012-02-28
+002657,中科金财,2012-02-28
+002658,雪迪龙,2012-03-09
+002659,凯文教育,2012-03-09
+002660,茂硕电源,2012-03-16
+002661,克明食品,2012-03-16
+002662,京威股份,2012-03-09
+002663,普邦股份,2012-03-16
+002664,信质集团,2012-03-16
+002665,首航高科,2012-03-27
+002666,德联集团,2012-03-27
+002667,威领股份,2012-03-29
+002668,奥马电器,2012-04-16
+002669,康达新材,2012-04-16
+002670,国盛金控,2012-04-16
+002671,龙泉股份,2012-04-26
+002672,东江环保,2012-04-26
+002673,西部证券,2012-05-03
+002674,兴业科技,2012-05-07
+002675,东诚药业,2012-05-25
+002676,顺威股份,2012-05-25
+002677,浙江美大,2012-05-25
+002678,珠江钢琴,2012-05-30
+002679,福建金森,2012-06-05
+002680,长生退,
+002681,奋达科技,2012-06-05
+002682,龙洲股份,2012-06-12
+002683,广东宏大,2012-06-12
+002684,猛狮退,
+002685,华东重机,2012-06-12
+002686,亿利达,2012-07-03
+002687,乔治白,2012-07-13
+002688,金河生物,2012-07-13
+002689,远大智能,2012-07-17
+002690,美亚光电,2012-07-31
+002691,冀凯股份,2012-07-31
+002692,ST远程,2012-08-08
+002693,双成药业,2012-08-08
+002694,顾地科技,2012-08-16
+002695,煌上煌,2012-09-05
+002696,百洋股份,2012-09-05
+002697,红旗连锁,2012-09-05
+002698,博实股份,2012-09-11
+002699,*ST美盛,2012-09-11
+002700,ST浩源,2012-09-21
+002701,奥瑞金,2012-10-11
+002702,海欣食品,2012-10-11
+002703,浙江世宝,2012-11-02
+002705,新宝股份,2014-01-21
+002706,良信股份,2014-01-21
+002707,众信旅游,2014-01-23
+002708,光洋股份,2014-01-21
+002709,天赐材料,2014-01-23
+002711,欧浦退,
+002712,思美传媒,2014-01-23
+002713,东易日盛,2014-02-19
+002714,牧原股份,2014-01-28
+002715,登云股份,2014-02-19
+002716,金贵银业,2014-01-28
+002717,岭南股份,2014-02-19
+002718,友邦吊顶,2014-01-28
+002719,麦趣尔,2014-01-28
+002721,*ST金一,2014-01-27
+002722,物产金轮,2014-01-28
+002723,小崧股份,2014-01-29
+002724,海洋王,2014-11-04
+002725,跃岭股份,2014-01-29
+002726,龙大美食,2014-06-26
+002727,一心堂,2014-07-02
+002728,特一药业,2014-07-31
+002729,好利科技,2014-09-12
+002730,电光科技,2014-10-09
+002731,萃华珠宝,2014-11-04
+002732,燕塘乳业,2014-12-05
+002733,雄韬股份,2014-12-03
+002734,利民股份,2015-01-27
+002735,王子新材,2014-12-03
+002736,国信证券,2014-12-29
+002737,葵花药业,2014-12-30
+002738,中矿资源,2014-12-30
+002739,万达电影,2015-01-22
+002740,*ST爱迪,2015-01-22
+002741,光华科技,2015-02-16
+002742,ST三圣,2015-02-17
+002743,富煌钢构,2015-02-17
+002745,木林森,2015-02-17
+002746,仙坛股份,2015-02-16
+002747,埃斯顿,2015-03-20
+002748,世龙实业,2015-03-19
+002749,国光股份,2015-03-20
+002750,龙津药业,2015-03-24
+002751,易尚退,
+002752,昇兴股份,2015-04-22
+002753,永东股份,2015-05-19
+002755,奥赛康,2015-05-15
+002756,永兴材料,2015-05-15
+002757,南兴股份,2015-05-27
+002758,浙农股份,2015-05-27
+002759,天际股份,2015-05-28
+002760,凤形股份,2015-06-11
+002761,浙江建投,2015-06-10
+002762,金发拉比,2015-06-10
+002763,汇洁股份,2015-06-10
+002765,蓝黛科技,2015-06-12
+002766,索菱股份,2015-06-11
+002767,先锋电子,2015-06-12
+002768,国恩股份,2015-06-30
+002769,普路通,2015-06-29
+002770,科迪退,
+002771,真视通,2015-06-29
+002772,众兴菌业,2015-06-26
+002773,康弘药业,2015-06-26
+002774,快意电梯,2017-03-24
+002775,文科园林,2015-06-29
+002776,*ST柏龙,2015-06-26
+002777,久远银海,2015-12-31
+002778,中晟高科,2016-01-06
+002779,中坚科技,2015-12-09
+002780,三夫户外,2015-12-09
+002781,奇信退,
+002782,可立克,2015-12-22
+002783,凯龙股份,2015-12-09
+002785,万里石,2015-12-23
+002786,银宝山新,2015-12-23
+002787,华源控股,2015-12-31
+002788,鹭燕医药,2016-02-18
+002789,建艺集团,2016-03-11
+002790,瑞尔特,2016-03-08
+002791,坚朗五金,2016-03-29
+002792,通宇通讯,2016-03-28
+002793,罗欣药业,2016-04-15
+002795,永和智控,2016-04-28
+002796,世嘉科技,2016-05-10
+002797,第一创业,2016-05-11
+002798,帝欧家居,2016-05-25
+002799,环球印务,2016-06-08
+002800,ST天顺,2016-05-30
+002801,微光股份,2016-06-22
+002802,洪汇新材,2016-06-29
+002803,吉宏股份,2016-07-12
+002805,丰元股份,2016-07-07
+002806,华锋股份,2016-07-26
+002807,江阴银行,2016-09-02
+002808,ST恒久,2016-08-12
+002809,红墙股份,2016-08-23
+002810,山东赫达,2016-08-26
+002811,郑中设计,2016-09-08
+002812,恩捷股份,2016-09-14
+002813,路畅科技,2016-10-12
+002815,崇达技术,2016-10-12
+002816,*ST和科,2016-10-25
+002817,黄山胶囊,2016-10-25
+002818,富森美,2016-11-09
+002819,东方中科,2016-11-11
+002820,桂发祥,2016-11-18
+002821,凯莱英,2016-11-18
+002822,中装建设,2016-11-29
+002823,凯中精密,2016-11-24
+002824,和胜股份,2017-01-12
+002825,纳尔股份,2016-11-29
+002826,易明医药,2016-12-09
+002827,高争民爆,2016-12-09
+002828,贝肯能源,2016-12-08
+002829,星网宇达,2016-12-13
+002830,名雕股份,2016-12-13
+002831,裕同科技,2016-12-16
+002832,比音勒芬,2016-12-23
+002833,弘亚数控,2016-12-28
+002835,同为股份,2016-12-28
+002836,新宏泽,2016-12-29
+002837,英维克,2016-12-29
+002838,道恩股份,2017-01-06
+002839,张家港行,2017-01-24
+002840,华统股份,2017-01-10
+002841,视源股份,2017-01-19
+002842,翔鹭钨业,2017-01-19
+002843,泰嘉股份,2017-01-20
+002845,同兴达,2017-01-25
+002846,英联股份,2017-02-07
+002847,盐津铺子,2017-02-08
+002848,高斯贝尔,2017-02-13
+002849,威星智能,2017-02-17
+002850,科达利,2017-03-02
+002851,麦格米特,2017-03-06
+002852,道道全,2017-03-10
+002853,皮阿诺,2017-03-10
+002855,捷荣技术,2017-03-21
+002856,美芝股份,2017-03-20
+002857,三晖电气,2017-03-23
+002858,力盛体育,2017-03-24
+002859,洁美科技,2017-04-07
+002860,星帅尔,2017-04-12
+002861,瀛通通讯,2017-04-13
+002862,实丰文化,2017-04-11
+002863,今飞凯达,2017-04-18
+002864,盘龙药业,2017-11-16
+002865,钧达股份,2017-04-25
+002866,传艺科技,2017-04-26
+002867,周大生,2017-04-27
+002868,绿康生化,2017-05-03
+002869,金溢科技,2017-05-15
+002870,香山股份,2017-05-15
+002871,伟隆股份,2017-05-11
+002872,ST天圣,2017-05-19
+002873,新天药业,2017-05-19
+002875,安奈儿,2017-06-01
+002876,三利谱,2017-05-25
+002877,智能自控,2017-06-05
+002878,元隆雅图,2017-06-06
+002879,长缆科技,2017-07-07
+002880,卫光生物,2017-06-16
+002881,美格智能,2017-06-22
+002882,金龙羽,2017-07-17
+002883,中设股份,2017-06-20
+002884,凌霄泵业,2017-07-11
+002885,京泉华,2017-06-27
+002886,沃特股份,2017-06-27
+002887,绿茵生态,2017-08-01
+002888,惠威科技,2017-07-21
+002889,东方嘉盛,2017-07-31
+002890,弘宇股份,2017-08-02
+002891,中宠股份,2017-08-21
+002892,科力尔,2017-08-17
+002893,京能热力,2017-09-15
+002895,川恒股份,2017-08-25
+002896,中大力德,2017-08-29
+002897,意华股份,2017-09-07
+002898,赛隆药业,2017-09-12
+002899,英派斯,2017-09-15
+002900,哈三联,2017-09-22
+002901,大博医疗,2017-09-22
+002902,铭普光磁,2017-09-29
+002903,宇环数控,2017-10-13
+002905,金逸影视,2017-10-16
+002906,华阳集团,2017-10-13
+002907,华森制药,2017-10-20
+002908,德生科技,2017-10-20
+002909,集泰股份,2017-10-26
+002910,庄园牧场,2017-10-31
+002911,佛燃能源,2017-11-22
+002912,中新赛克,2017-11-21
+002913,奥士康,2017-12-01
+002915,中欣氟材,2017-12-05
+002916,深南电路,2017-12-13
+002917,金奥博,2017-12-08
+002918,蒙娜丽莎,2017-12-19
+002919,名臣健康,2017-12-18
+002920,德赛西威,2017-12-26
+002921,联诚精密,2017-12-27
+002922,伊戈尔,2017-12-29
+002923,润都股份,2018-01-05
+002925,盈趣科技,2018-01-15
+002926,华西证券,2018-02-05
+002927,泰永长征,2018-02-23
+002928,华夏航空,2018-03-02
+002929,润建股份,2018-03-01
+002930,宏川智慧,2018-03-28
+002931,锋龙股份,2018-04-03
+002932,明德生物,2018-07-10
+002933,新兴装备,2018-08-28
+002935,天奥电子,2018-09-03
+002936,郑州银行,2018-09-19
+002937,兴瑞科技,2018-09-26
+002938,鹏鼎控股,2018-09-18
+002939,长城证券,2018-10-26
+002940,昂利康,2018-10-23
+002941,新疆交建,2018-11-28
+002942,新农股份,2018-12-05
+002943,宇晶股份,2018-11-29
+002945,华林证券,2019-01-17
+002946,新乳业,2019-01-25
+002947,恒铭达,2019-02-01
+002948,青岛银行,2019-01-16
+002949,华阳国际,2019-02-26
+002950,奥美医疗,2019-03-11
+002951,ST金时,2019-03-15
+002952,亚世光电,2019-03-28
+002953,日丰股份,2019-05-09
+002955,鸿合科技,2019-05-23
+002956,西麦食品,2019-06-19
+002957,科瑞技术,2019-07-26
+002958,青农商行,2019-03-26
+002959,小熊电器,2019-08-23
+002960,青鸟消防,2019-08-09
+002961,瑞达期货,2019-09-05
+002962,五方光电,2019-09-17
+002963,豪尔赛,2019-10-28
+002965,祥鑫科技,2019-10-25
+002966,苏州银行,2019-08-02
+002967,广电计量,2019-11-08
+002968,新大正,2019-12-03
+002969,嘉美包装,2019-12-02
+002970,锐明技术,2019-12-17
+002971,和远气体,2020-01-13
+002972,科安达,2019-12-27
+002973,侨银股份,2020-01-06
+002975,博杰股份,2020-02-05
+002976,瑞玛精密,2020-03-06
+002977,天箭科技,2020-03-17
+002978,安宁股份,2020-04-17
+002979,雷赛智能,2020-04-08
+002980,华盛昌,2020-04-15
+002981,朝阳科技,2020-04-17
+002982,湘佳股份,2020-04-24
+002983,芯瑞达,2020-04-28
+002984,森麒麟,2020-09-11
+002985,北摩高科,2020-04-29
+002986,宇新股份,2020-06-02
+002987,京北方,2020-05-07
+002988,豪美新材,2020-05-18
+002989,中天精装,2020-06-10
+002990,盛视科技,2020-05-25
+002991,甘源食品,2020-07-31
+002992,宝明科技,2020-08-03
+002993,奥海科技,2020-08-17
+002995,天地在线,2020-08-05
+002996,顺博合金,2020-08-28
+002997,瑞鹄模具,2020-09-03
+002998,优彩资源,2020-09-25
+002999,天禾股份,2020-09-03
+003000,劲仔食品,2020-09-14
+003001,中岩大地,2020-10-13
+003002,壶化股份,2020-09-22
+003003,天元股份,2020-09-21
+003004,声迅股份,2020-11-26
+003005,竞业达,2020-09-22
+003006,百亚股份,2020-09-21
+003007,直真科技,2020-09-23
+003008,开普检测,2020-09-23
+003009,中天火箭,2020-09-25
+003010,若羽臣,2020-09-25
+003011,海象新材,2020-09-30
+003012,东鹏控股,2020-10-19
+003013,地铁设计,2020-10-22
+003015,日久光电,2020-10-21
+003016,欣贺股份,2020-10-26
+003017,大洋生物,2020-10-26
+003018,金富科技,2020-11-06
+003019,宸展光电,2020-11-17
+003020,立方制药,2020-12-15
+003021,兆威机电,2020-12-04
+003022,联泓新科,2020-12-08
+003023,彩虹集团,2020-12-11
+003025,思进智能,2020-12-11
+003026,中晶科技,2020-12-18
+003027,同兴环保,2020-12-18
+003028,振邦智能,2020-12-28
+003029,吉大正元,2020-12-24
+003030,祖名股份,2021-01-06
+003031,中瓷电子,2021-01-04
+003032,传智教育,2021-01-12
+003033,征和工业,2021-01-11
+003035,南网能源,2021-01-19
+003036,泰坦股份,2021-01-28
+003037,三和管桩,2021-02-04
+003038,鑫铂股份,2021-02-10
+003039,顺控发展,2021-03-08
+003040,楚天龙,2021-03-22
+003041,真爱美家,2021-04-06
+003042,中农联合,2021-04-06
+003043,华亚智能,2021-04-06
+003816,中国广核,2019-08-26
+200002,万科B,
+200003,PT金田B,
+200011,深物业B,
+200012,南  玻Ｂ,
+200013,*ST石化B,
+200015,PT中浩B,
+200016,深康佳Ｂ,
+200017,深中华B,
+200018,神城B退,
+200019,深粮B,
+200020,深华发Ｂ,
+200024,招商局B,
+200025,特  力Ｂ,
+200026,飞亚达Ｂ,
+200028,一致Ｂ,
+200029,深深房Ｂ,
+200030,富奥B,
+200037,深南电B,
+200039,中集B,
+200041,*ST本实B,
+200045,深纺织Ｂ,
+200053,深基地B,
+200054,建车B,
+200055,方大Ｂ,
+200056,皇庭B,
+200057,*ST大洋B,
+200058,深赛格B,
+200152,山航B退,
+200160,东沣B退,
+200168,*ST舜喆B,
+200413,东旭B,
+200418,小天鹅B,
+200429,粤高速Ｂ,
+200468,宁通信B,
+200488,晨  鸣Ｂ,
+200505,京粮B,
+200512,闽灿坤Ｂ,
+200513,丽珠B,
+200521,虹美菱B,
+200530,冰山B,
+200539,粤电力Ｂ,
+200541,粤照明Ｂ,
+200550,江  铃Ｂ,
+200553,安道麦B,
+200570,苏常柴Ｂ,
+200581,苏威孚Ｂ,
+200596,古井贡Ｂ,
+200613,东海B退,
+200625,长  安Ｂ,
+200706,瓦轴B,
+200725,京东方Ｂ,
+200726,鲁  泰Ｂ,
+200761,本钢板Ｂ,
+200770,武锅B退,
+200771,杭汽轮Ｂ,
+200869,张  裕Ｂ,
+200986,粤华包B,
+200992,中  鲁Ｂ,
+201872,招港B,
+300001,特锐德,2009-10-30
+300002,神州泰岳,2009-10-30
+300003,乐普医疗,2009-10-30
+300004,南风股份,2009-10-30
+300005,探路者,2009-10-30
+300006,莱美药业,2009-10-30
+300007,汉威科技,2009-10-30
+300008,天海防务,2009-10-30
+300009,安科生物,2009-10-30
+300010,*ST豆神,2009-10-30
+300011,鼎汉技术,2009-10-30
+300012,华测检测,2009-10-30
+300013,新宁物流,2009-10-30
+300014,亿纬锂能,2009-10-30
+300015,爱尔眼科,2009-10-30
+300016,北陆药业,2009-10-30
+300017,网宿科技,2009-10-30
+300018,中元股份,2009-10-30
+300019,硅宝科技,2009-10-30
+300020,银江技术,2009-10-30
+300021,大禹节水,2009-10-30
+300022,吉峰科技,2009-10-30
+300023,宝德退,
+300024,机器人,2009-10-30
+300025,华星创业,2009-10-30
+300026,红日药业,2009-10-30
+300027,华谊兄弟,2009-10-30
+300028,金亚退,
+300029,ST天龙,2009-12-25
+300030,阳普医疗,2009-12-25
+300031,宝通科技,2009-12-25
+300032,金龙机电,2009-12-25
+300033,同花顺,2009-12-25
+300034,钢研高纳,2009-12-25
+300035,中科电气,2009-12-25
+300036,超图软件,2009-12-25
+300037,新宙邦,2010-01-08
+300038,数知退,
+300039,上海凯宝,2010-01-08
+300040,九洲集团,2010-01-08
+300041,回天新材,2010-01-08
+300042,朗科科技,2010-01-08
+300043,星辉娱乐,2010-01-20
+300044,赛为智能,2010-01-20
+300045,华力创通,2010-01-20
+300046,台基股份,2010-01-20
+300047,天源迪科,2010-01-20
+300048,合康新能,2010-01-20
+300049,福瑞股份,2010-01-20
+300050,世纪鼎利,2010-01-20
+300051,琏升科技,2010-02-11
+300052,中青宝,2010-02-11
+300053,航宇微,2010-02-11
+300054,鼎龙股份,2010-02-11
+300055,万邦达,2010-02-26
+300056,中创环保,2010-02-26
+300057,万顺新材,2010-02-26
+300058,蓝色光标,2010-02-26
+300059,东方财富,2010-03-19
+300061,旗天科技,2010-03-19
+300062,中能电气,2010-03-19
+300063,天龙集团,2010-03-26
+300064,金刚退,
+300065,海兰信,2010-03-26
+300066,三川智慧,2010-03-26
+300067,安诺其,2010-04-21
+300068,南都电源,2010-04-21
+300069,金利华电,2010-04-21
+300070,碧水源,2010-04-21
+300071,福石控股,2010-04-21
+300072,海新能科,2010-04-27
+300073,当升科技,2010-04-27
+300074,华平股份,2010-04-27
+300075,数字政通,2010-04-27
+300076,GQY视讯,2010-04-30
+300077,国民技术,2010-04-30
+300078,思创医惠,2010-04-30
+300079,数码视讯,2010-04-30
+300080,易成新能,2010-06-25
+300081,恒信东方,2010-05-20
+300082,奥克股份,2010-05-20
+300083,创世纪,2010-05-20
+300084,海默科技,2010-05-20
+300085,银之杰,2010-05-26
+300086,康芝药业,2010-05-26
+300087,荃银高科,2010-05-26
+300088,长信科技,2010-05-26
+300089,文化退,
+300090,盛运退,
+300091,金通灵,2010-06-25
+300092,科新机电,2010-07-08
+300093,金刚光伏,2010-07-08
+300094,国联水产,2010-07-08
+300095,华伍股份,2010-07-28
+300096,易联众,2010-07-28
+300097,智云股份,2010-07-28
+300098,高新兴,2010-07-28
+300099,精准信息,2010-08-06
+300100,双林股份,2010-08-06
+300101,振芯科技,2010-08-06
+300102,乾照光电,2010-08-12
+300103,达刚控股,2010-08-12
+300104,乐视退,
+300105,龙源技术,2010-08-20
+300106,西部牧业,2010-08-20
+300107,建新股份,2010-08-20
+300108,*ST吉药,2010-08-25
+300109,新开源,2010-08-25
+300110,华仁药业,2010-08-25
+300111,向日葵,2010-08-27
+300112,万讯自控,2010-08-27
+300113,顺网科技,2010-08-27
+300114,中航电测,2010-08-27
+300115,长盈精密,2010-09-02
+300116,保力新,2010-09-02
+300117,嘉寓股份,2010-09-02
+300118,东方日升,2010-09-02
+300119,瑞普生物,2010-09-17
+300120,经纬辉开,2010-09-17
+300121,阳谷华泰,2010-09-17
+300122,智飞生物,2010-09-28
+300123,亚光科技,2010-09-28
+300124,汇川技术,2010-09-28
+300125,聆达股份,2010-10-13
+300126,锐奇股份,2010-10-13
+300127,银河磁体,2010-10-13
+300128,锦富技术,2010-10-13
+300129,泰胜风能,2010-10-19
+300130,新国都,2010-10-19
+300131,英唐智控,2010-10-19
+300132,青松股份,2010-10-26
+300133,华策影视,2010-10-26
+300134,大富科技,2010-10-26
+300135,宝利国际,2010-10-26
+300136,信维通信,2010-11-05
+300137,先河环保,2010-11-05
+300138,晨光生物,2010-11-05
+300139,晓程科技,2010-11-12
+300140,节能环境,2010-11-12
+300141,和顺电气,2010-11-12
+300142,沃森生物,2010-11-12
+300143,盈康生命,2010-12-09
+300144,宋城演艺,2010-12-09
+300145,中金环境,2010-12-09
+300146,汤臣倍健,2010-12-15
+300147,香雪制药,2010-12-15
+300148,天舟文化,2010-12-15
+300149,睿智医药,2010-12-22
+300150,世纪瑞尔,2010-12-22
+300151,昌红科技,2010-12-22
+300152,新动力,2010-12-29
+300153,科泰电源,2010-12-29
+300154,瑞凌股份,2010-12-29
+300155,安居宝,2011-01-07
+300156,神雾退,
+300157,新锦动力,2011-01-07
+300158,振东制药,2011-01-07
+300159,新研股份,2011-01-07
+300160,秀强股份,2011-01-13
+300161,华中数控,2011-01-13
+300162,雷曼光电,2011-01-13
+300163,先锋新材,2011-01-13
+300164,通源石油,2011-01-13
+300165,天瑞仪器,2011-01-25
+300166,东方国信,2011-01-25
+300167,ST迪威迅,2011-01-25
+300168,万达信息,2011-01-25
+300169,天晟新材,2011-01-25
+300170,汉得信息,2011-02-01
+300171,东富龙,2011-02-01
+300172,中电环保,2011-02-01
+300173,福能东方,2011-02-01
+300174,元力股份,2011-02-01
+300175,朗源股份,2011-02-15
+300176,派生科技,2011-02-15
+300177,中海达,2011-02-15
+300178,腾邦退,
+300179,四方达,2011-02-15
+300180,华峰超纤,2011-02-22
+300181,佐力药业,2011-02-22
+300182,捷成股份,2011-02-22
+300183,东软载波,2011-02-22
+300184,力源信息,2011-02-22
+300185,通裕重工,2011-03-08
+300186,大华农,
+300187,永清环保,2011-03-08
+300188,美亚柏科,2011-03-16
+300189,神农科技,2011-03-16
+300190,维尔利,2011-03-16
+300191,潜能恒信,2011-03-16
+300192,科德教育,2011-03-22
+300193,佳士科技,2011-03-22
+300194,福安药业,2011-03-22
+300195,长荣股份,2011-03-29
+300196,长海股份,2011-03-29
+300197,节能铁汉,2011-03-29
+300198,纳川股份,2011-04-07
+300199,翰宇药业,2011-04-07
+300200,高盟新材,2011-04-07
+300201,海伦哲,2011-04-07
+300202,聚龙退,
+300203,聚光科技,2011-04-15
+300204,舒泰神,2011-04-15
+300205,天喻信息,2011-04-21
+300206,理邦仪器,2011-04-21
+300207,欣旺达,2011-04-21
+300208,青岛中程,2011-04-26
+300209,ST有棵树,2011-04-26
+300210,森远股份,2011-04-26
+300211,亿通科技,2011-05-05
+300212,易华录,2011-05-05
+300213,佳讯飞鸿,2011-05-05
+300214,日科化学,2011-05-11
+300215,电科院,2011-05-11
+300216,千山退,
+300217,东方电热,2011-05-18
+300218,安利股份,2011-05-18
+300219,鸿利智汇,2011-05-18
+300220,ST金运,2011-05-25
+300221,银禧科技,2011-05-25
+300222,科大智能,2011-05-25
+300223,北京君正,2011-05-31
+300224,正海磁材,2011-05-31
+300225,金力泰,2011-05-31
+300226,上海钢联,2011-06-08
+300227,光韵达,2011-06-08
+300228,富瑞特装,2011-06-08
+300229,拓尔思,2011-06-15
+300230,永利股份,2011-06-15
+300231,银信科技,2011-06-15
+300232,洲明科技,2011-06-22
+300233,金城医药,2011-06-22
+300234,开尔新材,2011-06-22
+300235,方直科技,2011-06-29
+300236,上海新阳,2011-06-29
+300237,美晨生态,2011-06-29
+300238,冠昊生物,2011-07-06
+300239,东宝生物,2011-07-06
+300240,飞力达,2011-07-06
+300241,瑞丰光电,2011-07-12
+300242,佳云科技,2011-07-12
+300243,瑞丰高材,2011-07-12
+300244,迪安诊断,2011-07-19
+300245,天玑科技,2011-07-19
+300246,宝莱特,2011-07-19
+300247,融捷健康,2011-07-29
+300248,新开普,2011-07-29
+300249,依米康,2011-08-03
+300250,初灵信息,2011-08-03
+300251,光线传媒,2011-08-03
+300252,金信诺,2011-08-18
+300253,卫宁健康,2011-08-18
+300254,仟源医药,2011-08-19
+300255,常山药业,2011-08-19
+300256,星星科技,2011-08-19
+300257,开山股份,2011-08-19
+300258,精锻科技,2011-08-26
+300259,新天科技,2011-08-31
+300260,新莱应材,2011-09-06
+300261,雅本化学,2011-09-06
+300262,巴安水务,2011-09-16
+300263,隆华科技,2011-09-16
+300264,佳创视讯,2011-09-16
+300265,通光线缆,2011-09-16
+300266,兴源环境,2011-09-27
+300267,尔康制药,2011-09-27
+300268,*ST佳沃,2011-09-27
+300269,联建光电,2011-10-12
+300270,中威电子,2011-10-12
+300271,华宇软件,2011-10-26
+300272,开能健康,2011-11-02
+300273,和佳退,
+300274,阳光电源,2011-11-02
+300275,梅安森,2011-11-02
+300276,三丰智能,2011-11-15
+300277,海联讯,2011-11-23
+300278,华昌达,2011-12-16
+300279,和晶科技,2011-12-29
+300280,紫天科技,2011-12-29
+300281,金明精机,2011-12-29
+300282,*ST三盛,2011-12-29
+300283,温州宏丰,2012-01-10
+300284,苏交科,2012-01-10
+300285,国瓷材料,2012-01-13
+300286,安科瑞,2012-01-13
+300287,飞利信,2012-02-01
+300288,朗玛信息,2012-02-16
+300289,利德曼,2012-02-16
+300290,荣科科技,2012-02-16
+300291,百纳千成,2012-02-09
+300292,吴通控股,2012-02-29
+300293,蓝英装备,2012-03-08
+300294,博雅生物,2012-03-08
+300295,三六五网,2012-03-15
+300296,利亚德,2012-03-15
+300297,蓝盾退,
+300298,三诺生物,2012-03-19
+300299,富春股份,2012-03-19
+300300,海峡创新,2012-03-19
+300301,*ST长方,2012-03-21
+300302,同有科技,2012-03-21
+300303,聚飞光电,2012-03-19
+300304,云意电气,2012-03-21
+300305,裕兴股份,2012-03-29
+300306,远方信息,2012-03-29
+300307,慈星股份,2012-03-29
+300308,中际旭创,2012-04-10
+300309,吉艾退,
+300310,宜通世纪,2012-04-25
+300311,任子行,2012-04-25
+300312,邦讯退,
+300313,*ST天山,2012-04-25
+300314,戴维医疗,2012-05-08
+300315,掌趣科技,2012-05-11
+300316,晶盛机电,2012-05-11
+300317,珈伟新能,2012-05-11
+300318,博晖创新,2012-05-23
+300319,麦捷科技,2012-05-23
+300320,海达股份,2012-06-01
+300321,同大股份,2012-05-23
+300322,硕贝德,2012-06-08
+300323,华灿光电,2012-06-01
+300324,旋极信息,2012-06-08
+300325,德威退,
+300326,凯利泰,2012-06-13
+300327,中颖电子,2012-06-13
+300328,宜安科技,2012-06-19
+300329,海伦钢琴,2012-06-19
+300330,计通退,
+300331,苏大维格,2012-06-28
+300332,天壕能源,2012-06-28
+300333,兆日科技,2012-06-28
+300334,津膜科技,2012-07-05
+300335,迪森股份,2012-07-10
+300336,新文退,
+300337,银邦股份,2012-07-18
+300338,开元教育,2012-07-26
+300339,润和软件,2012-07-18
+300340,科恒股份,2012-07-26
+300341,麦克奥迪,2012-07-26
+300342,天银机电,2012-07-26
+300343,联创股份,2012-08-01
+300344,立方数科,2012-08-01
+300345,华民股份,2012-08-01
+300346,南大光电,2012-08-07
+300347,泰格医药,2012-08-17
+300348,长亮科技,2012-08-17
+300349,金卡智能,2012-08-17
+300350,华鹏飞,2012-08-21
+300351,永贵电器,2012-09-20
+300352,北信源,2012-09-12
+300353,东土科技,2012-09-27
+300354,东华测试,2012-09-20
+300355,蒙草生态,2012-09-27
+300356,光一退,
+300357,我武生物,2014-01-21
+300358,楚天科技,2014-01-21
+300359,全通教育,2014-01-21
+300360,炬华科技,2014-01-21
+300362,天翔退,
+300363,博腾股份,2014-01-29
+300364,中文在线,2015-01-21
+300365,恒华科技,2014-01-23
+300366,创意信息,2014-01-27
+300367,网力退,
+300368,汇金股份,2014-01-23
+300369,绿盟科技,2014-01-29
+300370,安控科技,2014-01-23
+300371,汇中股份,2014-01-23
+300372,欣泰退,
+300373,扬杰科技,2014-01-23
+300374,中铁装配,2015-03-19
+300375,鹏翎股份,2014-01-27
+300376,易事特,2014-01-27
+300377,赢时胜,2014-01-27
+300378,鼎捷软件,2014-01-27
+300379,东方通,2014-01-28
+300380,安硕信息,2014-01-28
+300381,溢多利,2014-01-28
+300382,斯莱克,2014-01-29
+300383,光环新网,2014-01-29
+300384,三联虹普,2014-08-01
+300385,雪浪环境,2014-06-26
+300386,飞天诚信,2014-06-26
+300387,富邦股份,2014-07-02
+300388,节能国祯,2014-08-01
+300389,艾比森,2014-08-01
+300390,天华新能,2014-07-31
+300391,长药控股,2014-08-01
+300392,腾信退,
+300393,中来股份,2014-09-12
+300394,天孚通信,2015-02-17
+300395,菲利华,2014-09-10
+300396,迪瑞医疗,2014-09-10
+300397,天和防务,2014-09-10
+300398,飞凯材料,2014-10-09
+300399,天利科技,2014-10-09
+300400,劲拓股份,2014-10-10
+300401,花园生物,2014-10-09
+300402,宝色股份,2014-10-10
+300403,汉宇集团,2014-10-30
+300404,博济医药,2015-04-24
+300405,科隆股份,2014-10-30
+300406,九强生物,2014-10-30
+300407,凯发电气,2014-12-03
+300408,三环集团,2014-12-03
+300409,道氏技术,2014-12-03
+300410,正业科技,2014-12-31
+300411,金盾股份,2014-12-31
+300412,迦南科技,2014-12-31
+300413,芒果超媒,2015-01-21
+300414,中光防雷,2015-05-13
+300415,伊之密,2015-01-23
+300416,苏试试验,2015-01-22
+300417,南华仪器,2015-01-23
+300418,昆仑万维,2015-01-21
+300419,浩丰科技,2015-01-22
+300420,五洋停车,2015-02-17
+300421,力星股份,2015-02-17
+300422,博世科,2015-02-17
+300423,昇辉科技,2015-02-17
+300424,航新科技,2015-04-22
+300425,中建环能,2015-02-16
+300426,唐德影视,2015-02-17
+300427,*ST红相,2015-02-17
+300428,立中集团,2015-03-19
+300429,强力新材,2015-03-24
+300430,诚益通,2015-03-19
+300431,暴风退,
+300432,富临精工,2015-03-19
+300433,蓝思科技,2015-03-18
+300434,金石亚药,2015-04-24
+300435,中泰股份,2015-03-26
+300436,广生堂,2015-04-22
+300437,清水源,2015-04-23
+300438,鹏辉能源,2015-04-24
+300439,美康生物,2015-04-22
+300440,运达科技,2015-04-23
+300441,鲍斯股份,2015-04-23
+300442,润泽科技,2015-04-24
+300443,金雷股份,2015-04-22
+300444,双杰电气,2015-04-23
+300445,康斯特,2015-04-24
+300446,乐凯新材,2015-04-23
+300447,全信股份,2015-04-22
+300448,浩云科技,2015-04-24
+300449,汉邦高科,2015-04-22
+300450,先导智能,2015-05-18
+300451,创业慧康,2015-05-14
+300452,山河药辅,2015-05-15
+300453,三鑫医疗,2015-05-15
+300454,深信服,2018-05-16
+300455,航天智装,2015-05-15
+300456,赛微电子,2015-05-14
+300457,赢合科技,2015-05-14
+300458,全志科技,2015-05-15
+300459,汤姆猫,2015-05-15
+300460,惠伦晶体,2015-05-15
+300461,田中精机,2015-05-19
+300462,华铭智能,2015-05-27
+300463,迈克生物,2015-05-28
+300464,星徽股份,2015-06-10
+300465,高伟达,2015-05-28
+300466,赛摩智能,2015-05-28
+300467,迅游科技,2015-05-27
+300468,四方精创,2015-05-27
+300469,信息发展,2015-06-11
+300470,中密控股,2015-06-12
+300471,厚普股份,2015-06-11
+300472,新元科技,2015-06-11
+300473,德尔股份,2015-06-12
+300474,景嘉微,2016-03-31
+300475,香农芯创,2015-06-10
+300476,胜宏科技,2015-06-11
+300477,合纵科技,2015-06-10
+300478,杭州高新,2015-06-10
+300479,神思电子,2015-06-12
+300480,光力科技,2015-07-02
+300481,濮阳惠成,2015-06-30
+300482,万孚生物,2015-06-30
+300483,首华燃气,2015-06-30
+300484,蓝海华腾,2016-03-22
+300485,赛升药业,2015-06-26
+300486,东杰智能,2015-06-30
+300487,蓝晓科技,2015-07-02
+300488,恒锋工具,2015-07-01
+300489,光智科技,2015-07-01
+300490,华自科技,2015-12-31
+300491,通合科技,2015-12-31
+300492,华图山鼎,2015-12-23
+300493,润欣科技,2015-12-10
+300494,盛天网络,2015-12-31
+300495,*ST美尚,2015-12-22
+300496,中科创达,2015-12-10
+300497,富祥药业,2015-12-22
+300498,温氏股份,2015-11-02
+300499,高澜股份,2016-02-02
+300500,启迪设计,2016-02-04
+300501,海顺新材,2016-02-04
+300502,新易盛,2016-03-03
+300503,昊志机电,2016-03-09
+300504,天邑股份,2018-03-30
+300505,川金诺,2016-03-15
+300506,名家汇,2016-03-24
+300507,苏奥传感,2016-04-29
+300508,维宏股份,2016-04-19
+300509,新美星,2016-04-25
+300510,金冠股份,2016-05-06
+300511,雪榕生物,2016-05-04
+300512,中亚股份,2016-05-26
+300513,恒实科技,2016-05-30
+300514,友讯达,2017-04-26
+300515,三德科技,2016-06-08
+300516,久之洋,2016-06-02
+300517,海波重科,2016-07-19
+300518,盛讯达,2016-06-24
+300519,新光药业,2016-06-24
+300520,科大国创,2016-07-08
+300521,爱司凯,2016-07-05
+300522,世名科技,2016-07-05
+300523,辰安科技,2016-07-26
+300525,博思软件,2016-07-26
+300526,中潜退,
+300527,中船应急,2016-08-05
+300528,幸福蓝海,2016-08-08
+300529,健帆生物,2016-08-02
+300530,领湃科技,2016-08-09
+300531,优博讯,2016-08-09
+300532,今天国际,2016-08-18
+300533,冰川网络,2016-08-18
+300534,陇神戎发,2016-09-13
+300535,达威股份,2016-08-12
+300536,农尚环境,2016-09-20
+300537,广信材料,2016-08-30
+300538,同益股份,2016-08-26
+300539,横河精密,2016-08-30
+300540,蜀道装备,2016-08-23
+300541,先进数通,2016-09-13
+300542,新晨科技,2016-09-20
+300543,朗科智能,2016-09-08
+300545,联得装备,2016-09-28
+300546,雄帝科技,2016-09-28
+300547,川环科技,2016-09-30
+300548,博创科技,2016-10-12
+300549,优德精密,2016-09-30
+300550,和仁科技,2016-10-18
+300551,古鳌科技,2016-10-18
+300552,万集科技,2016-10-21
+300553,集智股份,2016-10-21
+300554,三超新材,2017-04-21
+300555,ST路通,2016-10-18
+300556,丝路视觉,2016-11-04
+300557,理工光科,2016-11-01
+300558,贝达药业,2016-11-07
+300559,佳发教育,2016-11-01
+300560,中富通,2016-11-01
+300561,汇金科技,2016-11-17
+300562,乐心医疗,2016-11-16
+300563,神宇股份,2016-11-14
+300564,筑博设计,2019-11-08
+300565,科信技术,2016-11-22
+300566,激智科技,2016-11-15
+300567,精测电子,2016-11-22
+300568,星源材质,2016-12-01
+300569,天能重工,2016-11-25
+300570,太辰光,2016-12-06
+300571,平治信息,2016-12-13
+300572,安车检测,2016-12-06
+300573,兴齐眼药,2016-12-08
+300575,中旗股份,2016-12-20
+300576,容大感光,2016-12-20
+300577,开润股份,2016-12-21
+300578,会畅通讯,2017-01-25
+300579,数字认证,2016-12-23
+300580,贝斯特,2017-01-11
+300581,晨曦航空,2016-12-20
+300582,英飞特,2016-12-28
+300583,赛托生物,2017-01-06
+300584,海辰药业,2017-01-12
+300585,奥联电子,2016-12-29
+300586,美联新材,2017-01-04
+300587,天铁股份,2017-01-05
+300588,熙菱信息,2017-01-05
+300589,江龙船艇,2017-01-13
+300590,移为通信,2017-01-11
+300591,万里马,2017-01-10
+300592,华凯易佰,2017-01-20
+300593,新雷能,2017-01-13
+300594,朗进科技,2019-06-21
+300595,欧普康视,2017-01-17
+300596,利安隆,2017-01-19
+300597,吉大通信,2017-01-23
+300598,诚迈科技,2017-01-20
+300599,雄塑科技,2017-01-23
+300600,国瑞科技,2017-01-25
+300601,康泰生物,2017-02-07
+300602,飞荣达,2017-01-26
+300603,立昂技术,2017-01-26
+300604,长川科技,2017-04-17
+300605,恒锋信息,2017-02-08
+300606,金太阳,2017-02-08
+300607,拓斯达,2017-02-09
+300608,思特奇,2017-02-13
+300609,汇纳科技,2017-02-15
+300610,晨化股份,2017-02-13
+300611,美力科技,2017-02-20
+300612,宣亚国际,2017-02-15
+300613,富瀚微,2017-02-20
+300614,百川畅银,2021-05-25
+300615,欣天科技,2017-02-15
+300616,尚品宅配,2017-03-07
+300617,安靠智电,2017-02-28
+300618,寒锐钴业,2017-03-06
+300619,金银河,2017-03-01
+300620,光库科技,2017-03-10
+300621,维业股份,2017-03-16
+300622,博士眼镜,2017-03-15
+300623,捷捷微电,2017-03-14
+300624,万兴科技,2018-01-18
+300625,三雄极光,2017-03-17
+300626,华瑞股份,2017-03-20
+300627,华测导航,2017-03-21
+300628,亿联网络,2017-03-17
+300629,新劲刚,2017-03-24
+300630,普利制药,2017-03-28
+300631,久吾高科,2017-03-23
+300632,光莆股份,2017-04-06
+300633,开立医疗,2017-04-06
+300634,彩讯股份,2018-03-23
+300635,中达安,2017-03-31
+300636,同和药业,2017-03-31
+300637,扬帆新材,2017-04-12
+300638,广和通,2017-04-13
+300639,凯普生物,2017-04-12
+300640,德艺文创,2017-04-17
+300641,正丹股份,2017-04-18
+300642,透景生命,2017-04-21
+300643,万通智控,2017-05-05
+300644,南京聚隆,2018-02-06
+300645,正元智慧,2017-04-21
+300647,超频三,2017-05-03
+300648,星云股份,2017-04-25
+300649,杭州园林,2017-05-05
+300650,太龙股份,2017-05-03
+300651,金陵体育,2017-05-09
+300652,雷迪克,2017-05-16
+300653,正海生物,2017-05-16
+300654,世纪天鸿,2017-09-26
+300655,晶瑞电材,2017-05-23
+300656,民德电子,2017-05-19
+300657,弘信电子,2017-05-23
+300658,延江股份,2017-06-02
+300659,中孚信息,2017-05-26
+300660,江苏雷利,2017-06-02
+300661,圣邦股份,2017-06-06
+300662,科锐国际,2017-06-08
+300663,科蓝软件,2017-06-08
+300664,鹏鹞环保,2018-01-05
+300665,飞鹿股份,2017-06-13
+300666,江丰电子,2017-06-15
+300667,必创科技,2017-06-19
+300668,杰恩设计,2017-06-19
+300669,沪宁股份,2017-06-29
+300670,大烨智能,2017-07-03
+300671,富满微,2017-07-05
+300672,国科微,2017-07-12
+300673,佩蒂股份,2017-07-11
+300674,宇信科技,2018-11-07
+300675,建科院,2017-07-19
+300676,华大基因,2017-07-14
+300677,英科医疗,2017-07-21
+300678,中科信息,2017-07-28
+300679,电连技术,2017-07-31
+300680,隆盛科技,2017-07-25
+300681,英搏尔,2017-07-25
+300682,朗新科技,2017-08-01
+300683,海特生物,2017-08-08
+300684,中石科技,2017-12-27
+300685,艾德生物,2017-08-02
+300686,智动力,2017-08-04
+300687,赛意信息,2017-08-03
+300688,创业黑马,2017-08-10
+300689,澄天伟业,2017-08-09
+300690,双一科技,2017-08-08
+300691,联合光电,2017-08-11
+300692,中环环保,2017-08-21
+300693,盛弘股份,2017-08-22
+300694,蠡湖股份,2018-10-15
+300695,兆丰股份,2017-09-08
+300696,爱乐达,2017-08-22
+300697,电工合金,2017-09-07
+300698,万马科技,2017-08-31
+300699,光威复材,2017-09-01
+300700,岱勒新材,2017-09-12
+300701,森霸传感,2017-09-15
+300702,天宇股份,2017-09-19
+300703,创源股份,2017-09-19
+300705,九典制药,2017-10-10
+300706,阿石创,2017-09-26
+300707,威唐工业,2017-10-10
+300708,聚灿光电,2017-10-16
+300709,精研科技,2017-10-19
+300710,万隆光电,2017-10-19
+300711,广哈通信,2017-11-01
+300712,永福股份,2017-10-31
+300713,英可瑞,2017-11-01
+300715,凯伦股份,2017-10-26
+300716,泉为科技,2017-11-09
+300717,华信新材,2017-11-06
+300718,长盛轴承,2017-11-06
+300719,安达维尔,2017-11-09
+300720,海川智能,2017-11-06
+300721,怡达股份,2017-11-15
+300722,新余国科,2017-11-10
+300723,一品红,2017-11-16
+300724,捷佳伟创,2018-08-10
+300725,药石科技,2017-11-10
+300726,宏达电子,2017-11-21
+300727,润禾材料,2017-11-27
+300729,乐歌股份,2017-12-01
+300730,科创信息,2017-12-05
+300731,科创新源,2017-12-08
+300732,设研院,2017-12-12
+300733,西菱动力,2018-01-16
+300735,光弘科技,2017-12-29
+300736,百邦科技,2018-01-09
+300737,科顺股份,2018-01-25
+300738,奥飞数据,2018-01-19
+300739,明阳电路,2018-02-01
+300740,水羊股份,2018-02-08
+300741,华宝股份,2018-03-01
+300742,*ST越博,2018-05-08
+300743,天地数码,2018-04-27
+300745,欣锐科技,2018-05-23
+300746,汉嘉设计,2018-05-25
+300747,锐科激光,2018-06-25
+300748,金力永磁,2018-09-21
+300749,顶固集创,2018-09-25
+300750,宁德时代,2018-06-11
+300751,迈为股份,2018-11-09
+300752,隆利科技,2018-11-30
+300753,爱朋医疗,2018-12-13
+300755,华致酒行,2019-01-29
+300756,金马游乐,2018-12-28
+300757,罗博特科,2019-01-08
+300758,七彩化学,2019-02-22
+300759,康龙化成,2019-01-28
+300760,迈瑞医疗,2018-10-16
+300761,立华股份,2019-02-18
+300762,上海瀚讯,2019-03-14
+300763,锦浪科技,2019-03-19
+300765,新诺威,2019-03-22
+300766,每日互动,2019-03-25
+300767,震安科技,2019-03-29
+300768,迪普科技,2019-04-12
+300769,德方纳米,2019-04-15
+300770,新媒股份,2019-04-19
+300771,智莱科技,2019-04-22
+300772,运达股份,2019-04-26
+300773,拉卡拉,2019-04-25
+300774,倍杰特,2021-08-04
+300775,三角防务,2019-05-21
+300776,帝尔激光,2019-05-17
+300777,中简科技,2019-05-16
+300778,新城市,2019-05-10
+300779,惠城环保,2019-05-22
+300780,德恩精工,2019-05-31
+300781,因赛集团,2019-06-06
+300782,卓胜微,2019-06-18
+300783,三只松鼠,2019-07-12
+300785,值得买,2019-07-15
+300786,国林科技,2019-07-23
+300787,海能实业,2019-08-15
+300788,中信出版,2019-07-05
+300789,唐源电气,2019-08-28
+300790,宇瞳光学,2019-09-20
+300791,仙乐健康,2019-09-25
+300792,壹网壹创,2019-09-27
+300793,佳禾智能,2019-10-18
+300795,米奥会展,2019-10-22
+300796,贝斯美,2019-11-15
+300797,钢研纳克,2019-11-01
+300798,锦鸡股份,2019-11-22
+300799,*ST左江,2019-10-29
+300800,力合科技,2019-11-06
+300801,泰和科技,2019-11-28
+300802,矩子科技,2019-11-14
+300803,指南针,2019-11-18
+300804,广康生化,2023-06-27
+300805,电声股份,2019-11-21
+300806,斯迪克,2019-11-25
+300807,天迈科技,2019-12-19
+300808,久量股份,2019-11-29
+300809,华辰装备,2019-12-04
+300810,中科海讯,2019-12-06
+300811,铂科新材,2019-12-30
+300812,易天股份,2020-01-09
+300813,泰林生物,2020-01-14
+300814,中富电路,2021-08-12
+300815,玉禾田,2020-01-23
+300816,艾可蓝,2020-02-10
+300817,双飞股份,2020-02-18
+300818,耐普矿机,2020-02-12
+300819,聚杰微纤,2020-03-12
+300820,英杰电气,2020-02-13
+300821,东岳硅材,2020-03-12
+300822,贝仕达克,2020-03-13
+300823,建科机械,2020-03-19
+300824,北鼎股份,2020-06-19
+300825,阿尔特,2020-03-27
+300826,测绘股份,2020-04-03
+300827,上能电气,2020-04-10
+300828,锐新科技,2020-04-21
+300829,金丹科技,2020-04-22
+300830,金现代,2020-05-06
+300831,派瑞股份,2020-05-07
+300832,新产业,2020-05-12
+300833,浩洋股份,2020-05-20
+300834,星辉环材,2022-01-13
+300835,龙磁科技,2020-05-25
+300836,佰奥智能,2020-05-28
+300837,浙矿股份,2020-06-05
+300838,浙江力诺,2020-06-08
+300839,博汇股份,2020-06-30
+300840,酷特智能,2020-07-08
+300841,康华生物,2020-06-16
+300842,帝科股份,2020-06-18
+300843,胜蓝股份,2020-07-02
+300844,山水比德,2021-08-13
+300845,捷安高科,2020-07-03
+300846,首都在线,2020-07-01
+300847,中船汉光,2020-07-09
+300848,美瑞新材,2020-07-20
+300849,锦盛新材,2020-07-10
+300850,新强联,2020-07-13
+300851,交大思诺,2020-07-17
+300852,四会富仕,2020-07-13
+300853,申昊科技,2020-07-24
+300854,中兰环保,2021-09-16
+300855,图南股份,2020-07-23
+300856,科思股份,2020-07-22
+300857,协创数据,2020-07-27
+300858,科拓生物,2020-07-27
+300859,*ST西域,2020-08-06
+300860,锋尚文化,2020-08-24
+300861,美畅股份,2020-08-24
+300862,蓝盾光电,2020-08-24
+300863,卡倍亿,2020-08-24
+300864,南大环境,2020-08-24
+300865,大宏立,2020-08-24
+300866,安克创新,2020-08-24
+300867,圣元环保,2020-08-24
+300868,杰美特,2020-08-24
+300869,康泰医学,2020-08-24
+300870,欧陆通,2020-08-24
+300871,回盛生物,2020-08-24
+300872,天阳科技,2020-08-24
+300873,海晨股份,2020-08-24
+300875,捷强装备,2020-08-24
+300876,蒙泰高新,2020-08-24
+300877,金春股份,2020-08-24
+300878,维康药业,2020-08-24
+300879,大叶股份,2020-09-01
+300880,迦南智能,2020-09-01
+300881,盛德鑫泰,2020-09-01
+300882,万胜智能,2020-09-10
+300883,龙利得,2020-09-10
+300884,狄耐克,2020-11-12
+300885,海昌新材,2020-09-10
+300886,华业香料,2020-09-16
+300887,谱尼测试,2020-09-16
+300888,稳健医疗,2020-09-17
+300889,爱克股份,2020-09-16
+300890,翔丰华,2020-09-17
+300891,惠云钛业,2020-09-17
+300892,品渥食品,2020-09-24
+300893,松原股份,2020-09-24
+300894,火星人,2020-12-31
+300895,铜牛信息,2020-09-24
+300896,爱美客,2020-09-28
+300897,山科智能,2020-09-28
+300898,熊猫乳品,2020-10-16
+300899,上海凯鑫,2020-10-16
+300900,广联航空,2020-10-29
+300901,中胤时尚,2020-10-29
+300902,国安达,2020-10-29
+300903,科翔股份,2020-11-05
+300904,威力传动,2023-08-09
+300905,宝丽迪,2020-11-05
+300906,日月明,2020-11-05
+300907,康平科技,2020-11-18
+300908,仲景食品,2020-11-23
+300909,汇创达,2020-11-18
+300910,瑞丰新材,2020-11-27
+300911,亿田智能,2020-12-03
+300912,凯龙高科,2020-12-07
+300913,兆龙互连,2020-12-07
+300915,海融科技,2020-12-02
+300916,朗特智能,2020-12-02
+300917,特发服务,2020-12-21
+300918,南山智尚,2020-12-22
+300919,中伟股份,2020-12-23
+300920,润阳科技,2020-12-25
+300921,南凌科技,2020-12-22
+300922,天秦装备,2020-12-25
+300923,研奥股份,2020-12-24
+300925,法本信息,2020-12-30
+300926,博俊科技,2021-01-07
+300927,江天化学,2021-01-07
+300928,华安鑫创,2021-01-06
+300929,华骐环保,2021-01-20
+300930,屹通新材,2021-01-21
+300931,通用电梯,2021-01-21
+300932,三友联众,2021-01-22
+300933,中辰股份,2021-01-22
+300935,盈建科,2021-01-20
+300936,中英科技,2021-01-26
+300937,药易购,2021-01-27
+300938,信测标准,2021-01-27
+300939,秋田微,2021-01-28
+300940,南极光,2021-02-03
+300941,创识科技,2021-02-09
+300942,易瑞生物,2021-02-09
+300943,春晖智控,2021-02-10
+300945,曼卡龙,2021-02-10
+300946,恒而达,2021-02-08
+300947,德必集团,2021-02-10
+300948,冠中生态,2021-02-25
+300949,奥雅股份,2021-02-26
+300950,德固特,2021-03-03
+300951,博硕科技,2021-02-26
+300952,恒辉安防,2021-03-11
+300953,震裕科技,2021-03-18
+300955,嘉亨家化,2021-03-24
+300956,英力股份,2021-03-26
+300957,贝泰妮,2021-03-25
+300958,建工修复,2021-03-29
+300959,线上线下,2021-03-22
+300960,通业科技,2021-03-29
+300961,深水海纳,2021-03-30
+300962,中金辐照,2021-04-09
+300963,中洲特材,2021-04-09
+300964,本川智能,2021-08-05
+300965,恒宇信通,2021-04-02
+300966,共同药业,2021-04-09
+300967,晓鸣股份,2021-04-13
+300968,格林精密,2021-04-15
+300969,恒帅股份,2021-04-12
+300970,华绿生物,2021-04-12
+300971,博亚精工,2021-04-15
+300972,万辰集团,2021-04-19
+300973,立高食品,2021-04-15
+300975,商络电子,2021-04-21
+300976,达瑞电子,2021-04-19
+300977,深圳瑞捷,2021-04-20
+300978,东箭科技,2021-04-26
+300979,华利集团,2021-04-26
+300980,祥源新材,2021-04-21
+300981,中红医疗,2021-04-27
+300982,苏文电能,2021-04-27
+300983,尤安设计,2021-04-20
+300984,金沃股份,2021-06-18
+300985,致远新能,2021-04-29
+300986,志特新材,2021-04-30
+300987,川网传媒,2021-05-11
+300988,津荣天宇,2021-05-12
+300989,蕾奥规划,2021-05-07
+300990,同飞股份,2021-05-12
+300991,创益通,2021-05-20
+300992,泰福泵业,2021-05-25
+300993,玉马遮阳,2021-05-24
+300994,久祺股份,2021-08-12
+300995,奇德新材,2021-05-26
+300996,普联软件,2021-06-03
+300997,欢乐家,2021-06-02
+300998,宁波方正,2021-06-02
+300999,金龙鱼,2020-10-15
+301000,肇民科技,2021-05-28
+301001,凯淳股份,2021-05-28
+301002,崧盛股份,2021-06-07
+301003,江苏博云,2021-06-01
+301004,嘉益股份,2021-06-25
+301005,超捷股份,2021-06-01
+301006,迈拓股份,2021-06-07
+301007,德迈仕,2021-06-16
+301008,宏昌科技,2021-06-11
+301009,可靠股份,2021-06-17
+301010,晶雪节能,2021-06-18
+301011,华立科技,2021-06-17
+301012,扬电科技,2021-06-22
+301013,利和兴,2021-06-29
+301015,百洋医药,2021-06-30
+301016,雷尔伟,2021-06-30
+301017,漱玉平民,2021-07-05
+301018,申菱环境,2021-07-07
+301019,宁波色母,2021-06-28
+301020,密封科技,2021-07-06
+301021,英诺激光,2021-07-06
+301022,海泰科,2021-07-02
+301023,江南奕帆,2021-07-07
+301024,霍普股份,2021-07-28
+301025,读客文化,2021-07-19
+301026,浩通科技,2021-07-16
+301027,华蓝集团,2021-07-15
+301028,东亚机械,2021-07-20
+301029,怡合达,2021-07-23
+301030,仕净科技,2021-07-22
+301031,中熔电气,2021-07-15
+301032,新柴股份,2021-07-22
+301033,迈普医学,2021-07-26
+301035,润丰股份,2021-07-28
+301036,双乐股份,2021-07-29
+301037,保立佳,2021-07-30
+301038,深水规院,2021-08-04
+301039,中集车辆,2021-07-08
+301040,中环海陆,2021-08-03
+301041,金百泽,2021-08-11
+301042,安联锐视,2021-08-05
+301043,绿岛风,2021-08-11
+301045,天禄科技,2021-08-13
+301046,能辉科技,2021-08-17
+301047,义翘神州,2021-08-16
+301048,金鹰重工,2021-08-18
+301049,超越科技,2021-08-24
+301050,雷电微力,2021-08-24
+301051,信濠光电,2021-08-27
+301052,果麦文化,2021-08-30
+301053,远信工业,2021-09-01
+301055,张小泉,2021-09-06
+301056,森赫股份,2021-09-07
+301057,汇隆新材,2021-09-09
+301058,中粮科工,2021-09-09
+301059,金三江,2021-09-13
+301060,兰卫医学,2021-09-13
+301061,匠心家居,2021-09-13
+301062,上海艾录,2021-09-14
+301063,海锅股份,2021-09-24
+301065,本立科技,2021-09-14
+301066,万事利,2021-09-22
+301067,显盈科技,2021-09-22
+301068,大地海洋,2021-09-28
+301069,凯盛新材,2021-09-27
+301070,开勒股份,2021-09-23
+301071,力量钻石,2021-09-24
+301072,中捷精工,2021-09-29
+301073,君亭酒店,2021-09-30
+301075,多瑞医药,2021-09-29
+301076,新瀚新材,2021-10-11
+301077,星华新材,2021-09-30
+301078,孩子王,2021-10-14
+301079,邵阳液压,2021-10-19
+301080,百普赛斯,2021-10-18
+301081,严牌股份,2021-10-20
+301082,久盛电气,2021-10-27
+301083,百胜智能,2021-10-21
+301085,亚康股份,2021-10-18
+301086,鸿富瀚,2021-10-20
+301087,可孚医疗,2021-10-25
+301088,戎美股份,2021-10-28
+301089,拓新药业,2021-10-27
+301090,华润材料,2021-10-26
+301091,深城交,2021-10-29
+301092,争光股份,2021-11-02
+301093,华兰股份,2021-11-01
+301095,广立微,2022-08-05
+301096,百诚医药,2021-12-20
+301097,天益医疗,2022-04-07
+301098,金埔园林,2021-11-12
+301099,雅创电子,2021-11-22
+301100,风光股份,2021-12-17
+301101,明月镜片,2021-12-16
+301102,兆讯传媒,2022-03-28
+301103,何氏眼科,2022-03-22
+301105,鸿铭股份,2022-12-30
+301106,骏成科技,2022-01-28
+301107,瑜欣电子,2022-05-24
+301108,洁雅股份,2021-12-03
+301109,军信股份,2022-04-13
+301110,青木股份,2022-03-11
+301111,粤万年青,2021-12-07
+301112,信邦智能,2022-06-29
+301113,雅艺科技,2021-12-22
+301115,建科股份,2022-08-31
+301116,益客食品,2022-01-18
+301117,佳缘科技,2022-01-17
+301118,恒光股份,2021-11-18
+301119,正强股份,2021-11-22
+301120,新特电气,2022-04-19
+301121,紫建电子,2022-08-08
+301122,采纳股份,2022-01-26
+301123,奕东电子,2022-01-25
+301125,腾亚精工,2022-06-08
+301126,达嘉维康,2021-12-07
+301127,天源环保,2021-12-30
+301128,强瑞技术,2021-11-10
+301129,瑞纳智能,2021-11-02
+301130,西点药业,2022-02-23
+301131,聚赛龙,2022-03-14
+301132,满坤科技,2022-08-10
+301133,金钟股份,2021-11-26
+301135,瑞德智能,2022-04-12
+301136,招标股份,2022-01-11
+301137,哈焊华通,2022-03-22
+301138,华研精机,2021-12-15
+301139,元道通信,2022-07-08
+301141,中科磁业,2023-04-03
+301148,嘉戎技术,2022-04-21
+301149,隆华新材,2021-11-10
+301150,中一科技,2022-04-21
+301151,冠龙节能,2022-04-11
+301152,天力锂能,2022-08-29
+301153,中科江南,2022-05-18
+301155,海力风电,2021-11-24
+301156,美农生物,2022-06-17
+301157,华塑科技,2023-03-09
+301158,德石股份,2022-01-17
+301159,三维天地,2022-01-07
+301160,翔楼新材,2022-06-06
+301161,唯万密封,2022-09-14
+301162,国能日新,2022-04-29
+301163,宏德股份,2022-04-19
+301165,锐捷网络,2022-11-21
+301166,优宁维,2021-12-28
+301167,建研设计,2021-12-06
+301168,通灵股份,2021-12-10
+301169,零点有数,2021-11-03
+301170,锡南科技,2023-06-27
+301171,易点天下,2022-08-19
+301172,君逸数码,2023-07-26
+301175,中科环保,2022-07-08
+301176,逸豪新材,2022-09-28
+301177,迪阿股份,2021-12-15
+301178,天亿马,2021-11-12
+301179,泽宇智能,2021-12-08
+301180,万祥科技,2021-11-16
+301181,标榜股份,2022-02-21
+301182,凯旺科技,2021-12-23
+301183,东田微,2022-05-24
+301185,鸥玛软件,2021-11-19
+301186,超达装备,2021-12-23
+301187,欧圣电气,2022-04-22
+301188,力诺特玻,2021-11-11
+301189,奥尼电子,2021-12-28
+301190,善水科技,2021-12-24
+301191,菲菱科思,2022-05-26
+301192,泰祥股份,2022-08-11
+301193,家联科技,2021-12-09
+301195,北路智控,2022-08-01
+301196,唯科科技,2022-01-11
+301197,工大科雅,2022-08-08
+301198,喜悦智行,2021-12-02
+301199,迈赫股份,2021-12-07
+301200,大族数控,2022-02-28
+301201,诚达药业,2022-01-20
+301202,朗威股份,2023-07-05
+301203,国泰环保,2023-04-04
+301205,联特科技,2022-09-13
+301206,三元生物,2022-02-10
+301207,华兰疫苗,2022-02-18
+301208,中亦科技,2022-07-07
+301209,联合化学,2022-08-25
+301210,金杨股份,2023-06-30
+301211,亨迪药业,2021-12-22
+301212,联盛化学,2022-04-19
+301213,观想科技,2021-12-06
+301215,中汽股份,2022-03-08
+301216,万凯新材,2022-03-29
+301217,铜冠铜箔,2022-01-27
+301218,华是科技,2022-03-07
+301219,腾远钴业,2022-03-17
+301220,亚香股份,2022-06-22
+301221,光庭信息,2021-12-22
+301222,浙江恒威,2022-03-09
+301223,中荣股份,2022-10-26
+301225,恒勃股份,2023-06-16
+301226,祥明智能,2022-03-25
+301227,森鹰窗业,2022-09-26
+301228,实朴检测,2022-01-28
+301229,纽泰格,2022-02-22
+301230,泓博医药,2022-11-01
+301231,荣信文化,2022-09-08
+301232,飞沃科技,2023-06-15
+301233,盛帮股份,2022-07-06
+301234,五洲医疗,2022-07-05
+301235,华康医疗,2022-01-28
+301236,软通动力,2022-03-15
+301237,和顺科技,2022-03-23
+301238,瑞泰新材,2022-06-17
+301239,普瑞眼科,2022-07-05
+301246,宏源药业,2023-03-20
+301248,杰创智能,2022-04-20
+301251,威尔高,2023-09-06
+301252,同星科技,2023-05-25
+301255,通力科技,2022-12-27
+301256,华融化学,2022-03-22
+301257,普蕊斯,2022-05-17
+301258,富士莱,2022-03-29
+301259,艾布鲁,2022-04-26
+301260,格力博,2023-02-08
+301261,恒工精密,2023-07-10
+301262,海看股份,2023-06-20
+301263,泰恩康,2022-03-29
+301265,华新环保,2022-12-16
+301266,宇邦新材,2022-06-08
+301267,华厦眼科,2022-11-07
+301268,铭利达,2022-04-07
+301269,华大九天,2022-07-29
+301270,汉仪股份,2022-08-31
+301272,英华特,2023-07-13
+301273,瑞晨环保,2022-10-25
+301276,嘉曼服饰,2022-09-09
+301277,新天地,2022-11-16
+301278,快可电子,2022-08-04
+301279,金道科技,2022-04-13
+301280,珠城科技,2022-12-26
+301281,科源制药,2023-04-04
+301282,金禄电子,2022-08-26
+301283,聚胶股份,2022-09-02
+301285,鸿日达,2022-09-28
+301286,侨源股份,2022-06-14
+301287,康力源,2023-06-14
+301288,清研环境,2022-04-22
+301289,国缆检测,2022-06-22
+301290,东星医疗,2022-11-30
+301291,明阳电气,2023-06-30
+301292,海科新源,2023-07-07
+301293,三博脑科,2023-05-05
+301295,美硕科技,2023-06-28
+301296,新巨丰,2022-09-02
+301297,富乐德,2022-12-30
+301298,东利机械,2022-06-06
+301299,卓创资讯,2022-10-19
+301300,远翔新材,2022-08-19
+301301,川宁生物,2022-12-27
+301302,华如科技,2022-06-23
+301303,真兰仪表,2023-02-20
+301305,朗坤环境,2023-05-23
+301306,西测测试,2022-07-26
+301307,美利信,2023-04-24
+301308,江波龙,2022-08-05
+301309,万得凯,2022-09-19
+301310,鑫宏业,2023-06-02
+301311,昆船智能,2022-11-30
+301312,智立方,2022-07-11
+301313,凡拓数创,2022-09-30
+301314,科瑞思,2023-03-28
+301315,威士顿,2023-06-21
+301316,慧博云通,2022-10-13
+301317,鑫磊股份,2023-01-19
+301318,维海德,2022-08-10
+301319,唯特偶,2022-09-29
+301320,豪江智能,2023-06-09
+301321,翰博高新,2022-08-18
+301322,绿通科技,2023-03-06
+301323,新莱福,2023-06-06
+301325,曼恩斯特,2023-05-12
+301326,捷邦科技,2022-09-21
+301327,华宝新能,2022-09-19
+301328,维峰电子,2022-09-08
+301329,信音电子,2023-07-17
+301330,熵基科技,2022-08-17
+301331,恩威医药,2022-09-21
+301332,德尔玛,2023-05-18
+301333,诺思格,2022-08-02
+301335,天元宠物,2022-11-18
+301336,趣睡科技,2022-08-12
+301337,亚华电子,2023-05-26
+301338,凯格精机,2022-08-16
+301339,通行宝,2022-09-09
+301345,涛涛车业,2023-03-21
+301348,蓝箭电子,2023-08-10
+301349,信德新材,2022-09-09
+301353,普莱得,2023-05-30
+301355,南王科技,2023-06-12
+301356,天振股份,2022-11-14
+301357,北方长龙,2023-04-18
+301358,湖南裕能,2023-02-09
+301359,东南电子,2022-11-09
+301360,荣旗科技,2023-04-25
+301361,众智科技,2022-11-16
+301362,民爆光电,2023-08-04
+301363,美好医疗,2022-10-12
+301365,矩阵股份,2022-11-22
+301366,一博科技,2022-09-26
+301367,怡和嘉业,2022-11-01
+301368,丰立智能,2022-12-15
+301369,联动科技,2022-09-22
+301370,国科恒泰,2023-07-12
+301371,敷尔佳,2023-08-01
+301372,科净源,2023-08-11
+301373,凌玮科技,2023-02-08
+301376,致欧科技,2023-06-21
+301377,鼎泰高科,2022-11-22
+301378,通达海,2023-03-20
+301379,天山电子,2022-11-01
+301380,挖金客,2022-10-25
+301381,赛维时代,2023-07-12
+301382,蜂助手,2023-05-17
+301383,天键股份,2023-06-09
+301386,未来电器,2023-03-29
+301387,光大同创,2023-04-18
+301388,欣灵电气,2022-11-09
+301389,隆扬电子,2022-10-31
+301390,经纬股份,2023-05-08
+301391,卡莱特,2022-12-01
+301393,昊帆生物,2023-07-12
+301395,仁信新材,2023-07-03
+301396,宏景科技,2022-11-11
+301397,溯联股份,2023-06-28
+301398,星源卓镁,2022-12-15
+301399,英特科技,2023-05-23
+301408,华人健康,2023-03-01
+301418,协昌科技,2023-08-21
+301419,阿莱德,2023-02-09
+301421,波长光电,2023-08-23
+301428,世纪恒通,2023-05-19
+301429,森泰股份,2023-04-17
+301439,泓淋电力,2023-03-17
+301446,福事特,2023-07-25
+301448,开创电气,2023-06-19
+301456,盘古智能,2023-07-14
+301468,博盈特焊,2023-07-24
+301469,恒达新材,2023-08-22
+301486,致尚科技,2023-07-07
+301487,盟固利,2023-08-09
+301488,豪恩汽电,2023-07-04
+301498,乖宝宠物,2023-08-16
+301499,维科精密,2023-07-21
+301500,飞南资源,2023-09-21
+301503,智迪科技,2023-07-17
+301505,苏州规划,2023-07-19
+301507,民生健康,2023-09-05
+301509,金凯生科,2023-08-03
+301510,固高科技,2023-08-15
+301511,德福科技,2023-08-17
+301512,智信精密,2023-07-20
+301515,港通医疗,2023-07-25
+301517,陕西华达,2023-10-17
+301518,长华化学,2023-08-03
+301519,舜禹股份,2023-07-27
+301520,万邦医药,2023-09-25
+301525,儒竞科技,2023-08-30
+301528,多浦乐,2023-08-28
+301529,福赛科技,2023-09-11
+301533,威马农机,2023-08-18
+301548,崇德科技,2023-09-20
+301550,斯菱股份,2023-09-15
+301558,三态股份,2023-09-28
+301559,中集环科,2023-10-11
+430017,星昊医药,2023-05-31
+430047,诺思兰德,2020-11-24
+430090,同辉信息,2021-08-09
+430139,华岭股份,2022-10-28
+430198,微创光电,2020-07-27
+430300,辰光医疗,2022-12-07
+430418,苏轴股份,2020-07-27
+430425,乐创技术,2023-01-30
+430476,海能技术,2022-10-14
+430478,峆一药业,2023-02-23
+430489,佳先股份,2020-07-27
+430510,丰光精密,2020-12-28
+430556,雅达股份,2023-03-17
+430564,天润科技,2022-06-17
+430685,新芝生物,2022-10-10
+430718,合肥高科,2022-12-22
+600000,浦发银行,1999-11-10
+600001,邯郸钢铁,
+600002,齐鲁石化,
+600003,ST东北高,
+600004,白云机场,2003-04-28
+600005,武钢股份,
+600006,东风汽车,1999-07-27
+600007,中国国贸,1999-03-12
+600008,首创环保,2000-04-27
+600009,上海机场,1998-02-18
+600010,包钢股份,2001-03-09
+600011,华能国际,2001-12-06
+600012,皖通高速,2003-01-07
+600015,华夏银行,2003-09-12
+600016,民生银行,2000-12-19
+600017,日照港  ,2006-10-17
+600018,上港集团,2000-07-19
+600019,宝钢股份,2000-12-12
+600020,中原高速,2003-08-08
+600021,上海电力,2003-10-29
+600022,山东钢铁,2004-06-29
+600023,浙能电力,2013-12-19
+600025,华能水电,2017-12-15
+600026,中远海能,2002-05-23
+600027,华电国际,2005-02-03
+600028,中国石化,2001-08-08
+600029,南方航空,2003-07-25
+600030,中信证券,2003-01-06
+600031,三一重工,2003-07-03
+600032,浙江新能,2021-05-25
+600033,福建高速,2001-02-09
+600035,楚天高速,2004-03-10
+600036,招商银行,2002-04-09
+600037,歌华有线,2001-02-08
+600038,中直股份,2000-12-18
+600039,四川路桥,2003-03-25
+600048,保利发展,2006-07-31
+600050,中国联通,2002-10-09
+600051,宁波联合,1997-04-10
+600052,东望时代,1997-04-15
+600053,九鼎投资,1997-04-18
+600054,黄山旅游,1997-05-06
+600055,万东医疗,1997-05-19
+600056,中国医药,1997-05-15
+600057,厦门象屿,1997-06-04
+600058,五矿发展,1997-05-28
+600059,古越龙山,1997-05-16
+600060,海信视像,1997-04-22
+600061,国投资本,1997-05-19
+600062,华润双鹤,1997-05-22
+600063,皖维高新,1997-05-28
+600064,南京高科,1997-05-06
+600065,*ST联谊,
+600066,宇通客车,1997-05-08
+600067,冠城大通,1997-05-08
+600068,葛洲坝,
+600069,退市银鸽,
+600070,ST富润  ,1997-06-04
+600071,凤凰光学,1997-05-28
+600072,中船科技,1997-06-03
+600073,上海梅林,1997-07-04
+600074,退市保千,
+600075,新疆天业,1997-06-17
+600076,康欣新材,1997-05-26
+600077,*ST宋都,
+600078,ST澄星  ,1997-06-27
+600079,人福医药,1997-06-06
+600080,金花股份,1997-06-12
+600081,东风科技,1997-07-03
+600082,海泰发展,1997-06-20
+600083,博信股份,1997-06-06
+600084,中葡股份,1997-07-11
+600085,同仁堂  ,1997-06-25
+600086,退市金钰,
+600087,退市长油,
+600088,中视传媒,1997-06-16
+600089,特变电工,1997-06-18
+600090,退市济堂,
+600091,退市明科,
+600092,S*ST精密,
+600093,退市易见,
+600094,大名城  ,1997-07-03
+600095,湘财股份,1997-07-08
+600096,云天化  ,1997-07-09
+600097,开创国际,1997-06-19
+600098,广州发展,1997-07-18
+600099,林海股份,1997-07-04
+600100,同方股份,1997-06-27
+600101,明星电力,1997-06-27
+600102,莱钢股份,
+600103,青山纸业,1997-07-03
+600104,上汽集团,1997-11-25
+600105,永鼎股份,1997-09-29
+600106,重庆路桥,1997-06-18
+600107,美尔雅  ,1997-11-06
+600108,亚盛集团,1997-08-18
+600109,国金证券,1997-08-07
+600110,诺德股份,1997-10-07
+600111,北方稀土,1997-09-24
+600112,ST天成  ,1997-11-27
+600113,浙江东日,1997-10-21
+600114,东睦股份,2004-05-11
+600115,中国东航,1997-11-05
+600116,三峡水利,1997-08-04
+600117,*ST西钢 ,1997-10-15
+600118,中国卫星,1997-09-08
+600119,长江投资,1998-01-15
+600120,浙江东方,1997-12-01
+600121,郑州煤电,1998-01-07
+600122,*ST宏图,
+600123,兰花科创,1998-12-17
+600125,铁龙物流,1998-05-11
+600126,杭钢股份,1998-03-11
+600127,金健米业,1998-05-06
+600128,苏豪弘业,1997-09-01
+600129,太极集团,1997-11-18
+600130,波导股份,2000-07-06
+600131,国网信通,1998-04-02
+600132,重庆啤酒,1997-10-30
+600133,东湖高新,1998-02-12
+600135,乐凯胶片,1998-01-22
+600136,*ST明诚 ,1998-03-03
+600137,浪莎股份,1998-04-16
+600138,中青旅  ,1997-12-03
+600139,*ST西源,
+600141,兴发集团,1999-06-16
+600143,金发科技,2004-06-23
+600145,退市新亿,
+600146,退市环球,
+600148,长春一东,1998-05-20
+600149,廊坊发展,1999-10-14
+600150,中国船舶,1998-05-20
+600151,航天机电,1998-06-05
+600152,维科技术,1998-06-09
+600153,建发股份,1998-06-16
+600155,华创云信,1998-09-18
+600156,华升股份,1998-05-27
+600157,永泰能源,1998-05-13
+600158,中体产业,1998-03-27
+600159,大龙地产,1998-05-26
+600160,巨化股份,1998-06-26
+600161,天坛生物,1998-06-16
+600162,香江控股,1998-06-09
+600163,中闽能源,1998-06-02
+600165,宁科生物,1998-05-29
+600166,福田汽车,1998-06-02
+600167,联美控股,1999-01-28
+600168,武汉控股,1998-04-27
+600169,太原重工,1998-09-04
+600170,上海建工,1998-06-23
+600171,上海贝岭,1998-09-24
+600172,黄河旋风,1998-11-26
+600173,卧龙地产,1999-04-15
+600175,退市美都,
+600176,中国巨石,1999-04-22
+600177,雅戈尔  ,1998-11-19
+600178,东安动力,1998-10-14
+600179,安通控股,1998-11-04
+600180,瑞茂通  ,1998-07-03
+600181,S*ST云大,
+600182,S佳通   ,1999-05-07
+600183,生益科技,1998-10-28
+600184,光电股份,2003-11-06
+600185,格力地产,1999-06-11
+600186,莲花健康,1998-08-25
+600187,国中水务,1998-11-11
+600188,兖矿能源,1998-07-01
+600189,泉阳泉  ,1998-10-07
+600190,锦州港  ,1999-06-09
+600191,华资实业,1998-12-10
+600192,长城电工,1998-12-24
+600193,创兴资源,1999-05-27
+600195,中牧股份,1999-01-07
+600196,复星医药,1998-08-07
+600197,伊力特  ,1999-09-16
+600198,大唐电信,1998-10-21
+600199,金种子酒,1998-08-12
+600200,江苏吴中,1999-04-01
+600201,生物股份,1999-01-15
+600202,哈空调  ,1999-06-03
+600203,福日电子,1999-05-14
+600205,S山东铝,
+600206,有研新材,1999-03-19
+600207,安彩高科,1999-07-14
+600208,新湖中宝,1999-06-23
+600209,退市罗顿,
+600210,紫江企业,1999-08-24
+600211,西藏药业,1999-07-21
+600212,绿能慧充,1999-08-17
+600213,亚星客车,1999-08-31
+600215,派斯林  ,1999-09-09
+600216,浙江医药,1999-10-21
+600217,中再资环,1999-12-16
+600218,全柴动力,1998-12-03
+600219,南山铝业,1999-12-23
+600220,江苏阳光,1999-09-27
+600221,海航控股,1999-11-25
+600222,太龙药业,1999-11-05
+600223,福瑞达  ,2000-01-13
+600225,卓朗科技,2000-01-27
+600226,瀚叶股份,1999-11-16
+600227,赤天化  ,2000-02-21
+600228,返利科技,1999-01-19
+600229,城市传媒,2000-03-09
+600230,沧州大化,2000-04-06
+600231,凌钢股份,2000-05-11
+600232,金鹰股份,2000-06-02
+600233,圆通速递,2000-06-08
+600234,科新发展,2000-06-15
+600235,民丰特纸,2000-06-15
+600236,桂冠电力,2000-03-23
+600237,铜峰电子,2000-06-09
+600238,海南椰岛,2000-01-20
+600239,云南城投,1999-12-02
+600240,退市华业,
+600241,时代万恒,2000-11-28
+600242,退市中昌,
+600243,青海华鼎,2000-11-20
+600246,万通发展,2000-09-22
+600247,*ST成城,
+600248,陕建股份,2000-06-22
+600249,两面针  ,2004-01-30
+600250,南纺股份,2001-03-06
+600251,冠农股份,2003-06-09
+600252,中恒集团,2000-11-30
+600253,天方药业,
+600255,鑫科材料,2000-11-22
+600256,广汇能源,2000-05-26
+600257,大湖股份,2000-06-12
+600258,首旅酒店,2000-06-01
+600259,广晟有色,2000-05-25
+600260,*ST凯乐,
+600261,阳光照明,2000-07-20
+600262,北方股份,2000-06-30
+600263,路桥建设,
+600265,ST景谷  ,2000-08-25
+600266,城建发展,1999-02-03
+600267,海正药业,2000-07-25
+600268,国电南自,1999-11-18
+600269,赣粤高速,2000-05-18
+600270,外运发展,
+600271,航天信息,2003-07-11
+600272,开开实业,2001-02-28
+600273,嘉化能源,2003-06-27
+600275,退市昌鱼,
+600276,恒瑞医药,2000-10-18
+600277,亿利洁能,2000-07-25
+600278,东方创业,2000-07-12
+600279,重庆港  ,2000-07-31
+600280,中央商场,2000-09-26
+600281,华阳新材,2000-11-09
+600282,南钢股份,2000-09-19
+600283,钱江水利,2000-10-18
+600284,浦东建设,2004-03-16
+600285,羚锐制药,2000-10-18
+600286,S*ST国瓷,
+600287,江苏舜天,2000-09-01
+600288,大恒科技,2000-11-29
+600289,ST信通  ,2000-07-20
+600290,*ST华仪 ,2000-11-06
+600291,退市西水,
+600292,远达环保,2000-11-01
+600293,三峡新材,2000-09-19
+600295,鄂尔多斯,2001-04-26
+600296,S兰铝,
+600297,广汇汽车,2000-11-16
+600298,安琪酵母,2000-08-18
+600299,安迪苏  ,2000-04-20
+600300,维维股份,2000-06-30
+600301,华锡有色,2000-07-12
+600302,标准股份,2000-12-13
+600303,ST曙光  ,2000-12-26
+600305,恒顺醋业,2001-02-06
+600306,*ST商城 ,2000-12-26
+600307,酒钢宏兴,2000-12-20
+600308,华泰股份,2000-09-28
+600309,万华化学,2001-01-05
+600310,广西能源,2001-02-28
+600311,*ST荣华,
+600312,平高电气,2001-02-21
+600313,农发种业,2001-01-19
+600315,上海家化,2001-03-15
+600316,洪都航空,2000-12-15
+600317,营口港,
+600318,新力金融,2000-12-08
+600319,亚星化学,2001-03-26
+600320,振华重工,2000-12-21
+600321,正源股份,2001-05-24
+600322,津投城开,2001-09-10
+600323,瀚蓝环境,2000-12-25
+600325,华发股份,2004-02-25
+600326,西藏天路,2001-01-16
+600327,大东方  ,2002-06-25
+600328,中盐化工,2000-12-22
+600329,达仁堂  ,2001-06-06
+600330,天通股份,2001-01-18
+600331,宏达股份,2001-12-20
+600332,白云山  ,2001-02-06
+600333,长春燃气,2000-12-11
+600335,国机汽车,2001-03-05
+600336,澳柯玛  ,2000-12-29
+600337,美克家居,2000-11-27
+600338,西藏珠峰,2000-12-27
+600339,中油工程,2000-12-25
+600340,华夏幸福,2003-12-30
+600343,航天动力,2003-04-08
+600345,长江通信,2000-12-22
+600346,恒力石化,2001-08-20
+600348,华阳股份,2003-08-21
+600350,山东高速,2002-03-18
+600351,亚宝药业,2002-09-26
+600352,浙江龙盛,2003-08-01
+600353,旭光电子,2002-11-20
+600354,敦煌种业,2004-01-15
+600355,精伦电子,2002-06-13
+600356,恒丰纸业,2001-04-19
+600357,承德钒钛,
+600358,国旅联合,2000-09-22
+600359,新农开发,1999-04-29
+600360,华微电子,2001-03-16
+600361,创新新材,2001-11-29
+600362,江西铜业,2002-01-11
+600363,联创光电,2001-03-29
+600365,ST通葡  ,2001-01-15
+600366,宁波韵升,2000-10-30
+600367,红星发展,2001-03-20
+600368,五洲交通,2000-12-21
+600369,西南证券,2001-01-09
+600370,三房巷  ,2003-03-06
+600371,万向德农,2002-09-16
+600372,中航机载,2001-07-06
+600373,中文传媒,2002-03-04
+600375,汉马科技,2003-04-01
+600376,首开股份,2001-03-12
+600377,宁沪高速,2001-01-16
+600378,昊华科技,2001-01-11
+600379,宝光股份,2002-01-16
+600380,健康元  ,2001-06-08
+600381,青海春天,2001-05-08
+600382,广东明珠,2001-01-18
+600383,金地集团,2001-04-12
+600385,退市金泰,
+600386,北巴传媒,2001-02-16
+600387,ST海越  ,2004-02-18
+600388,龙净环保,2000-12-29
+600389,江山股份,2001-01-10
+600390,五矿资本,2001-01-15
+600391,航发科技,2001-12-12
+600392,盛和资源,2003-05-29
+600393,ST粤泰,
+600395,盘江股份,2001-05-31
+600396,*ST金山 ,2001-03-28
+600397,安源煤业,2002-07-02
+600398,海澜之家,2000-12-28
+600399,抚顺特钢,2000-12-29
+600400,红豆股份,2001-01-08
+600401,退市海润,
+600403,大有能源,2003-10-09
+600405,动力源  ,2004-04-01
+600406,国电南瑞,2003-10-16
+600408,安泰集团,2003-02-12
+600409,三友化工,2003-06-18
+600410,华胜天成,2004-04-27
+600415,小商品城,2002-05-09
+600416,湘电股份,2002-07-18
+600418,江淮汽车,2001-08-24
+600419,天润乳业,2001-06-28
+600420,国药现代,2004-06-16
+600421,华嵘控股,2004-06-07
+600422,昆药集团,2000-12-06
+600423,柳化股份,2003-07-17
+600425,青松建化,2003-07-24
+600426,华鲁恒升,2002-06-20
+600428,中远海特,2002-04-18
+600429,三元股份,2003-09-15
+600432,退市吉恩,
+600433,冠豪高新,2003-06-19
+600435,北方导航,2003-07-04
+600436,片仔癀  ,2003-06-16
+600438,通威股份,2004-03-02
+600439,瑞贝卡  ,2003-07-10
+600444,国机通用,2004-02-19
+600446,金证股份,2003-12-24
+600448,华纺股份,2001-09-03
+600449,宁夏建材,2003-08-29
+600452,涪陵电力,2004-03-03
+600455,博通股份,2004-03-29
+600456,宝钛股份,2002-04-12
+600458,时代新材,2002-12-19
+600459,贵研铂业,2003-05-16
+600460,士兰微  ,2003-03-11
+600461,洪城环境,2004-06-01
+600462,ST九有  ,2003-09-03
+600463,空港股份,2004-03-18
+600466,*ST蓝光,
+600467,好当家  ,2004-04-05
+600468,百利电气,2001-06-15
+600469,风神股份,2003-10-21
+600470,六国化工,2004-03-05
+600472,包头铝业,
+600475,华光环能,2003-07-21
+600476,湘邮科技,2003-12-10
+600477,杭萧钢构,2003-11-10
+600478,科力远  ,2003-09-18
+600479,千金药业,2004-03-12
+600480,凌云股份,2003-08-15
+600481,双良节能,2003-04-22
+600482,中国动力,2004-07-14
+600483,福能股份,2004-05-31
+600485,*ST信威,
+600486,扬农化工,2002-04-25
+600487,亨通光电,2003-08-22
+600488,津药药业,2001-06-18
+600489,中金黄金,2003-08-14
+600490,鹏欣资源,2003-06-26
+600491,龙元建设,2004-05-24
+600493,凤竹纺织,2004-04-21
+600495,晋西车轴,2004-05-26
+600496,精工钢构,2002-06-05
+600497,驰宏锌锗,2004-04-20
+600498,烽火通信,2001-08-23
+600499,科达制造,2002-10-10
+600500,中化国际,2000-03-01
+600501,航天晨光,2001-06-15
+600502,安徽建工,2003-04-15
+600503,华丽家族,2002-07-09
+600505,西昌电力,2002-05-30
+600506,统一股份,2001-12-26
+600507,方大特钢,2003-09-30
+600508,上海能源,2001-08-29
+600509,天富能源,2002-02-28
+600510,黑牡丹  ,2002-06-18
+600511,国药股份,2002-11-27
+600512,腾达建设,2002-12-26
+600513,联环药业,2003-03-19
+600515,海南机场,2002-08-06
+600516,方大炭素,2002-08-30
+600517,国网英大,2003-10-10
+600518,ST康美  ,2001-03-19
+600519,贵州茅台,2001-08-27
+600520,文一科技,2002-01-08
+600521,华海药业,2003-03-04
+600522,中天科技,2002-10-24
+600523,贵航股份,2001-12-27
+600525,长园集团,2002-12-02
+600526,菲达环保,2002-07-22
+600527,江南高纤,2003-11-27
+600528,中铁工业,2001-05-28
+600529,山东药玻,2002-06-03
+600530,ST交昂  ,2001-07-02
+600531,豫光金铅,2002-07-30
+600532,退市未来,
+600533,栖霞建设,2002-03-28
+600535,天士力  ,2002-08-23
+600536,中国软件,2002-05-17
+600537,亿晶光电,2003-01-23
+600538,国发股份,2003-01-14
+600539,狮头股份,2001-08-24
+600540,新赛股份,2004-01-07
+600543,*ST莫高 ,2004-03-24
+600545,卓郎智能,2003-12-03
+600546,山煤国际,2003-07-31
+600547,山东黄金,2003-08-28
+600548,深高速  ,2001-12-25
+600549,厦门钨业,2002-11-07
+600550,保变电气,2001-02-28
+600551,时代出版,2002-09-05
+600552,凯盛科技,2002-11-08
+600553,太行水泥,
+600555,退市海创,
+600556,天下秀  ,2001-08-07
+600557,康缘药业,2002-09-18
+600558,大西洋  ,2001-02-27
+600559,老白干酒,2002-10-29
+600560,金自天正,2002-09-19
+600561,江西长运,2002-07-16
+600562,国睿科技,2003-01-28
+600563,法拉电子,2002-12-10
+600565,迪马股份,2002-07-23
+600566,济川药业,2001-08-22
+600567,山鹰国际,2001-12-18
+600568,ST中珠  ,2001-05-18
+600569,安阳钢铁,2001-08-20
+600570,恒生电子,2003-12-16
+600571,信雅达  ,2002-11-01
+600572,康恩贝  ,2004-04-12
+600573,惠泉啤酒,2003-02-26
+600575,淮河能源,2003-03-28
+600576,祥源文旅,2003-02-20
+600577,精达股份,2002-09-11
+600578,京能电力,2002-05-10
+600579,克劳斯  ,2002-08-09
+600580,卧龙电驱,2002-06-06
+600581,八一钢铁,2002-08-16
+600582,天地科技,2002-05-15
+600583,海油工程,2002-02-05
+600584,长电科技,2003-06-03
+600585,海螺水泥,2002-02-07
+600586,金晶科技,2002-08-15
+600587,新华医疗,2002-09-27
+600588,用友网络,2001-05-18
+600589,*ST榕泰 ,2001-06-12
+600590,泰豪科技,2002-07-03
+600591,*ST上航,
+600592,龙溪股份,2002-08-05
+600593,大连圣亚,2002-07-11
+600594,益佰制药,2004-03-23
+600595,中孚实业,2002-06-26
+600596,新安股份,2001-09-06
+600597,光明乳业,2002-08-28
+600598,北大荒  ,2002-03-29
+600599,ST熊猫  ,2001-08-28
+600600,青岛啤酒,1993-08-27
+600601,方正科技,1990-12-19
+600602,云赛智联,1990-12-19
+600603,广汇物流,1992-01-13
+600604,市北高新,1992-03-27
+600605,汇通能源,1992-03-27
+600606,绿地控股,1992-03-27
+600607,上实医药,
+600608,ST沪科  ,1992-03-27
+600609,金杯汽车,1992-07-24
+600610,中毅达  ,1992-08-05
+600611,大众交通,1992-08-07
+600612,老凤祥  ,1992-08-14
+600613,神奇制药,1992-08-20
+600614,退市鹏起,
+600615,丰华股份,1992-09-10
+600616,金枫酒业,1992-09-29
+600617,国新能源,1992-10-13
+600618,氯碱化工,1992-11-13
+600619,海立股份,1992-11-16
+600620,天宸股份,1992-11-17
+600621,华鑫股份,1992-12-02
+600622,光大嘉宝,1992-12-03
+600623,华谊集团,1992-12-04
+600624,复旦复华,1993-01-05
+600625,PT水仙,
+600626,申达股份,1993-01-07
+600627,上电股份,
+600628,新世界  ,1993-01-19
+600629,华建集团,1993-02-09
+600630,龙头股份,1993-02-09
+600631,百联股份(已合并),
+600632,华联商厦,
+600633,浙数文化,1993-03-04
+600634,退市富控,
+600635,大众公用,1993-03-04
+600636,国新文化,1993-03-16
+600637,东方明珠,1993-03-16
+600638,新黄浦  ,1993-03-26
+600639,浦东金桥,1993-03-26
+600640,国脉文化,1993-04-07
+600641,万业企业,1993-04-07
+600642,申能股份,1993-04-16
+600643,爱建集团,1993-04-26
+600644,乐山电力,1993-04-26
+600645,中源协和,1993-05-04
+600646,ST国嘉,
+600647,*ST同达 ,1993-05-04
+600648,外高桥  ,1993-05-04
+600649,城投控股,1993-05-18
+600650,锦江在线,1993-06-07
+600651,飞乐音响,1990-12-19
+600652,退市游久,
+600653,申华控股,1990-12-19
+600654,ST中安  ,1990-12-19
+600655,豫园股份,1992-09-02
+600656,退市博元,
+600657,信达地产,1993-05-24
+600658,电子城  ,1993-05-24
+600659,*ST花雕,
+600660,福耀玻璃,1993-06-10
+600661,昂立教育,1993-06-14
+600662,外服控股,1993-06-14
+600663,陆家嘴  ,1993-06-28
+600664,哈药股份,1993-06-29
+600665,天地源  ,1993-07-09
+600666,ST瑞德  ,1993-07-12
+600667,太极实业,1993-07-28
+600668,尖峰集团,1993-07-28
+600669,*ST鞍成,
+600670,*ST斯达,
+600671,*ST目药 ,1993-08-23
+600672,*ST华圣,
+600673,东阳光  ,1993-09-17
+600674,川投能源,1993-09-24
+600675,中华企业,1993-09-24
+600676,交运股份,1993-09-28
+600677,*ST航通,
+600678,四川金顶,1993-10-08
+600679,上海凤凰,1993-10-08
+600680,*ST上普,
+600681,百川能源,1993-10-18
+600682,南京新百,1993-10-18
+600683,京投发展,1993-10-25
+600684,珠江股份,1993-10-28
+600685,中船防务,1993-10-28
+600686,金龙汽车,1993-11-08
+600687,退市刚泰,
+600688,上海石化,1993-11-08
+600689,上海三毛,1993-11-08
+600690,海尔智家,1993-11-19
+600691,阳煤化工,1993-11-19
+600692,亚通股份,1993-11-19
+600693,东百集团,1993-11-22
+600694,大商股份,1993-11-22
+600695,退市绿庭,
+600696,岩石股份,1993-12-06
+600697,欧亚集团,1993-12-06
+600698,湖南天雁,1993-12-06
+600699,均胜电子,1993-12-06
+600700,*ST数码,
+600701,退市工新,
+600702,舍得酒业,1996-05-24
+600703,三安光电,1996-05-28
+600704,物产中大,1996-06-06
+600705,中航产融,1996-05-16
+600706,曲江文旅,1996-05-16
+600707,彩虹股份,1996-05-20
+600708,光明地产,1996-06-06
+600709,ST生态,
+600710,苏美达  ,1996-07-01
+600711,盛屯矿业,1996-05-31
+600712,南宁百货,1996-06-26
+600713,南京医药,1996-07-01
+600714,金瑞矿业,1996-06-06
+600715,文投控股,1996-07-01
+600716,凤凰股份,1996-07-02
+600717,天津港  ,1996-06-14
+600718,东软集团,1996-06-18
+600719,大连热电,1996-07-16
+600720,祁连山  ,1996-07-16
+600721,百花医药,1996-06-26
+600722,金牛化工,1996-06-26
+600723,首商股份,
+600724,宁波富达,1996-07-16
+600725,云维股份,1996-07-02
+600726,华电能源,1996-07-01
+600727,鲁北化工,1996-07-02
+600728,佳都科技,1996-07-16
+600729,重庆百货,1996-07-02
+600730,中国高科,1996-07-26
+600731,湖南海利,1996-08-02
+600732,爱旭股份,1996-08-16
+600733,北汽蓝谷,1996-08-16
+600734,ST实达  ,1996-08-08
+600735,新华锦  ,1996-07-26
+600736,苏州高新,1996-08-15
+600737,中粮糖业,1996-07-31
+600738,丽尚国潮,1996-08-02
+600739,辽宁成大,1996-08-19
+600740,山西焦化,1996-08-08
+600741,华域汽车,1996-08-26
+600742,一汽富维,1996-08-26
+600743,华远地产,1996-09-09
+600744,华银电力,1996-09-05
+600745,闻泰科技,1996-08-28
+600746,江苏索普,1996-09-18
+600747,退市大控,
+600748,上实发展,1996-09-25
+600749,西藏旅游,1996-10-15
+600750,江中药业,1996-09-23
+600751,海航科技,1996-09-09
+600752,*ST哈慈,
+600753,庚星股份,1996-09-27
+600754,锦江酒店,1996-10-11
+600755,厦门国贸,1996-10-03
+600756,浪潮软件,1996-09-23
+600757,长江传媒,1996-10-03
+600758,辽宁能源,1996-10-29
+600759,*ST洲际 ,1996-10-08
+600760,中航沈飞,1996-10-11
+600761,安徽合力,1996-10-09
+600762,S*ST金荔,
+600763,通策医疗,1996-10-30
+600764,中国海防,1996-11-04
+600765,中航重机,1996-11-06
+600766,*ST园城 ,1996-10-28
+600767,退市运盛,
+600768,宁波富邦,1996-11-11
+600769,祥龙电业,1996-11-01
+600770,综艺股份,1996-11-20
+600771,广誉远  ,1996-11-05
+600772,S*ST龙昌,
+600773,西藏城投,1996-11-08
+600774,汉商集团,1996-11-08
+600775,南京熊猫,1996-11-18
+600776,东方通信,1996-11-26
+600777,新潮能源,1996-11-21
+600778,友好集团,1996-12-03
+600779,水井坊  ,1996-12-06
+600780,通宝能源,1996-12-05
+600781,退市辅仁,
+600782,新钢股份,1996-12-25
+600783,鲁信创投,1996-12-25
+600784,鲁银投资,1996-12-25
+600785,新华百货,1997-01-08
+600786,东方锅炉,
+600787,中储股份,1997-01-21
+600788,*ST达曼,
+600789,鲁抗医药,1997-02-26
+600790,轻纺城  ,1997-02-28
+600791,京能置业,1997-01-30
+600792,云煤能源,1997-01-23
+600793,宜宾纸业,1997-02-20
+600794,保税科技,1997-03-06
+600795,国电电力,1997-03-18
+600796,钱江生化,1997-04-08
+600797,浙大网新,1997-04-18
+600798,宁波海运,1997-04-23
+600799,*ST龙科,
+600800,渤海化学,1993-12-06
+600801,华新水泥,1994-01-03
+600802,福建水泥,1994-01-03
+600803,新奥股份,1994-01-03
+600804,ST鹏博士,1994-01-03
+600805,悦达投资,1994-01-03
+600806,退市昆机,
+600807,济南高新,1994-01-03
+600808,马钢股份,1994-01-06
+600809,山西汾酒,1994-01-06
+600810,神马股份,1994-01-06
+600811,东方集团,1994-01-06
+600812,华北制药,1994-01-14
+600813,ST鞍一工,
+600814,杭州解百,1994-01-14
+600815,厦工股份,1994-01-28
+600816,ST建元  ,1994-01-28
+600817,宇通重工,1994-01-28
+600818,中路股份,1994-01-28
+600819,耀皮玻璃,1994-01-28
+600820,隧道股份,1994-01-28
+600821,金开新能,1994-01-28
+600822,上海物贸,1994-02-04
+600823,ST世茂  ,1994-02-04
+600824,益民集团,1994-02-04
+600825,新华传媒,1994-02-04
+600826,兰生股份,1994-02-04
+600827,百联股份,1994-02-04
+600828,茂业商业,1994-02-24
+600829,人民同泰,1994-02-24
+600830,香溢融通,1994-02-24
+600831,广电网络,1994-02-24
+600832,东方明珠,
+600833,第一医药,1994-02-24
+600834,申通地铁,1994-02-24
+600835,上海机电,1994-02-24
+600836,上海易连,1994-02-24
+600837,海通证券,1994-02-24
+600838,上海九百,1994-02-24
+600839,四川长虹,1994-03-11
+600840,新湖创业,
+600841,动力新科,1994-03-11
+600842,中西药业,
+600843,上工申贝,1994-03-11
+600844,丹化科技,1994-03-11
+600845,宝信软件,1994-03-11
+600846,同济科技,1994-03-11
+600847,万里股份,1994-03-24
+600848,上海临港,1994-03-24
+600850,电科数字,1994-03-24
+600851,海欣股份,1994-04-04
+600852,*ST中川,
+600853,龙建股份,1994-04-04
+600854,春兰股份,1994-04-25
+600855,航天长峰,1994-04-25
+600856,退市中天,
+600857,宁波中百,1994-04-25
+600858,银座股份,1994-05-06
+600859,王府井  ,1994-05-06
+600860,京城股份,1994-05-06
+600861,北京人力,1994-05-20
+600862,中航高科,1994-05-20
+600863,内蒙华电,1994-05-20
+600864,哈投股份,1994-08-09
+600865,百大集团,1994-08-09
+600866,星湖科技,1994-08-18
+600867,通化东宝,1994-08-24
+600868,梅雁吉祥,1994-09-12
+600869,远东股份,1995-02-06
+600870,退市厦华,
+600871,石化油服,1995-04-11
+600872,中炬高新,1995-01-24
+600873,梅花生物,1995-02-17
+600874,创业环保,1995-06-30
+600875,东方电气,1995-10-10
+600876,凯盛新能,1995-10-31
+600877,电科芯片,1995-10-13
+600878,*ST北科,
+600879,航天电子,1995-11-15
+600880,博瑞传播,1995-11-15
+600881,亚泰集团,1995-11-15
+600882,妙可蓝多,1995-12-06
+600883,博闻科技,1995-12-08
+600884,杉杉股份,1996-01-30
+600885,宏发股份,1996-02-05
+600886,国投电力,1996-01-18
+600887,伊利股份,1996-03-12
+600888,新疆众和,1996-02-15
+600889,南京化纤,1996-03-08
+600890,退市中房,
+600891,退市秋林,
+600892,大晟文化,1996-03-15
+600893,航发动力,1996-04-08
+600894,广日股份,1996-03-28
+600895,张江高科,1996-04-22
+600896,退市海医,
+600897,厦门空港,1996-05-31
+600898,ST美讯  ,1996-04-18
+600899,*ST信联,
+600900,长江电力,2003-11-18
+600901,江苏金租,2018-03-01
+600903,贵州燃气,2017-11-07
+600905,三峡能源,2021-06-10
+600906,财达证券,2021-05-07
+600908,无锡银行,2016-09-23
+600909,华安证券,2016-12-06
+600916,中国黄金,2021-02-05
+600917,重庆燃气,2014-09-30
+600918,中泰证券,2020-06-03
+600919,江苏银行,2016-08-02
+600925,苏能股份,2023-03-29
+600926,杭州银行,2016-10-27
+600927,永安期货,2021-12-23
+600928,西安银行,2019-03-01
+600929,雪天盐业,2018-03-26
+600933,爱柯迪  ,2017-11-17
+600935,华塑股份,2021-11-26
+600936,广西广电,2016-08-15
+600938,中国海油,2022-04-21
+600939,重庆建工,2017-02-21
+600941,中国移动,2022-01-05
+600955,维远股份,2021-09-15
+600956,新天绿能,2020-06-29
+600958,东方证券,2015-03-23
+600959,江苏有线,2015-04-28
+600960,渤海汽车,2004-04-07
+600961,株冶集团,2004-08-30
+600962,国投中鲁,2004-06-22
+600963,岳阳林纸,2004-05-25
+600965,福成股份,2004-07-13
+600966,博汇纸业,2004-06-08
+600967,内蒙一机,2004-05-18
+600968,海油发展,2019-06-26
+600969,郴电国际,2004-04-08
+600970,中材国际,2005-04-12
+600971,恒源煤电,2004-08-17
+600973,宝胜股份,2004-08-02
+600975,新五丰  ,2004-06-09
+600976,健民集团,2004-04-19
+600977,中国电影,2016-08-09
+600978,*ST宜生,
+600979,广安爱众,2004-09-06
+600980,北矿科技,2004-05-12
+600981,汇鸿集团,2004-06-30
+600982,宁波能源,2004-07-06
+600983,惠而浦  ,2004-07-27
+600984,建设机械,2004-07-07
+600985,淮北矿业,2004-04-28
+600986,浙文互联,2004-04-26
+600987,航民股份,2004-08-09
+600988,赤峰黄金,2004-04-14
+600989,宝丰能源,2019-05-16
+600990,四创电子,2004-05-10
+600991,广汽长丰,
+600992,贵绳股份,2004-05-14
+600993,马应龙  ,2004-05-17
+600995,南网储能,2004-06-15
+600996,贵广网络,2016-12-26
+600997,开滦股份,2004-06-02
+600998,九州通  ,2010-11-02
+600999,招商证券,2009-11-17
+601000,唐山港  ,2010-07-05
+601001,晋控煤业,2006-06-23
+601002,晋亿实业,2007-01-26
+601003,柳钢股份,2007-02-27
+601005,重庆钢铁,2007-02-28
+601006,大秦铁路,2006-08-01
+601007,金陵饭店,2007-04-06
+601008,连云港  ,2007-04-26
+601009,南京银行,2007-07-19
+601010,文峰股份,2011-06-03
+601011,宝泰隆  ,2011-03-09
+601012,隆基绿能,2012-04-11
+601015,陕西黑猫,2014-11-05
+601016,节能风电,2014-09-29
+601018,宁波港  ,2010-09-28
+601019,山东出版,2017-11-22
+601020,华钰矿业,2016-03-16
+601021,春秋航空,2015-01-21
+601022,宁波远洋,2022-12-08
+601028,玉龙股份,2011-11-07
+601038,一拖股份,2012-08-08
+601058,赛轮轮胎,2011-06-30
+601059,信达证券,2023-02-01
+601061,中信金属,2023-04-10
+601065,江盐集团,2023-04-10
+601066,中信建投,2018-06-20
+601068,中铝国际,2018-08-31
+601069,西部黄金,2015-01-22
+601077,渝农商行,2019-10-29
+601086,国芳集团,2017-09-29
+601088,中国神华,2007-10-09
+601089,福元医药,2022-06-30
+601098,中南传媒,2010-10-28
+601099,太平洋  ,2007-12-28
+601100,恒立液压,2011-10-28
+601101,昊华能源,2010-03-31
+601106,中国一重,2010-02-09
+601107,四川成渝,2009-07-27
+601108,财通证券,2017-10-24
+601111,中国国航,2006-08-18
+601113,华鼎股份,2011-05-09
+601116,三江购物,2011-03-02
+601117,中国化学,2010-01-07
+601118,海南橡胶,2011-01-07
+601121,宝地矿业,2023-03-10
+601126,四方股份,2010-12-31
+601127,赛力斯  ,2016-06-15
+601128,常熟银行,2016-09-30
+601133,柏诚股份,2023-04-10
+601136,首创证券,2022-12-22
+601137,博威合金,2011-01-27
+601138,工业富联,2018-06-08
+601139,深圳燃气,2009-12-25
+601155,新城控股,2015-12-04
+601156,东航物流,2021-06-09
+601158,重庆水务,2010-03-29
+601162,天风证券,2018-10-19
+601163,三角轮胎,2016-09-09
+601166,兴业银行,2007-02-05
+601168,西部矿业,2007-07-12
+601169,北京银行,2007-09-19
+601177,杭齿前进,2010-10-11
+601179,中国西电,2010-01-28
+601186,中国铁建,2008-03-10
+601187,厦门银行,2020-10-27
+601188,龙江交通,2010-03-19
+601198,东兴证券,2015-02-26
+601199,江南水务,2011-03-17
+601200,上海环境,2017-03-31
+601208,东材科技,2011-05-20
+601211,国泰君安,2015-06-26
+601212,白银有色,2017-02-15
+601216,君正集团,2011-02-22
+601218,吉鑫科技,2011-05-06
+601222,林洋能源,2011-08-08
+601225,陕西煤业,2014-01-28
+601226,华电重工,2014-12-11
+601228,广州港  ,2017-03-29
+601229,上海银行,2016-11-16
+601231,环旭电子,2012-02-20
+601233,桐昆股份,2011-05-18
+601236,红塔证券,2019-07-05
+601238,广汽集团,2012-03-29
+601258,*ST庞大,
+601268,*ST二重,
+601279,英利汽车,2021-04-15
+601288,农业银行,2010-07-15
+601298,青岛港  ,2019-01-21
+601299,中国北车,
+601311,骆驼股份,2011-06-02
+601318,中国平安,2007-03-01
+601319,中国人保,2018-11-16
+601326,秦港股份,2017-08-16
+601328,交通银行,2007-05-15
+601330,绿色动力,2018-06-11
+601333,广深铁路,2006-12-22
+601336,新华保险,2011-12-16
+601339,百隆东方,2012-06-12
+601360,三六零  ,2012-01-16
+601366,利群股份,2017-04-12
+601368,绿城水务,2015-06-12
+601369,陕鼓动力,2010-04-28
+601375,中原证券,2017-01-03
+601377,兴业证券,2010-10-13
+601388,怡球资源,2012-04-23
+601390,中国中铁,2007-12-03
+601398,工商银行,2006-10-27
+601399,国机重装,2020-06-08
+601456,国联证券,2020-07-31
+601500,通用股份,2016-09-19
+601512,中新集团,2019-12-20
+601515,东风股份,2012-02-16
+601518,吉林高速,2010-03-19
+601519,大智慧  ,2011-01-28
+601528,瑞丰银行,2021-06-25
+601555,东吴证券,2011-12-12
+601558,退市锐电,
+601566,九牧王  ,2011-05-30
+601567,三星医疗,2011-06-15
+601568,北元集团,2020-10-20
+601577,长沙银行,2018-09-26
+601579,会稽山  ,2014-08-25
+601588,北辰实业,2006-10-16
+601595,上海电影,2016-08-17
+601598,中国外运,2019-01-18
+601599,浙文影业,2011-05-27
+601600,中国铝业,2007-04-30
+601601,中国太保,2007-12-25
+601606,长城军工,2018-08-06
+601607,上海医药,1994-03-24
+601608,中信重工,2012-07-06
+601609,金田股份,2020-04-22
+601611,中国核建,2016-06-06
+601615,明阳智能,2019-01-23
+601616,广电电气,2011-02-01
+601618,中国中冶,2009-09-21
+601619,嘉泽新能,2017-07-20
+601628,中国人寿,2007-01-09
+601633,长城汽车,2011-09-28
+601636,旗滨集团,2011-08-12
+601658,邮储银行,2019-12-10
+601665,齐鲁银行,2021-06-18
+601666,平煤股份,2006-11-23
+601668,中国建筑,2009-07-29
+601669,中国电建,2011-10-18
+601677,明泰铝业,2011-09-19
+601678,滨化股份,2010-02-23
+601686,友发集团,2020-12-04
+601688,华泰证券,2010-02-26
+601689,拓普集团,2015-03-19
+601696,中银证券,2020-02-26
+601698,中国卫通,2019-06-28
+601699,潞安环能,2006-09-22
+601700,风范股份,2011-01-18
+601702,华峰铝业,2020-09-07
+601717,郑煤机  ,2010-08-03
+601718,际华集团,2010-08-16
+601727,上海电气,2008-12-05
+601728,中国电信,2021-08-20
+601766,中国中车,2008-08-18
+601777,力帆科技,2010-11-25
+601778,晶科科技,2020-05-19
+601788,光大证券,2009-08-18
+601789,宁波建工,2011-08-16
+601798,蓝科高新,2011-06-22
+601799,星宇股份,2011-02-01
+601800,中国交建,2012-03-09
+601801,皖新传媒,2010-01-18
+601808,中海油服,2007-09-28
+601811,新华文轩,2016-08-08
+601816,京沪高铁,2020-01-16
+601818,光大银行,2010-08-18
+601825,沪农商行,2021-08-19
+601827,三峰环境,2020-06-05
+601828,美凯龙  ,2018-01-17
+601838,成都银行,2018-01-31
+601857,中国石油,2007-11-05
+601858,中国科传,2017-01-18
+601860,紫金银行,2019-01-03
+601865,福莱特  ,2019-02-15
+601866,中远海发,2007-12-12
+601868,中国能建,2021-09-28
+601869,长飞光纤,2018-07-20
+601872,招商轮船,2006-12-01
+601877,正泰电器,2010-01-21
+601878,浙商证券,2017-06-26
+601880,辽港股份,2010-12-06
+601881,中国银河,2017-01-23
+601882,海天精工,2016-11-07
+601886,江河集团,2011-08-18
+601888,中国中免,2009-10-15
+601890,亚星锚链,2010-12-28
+601898,中煤能源,2008-02-01
+601899,紫金矿业,2008-04-25
+601900,南方传媒,2016-02-15
+601901,方正证券,2011-08-10
+601908,京运通  ,2011-09-08
+601916,浙商银行,2019-11-26
+601918,新集能源,2007-12-19
+601919,中远海控,2007-06-26
+601921,浙版传媒,2021-07-23
+601928,凤凰传媒,2011-11-30
+601929,吉视传媒,2012-02-23
+601933,永辉超市,2010-12-15
+601939,建设银行,2007-09-25
+601949,中国出版,2017-08-21
+601952,苏垦农发,2017-05-15
+601956,东贝集团,2020-12-25
+601958,金钼股份,2008-04-17
+601963,重庆银行,2021-02-05
+601965,中国汽研,2012-06-11
+601966,玲珑轮胎,2016-07-06
+601968,宝钢包装,2015-06-11
+601969,海南矿业,2014-12-09
+601975,招商南油,2019-01-08
+601985,中国核电,2015-06-10
+601988,中国银行,2006-07-05
+601989,中国重工,2009-12-16
+601990,南京证券,2018-06-13
+601991,大唐发电,2006-12-20
+601992,金隅集团,2011-03-01
+601995,中金公司,2020-11-02
+601996,丰林集团,2011-09-29
+601997,贵阳银行,2016-08-16
+601998,中信银行,2007-04-27
+601999,出版传媒,2007-12-21
+603000,人民网  ,2012-04-27
+603001,ST奥康  ,2012-04-26
+603002,宏昌电子,2012-05-18
+603003,龙宇股份,2012-08-17
+603005,晶方科技,2014-02-10
+603006,联明股份,2014-06-30
+603007,ST花王  ,2016-08-26
+603008,喜临门  ,2012-07-17
+603009,北特科技,2014-07-18
+603010,万盛股份,2014-10-10
+603011,合锻智能,2014-11-07
+603012,创力集团,2015-03-20
+603013,亚普股份,2018-05-09
+603015,弘讯科技,2015-03-03
+603016,新宏泰  ,2016-07-01
+603017,XD中衡设,2014-12-31
+603018,华设集团,2014-10-13
+603019,中科曙光,2014-11-06
+603020,爱普股份,2015-03-25
+603021,山东华鹏,2015-04-23
+603022,新通联  ,2015-05-18
+603023,威帝股份,2015-05-27
+603025,大豪科技,2015-04-22
+603026,胜华新材,2015-05-29
+603027,千禾味业,2016-03-07
+603028,赛福天  ,2016-03-31
+603029,天鹅股份,2016-04-27
+603030,*ST全筑 ,2015-03-20
+603031,安孚科技,2016-08-22
+603032,德新科技,2017-01-05
+603033,三维股份,2016-12-07
+603035,常熟汽饰,2017-01-05
+603036,如通股份,2016-12-09
+603037,凯众股份,2017-01-20
+603038,华立股份,2017-01-16
+603039,泛微网络,2017-01-13
+603040,新坐标  ,2017-02-09
+603041,美思德  ,2017-03-30
+603042,华脉科技,2017-06-02
+603043,广州酒家,2017-06-27
+603045,福达合金,2018-05-17
+603048,浙江黎明,2021-11-16
+603050,科林电气,2017-04-14
+603051,鹿山新材,2022-03-25
+603052,可川科技,2022-10-11
+603053,成都燃气,2019-12-17
+603055,台华新材,2017-09-21
+603056,德邦股份,2018-01-16
+603057,紫燕食品,2022-09-26
+603058,永吉股份,2016-12-23
+603059,倍加洁  ,2018-03-02
+603060,国检集团,2016-11-09
+603061,金海通,2023-03-03
+603063,禾望电气,2017-07-28
+603065,宿迁联盛,2023-03-21
+603066,音飞储存,2015-06-11
+603067,振华股份,2016-09-13
+603068,博通集成,2019-04-15
+603069,海汽集团,2016-07-12
+603070,万控智造,2022-03-10
+603071,物产环能,2021-12-16
+603073,彩蝶实业,2023-03-16
+603075,热威股份,2023-09-11
+603076,乐惠国际,2017-11-13
+603077,和邦生物,2012-07-31
+603078,江化微  ,2017-04-10
+603079,圣达生物,2017-08-23
+603080,新疆火炬,2018-01-03
+603081,大丰实业,2017-04-20
+603083,剑桥科技,2017-11-10
+603085,天成自控,2015-06-30
+603086,先达股份,2017-05-11
+603087,甘李药业,2020-06-29
+603088,宁波精达,2014-11-11
+603089,正裕工业,2017-01-26
+603090,宏盛股份,2016-08-31
+603093,南华期货,2019-08-30
+603095,越剑智能,2020-04-15
+603096,新经典  ,2017-04-25
+603097,江苏华辰,2022-05-12
+603098,森特股份,2016-12-16
+603099,长白山  ,2014-08-22
+603100,川仪股份,2014-08-05
+603101,汇嘉时代,2016-05-06
+603102,百合股份,2022-01-25
+603103,横店影视,2017-10-12
+603105,芯能科技,2018-07-09
+603106,恒银科技,2017-09-20
+603108,润达医疗,2015-05-27
+603109,神驰机电,2019-12-31
+603110,东方材料,2017-10-13
+603111,康尼机电,2014-08-01
+603112,华翔股份,2020-09-17
+603113,金能科技,2017-05-11
+603115,海星股份,2019-08-09
+603116,红蜻蜓  ,2015-06-29
+603117,ST万林  ,2015-06-29
+603118,共进股份,2015-02-25
+603119,浙江荣泰,2023-08-01
+603121,华培动力,2019-01-11
+603122,合富中国,2022-02-16
+603123,翠微股份,2012-05-03
+603125,常青科技,2023-04-10
+603126,中材节能,2014-07-31
+603127,昭衍新药,2017-08-25
+603128,华贸物流,2012-05-29
+603129,春风动力,2017-08-18
+603130,云中马,2022-11-18
+603131,上海沪工,2016-06-07
+603132,金徽股份,2022-02-22
+603133,*ST碳元 ,2017-03-20
+603135,中重科技,2023-04-10
+603136,天目湖  ,2017-09-27
+603137,恒尚节能,2023-04-19
+603138,海量数据,2017-03-06
+603139,康惠制药,2017-04-21
+603150,万朗磁塑,2022-01-24
+603151,邦基科技,2022-10-19
+603153,上海建科,2023-03-13
+603155,新亚强,2020-09-01
+603156,养元饮品,2018-02-12
+603157,退市拉夏,
+603158,腾龙股份,2015-03-20
+603159,上海亚虹,2016-08-12
+603160,汇顶科技,2016-10-17
+603161,科华控股,2018-01-05
+603162,海通发展,2023-03-29
+603163,圣晖集成,2022-10-13
+603165,荣晟环保,2017-01-17
+603166,福达股份,2014-11-27
+603167,渤海轮渡,2012-09-06
+603168,莎普爱思,2014-07-02
+603169,兰石重装,2014-10-09
+603170,宝立食品,2022-07-15
+603171,税友股份,2021-06-30
+603172,万丰股份,2023-05-10
+603173,福斯达,2023-01-30
+603176,汇通集团,2021-12-31
+603177,德创环保,2017-02-07
+603178,圣龙股份,2017-03-28
+603179,新泉股份,2017-03-17
+603180,金牌厨柜,2017-05-12
+603181,皇马科技,2017-08-24
+603182,嘉华股份,2022-09-09
+603183,建研院  ,2017-09-05
+603185,弘元绿能,2018-12-28
+603186,华正新材,2017-01-03
+603187,海容冷链,2018-11-29
+603188,亚邦股份,2014-09-09
+603189,网达软件,2016-09-14
+603190,亚通精工,2023-02-17
+603191,望变电气,2022-04-28
+603192,汇得科技,2018-08-28
+603193,润本股份,2023-10-17
+603195,公牛集团,2020-02-06
+603196,日播时尚,2017-05-31
+603197,保隆科技,2017-05-19
+603198,迎驾贡酒,2015-05-28
+603199,九华旅游,2015-03-26
+603200,上海洗霸,2017-06-01
+603201,常润股份,2022-07-29
+603203,快克智能,2016-11-08
+603206,嘉环科技,2022-05-06
+603208,江山欧派,2017-02-10
+603209,兴通股份,2022-03-24
+603211,晋拓股份,2022-07-25
+603212,赛伍技术,2020-04-30
+603213,镇洋发展,2021-11-11
+603214,爱婴室  ,2018-03-30
+603215,比依股份,2022-02-18
+603216,梦天家居,2021-12-15
+603217,元利科技,2019-06-20
+603218,日月股份,2016-12-28
+603219,富佳股份,2021-11-22
+603220,中贝通信,2018-11-15
+603221,爱丽家居,2020-03-23
+603222,济民医疗,2015-02-17
+603223,恒通股份,2015-06-30
+603225,新凤鸣  ,2017-04-18
+603226,菲林格尔,2017-06-15
+603227,雪峰科技,2015-05-15
+603228,景旺电子,2017-01-06
+603229,奥翔药业,2017-05-09
+603230,内蒙新华,2021-12-24
+603232,格尔软件,2017-04-21
+603233,大参林  ,2017-07-31
+603235,天新药业,2022-07-12
+603236,移远通信,2019-07-16
+603237,五芳斋,2022-08-31
+603238,诺邦股份,2017-02-22
+603239,浙江仙通,2016-12-30
+603255,鼎际得,2022-08-18
+603256,宏和科技,2019-07-19
+603258,电魂网络,2016-10-26
+603259,药明康德,2018-05-08
+603260,合盛硅业,2017-10-30
+603261,立航科技,2022-03-15
+603266,天龙股份,2017-01-10
+603267,鸿远电子,2019-05-15
+603268,松发股份,2015-03-19
+603269,海鸥股份,2017-05-17
+603270,金帝股份,2023-09-01
+603272,联翔股份,2022-05-20
+603275,众辰科技,2023-08-23
+603276,恒兴新材,2023-09-25
+603277,银都股份,2017-09-11
+603278,大业股份,2017-11-13
+603279,景津装备,2019-07-29
+603280,南方路机,2022-11-08
+603281,江瀚新材,2023-01-31
+603282,亚光股份,2023-03-15
+603283,赛腾股份,2017-12-25
+603286,日盈电子,2017-06-27
+603288,海天味业,2014-02-11
+603289,泰瑞机器,2017-10-31
+603290,斯达半导,2020-02-04
+603291,联合水务,2023-03-27
+603296,华勤技术,2023-08-08
+603297,永新光学,2018-09-10
+603298,杭叉集团,2016-12-27
+603299,苏盐井神,2015-12-31
+603300,华铁应急,2015-05-29
+603301,振德医疗,2018-04-12
+603303,得邦照明,2017-03-30
+603305,旭升集团,2017-07-10
+603306,华懋科技,2014-09-26
+603307,扬州金泉,2023-02-16
+603308,应流股份,2014-01-22
+603309,维力医疗,2015-03-02
+603311,金海高科,2015-05-18
+603313,梦百合  ,2016-10-13
+603315,福鞍股份,2015-04-24
+603316,诚邦股份,2017-06-19
+603317,天味食品,2019-04-16
+603318,水发燃气,2015-04-24
+603319,湘油泵  ,2016-11-30
+603320,迪贝电气,2017-05-02
+603321,梅轮电梯,2017-09-15
+603322,超讯通信,2016-07-28
+603323,苏农银行,2016-11-29
+603324,盛剑环境,2021-04-07
+603326,我乐家居,2017-06-16
+603327,福蓉科技,2019-05-23
+603328,依顿电子,2014-07-01
+603329,上海雅仕,2017-12-29
+603330,天洋新材,2017-02-13
+603331,百达精工,2017-07-05
+603332,苏州龙杰,2019-01-17
+603333,尚纬股份,2012-05-07
+603335,迪生力  ,2017-06-20
+603336,宏辉果蔬,2016-11-24
+603337,杰克股份,2017-01-19
+603338,浙江鼎力,2015-03-25
+603339,四方科技,2016-05-19
+603345,安井食品,2017-02-22
+603348,文灿股份,2018-04-26
+603351,威尔药业,2019-01-30
+603353,和顺石油,2020-04-07
+603355,莱克电气,2015-05-13
+603356,华菱精工,2018-01-24
+603357,设计总院,2017-08-01
+603358,华达科技,2017-01-25
+603359,东珠生态,2017-09-01
+603360,百傲化学,2017-02-06
+603363,傲农生物,2017-09-26
+603365,水星家纺,2017-11-20
+603366,日出东方,2012-05-21
+603367,辰欣药业,2017-09-29
+603368,柳药集团,2014-12-04
+603369,今世缘  ,2014-07-03
+603377,东方时尚,2016-02-05
+603378,亚士创能,2017-09-28
+603379,三美股份,2019-04-02
+603380,易德龙  ,2017-06-22
+603383,顶点软件,2017-05-22
+603385,惠达卫浴,2017-04-05
+603386,骏亚科技,2017-09-12
+603387,基蛋生物,2017-07-17
+603388,元成股份,2017-03-24
+603389,亚振家居,2016-12-15
+603390,通达电气,2019-11-25
+603392,万泰生物,2020-04-29
+603393,新天然气,2016-09-12
+603396,金辰股份,2017-10-18
+603398,沐邦高科,2015-12-09
+603399,吉翔股份,2012-08-24
+603408,建霖家居,2020-07-30
+603416,信捷电气,2016-12-21
+603421,鼎信通讯,2016-10-11
+603429,集友股份,2017-01-24
+603439,贵州三力,2020-04-28
+603444,吉比特  ,2017-01-04
+603456,九洲药业,2014-10-10
+603458,勘设股份,2017-08-09
+603466,风语筑  ,2017-10-20
+603477,巨星农牧,2017-12-18
+603486,科沃斯  ,2018-05-28
+603488,展鹏科技,2017-05-16
+603489,八方股份,2019-11-11
+603496,恒为科技,2017-06-07
+603499,翔港科技,2017-10-16
+603500,祥和实业,2017-09-04
+603501,韦尔股份,2017-05-04
+603505,金石资源,2017-05-03
+603506,南都物业,2018-02-01
+603507,振江股份,2017-11-06
+603508,思维列控,2015-12-24
+603511,爱慕股份,2021-05-31
+603515,欧普照明,2016-08-19
+603516,淳中科技,2018-02-02
+603517,绝味食品,2017-03-17
+603518,锦泓集团,2014-12-03
+603519,立霸股份,2015-03-19
+603520,司太立  ,2016-03-09
+603527,众源新材,2017-09-07
+603528,多伦科技,2016-05-03
+603529,爱玛科技,2021-06-15
+603530,神马电力,2019-08-05
+603533,掌阅科技,2017-09-21
+603535,嘉诚国际,2017-08-08
+603536,惠发食品,2017-06-13
+603538,美诺华  ,2017-04-07
+603551,奥普家居,2020-01-15
+603555,ST贵人  ,2014-01-24
+603556,海兴电力,2016-11-10
+603557,ST起步  ,2017-08-18
+603558,健盛集团,2015-01-27
+603559,ST通脉  ,2016-12-02
+603565,中谷物流,2020-09-25
+603566,普莱柯  ,2015-05-18
+603567,珍宝岛  ,2015-04-24
+603568,伟明环保,2015-05-28
+603569,长久物流,2016-08-10
+603577,汇金通  ,2016-12-22
+603578,三星新材,2017-03-06
+603579,荣泰健康,2017-01-11
+603580,艾艾精工,2017-05-25
+603583,捷昌驱动,2018-09-21
+603585,苏利股份,2016-12-14
+603586,金麒麟  ,2017-04-06
+603587,地素时尚,2018-06-22
+603588,高能环境,2014-12-29
+603589,口子窖  ,2015-06-29
+603590,康辰药业,2018-08-27
+603595,东尼电子,2017-07-12
+603596,伯特利  ,2018-04-27
+603598,引力传媒,2015-05-27
+603599,广信股份,2015-05-13
+603600,永艺股份,2015-01-23
+603601,再升科技,2015-01-22
+603602,纵横通信,2017-08-10
+603603,*ST博天 ,2017-02-17
+603605,珀莱雅  ,2017-11-15
+603606,东方电缆,2014-10-15
+603607,京华激光,2017-10-25
+603608,天创时尚,2016-02-18
+603609,禾丰股份,2014-08-08
+603610,麒盛科技,2019-10-29
+603611,诺力股份,2015-01-28
+603612,索通发展,2017-07-18
+603613,国联股份,2019-07-30
+603615,茶花股份,2017-02-13
+603616,韩建河山,2015-06-11
+603617,君禾股份,2017-07-03
+603618,杭电股份,2015-02-17
+603619,中曼石油,2017-11-17
+603626,科森科技,2017-02-09
+603628,清源股份,2017-01-12
+603629,利通电子,2018-12-24
+603630,拉芳家化,2017-03-13
+603633,徕木股份,2016-11-17
+603636,南威软件,2014-12-30
+603637,镇海股份,2017-02-08
+603638,艾迪精密,2017-01-20
+603639,海利尔  ,2017-01-12
+603648,畅联股份,2017-09-13
+603650,彤程新材,2018-06-27
+603655,朗博科技,2017-12-29
+603656,泰禾智能,2017-03-21
+603657,春光科技,2018-07-30
+603658,安图生物,2016-09-01
+603659,璞泰来  ,2017-11-03
+603660,苏州科达,2016-12-01
+603661,恒林股份,2017-11-21
+603662,柯力传感,2019-08-06
+603663,三祥新材,2016-08-01
+603665,康隆达  ,2017-03-13
+603666,亿嘉和  ,2018-06-12
+603667,五洲新春,2016-10-25
+603668,天马科技,2017-01-17
+603669,灵康药业,2015-05-28
+603676,卫信康  ,2017-07-21
+603677,奇精机械,2017-02-06
+603678,火炬电子,2015-01-26
+603679,华体科技,2017-06-21
+603680,今创集团,2018-02-27
+603681,永冠新材,2019-03-26
+603682,锦和商管,2020-04-21
+603683,晶华新材,2017-10-20
+603685,晨丰科技,2017-11-27
+603686,福龙马  ,2015-01-26
+603687,大胜达  ,2019-07-26
+603688,石英股份,2014-10-31
+603689,皖天然气,2017-01-10
+603690,至纯科技,2017-01-13
+603693,江苏新能,2018-07-03
+603696,安记食品,2015-12-09
+603697,有友食品,2019-05-08
+603698,航天工程,2015-01-28
+603699,纽威股份,2014-01-17
+603700,宁水集团,2019-01-22
+603701,德宏股份,2016-04-12
+603703,盛洋科技,2015-04-23
+603706,东方环宇,2018-07-09
+603707,健友股份,2017-07-19
+603708,家家悦  ,2016-12-13
+603709,中源家居,2018-02-08
+603711,香飘飘  ,2017-11-30
+603712,七一二  ,2018-02-26
+603713,密尔克卫,2018-07-13
+603716,塞力医疗,2016-10-31
+603717,天域生态,2017-03-27
+603718,海利生物,2015-05-15
+603719,良品铺子,2020-02-24
+603721,中广天择,2017-08-11
+603722,阿科力  ,2017-10-25
+603725,天安新材,2017-09-06
+603726,朗迪集团,2016-04-21
+603727,博迈科  ,2016-11-22
+603728,鸣志电器,2017-05-09
+603729,龙韵股份,2015-03-24
+603730,岱美股份,2017-07-28
+603733,仙鹤股份,2018-04-20
+603737,三棵树  ,2016-06-03
+603738,泰晶科技,2016-09-28
+603739,蔚蓝生物,2019-01-16
+603755,日辰股份,2019-08-28
+603757,大元泵业,2017-07-11
+603758,秦安股份,2017-05-17
+603759,海天股份,2021-03-26
+603766,隆鑫通用,2012-08-10
+603767,中马传动,2017-06-13
+603768,常青股份,2017-03-24
+603773,沃格光电,2018-04-17
+603776,永安行  ,2017-08-17
+603777,来伊份  ,2016-10-12
+603778,乾景园林,2015-12-31
+603779,威龙股份,2016-05-16
+603786,科博达  ,2019-10-15
+603787,新日股份,2017-04-27
+603788,宁波高发,2015-01-20
+603789,星光农机,2015-04-27
+603790,雅运股份,2018-09-12
+603797,联泰环保,2017-04-13
+603798,康普顿  ,2016-04-06
+603799,华友钴业,2015-01-29
+603800,道森股份,2015-12-10
+603801,志邦家居,2017-06-30
+603803,瑞斯康达,2017-04-20
+603806,福斯特  ,2014-09-05
+603808,歌力思  ,2015-04-22
+603809,豪能股份,2017-11-28
+603810,丰山集团,2018-09-17
+603811,诚意药业,2017-03-15
+603813,原尚股份,2017-09-18
+603815,交建股份,2019-10-21
+603816,顾家家居,2016-10-14
+603817,海峡环保,2017-02-20
+603818,曲美家居,2015-04-22
+603819,神力股份,2016-11-25
+603822,嘉澳环保,2016-04-28
+603823,百合花  ,2016-12-20
+603825,华扬联众,2017-08-02
+603826,坤彩科技,2017-04-14
+603828,柯利达  ,2015-02-26
+603829,洛凯股份,2017-10-17
+603833,欧派家居,2017-03-28
+603836,海程邦达,2021-05-26
+603838,四通股份,2015-07-01
+603839,安正时尚,2017-02-14
+603843,正平股份,2016-09-05
+603848,好太太  ,2017-12-01
+603855,华荣股份,2017-05-24
+603856,东宏股份,2017-11-06
+603858,步长制药,2016-11-18
+603859,能科科技,2016-10-21
+603860,中公高科,2017-08-02
+603861,白云电器,2016-03-22
+603863,松炀资源,2019-06-21
+603866,桃李面包,2015-12-22
+603867,新化股份,2019-06-27
+603868,飞科电器,2016-04-18
+603869,新智认知,2015-03-26
+603871,嘉友国际,2018-02-06
+603876,鼎胜新材,2018-04-18
+603877,太平鸟  ,2017-01-09
+603878,武进不锈,2016-12-19
+603879,永悦科技,2017-06-14
+603880,ST南卫  ,2017-08-07
+603881,数据港  ,2017-02-08
+603882,金域医学,2017-09-08
+603883,老百姓  ,2015-04-23
+603885,吉祥航空,2015-05-27
+603886,元祖股份,2016-12-28
+603887,城地香江,2016-10-10
+603888,新华网  ,2016-10-28
+603889,新澳股份,2014-12-31
+603890,春秋电子,2017-12-12
+603893,瑞芯微,2020-02-07
+603895,天永智能,2018-01-22
+603896,寿仙谷  ,2017-05-10
+603897,长城科技,2018-04-10
+603898,好莱客  ,2015-02-17
+603899,晨光股份,2015-01-27
+603900,莱绅通灵,2016-11-23
+603901,永创智能,2015-05-29
+603903,中持股份,2017-03-14
+603906,龙蟠科技,2017-04-10
+603908,牧高笛  ,2017-03-07
+603909,建发合诚,2016-06-28
+603912,佳力图  ,2017-11-01
+603915,国茂股份,2019-06-14
+603916,苏博特  ,2017-11-10
+603917,合力科技,2017-12-04
+603918,金桥信息,2015-05-28
+603919,金徽酒  ,2016-03-10
+603920,世运电路,2017-04-26
+603922,金鸿顺  ,2017-10-23
+603926,铁流股份,2017-05-10
+603927,中科软  ,2019-09-09
+603928,兴业股份,2016-12-12
+603929,亚翔集成,2016-12-30
+603931,格林达,2020-08-19
+603933,睿能科技,2017-07-06
+603936,博敏电子,2015-12-09
+603937,丽岛新材,2017-11-02
+603938,三孚股份,2017-06-28
+603939,益丰药房,2015-02-17
+603948,建业股份,2020-03-02
+603949,雪龙集团,2020-03-10
+603950,长源东谷,2020-05-26
+603955,大千生态,2017-03-10
+603956,威派格  ,2019-02-22
+603958,哈森股份,2016-06-29
+603959,百利科技,2016-05-17
+603960,克来机电,2017-03-14
+603963,大理药业,2017-09-22
+603966,法兰泰克,2017-01-25
+603967,中创物流,2019-04-29
+603968,醋化股份,2015-05-18
+603969,银龙股份,2015-02-27
+603970,中农立华,2017-11-16
+603976,正川股份,2017-08-22
+603977,国泰集团,2016-11-11
+603978,深圳新星,2017-08-07
+603979,金诚信  ,2015-06-30
+603980,吉华集团,2017-06-15
+603982,泉峰汽车,2019-05-22
+603983,丸美股份,2019-07-25
+603985,恒润股份,2017-05-05
+603986,兆易创新,2016-08-18
+603987,康德莱  ,2016-11-21
+603988,中电电机,2014-11-04
+603989,艾华集团,2015-05-15
+603990,麦迪科技,2016-12-08
+603991,至正股份,2017-03-08
+603992,松霖科技,2019-08-26
+603993,洛阳钼业,2012-10-09
+603995,甬金股份,2019-12-24
+603996,退市中新,
+603997,继峰股份,2015-03-02
+603998,方盛制药,2014-12-05
+603999,读者传媒,2015-12-10
+605001,威奥股份,2020-05-22
+605003,众望布艺,2020-09-08
+605005,合兴股份,2021-01-19
+605006,山东玻纤,2020-09-03
+605007,五洲特纸,2020-11-10
+605008,长鸿高科,2020-08-21
+605009,豪悦护理,2020-09-11
+605011,杭州热电,2021-06-30
+605016,百龙创园,2021-04-21
+605018,长华集团,2020-09-29
+605020,永和股份,2021-07-09
+605028,世茂能源,2021-07-12
+605033,美邦股份,2021-09-16
+605050,福然德,2020-09-24
+605055,迎丰股份,2021-01-29
+605056,咸亨国际,2021-07-20
+605058,澳弘电子,2020-10-21
+605060,联德股份,2021-03-01
+605066,天正电气,2020-08-07
+605068,明新旭腾,2020-11-23
+605069,正和生态,2021-08-16
+605077,华康股份,2021-02-09
+605080,浙江自然,2021-05-06
+605081,太和水,2021-02-09
+605086,龙高股份,2021-04-16
+605088,冠盛股份,2020-08-17
+605089,味知香,2021-04-27
+605090,九丰能源,2021-05-25
+605098,行动教育,2021-04-21
+605099,共创草坪,2020-09-30
+605100,华丰股份,2020-08-11
+605108,同庆楼,2020-07-16
+605111,新洁能,2020-09-28
+605116,奥锐特,2020-09-21
+605117,德业股份,2021-04-20
+605118,力鼎光电,2020-07-30
+605122,四方新材,2021-03-10
+605123,派克新材,2020-08-25
+605128,上海沿浦,2020-09-15
+605133,嵘泰股份,2021-02-24
+605136,丽人丽妆,2020-09-29
+605138,盛泰集团,2021-10-27
+605151,西上海,2020-12-15
+605155,西大门,2020-12-31
+605158,华达新材,2020-08-05
+605162,新中港,2021-07-07
+605166,聚合顺,2020-06-18
+605167,利柏特,2021-07-26
+605168,三人行,2020-05-28
+605169,洪通燃气,2020-10-30
+605177,东亚药业,2020-11-25
+605178,时空科技,2020-08-21
+605179,一鸣食品,2020-12-28
+605180,华生科技,2021-04-30
+605183,确成股份,2020-12-07
+605186,健麾信息,2020-12-22
+605188,国光连锁,2020-07-28
+605189,富春染织,2021-05-28
+605196,华通线缆,2021-05-11
+605198,安德利,2020-09-18
+605199,葫芦娃,2020-07-10
+605208,永茂泰,2021-03-08
+605218,伟时电子,2020-09-28
+605222,起帆电缆,2020-07-31
+605228,神通科技,2021-01-20
+605255,天普股份,2020-08-25
+605258,协和电子,2020-12-03
+605259,绿田机械,2021-06-15
+605266,健之佳,2020-12-01
+605268,王力安防,2021-02-24
+605277,新亚电子,2021-01-06
+605286,同力日升,2021-03-22
+605287,德才股份,2021-07-06
+605288,凯迪股份,2020-06-01
+605289,罗曼股份,2021-04-26
+605296,神农集团,2021-05-28
+605298,必得科技,2021-03-01
+605299,舒华体育,2020-12-15
+605300,佳禾食品,2021-04-30
+605303,园林股份,2021-03-01
+605305,中际联合,2021-05-06
+605318,法狮龙,2020-08-03
+605319,无锡振华,2021-06-07
+605333,沪光股份,2020-08-18
+605336,帅丰电器,2020-10-19
+605337,李子园,2021-02-08
+605338,巴比食品,2020-10-12
+605339,南侨食品,2021-05-18
+605358,立昂微,2020-09-11
+605365,立达信,2021-07-20
+605366,宏柏新材,2020-08-12
+605368,蓝天燃气,2021-01-29
+605369,拱东医疗,2020-09-16
+605376,博迁新材,2020-12-08
+605377,华旺科技,2020-12-28
+605378,野马电池,2021-04-12
+605388,均瑶健康,2020-08-18
+605389,长龄液压,2021-03-22
+605398,新炬网络,2021-01-21
+605399,晨光新材,2020-08-04
+605488,福莱新材,2021-05-13
+605499,东鹏饮料,2021-05-27
+605500,森林包装,2020-12-22
+605507,国邦医药,2021-08-02
+605555,德昌股份,2021-10-21
+605566,福莱蒽特,2021-10-25
+605567,春雪食品,2021-10-13
+605577,龙版传媒,2021-08-24
+605580,恒盛能源,2021-08-19
+605588,冠石科技,2021-08-12
+605589,圣泉集团,2021-08-10
+605598,上海港湾,2021-09-17
+605599,菜百股份,2021-09-09
+688001,华兴源创,2019-07-22
+688002,睿创微纳,2019-07-22
+688003,天准科技,2019-07-22
+688004,博汇科技,2020-06-12
+688005,容百科技,2019-07-22
+688006,杭可科技,2019-07-22
+688007,光峰科技,2019-07-22
+688008,澜起科技,2019-07-22
+688009,中国通号,2019-07-22
+688010,福光股份,2019-07-22
+688011,新光光电,2019-07-22
+688012,中微公司,2019-07-22
+688013,天臣医疗,2020-09-28
+688015,交控科技,2019-07-22
+688016,心脉医疗,2019-07-22
+688017,绿的谐波,2020-08-28
+688018,乐鑫科技,2019-07-22
+688019,安集科技,2019-07-22
+688020,方邦股份,2019-07-22
+688021,奥福环保,2019-11-06
+688022,瀚川智能,2019-07-22
+688023,安恒信息,2019-11-05
+688025,杰普特  ,2019-10-31
+688026,洁特生物,2020-01-22
+688027,国盾量子,2020-07-09
+688028,沃尔德  ,2019-07-22
+688029,南微医学,2019-07-22
+688030,山石网科,2019-09-30
+688031,星环科技,2022-10-18
+688032,禾迈股份,2021-12-20
+688033,天宜上佳,2019-07-22
+688035,德邦科技,2022-09-19
+688036,传音控股,2019-09-30
+688037,芯源微,2019-12-16
+688038,中科通达,2021-07-13
+688039,当虹科技,2019-12-11
+688041,海光信息,2022-08-12
+688045,必易微,2022-05-26
+688046,药康生物,2022-04-25
+688047,龙芯中科,2022-06-24
+688048,长光华芯,2022-04-01
+688049,炬芯科技,2021-11-29
+688050,爱博医疗,2020-07-29
+688051,佳华科技,2020-03-20
+688052,纳芯微,2022-04-22
+688053,思科瑞,2022-07-08
+688055,龙腾光电,2020-08-17
+688056,莱伯泰科,2020-09-02
+688057,金达莱,2020-11-11
+688058,宝兰德  ,2019-11-01
+688059,华锐精密,2021-02-08
+688060,云涌科技,2020-07-10
+688061,灿瑞科技,2022-10-18
+688062,迈威生物,2022-01-18
+688063,派能科技,2020-12-30
+688065,凯赛生物,2020-08-12
+688066,航天宏图,2019-07-22
+688067,爱威科技,2021-06-16
+688068,热景生物,2019-09-30
+688069,德林海,2020-07-22
+688070,纵横股份,2021-02-10
+688071,华依科技,2021-07-29
+688072,拓荆科技,2022-04-20
+688073,毕得医药,2022-10-11
+688075,安旭生物,2021-11-18
+688076,诺泰生物,2021-05-20
+688077,大地熊,2020-07-22
+688078,龙软科技,2019-12-30
+688079,美迪凯,2021-03-02
+688080,映翰通,2020-02-12
+688081,兴图新科,2020-01-06
+688082,盛美上海,2021-11-18
+688083,中望软件,2021-03-11
+688084,晶品特装,2022-12-08
+688085,三友医疗,2020-04-09
+688087,英科再生,2021-07-09
+688088,虹软科技,2019-07-22
+688089,嘉必优,2019-12-19
+688090,瑞松科技,2020-02-17
+688091,上海谊众,2021-09-09
+688092,爱科科技,2021-03-19
+688093,世华科技,2020-09-30
+688095,福昕软件,2020-09-08
+688096,京源环保,2020-04-09
+688097,博众精工,2021-05-12
+688098,申联生物,2019-10-28
+688099,晶晨股份,2019-08-08
+688100,威胜信息,2020-01-21
+688101,三达膜,2019-11-15
+688102,斯瑞新材,2022-03-16
+688103,国力股份,2021-09-10
+688105,诺唯赞,2021-11-15
+688106,金宏气体,2020-06-16
+688107,安路科技,2021-11-12
+688108,赛诺医疗,2019-10-30
+688109,品茗科技,2021-03-30
+688110,东芯股份,2021-12-10
+688111,金山办公,2019-11-18
+688112,鼎阳科技,2021-12-01
+688113,联测科技,2021-05-06
+688114,华大智造,2022-09-09
+688115,思林杰,2022-03-14
+688116,天奈科技,2019-09-25
+688117,圣诺生物,2021-06-03
+688118,普元信息,2019-12-04
+688119,中钢洛耐,2022-06-06
+688120,华海清科,2022-06-08
+688121,卓然股份,2021-09-06
+688122,西部超导,2019-07-22
+688123,聚辰股份,2019-12-23
+688125,安达智能,2022-04-15
+688126,沪硅产业,2020-04-20
+688127,蓝特光学,2020-09-21
+688128,中国电研,2019-11-05
+688129,东来技术,2020-10-23
+688130,晶华微,2022-07-29
+688131,皓元医药,2021-06-08
+688132,邦彦技术,2022-09-23
+688133,泰坦科技,2020-10-30
+688135,利扬芯片,2020-11-11
+688136,科兴制药,2020-12-14
+688137,近岸蛋白,2022-09-29
+688138,清溢光电,2019-11-20
+688139,海尔生物,2019-10-25
+688141,杰华特,2022-12-23
+688143,长盈通,2022-12-12
+688146,中船特气,2023-04-21
+688147,微导纳米,2022-12-23
+688148,芳源股份,2021-08-06
+688150,莱特光电,2022-03-18
+688151,华强科技,2021-12-06
+688152,麒麟信安,2022-10-28
+688153,唯捷创芯,2022-04-12
+688155,先惠技术,2020-08-11
+688156,路德环境,2020-09-22
+688157,松井股份,2020-06-09
+688158,优刻得,2020-01-20
+688159,有方科技,2020-01-23
+688160,步科股份,2020-11-12
+688161,威高骨科,2021-06-30
+688162,巨一科技,2021-11-10
+688163,赛伦生物,2022-03-11
+688165,埃夫特,2020-07-15
+688166,博瑞医药,2019-11-08
+688167,炬光科技,2021-12-24
+688168,安博通  ,2019-09-06
+688169,石头科技,2020-02-21
+688170,德龙激光,2022-04-29
+688171,纬德信息,2022-01-27
+688172,燕东微,2022-12-16
+688173,希荻微,2022-01-21
+688175,高凌信息,2022-03-15
+688176,亚虹医药,2022-01-07
+688177,百奥泰,2020-02-21
+688178,万德斯,2020-01-14
+688179,阿拉丁,2020-10-26
+688180,君实生物,2020-07-15
+688181,八亿时空,2020-01-06
+688182,灿勤科技,2021-11-16
+688183,生益电子,2021-02-25
+688184,帕瓦股份,2022-09-19
+688185,康希诺,2020-08-13
+688186,广大特材,2020-02-11
+688187,时代电气,2021-09-07
+688188,柏楚电子,2019-08-08
+688189,南新制药,2020-03-26
+688190,云路股份,2021-11-26
+688191,智洋创新,2021-04-08
+688192,迪哲医药,2021-12-10
+688193,仁度生物,2022-03-30
+688195,腾景科技,2021-03-26
+688196,卓越新能,2019-11-21
+688197,首药控股,2022-03-23
+688198,佰仁医疗,2019-12-09
+688199,久日新材,2019-11-05
+688200,华峰测控,2020-02-18
+688201,信安世纪,2021-04-21
+688202,美迪西  ,2019-11-05
+688203,海正生材,2022-08-16
+688205,德科立,2022-08-09
+688206,概伦电子,2021-12-28
+688207,格灵深瞳,2022-03-17
+688208,道通科技,2020-02-13
+688209,英集芯,2022-04-19
+688210,统联精密,2021-12-27
+688211,中科微至,2021-10-26
+688212,澳华内镜,2021-11-15
+688213,思特威,2022-05-20
+688215,瑞晟智能,2020-08-28
+688216,气派科技,2021-06-23
+688217,睿昂基因,2021-05-17
+688218,江苏北人,2019-12-11
+688219,会通股份,2020-11-18
+688220,翱捷科技,2022-01-14
+688221,前沿生物,2020-10-28
+688222,成都先导,2020-04-16
+688223,晶科能源,2022-01-26
+688225,亚信安全,2022-02-09
+688226,威腾电气,2021-07-07
+688227,品高股份,2021-12-30
+688228,开普云,2020-03-27
+688229,博睿数据,2020-08-17
+688230,芯导科技,2021-12-01
+688231,隆达股份,2022-07-22
+688232,新点软件,2021-11-17
+688233,神工股份,2020-02-21
+688234,天岳先进,2022-01-12
+688235,百济神州,2021-12-15
+688236,春立医疗,2021-12-30
+688237,超卓航科,2022-07-01
+688238,和元生物,2022-03-22
+688239,航宇科技,2021-07-05
+688244,永信至诚,2022-10-19
+688246,嘉和美康,2021-12-14
+688247,宣泰医药,2022-08-25
+688248,南网科技,2021-12-22
+688249,晶合集成,2023-05-05
+688251,井松智能,2022-06-06
+688252,天德钰,2022-09-27
+688253,英诺特,2022-07-28
+688255,凯尔达,2021-10-25
+688256,寒武纪,2020-07-20
+688257,新锐股份,2021-10-27
+688258,卓易信息,2019-12-09
+688259,创耀科技,2022-01-12
+688260,昀冢科技,2021-04-06
+688261,东微半导,2022-02-10
+688262,国芯科技,2022-01-06
+688265,南模生物,2021-12-28
+688266,泽璟制药,2020-01-23
+688267,中触媒,2022-02-16
+688268,华特气体,2019-12-26
+688269,凯立新材,2021-06-09
+688270,臻镭科技,2022-01-27
+688271,联影医疗,2022-08-22
+688272,*ST富吉,2021-10-18
+688273,麦澜德,2022-08-11
+688275,万润新能,2022-09-29
+688276,百克生物,2021-06-25
+688277,天智航,2020-07-07
+688278,特宝生物,2020-01-17
+688279,峰岹科技,2022-04-20
+688280,精进电动,2021-10-27
+688281,华秦科技,2022-03-07
+688282,理工导航,2022-03-18
+688283,坤恒顺维,2022-02-15
+688285,高铁电气,2021-10-20
+688286,敏芯股份,2020-08-10
+688287,观典防务,2022-05-25
+688288,鸿泉物联,2019-11-06
+688289,圣湘生物,2020-08-28
+688290,景业智能,2022-04-29
+688291,金橙子,2022-10-26
+688292,浩瀚深度,2022-08-18
+688293,奥浦迈,2022-09-02
+688295,中复神鹰,2022-04-06
+688296,和达科技,2021-07-27
+688297,中无人机,2022-06-29
+688298,东方生物,2020-02-05
+688299,长阳科技,2019-11-06
+688300,联瑞新材,2019-11-15
+688301,奕瑞科技,2020-09-18
+688302,海创药业,2022-04-12
+688303,大全能源,2021-07-22
+688305,科德数控,2021-07-09
+688306,均普智能,2022-03-22
+688307,中润光学,2023-02-16
+688308,欧科亿,2020-12-10
+688309,恒誉环保,2020-07-14
+688310,迈得医疗,2019-12-03
+688311,盟升电子,2020-07-31
+688312,燕麦科技,2020-06-08
+688313,仕佳光子,2020-08-12
+688314,康拓医疗,2021-05-18
+688315,诺禾致源,2021-04-13
+688316,青云科技,2021-03-16
+688317,之江生物,2021-01-18
+688318,财富趋势,2020-04-27
+688319,欧林生物,2021-06-08
+688320,禾川科技,2022-04-28
+688321,微芯生物,2019-08-12
+688322,奥比中光,2022-07-07
+688323,瑞华泰,2021-04-28
+688325,赛微微电,2022-04-22
+688326,经纬恒润,2022-04-19
+688327,云从科技,2022-05-27
+688328,深科达,2021-03-09
+688329,艾隆科技,2021-03-29
+688330,宏力达,2020-10-15
+688331,荣昌生物,2022-03-31
+688332,中科蓝讯,2022-07-15
+688333,铂力特  ,2019-07-22
+688334,西高院,2023-06-19
+688335,复洁环保,2020-08-17
+688336,三生国健,2020-07-22
+688337,普源精电,2022-04-08
+688338,赛科希德,2020-08-06
+688339,亿华通,2020-08-10
+688343,云天励飞,2023-04-04
+688345,博力威,2021-06-11
+688347,华虹公司,2023-08-07
+688348,昱能科技,2022-06-08
+688349,三一重能,2022-06-22
+688350,富淼科技,2021-01-28
+688351,微电生理,2022-08-31
+688352,颀中科技,2023-04-20
+688353,华盛锂电,2022-07-13
+688355,明志科技,2021-05-12
+688356,键凯科技,2020-08-26
+688357,建龙微纳,2019-12-04
+688358,祥生医疗,2019-12-03
+688359,三孚新科,2021-05-21
+688360,德马科技,2020-06-02
+688361,中科飞测,2023-05-19
+688362,甬矽电子,2022-11-16
+688363,华熙生物,2019-11-06
+688365,光云科技,2020-04-29
+688366,昊海生科,2019-10-30
+688367,工大高科,2021-06-28
+688368,晶丰明源,2019-10-14
+688369,致远互联,2019-10-31
+688370,丛麟科技,2022-08-25
+688371,菲沃泰,2022-08-02
+688372,伟测科技,2022-10-26
+688373,盟科药业,2022-08-05
+688375,国博电子,2022-07-22
+688376,美埃科技,2022-11-18
+688377,迪威尔,2020-07-08
+688378,奥来德,2020-09-03
+688379,华光新材,2020-08-19
+688380,中微半导,2022-08-05
+688381,帝奥微,2022-08-23
+688382,益方生物,2022-07-25
+688383,新益昌,2021-04-28
+688385,复旦微电,2021-08-04
+688386,泛亚微透,2020-10-16
+688387,信科移动,2022-09-26
+688388,嘉元科技,2019-07-22
+688389,普门科技,2019-11-05
+688390,固德威,2020-09-04
+688391,钜泉科技,2022-09-13
+688392,骄成超声,2022-09-27
+688393,安必平,2020-08-20
+688395,正弦电气,2021-04-29
+688396,华润微,2020-02-27
+688398,赛特新材,2020-02-11
+688399,硕世生物,2019-12-05
+688400,凌云光,2022-07-06
+688401,路维光电,2022-08-17
+688403,汇成股份,2022-08-18
+688408,中信博,2020-08-28
+688409,富创精密,2022-10-10
+688410,山外山,2022-12-26
+688416,恒烁股份,2022-08-29
+688418,震有科技,2020-07-22
+688419,耐科装备,2022-11-07
+688420,美腾科技,2022-12-09
+688425,铁建重工,2021-06-22
+688426,康为世纪,2022-10-25
+688428,诺诚健华,2022-09-21
+688429,时创能源,2023-06-29
+688432,有研硅,2022-11-10
+688433,华曙高科,2023-04-17
+688435,英方软件,2023-01-19
+688439,振华风光,2022-08-26
+688443,智翔金泰,2023-06-20
+688448,磁谷科技,2022-09-21
+688450,光格科技,2023-07-24
+688455,科捷智能,2022-09-15
+688456,有研粉材,2021-03-17
+688458,美芯晟,2023-05-22
+688459,哈铁科技,2022-10-12
+688466,金科环境,2020-05-08
+688468,科美诊断,2021-04-09
+688469,中芯集成,2023-05-10
+688472,阿特斯,2023-06-09
+688475,萤石网络,2022-12-28
+688478,晶升股份,2023-04-24
+688479,友车科技,2023-05-11
+688480,赛恩斯,2022-11-25
+688484,南芯科技,2023-04-07
+688485,九州一轨,2023-01-18
+688486,龙迅股份,2023-02-21
+688488,艾迪药业,2020-07-20
+688489,三未信安,2022-12-02
+688496,清越科技,2022-12-28
+688498,源杰科技,2022-12-21
+688499,利元亨,2021-07-01
+688500,*ST慧辰,2020-07-16
+688501,青达环保,2021-07-16
+688502,茂莱光学,2023-03-09
+688503,聚和材料,2022-12-09
+688505,复旦张江,2020-06-19
+688506,百利天恒,2023-01-06
+688507,索辰科技,2023-04-18
+688508,芯朋微,2020-07-22
+688509,正元地信,2021-07-30
+688510,航亚科技,2020-12-16
+688511,天微电子,2021-07-30
+688512,慧智微,2023-05-16
+688513,苑东生物,2020-09-02
+688515,裕太微,2023-02-10
+688516,奥特维,2020-05-21
+688517,金冠电气,2021-06-18
+688518,联赢激光,2020-06-22
+688519,南亚新材,2020-08-18
+688520,神州细胞,2020-06-22
+688521,芯原股份,2020-08-18
+688522,纳睿雷达,2023-03-01
+688523,航天环宇,2023-06-02
+688525,佰维存储,2022-12-30
+688526,科前生物,2020-09-22
+688528,秦川物联,2020-07-01
+688529,豪森股份,2020-11-09
+688531,日联科技,2023-03-31
+688533,上声电子,2021-04-19
+688535,华海诚科,2023-04-04
+688536,思瑞浦,2020-09-21
+688538,和辉光电,2021-05-28
+688539,高华科技,2023-04-18
+688543,国科军工,2023-06-21
+688548,广钢气体,2023-08-15
+688549,中巨芯,2023-09-08
+688550,瑞联新材,2020-09-02
+688551,科威尔,2020-09-10
+688552,航天南湖,2023-05-18
+688553,汇宇制药,2021-10-26
+688556,高测股份,2020-08-07
+688557,兰剑智能,2020-12-02
+688558,国盛智科,2020-06-30
+688559,海目星,2020-09-09
+688560,明冠新材,2020-12-24
+688561,奇安信,2020-07-22
+688562,航天软件,2023-05-24
+688563,航材股份,2023-07-19
+688565,力源科技,2021-05-13
+688566,吉贝尔,2020-05-18
+688567,孚能科技,2020-07-17
+688568,中科星图,2020-07-08
+688569,铁科轨道,2020-08-31
+688570,天玛智控,2023-06-05
+688571,杭华股份,2020-12-11
+688573,信宇人,2023-08-17
+688575,亚辉龙,2021-05-17
+688576,西山科技,2023-06-06
+688577,浙海德曼,2020-09-16
+688578,艾力斯,2020-12-02
+688579,山大地纬,2020-07-17
+688580,伟思医疗,2020-07-21
+688581,安杰思,2023-05-19
+688582,芯动联科,2023-06-30
+688585,上纬新材,2020-09-28
+688586,江航装备,2020-07-31
+688588,凌志软件,2020-05-11
+688589,力合微,2020-07-22
+688590,新致软件,2020-12-07
+688591,泰凌微,2023-08-25
+688592,司南导航,2023-08-16
+688593,新相微,2023-06-01
+688595,芯海科技,2020-09-28
+688596,正帆科技,2020-08-20
+688597,煜邦电力,2021-06-17
+688598,金博股份,2020-05-18
+688599,天合光能,2020-06-10
+688600,皖仪科技,2020-07-03
+688601,力芯微,2021-06-28
+688602,康鹏科技,2023-07-20
+688603,天承科技,2023-07-10
+688606,奥泰生物,2021-03-25
+688607,康众医疗,2021-02-01
+688608,恒玄科技,2020-12-16
+688609,九联科技,2021-03-23
+688610,埃科光电,2023-07-19
+688611,杭州柯林,2021-04-12
+688612,威迈斯,2023-07-26
+688613,奥精医疗,2021-05-21
+688616,西力科技,2021-03-18
+688617,惠泰医疗,2021-01-07
+688618,三旺通信,2020-12-30
+688619,罗普特,2021-02-23
+688620,安凯微,2023-06-27
+688621,阳光诺和,2021-06-21
+688622,禾信仪器,2021-09-13
+688623,双元科技,2023-06-08
+688625,呈和科技,2021-06-07
+688626,翔宇医疗,2021-03-31
+688627,精智达,2023-07-18
+688628,优利德,2021-02-01
+688629,华丰科技,2023-06-27
+688630,芯碁微装,2021-04-01
+688631,莱斯信息,2023-06-28
+688633,星球石墨,2021-03-24
+688636,智明达,2021-04-08
+688638,誉辰智能,2023-07-12
+688639,华恒生物,2021-04-22
+688646,逸飞激光,2023-07-28
+688651,盛邦安全,2023-07-26
+688655,迅捷兴,2021-05-11
+688656,浩欧博,2021-01-13
+688657,浩辰软件,2023-10-10
+688658,悦康药业,2020-12-24
+688659,元琛科技,2021-03-31
+688660,电气风电,2021-05-19
+688661,和林微纳,2021-03-29
+688662,富信科技,2021-04-01
+688663,新风光,2021-04-13
+688665,四方光电,2021-02-09
+688667,菱电电控,2021-03-12
+688668,鼎通科技,2020-12-21
+688669,聚石化学,2021-01-25
+688670,金迪克,2021-08-02
+688671,碧兴物联,2023-08-09
+688676,金盘科技,2021-03-09
+688677,海泰新光,2021-02-26
+688678,福立旺,2020-12-23
+688679,通源环境,2020-12-25
+688680,海优新材,2021-01-22
+688681,科汇股份,2021-06-16
+688682,霍莱沃,2021-04-20
+688683,莱尔科技,2021-04-12
+688685,迈信林,2021-05-13
+688686,奥普特,2020-12-31
+688687,凯因科技,2021-02-08
+688689,银河微电,2021-01-27
+688690,纳微科技,2021-06-23
+688693,锴威特,2023-08-18
+688696,极米科技,2021-03-03
+688697,纽威数控,2021-09-17
+688698,伟创电气,2020-12-29
+688699,明微电子,2020-12-18
+688700,东威科技,2021-06-15
+688701,卓锦股份,2021-09-16
+688702,盛科通信,2023-09-14
+688707,振华新材,2021-09-14
+688711,宏微科技,2021-09-01
+688716,中研股份,2023-09-20
+688718,唯赛勃,2021-07-28
+688719,爱科赛博,2023-09-28
+688722,同益中,2021-10-19
+688728,格科微,2021-08-18
+688733,壹石通,2021-08-17
+688737,中自科技,2021-10-22
+688739,成大生物,2021-10-28
+688766,普冉股份,2021-08-23
+688767,博拓生物,2021-09-08
+688768,容知日新,2021-07-26
+688772,珠海冠宇,2021-10-15
+688776,国光电气,2021-08-31
+688777,中控技术,2020-11-24
+688778,厦钨新能,2021-08-05
+688779,长远锂科,2021-08-11
+688786,悦安新材,2021-08-26
+688787,海天瑞声,2021-08-13
+688788,科思科技,2020-10-22
+688789,宏华数科,2021-07-08
+688793,倍轻松,2021-07-15
+688798,艾为电子,2021-08-16
+688799,华纳药厂,2021-07-13
+688800,瑞可达,2021-07-22
+688819,天能股份,2021-01-18
+688981,中芯国际,2020-07-16
+689009,九号公司,2020-10-29
+830779,武汉蓝电,2023-06-01
+830799,艾融软件,2020-07-27
+830809,安达科技,2023-03-23
+830832,齐鲁华信,2021-02-23
+830839,万通液压,2020-11-09
+830879,基康仪器,2022-12-20
+830896,旺成科技,2023-04-19
+830946,森萱医药,2020-07-27
+830964,润农节水,2020-07-27
+830974,凯大催化,2023-03-08
+831010,凯添燃气,2020-07-27
+831039,国义招标,2021-08-18
+831087,秋乐种业,2022-12-07
+831152,昆工科技,2022-09-01
+831167,鑫汇科,2022-05-27
+831195,三祥科技,2022-12-30
+831278,泰德股份,2022-06-20
+831304,迪尔化工,2023-04-18
+831305,海希通讯,2021-11-05
+831370,新安洁,2020-07-27
+831445,龙竹科技,2020-07-27
+831526,凯华材料,2022-12-22
+831627,力王股份,2023-09-07
+831641,格利尔,2022-12-02
+831689,克莱特,2022-03-21
+831726,朱老六,2021-05-27
+831768,拾比佰,2021-06-28
+831832,科达自控,2021-11-15
+831834,三维股份,2022-08-22
+831855,浙江大农,2022-12-29
+831856,浩淼科技,2020-12-25
+831906,舜宇精工,2023-02-22
+831961,创远信科,2020-07-27
+832000,安徽凤凰,2020-12-23
+832023,田野股份,2023-02-02
+832089,禾昌聚合,2021-11-09
+832110,雷特科技,2022-12-06
+832145,恒合股份,2021-11-15
+832149,利尔达,2023-02-17
+832171,志晟信息,2021-11-15
+832175,东方碳素,2023-06-30
+832225,利通科技,2021-02-25
+832278,鹿得医疗,2020-07-27
+832317,观典防务,2020-07-27
+832419,路斯股份,2022-03-11
+832469,富恒新材,2023-09-18
+832471,美邦科技,2023-05-25
+832491,奥迪威,2022-06-14
+832566,梓橦宫,2021-08-13
+832651,天罡股份,2023-06-27
+832662,方盛股份,2022-11-28
+832735,德源药业,2021-02-19
+832786,骑士乳业,2023-10-13
+832802,保丽洁,2023-02-06
+832876,慧为智能,2022-11-09
+832885,星辰科技,2021-07-08
+832978,开特股份,2023-09-28
+832982,锦波生物,2023-07-20
+833075,柏星龙,2022-12-14
+833171,国航远洋,2022-12-15
+833230,欧康医药,2022-12-09
+833266,生物谷,2020-07-27
+833346,威贸电子,2022-02-23
+833394,民士达,2023-04-25
+833427,华维设计,2021-02-05
+833429,康比特,2022-12-15
+833454,同心传动,2021-11-15
+833455,汇隆活塞,2023-06-21
+833509,同惠电子,2021-01-11
+833523,德瑞锂电,2021-06-03
+833533,骏创科技,2022-05-24
+833575,康乐卫士,2023-03-15
+833580,科创新材,2022-05-13
+833751,惠同新材,2023-07-17
+833781,瑞奇智造,2022-12-26
+833819,颖泰生物,2020-07-27
+833873,中设咨询,2021-11-15
+833874,泰祥股份,2020-07-27
+833914,远航精密,2022-11-11
+833943,优机股份,2022-06-24
+833994,翰博高新,2020-07-27
+834014,特瑞斯,2022-12-13
+834021,流金科技,2020-07-27
+834033,康普化学,2022-12-21
+834058,华洋赛车,2023-08-10
+834062,科润智控,2022-07-13
+834261,一诺威,2023-04-03
+834407,驰诚股份,2023-02-16
+834415,恒拓开源,2020-07-27
+834475,三友科技,2020-07-27
+834599,同力股份,2021-02-22
+834639,晨光电缆,2022-07-12
+834682,球冠电缆,2020-07-27
+834765,美之高,2021-07-05
+834770,艾能聚,2023-02-28
+834950,迅安科技,2023-01-11
+835174,五新隧装,2021-08-20
+835179,凯德石英,2022-03-04
+835184,国源科技,2020-07-27
+835185,贝特瑞,2020-07-27
+835207,众诚科技,2022-09-23
+835237,力佳科技,2022-11-25
+835305,云创数据,2021-08-26
+835368,连城数控,2020-07-27
+835508,殷图网联,2020-07-27
+835640,富士达,2020-07-27
+835670,数字人,2020-12-08
+835857,百甲科技,2023-03-14
+835892,中科美菱,2022-10-18
+835985,海泰新能,2022-08-08
+836077,吉林碳谷,2021-08-31
+836149,旭杰科技,2020-07-27
+836208,青矩技术,2023-06-29
+836221,易实精密,2023-06-08
+836239,长虹能源,2021-02-09
+836247,华密新材,2022-12-23
+836260,中寰股份,2021-11-15
+836263,中航泰达,2020-07-27
+836270,天铭科技,2022-09-02
+836395,朗鸿科技,2022-09-01
+836414,欧普泰,2022-12-12
+836419,万德股份,2023-09-15
+836422,润普食品,2023-03-01
+836433,大唐药业,2020-07-27
+836504,博迅生物,2023-08-17
+836675,秉扬科技,2020-12-28
+836699,海达尔,2023-05-09
+836717,瑞星股份,2023-07-03
+836720,吉冈精密,2021-11-24
+836807,奔朗新材,2022-12-20
+836826,盖世食品,2021-01-12
+836871,派特尔,2022-07-22
+836892,广咨国际,2021-10-28
+836942,恒立钻具,2022-12-08
+836957,汉维科技,2022-12-14
+837006,晟楠科技,2023-05-18
+837046,亿能电力,2022-10-13
+837092,汉鑫科技,2021-11-15
+837174,宏裕包材,2023-08-18
+837212,智新电子,2021-06-08
+837242,建邦科技,2020-07-27
+837344,三元基因,2021-01-08
+837592,华信永道,2023-07-10
+837663,明阳科技,2023-03-15
+837748,路桥信息,2023-08-16
+837821,则成电子,2022-07-06
+838030,德众汽车,2020-11-27
+838163,方大新材,2020-07-27
+838171,邦德股份,2022-06-02
+838227,美登科技,2022-12-28
+838262,太湖雪,2022-12-30
+838275,驱动力,2021-01-25
+838402,硅烷科技,2022-09-28
+838670,恒进感应,2022-07-05
+838701,豪声电子,2023-07-19
+838810,春光药装,2022-12-16
+838837,华原股份,2023-05-15
+838924,广脉科技,2021-11-03
+838971,天马新材,2022-09-27
+839167,同享科技,2020-07-27
+839273,一致魔芋,2023-02-21
+839371,欧福蛋业,2023-01-18
+839680,广道数字,2021-11-15
+839719,宁新新材,2023-05-26
+839725,惠丰钻石,2022-07-18
+839729,永顺生物,2020-07-27
+839790,联迪信息,2022-09-02
+839792,东和新材,2023-03-30
+839946,华阳变速,2021-07-20
+870199,倍益康,2022-12-01
+870204,沪江材料,2022-01-18
+870299,灿能电力,2022-06-10
+870357,雅葆轩,2022-11-18
+870436,大地电气,2021-11-15
+870508,丰安股份,2022-12-16
+870726,鸿智科技,2023-08-08
+870866,绿亨科技,2022-12-09
+870976,视声智能,2023-09-01
+871245,威博液压,2022-01-06
+871396,常辅股份,2020-11-18
+871478,巨能股份,2023-05-12
+871553,凯腾精工,2021-08-06
+871634,新威凌,2022-11-24
+871642,通易航天,2021-08-16
+871694,中裕科技,2023-04-24
+871753,天纺标,2022-10-31
+871857,泓禧科技,2022-02-28
+871970,大禹生物,2022-05-18
+871981,晶赛科技,2021-11-15
+872190,雷神科技,2022-12-23
+872351,华光源海,2022-12-29
+872374,云里物里,2022-11-29
+872392,佳合科技,2022-12-30
+872541,铁大科技,2023-03-10
+872808,曙光数创,2022-11-18
+872895,花溪科技,2023-04-06
+872925,锦好医疗,2021-10-25
+872953,国子软件,2023-08-23
+873001,纬达光电,2022-12-27
+873122,中纺标,2022-09-27
+873152,天宏锂电,2023-01-19
+873167,新赣江,2023-02-09
+873169,七丰精工,2022-04-15
+873223,荣亿精密,2022-06-09
+873305,九菱科技,2022-12-21
+873339,恒太照明,2022-11-17
+873527,夜光明,2022-10-27
+873576,天力复合,2023-07-12
+873593,鼎智科技,2023-04-13
+873665,科强股份,2023-09-26
+873726,卓兆点胶,2023-10-19
+900901,云赛Ｂ股,1992-02-21
+900902,市北B股 ,1992-07-01
+900903,大众Ｂ股,1992-07-22
+900904,神奇B股 ,1992-07-22
+900905,老凤祥Ｂ,1992-07-28
+900906,中毅达B ,1992-07-28
+900907,退市鹏B,
+900908,氯碱Ｂ股,1992-08-20
+900909,华谊B股 ,1992-08-28
+900910,海立Ｂ股,1993-01-18
+900911,金桥Ｂ股,1993-05-31
+900912,外高Ｂ股,1993-07-26
+900913,国新B股 ,1993-09-28
+900914,锦在线B ,1993-10-18
+900915,中路Ｂ股,1993-11-15
+900916,凤凰B股 ,1993-11-19
+900917,海欣Ｂ股,1993-12-08
+900918,耀皮Ｂ股,1993-12-10
+900919,退市庭B,
+900920,动力Ｂ股,1993-12-28
+900921,丹科B股 ,1993-12-28
+900922,三毛B股 ,1993-12-31
+900923,百联Ｂ股,1994-01-05
+900924,上工Ｂ股,1994-01-18
+900925,机电Ｂ股,1994-01-31
+900926,宝信Ｂ  ,1994-03-15
+900927,物贸Ｂ股,1994-03-30
+900928,临港B股 ,1994-04-29
+900929,锦旅Ｂ股,1994-09-28
+900930,*ST沪普B,
+900931,PT水仙B,
+900932,陆家Ｂ股,1994-11-22
+900933,华新B股,
+900934,锦江Ｂ股,1994-12-15
+900935,阳晨B股,
+900936,鄂资Ｂ股,1995-10-20
+900937,华电B股 ,1996-04-22
+900938,海科B   ,1996-04-30
+900939,汇丽B   ,1996-06-28
+900940,大名城B ,1996-07-26
+900941,东信Ｂ股,1996-08-09
+900942,黄山Ｂ股,1996-11-22
+900943,开开Ｂ股,1997-01-08
+900945,海控B股 ,1997-06-26
+900946,天雁B股 ,1997-06-17
+900947,振华Ｂ股,1997-08-05
+900948,伊泰Ｂ股,1997-08-08
+900949,东电B股,
+900950,新城B股,
+900951,退市大化,
+900952,锦港Ｂ股,1998-05-19
+900953,凯马Ｂ  ,1998-06-24
+900955,退市海B,
+900956,东贝B股,
+900957,凌云Ｂ股,2000-07-28
```

### Comparing `adata-1.2.4/adata/stock/cache/index_code_rel_ths.py` & `adata-2.0.0b0/adata/stock/cache/index_code_rel_ths.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-rel = {"000819": "1B0819", "1B0819": "000819", "000006": "1B0004", "1B0004": "000006", "000823": "1B0823",
-       "1B0823": "000823",
-       "000867": "1B0867", "1B0867": "000867", "000989": "1B0989", "1B0989": "000989", "000987": "1B0987",
-       "1B0987": "000987",
-       "000033": "1B0033", "1B0033": "000033", "000071": "1B0071", "1B0071": "000071", "000035": "1B0035",
-       "1B0035": "000035",
-       "000854": "1B0854", "1B0854": "000854", "000107": "1B0107", "1B0107": "000107", "000092": "1B0092",
-       "1B0092": "000092",
-       "000126": "1B0126", "1B0126": "000126", "000026": "1B0026", "1B0026": "000026", "000145": "1B0145",
-       "1B0145": "000145",
-       "000073": "1B0073", "1B0073": "000073", "000094": "1B0094", "1B0094": "000094", "000105": "1B0105",
-       "1B0105": "000105",
-       "000869": "1B0869", "1B0869": "000869", "000027": "1B0027", "1B0027": "000027", "000135": "1B0135",
-       "1B0135": "000135",
-       "000066": "1B0066", "1B0066": "000066", "000068": "1B0068", "1B0068": "000068", "000692": "1B0692",
-       "1B0692": "000692",
-       "000932": "1B0932", "1B0932": "000932", "000170": "1B0170", "1B0170": "000170", "000036": "1B0036",
-       "1B0036": "000036",
-       "000903": "1B0903", "1B0903": "000903", "000057": "1B0057", "1B0057": "000057", "000016": "1B0016",
-       "1B0016": "000016",
-       "000063": "1B0063", "1B0063": "000063", "000074": "1B0074", "1B0074": "000074", "000055": "1B0055",
-       "1B0055": "000055",
-       "000052": "1B0052", "1B0052": "000052", "000914": "1B0914", "1B0914": "000914", "000028": "1B0028",
-       "1B0028": "000028",
-       "000069": "1B0069", "1B0069": "000069", "000043": "1B0043", "1B0043": "000043", "000102": "1B0102",
-       "1B0102": "000102",
-       "000992": "1B0992", "1B0992": "000992", "000934": "1B0934", "1B0934": "000934", "000849": "1B0849",
-       "1B0849": "000849",
-       "000689": "1B0689", "1B0689": "000689", "000048": "1B0048", "1B0048": "000048", "000827": "1B0827",
-       "1B0827": "000827",
-       "000300": "1B0300", "1B0300": "000300", "000021": "1B0021", "1B0021": "000021", "000123": "1B0123",
-       "1B0123": "000123",
-       "000038": "1B0038", "1B0038": "000038", "000093": "1B0093", "1B0093": "000093", "000853": "1B0853",
-       "1B0853": "000853",
-       "000030": "1B0030", "1B0030": "000030", "000059": "1B0059", "1B0059": "000059", "000117": "1B0117",
-       "1B0117": "000117",
-       "000155": "1B0155", "1B0155": "000155", "000906": "1B0906", "1B0906": "000906", "000010": "1B0007",
-       "1B0007": "000010",
-       "000049": "1B0049", "1B0049": "000049", "000050": "1B0050", "1B0050": "000050", "000974": "1B0974",
-       "1B0974": "000974",
-       "000104": "1B0104", "1B0104": "000104", "000125": "1B0125", "1B0125": "000125", "000141": "1B0141",
-       "1B0141": "000141",
-       "000018": "1B0018", "1B0018": "000018", "000019": "1B0019", "1B0019": "000019", "000003": "1A0003",
-       "1A0003": "000003",
-       "000029": "1B0029", "1B0029": "000029", "000054": "1B0054", "1B0054": "000054", "000096": "1B0096",
-       "1B0096": "000096",
-       "000697": "1B0697", "1B0697": "000697", "000031": "1B0031", "1B0031": "000031", "000137": "1B0137",
-       "1B0137": "000137",
-       "000119": "1B0119", "1B0119": "000119", "000149": "1B0149", "1B0149": "000149", "000056": "1B0056",
-       "1B0056": "000056",
-       "000047": "1B0047", "1B0047": "000047", "000051": "1B0051", "1B0051": "000051", "000108": "1B0108",
-       "1B0108": "000108",
-       "000053": "1B0053", "1B0053": "000053", "000058": "1B0058", "1B0058": "000058", "000901": "1B0901",
-       "1B0901": "000901",
-       "000986": "1B0986", "1B0986": "000986", "000159": "1B0159", "1B0159": "000159", "000133": "1B0133",
-       "1B0133": "000133",
-       "000132": "1B0132", "1B0132": "000132", "000158": "1B0158", "1B0158": "000158", "950096": "1B0865",
-       "1B0865": "950096",
-       "000090": "1B0090", "1B0090": "000090", "000928": "1B0928", "1B0928": "000928", "000032": "1B0032",
-       "1B0032": "000032",
-       "000147": "1B0147", "1B0147": "000147", "000148": "1B0148", "1B0148": "000148", "000905": "1B0905",
-       "1B0905": "000905",
-       "000064": "1B0064", "1B0064": "000064", "000091": "1B0091", "1B0091": "000091", "000011": "1B0008",
-       "1B0008": "000011",
-       "000687": "1B0687", "1B0687": "000687", "000060": "1B0060", "1B0060": "000060", "000004": "1B0001",
-       "1B0001": "000004",
-       "000856": "1B0856", "1B0856": "000856", "000065": "1B0065", "1B0065": "000065", "000070": "1B0070",
-       "1B0070": "000070",
-       "000098": "1B0098", "1B0098": "000098", "000847": "1B0847", "1B0847": "000847", "000100": "1B0100",
-       "1B0100": "000100",
-       "991001": "1C0003", "1C0003": "991001", "000067": "1B0067", "1B0067": "000067", "000852": "1B0852",
-       "1B0852": "000852",
-       "000005": "1B0002", "1B0002": "000005", "000802": "1B0802", "1B0802": "000802", "000020": "1B0020",
-       "1B0020": "000020",
-       "000001": "1A0001", "1A0001": "000001", "000017": "1B0017", "1B0017": "000017", "000134": "1B0134",
-       "1B0134": "000134",
-       "000002": "1A0002", "1A0002": "000002", "000099": "1B0099", "1B0099": "000099", "000076": "1B0076",
-       "1B0076": "000076",
-       "000044": "1B0044", "1B0044": "000044", "000982": "1B0982", "1B0982": "000982", "000009": "1B0009",
-       "1B0009": "000009",
-       "000046": "1B0046", "1B0046": "000046", "000103": "1B0103", "1B0103": "000103", "000891": "1B0891",
-       "1B0891": "000891",
-       "000095": "1B0095", "1B0095": "000095", "000160": "1B0160", "1B0160": "000160", "000851": "1B0851",
-       "1B0851": "000851",
-       "000690": "1B0690", "1B0690": "000690", "000008": "1B0006", "1B0006": "000008", "000045": "1B0045",
-       "1B0045": "000045",
-       "000161": "1B0161", "1B0161": "000161", "000153": "1B0153", "1B0153": "000153", "000146": "1B0146",
-       "1B0146": "000146",
-       "000913": "1B0913", "1B0913": "000913", "000139": "1B0139", "1B0139": "000139", "000042": "1B0042",
-       "1B0042": "000042",
-       "000129": "1B0129", "1B0129": "000129", "000122": "1B0122", "1B0122": "000122", "000062": "1B0062",
-       "1B0062": "000062",
-       "000693": "1B0693", "1B0693": "000693", "000115": "1B0115", "1B0115": "000115", "000106": "1B0106",
-       "1B0106": "000106",
-       "000034": "1B0034", "1B0034": "000034", "000040": "1B0040", "1B0040": "000040", "000110": "1B0110",
-       "1B0110": "000110",
-       "000128": "1B0128", "1B0128": "000128", "000072": "1B0072", "1B0072": "000072", "000118": "1B0118",
-       "1B0118": "000118",
-       "000860": "1B0860", "1B0860": "000860", "000120": "1B0120", "1B0120": "000120", "000991": "1B0991",
-       "1B0991": "000991",
-       "000114": "1B0114", "1B0114": "000114", "000933": "1B0933", "1B0933": "000933", "000142": "1B0142",
-       "1B0142": "000142",
-       "000152": "1B0152", "1B0152": "000152", "000111": "1B0111", "1B0111": "000111", "000097": "1B0097",
-       "1B0097": "000097",
-       "000814": "1B0814", "1B0814": "000814", "000138": "1B0138", "1B0138": "000138", "000695": "1B0695",
-       "1B0695": "000695",
-       "000136": "1B0136", "1B0136": "000136", "000037": "1B0037", "1B0037": "000037", "000858": "1B0858",
-       "1B0858": "000858",
-       "000993": "1B0993", "1B0993": "000993", "000935": "1B0935", "1B0935": "000935", "000688": "1B0688",
-       "1B0688": "000688",
-       "000078": "1B0078", "1B0078": "000078", "000162": "1B0162", "1B0162": "000162", "000015": "1B0015",
-       "1B0015": "000015",
-       "000116": "1B0116", "1B0116": "000116", "000061": "1B0061", "1B0061": "000061", "000863": "1B0863",
-       "1B0863": "000863",
-       "000022": "1B0022", "1B0022": "000022", "000101": "1B0101", "1B0101": "000101", "000012": "1B0012",
-       "1B0012": "000012",
-       "000683": "1B0683", "1B0683": "000683", "000007": "1B0005", "1B0005": "000007", "000130": "1B0130",
-       "1B0130": "000130",
-       "000079": "1B0079", "1B0079": "000079", "000077": "1B0077", "1B0077": "000077", "000113": "1B0113",
-       "1B0113": "000113",
-       "000075": "1B0075", "1B0075": "000075", "000121": "1B0121", "1B0121": "000121", "000857": "1B0857",
-       "1B0857": "000857",
-       "000682": "1B0682", "1B0682": "000682", "000025": "1B0025", "1B0025": "000025", "000041": "1B0041",
-       "1B0041": "000041",
-       "000039": "1B0039", "1B0039": "000039", "000151": "1B0151", "1B0151": "000151", "000109": "1B0109",
-       "1B0109": "000109",
-       "000150": "1B0150", "1B0150": "000150", "000112": "1B0112", "1B0112": "000112", "000685": "1B0685",
-       "1B0685": "000685",
-       "000131": "1B0131", "1B0131": "000131"}
+rel = {"000819": "1B0819", "1B0819": "000819", "000006": "1B0004", "1B0004": "000006", "000823": "1B0823",
+       "1B0823": "000823",
+       "000867": "1B0867", "1B0867": "000867", "000989": "1B0989", "1B0989": "000989", "000987": "1B0987",
+       "1B0987": "000987",
+       "000033": "1B0033", "1B0033": "000033", "000071": "1B0071", "1B0071": "000071", "000035": "1B0035",
+       "1B0035": "000035",
+       "000854": "1B0854", "1B0854": "000854", "000107": "1B0107", "1B0107": "000107", "000092": "1B0092",
+       "1B0092": "000092",
+       "000126": "1B0126", "1B0126": "000126", "000026": "1B0026", "1B0026": "000026", "000145": "1B0145",
+       "1B0145": "000145",
+       "000073": "1B0073", "1B0073": "000073", "000094": "1B0094", "1B0094": "000094", "000105": "1B0105",
+       "1B0105": "000105",
+       "000869": "1B0869", "1B0869": "000869", "000027": "1B0027", "1B0027": "000027", "000135": "1B0135",
+       "1B0135": "000135",
+       "000066": "1B0066", "1B0066": "000066", "000068": "1B0068", "1B0068": "000068", "000692": "1B0692",
+       "1B0692": "000692",
+       "000932": "1B0932", "1B0932": "000932", "000170": "1B0170", "1B0170": "000170", "000036": "1B0036",
+       "1B0036": "000036",
+       "000903": "1B0903", "1B0903": "000903", "000057": "1B0057", "1B0057": "000057", "000016": "1B0016",
+       "1B0016": "000016",
+       "000063": "1B0063", "1B0063": "000063", "000074": "1B0074", "1B0074": "000074", "000055": "1B0055",
+       "1B0055": "000055",
+       "000052": "1B0052", "1B0052": "000052", "000914": "1B0914", "1B0914": "000914", "000028": "1B0028",
+       "1B0028": "000028",
+       "000069": "1B0069", "1B0069": "000069", "000043": "1B0043", "1B0043": "000043", "000102": "1B0102",
+       "1B0102": "000102",
+       "000992": "1B0992", "1B0992": "000992", "000934": "1B0934", "1B0934": "000934", "000849": "1B0849",
+       "1B0849": "000849",
+       "000689": "1B0689", "1B0689": "000689", "000048": "1B0048", "1B0048": "000048", "000827": "1B0827",
+       "1B0827": "000827",
+       "000300": "1B0300", "1B0300": "000300", "000021": "1B0021", "1B0021": "000021", "000123": "1B0123",
+       "1B0123": "000123",
+       "000038": "1B0038", "1B0038": "000038", "000093": "1B0093", "1B0093": "000093", "000853": "1B0853",
+       "1B0853": "000853",
+       "000030": "1B0030", "1B0030": "000030", "000059": "1B0059", "1B0059": "000059", "000117": "1B0117",
+       "1B0117": "000117",
+       "000155": "1B0155", "1B0155": "000155", "000906": "1B0906", "1B0906": "000906", "000010": "1B0007",
+       "1B0007": "000010",
+       "000049": "1B0049", "1B0049": "000049", "000050": "1B0050", "1B0050": "000050", "000974": "1B0974",
+       "1B0974": "000974",
+       "000104": "1B0104", "1B0104": "000104", "000125": "1B0125", "1B0125": "000125", "000141": "1B0141",
+       "1B0141": "000141",
+       "000018": "1B0018", "1B0018": "000018", "000019": "1B0019", "1B0019": "000019", "000003": "1A0003",
+       "1A0003": "000003",
+       "000029": "1B0029", "1B0029": "000029", "000054": "1B0054", "1B0054": "000054", "000096": "1B0096",
+       "1B0096": "000096",
+       "000697": "1B0697", "1B0697": "000697", "000031": "1B0031", "1B0031": "000031", "000137": "1B0137",
+       "1B0137": "000137",
+       "000119": "1B0119", "1B0119": "000119", "000149": "1B0149", "1B0149": "000149", "000056": "1B0056",
+       "1B0056": "000056",
+       "000047": "1B0047", "1B0047": "000047", "000051": "1B0051", "1B0051": "000051", "000108": "1B0108",
+       "1B0108": "000108",
+       "000053": "1B0053", "1B0053": "000053", "000058": "1B0058", "1B0058": "000058", "000901": "1B0901",
+       "1B0901": "000901",
+       "000986": "1B0986", "1B0986": "000986", "000159": "1B0159", "1B0159": "000159", "000133": "1B0133",
+       "1B0133": "000133",
+       "000132": "1B0132", "1B0132": "000132", "000158": "1B0158", "1B0158": "000158", "950096": "1B0865",
+       "1B0865": "950096",
+       "000090": "1B0090", "1B0090": "000090", "000928": "1B0928", "1B0928": "000928", "000032": "1B0032",
+       "1B0032": "000032",
+       "000147": "1B0147", "1B0147": "000147", "000148": "1B0148", "1B0148": "000148", "000905": "1B0905",
+       "1B0905": "000905",
+       "000064": "1B0064", "1B0064": "000064", "000091": "1B0091", "1B0091": "000091", "000011": "1B0008",
+       "1B0008": "000011",
+       "000687": "1B0687", "1B0687": "000687", "000060": "1B0060", "1B0060": "000060", "000004": "1B0001",
+       "1B0001": "000004",
+       "000856": "1B0856", "1B0856": "000856", "000065": "1B0065", "1B0065": "000065", "000070": "1B0070",
+       "1B0070": "000070",
+       "000098": "1B0098", "1B0098": "000098", "000847": "1B0847", "1B0847": "000847", "000100": "1B0100",
+       "1B0100": "000100",
+       "991001": "1C0003", "1C0003": "991001", "000067": "1B0067", "1B0067": "000067", "000852": "1B0852",
+       "1B0852": "000852",
+       "000005": "1B0002", "1B0002": "000005", "000802": "1B0802", "1B0802": "000802", "000020": "1B0020",
+       "1B0020": "000020",
+       "000001": "1A0001", "1A0001": "000001", "000017": "1B0017", "1B0017": "000017", "000134": "1B0134",
+       "1B0134": "000134",
+       "000002": "1A0002", "1A0002": "000002", "000099": "1B0099", "1B0099": "000099", "000076": "1B0076",
+       "1B0076": "000076",
+       "000044": "1B0044", "1B0044": "000044", "000982": "1B0982", "1B0982": "000982", "000009": "1B0009",
+       "1B0009": "000009",
+       "000046": "1B0046", "1B0046": "000046", "000103": "1B0103", "1B0103": "000103", "000891": "1B0891",
+       "1B0891": "000891",
+       "000095": "1B0095", "1B0095": "000095", "000160": "1B0160", "1B0160": "000160", "000851": "1B0851",
+       "1B0851": "000851",
+       "000690": "1B0690", "1B0690": "000690", "000008": "1B0006", "1B0006": "000008", "000045": "1B0045",
+       "1B0045": "000045",
+       "000161": "1B0161", "1B0161": "000161", "000153": "1B0153", "1B0153": "000153", "000146": "1B0146",
+       "1B0146": "000146",
+       "000913": "1B0913", "1B0913": "000913", "000139": "1B0139", "1B0139": "000139", "000042": "1B0042",
+       "1B0042": "000042",
+       "000129": "1B0129", "1B0129": "000129", "000122": "1B0122", "1B0122": "000122", "000062": "1B0062",
+       "1B0062": "000062",
+       "000693": "1B0693", "1B0693": "000693", "000115": "1B0115", "1B0115": "000115", "000106": "1B0106",
+       "1B0106": "000106",
+       "000034": "1B0034", "1B0034": "000034", "000040": "1B0040", "1B0040": "000040", "000110": "1B0110",
+       "1B0110": "000110",
+       "000128": "1B0128", "1B0128": "000128", "000072": "1B0072", "1B0072": "000072", "000118": "1B0118",
+       "1B0118": "000118",
+       "000860": "1B0860", "1B0860": "000860", "000120": "1B0120", "1B0120": "000120", "000991": "1B0991",
+       "1B0991": "000991",
+       "000114": "1B0114", "1B0114": "000114", "000933": "1B0933", "1B0933": "000933", "000142": "1B0142",
+       "1B0142": "000142",
+       "000152": "1B0152", "1B0152": "000152", "000111": "1B0111", "1B0111": "000111", "000097": "1B0097",
+       "1B0097": "000097",
+       "000814": "1B0814", "1B0814": "000814", "000138": "1B0138", "1B0138": "000138", "000695": "1B0695",
+       "1B0695": "000695",
+       "000136": "1B0136", "1B0136": "000136", "000037": "1B0037", "1B0037": "000037", "000858": "1B0858",
+       "1B0858": "000858",
+       "000993": "1B0993", "1B0993": "000993", "000935": "1B0935", "1B0935": "000935", "000688": "1B0688",
+       "1B0688": "000688",
+       "000078": "1B0078", "1B0078": "000078", "000162": "1B0162", "1B0162": "000162", "000015": "1B0015",
+       "1B0015": "000015",
+       "000116": "1B0116", "1B0116": "000116", "000061": "1B0061", "1B0061": "000061", "000863": "1B0863",
+       "1B0863": "000863",
+       "000022": "1B0022", "1B0022": "000022", "000101": "1B0101", "1B0101": "000101", "000012": "1B0012",
+       "1B0012": "000012",
+       "000683": "1B0683", "1B0683": "000683", "000007": "1B0005", "1B0005": "000007", "000130": "1B0130",
+       "1B0130": "000130",
+       "000079": "1B0079", "1B0079": "000079", "000077": "1B0077", "1B0077": "000077", "000113": "1B0113",
+       "1B0113": "000113",
+       "000075": "1B0075", "1B0075": "000075", "000121": "1B0121", "1B0121": "000121", "000857": "1B0857",
+       "1B0857": "000857",
+       "000682": "1B0682", "1B0682": "000682", "000025": "1B0025", "1B0025": "000025", "000041": "1B0041",
+       "1B0041": "000041",
+       "000039": "1B0039", "1B0039": "000039", "000151": "1B0151", "1B0151": "000151", "000109": "1B0109",
+       "1B0109": "000109",
+       "000150": "1B0150", "1B0150": "000150", "000112": "1B0112", "1B0112": "000112", "000685": "1B0685",
+       "1B0685": "000685",
+       "000131": "1B0131", "1B0131": "000131"}
```

### Comparing `adata-1.2.4/adata/stock/info/concept/stock_concept_east.py` & `adata-2.0.0b0/adata/stock/info/concept/stock_concept_east.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-# -*- coding: utf-8 -*-
-"""
-@summary: 股票概念
-东方财富股票概念
-
-https://data.eastmoney.com/bkzj/gn.html
-
-单个股票的所有概念板块
-https://datacenter.eastmoney.com/securities/api/data/v1/get?reportName=RPT_F10_CORETHEME_BOARDTYPE&columns=SECUCODE%2CSECURITY_CODE%2CSECURITY_NAME_ABBR%2CNEW_BOARD_CODE%2CBOARD_NAME%2CSELECTED_BOARD_REASON%2CIS_PRECISE%2CBOARD_RANK%2CBOARD_YIELD%2CDERIVE_BOARD_CODE&quoteColumns=f3~05~NEW_BOARD_CODE~BOARD_YIELD&filter=(SECUCODE%3D%22600138.SH%22)(IS_PRECISE%3D%221%22)&pageNumber=1&pageSize=&sortTypes=1&sortColumns=BOARD_RANK&source=HSF10&client=PC&v=0029565688091059528
-@author: 1nchaos
-@date: 2023/3/30 16:17
-"""
-
-import pandas as pd
-
-from adata.common import requests
-from adata.common.utils.code_utils import compile_exchange_by_stock_code
-from adata.stock.info.concept.stock_concept_template import StockConceptTemplate
-
-
-class StockConceptEast(StockConceptTemplate):
-    """
-    东方财富股票概念
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def all_concept_code_east(self):
-        """
-        https://push2.eastmoney.com/api/qt/clist/get?pn=1&pz=1000&po=1&np=1&fields=f12%2Cf13%2Cf14%2Cf62&fid=f62&fs=m%3A90%2Bt%3A3
-        :return: 概念[[name,index_code，concept_code]]
-        """
-        url = f"https://push2.eastmoney.com/api/qt/clist/get" \
-              f"?pn=1&pz=1000&po=1&np=1&fields=f12%2Cf13%2Cf14%2Cf62&fid=f62&fs=m%3A90%2Bt%3A3"
-        res_json = requests.request('get', url, headers={}, proxies={}).json()
-        res_data = res_json['data']['diff']
-        data = []
-        for _ in res_data:
-            data.append({'index_code': _['f12'], 'concept_code': _['f12'], 'name': _['f14'], 'source': '东方财富'})
-        result_df = pd.DataFrame(data=data, columns=self._CONCEPT_CODE_COLUMNS)
-        return result_df
-
-    def concept_constituent_east(self, concept_code=None, wait_time=None):
-        """
-        https://data.eastmoney.com/bkzj/BK1085.html
-        https://push2.eastmoney.com/api/qt/clist/get?fid=f62&po=1&pz=1000&pn=1&np=1&fltt=2&invt=2&fs=b:BK0966&fields=f12,f14
-        :param wait_time: 等待时间：毫秒；表示每个请求的间隔时间，主要用于防止请求太频繁的限制。
-        :param concept_code: 概念代码，BK开头
-        :return: 概念的成分股
-        """
-        curr_page = 1
-        data = []
-        while curr_page < 6:
-            url = f"https://push2.eastmoney.com/api/qt/clist/get" \
-                  f"?fid=f62&po=1&pz=1000&pn={curr_page}&np=1&fltt=2&invt=2&fs=b:{concept_code}&fields=f12,f14"
-            res_json = requests.request('get', url, headers={}, proxies={}, wait_time=wait_time).json()
-            res_data = res_json['data']
-            if not res_data:
-                break
-            res_data = res_data['diff']
-            for _ in res_data:
-                data.append({'stock_code': _['f12'], 'short_name': _['f14']})
-            curr_page += 1
-        result_df = pd.DataFrame(data=data, columns=self._CONCEPT_CONSTITUENT_COLUMNS)
-        return result_df
-
-    def get_concept_east(self, stock_code: str = '000001'):
-        """
-        根据股票代码获取，股票所属的所有的概念信息
-        https://datacenter.eastmoney.com/securities/api/data/v1/get?
-        reportName=RPT_F10_CORETHEME_BOARDTYPE
-        &columns=SECUCODE%2CSECURITY_CODE%2CSECURITY_NAME_ABBR%2CNEW_BOARD_CODE%2CBOARD_NAME%2CSELECTED_BOARD_REASON%2CIS_PRECISE%2CBOARD_RANK%2CBOARD_YIELD%2CDERIVE_BOARD_CODE
-        &quoteColumns=f3~05~NEW_BOARD_CODE~BOARD_YIELD
-        &filter=(SECUCODE%3D%22600138.SH%22)(IS_PRECISE%3D%221%22)
-        &pageNumber=1&pageSize=&sortTypes=1&sortColumns=BOARD_RANK&source=HSF10&client=PC&v=0029565688091059528
-        :param stock_code: 股票代码
-        :return: 概念信息
-        """
-        stock_code = compile_exchange_by_stock_code(stock_code)
-        url = f"https://datacenter.eastmoney.com/securities/api/data/v1/get?" \
-              f"reportName=RPT_F10_CORETHEME_BOARDTYPE&" \
-              f"columns=SECUCODE%2CSECURITY_CODE%2CSECURITY_NAME_ABBR%2CNEW_BOARD_CODE%2CBOARD_NAME%2CSELECTED_BOARD_REASON%2CIS_PRECISE%2CBOARD_RANK%2CBOARD_YIELD%2CDERIVE_BOARD_CODE&" \
-              f"quoteColumns=f3~05~NEW_BOARD_CODE~BOARD_YIELD&" \
-              f"filter=(SECUCODE%3D%22{stock_code}%22)(IS_PRECISE%3D%221%22)&pageNumber=1&pageSize=50&sortTypes=1&" \
-              f"sortColumns=BOARD_RANK&source=HSF10&client=PC"
-        res_json = requests.request('get', url, headers={}, proxies={}).json()
-        # 1. 返回结果判断
-        if not res_json['success']:
-            return pd.DataFrame(data=[], columns=self._CONCEPT_INFO_COLUMNS)
-
-        # 2. 正常返回数据结果封装
-        res_data = res_json['result']['data']
-        data = []
-        for _ in res_data:
-            # ['stock_code', 'short_name', 'concept_code', 'name', 'reason', 'source']
-            data.append({'stock_code': _['SECURITY_CODE'], 'concept_code': _['NEW_BOARD_CODE'],
-                         'name': _['BOARD_NAME'],
-                         'reason': _['SELECTED_BOARD_REASON'], 'source': '东方财富'})
-        result_df = pd.DataFrame(data=data, columns=self._CONCEPT_INFO_COLUMNS)
-        return result_df
-
-
-if __name__ == '__main__':
-    print(StockConceptEast().all_concept_code_east())
-    print(StockConceptEast().concept_constituent_east(concept_code="BK0637"))
-    print(StockConceptEast().get_concept_east(stock_code="600020").to_string())
+# -*- coding: utf-8 -*-
+"""
+@summary: 股票概念
+东方财富股票概念
+
+https://data.eastmoney.com/bkzj/gn.html
+
+单个股票的所有概念板块
+https://datacenter.eastmoney.com/securities/api/data/v1/get?reportName=RPT_F10_CORETHEME_BOARDTYPE&columns=SECUCODE%2CSECURITY_CODE%2CSECURITY_NAME_ABBR%2CNEW_BOARD_CODE%2CBOARD_NAME%2CSELECTED_BOARD_REASON%2CIS_PRECISE%2CBOARD_RANK%2CBOARD_YIELD%2CDERIVE_BOARD_CODE&quoteColumns=f3~05~NEW_BOARD_CODE~BOARD_YIELD&filter=(SECUCODE%3D%22600138.SH%22)(IS_PRECISE%3D%221%22)&pageNumber=1&pageSize=&sortTypes=1&sortColumns=BOARD_RANK&source=HSF10&client=PC&v=0029565688091059528
+@author: 1nchaos
+@date: 2023/3/30 16:17
+"""
+
+import pandas as pd
+
+from adata.common import requests
+from adata.common.utils.code_utils import compile_exchange_by_stock_code
+from adata.stock.info.concept.stock_concept_template import StockConceptTemplate
+
+
+class StockConceptEast(StockConceptTemplate):
+    """
+    东方财富股票概念
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def all_concept_code_east(self):
+        """
+        https://push2.eastmoney.com/api/qt/clist/get?pn=1&pz=1000&po=1&np=1&fields=f12%2Cf13%2Cf14%2Cf62&fid=f62&fs=m%3A90%2Bt%3A3
+        :return: 概念[[name,index_code，concept_code]]
+        """
+        url = f"https://push2.eastmoney.com/api/qt/clist/get" \
+              f"?pn=1&pz=1000&po=1&np=1&fields=f12%2Cf13%2Cf14%2Cf62&fid=f62&fs=m%3A90%2Bt%3A3"
+        res_json = requests.request('get', url, headers={}, proxies={}).json()
+        res_data = res_json['data']['diff']
+        data = []
+        for _ in res_data:
+            data.append({'index_code': _['f12'], 'concept_code': _['f12'], 'name': _['f14'], 'source': '东方财富'})
+        result_df = pd.DataFrame(data=data, columns=self._CONCEPT_CODE_COLUMNS)
+        return result_df
+
+    def concept_constituent_east(self, concept_code=None, wait_time=None):
+        """
+        https://data.eastmoney.com/bkzj/BK1085.html
+        https://push2.eastmoney.com/api/qt/clist/get?fid=f62&po=1&pz=1000&pn=1&np=1&fltt=2&invt=2&fs=b:BK0966&fields=f12,f14
+        :param wait_time: 等待时间：毫秒；表示每个请求的间隔时间，主要用于防止请求太频繁的限制。
+        :param concept_code: 概念代码，BK开头
+        :return: 概念的成分股
+        """
+        curr_page = 1
+        data = []
+        while curr_page < 6:
+            url = f"https://push2.eastmoney.com/api/qt/clist/get" \
+                  f"?fid=f62&po=1&pz=1000&pn={curr_page}&np=1&fltt=2&invt=2&fs=b:{concept_code}&fields=f12,f14"
+            res_json = requests.request('get', url, headers={}, proxies={}, wait_time=wait_time).json()
+            res_data = res_json['data']
+            if not res_data:
+                break
+            res_data = res_data['diff']
+            for _ in res_data:
+                data.append({'stock_code': _['f12'], 'short_name': _['f14']})
+            curr_page += 1
+        result_df = pd.DataFrame(data=data, columns=self._CONCEPT_CONSTITUENT_COLUMNS)
+        return result_df
+
+    def get_concept_east(self, stock_code: str = '000001'):
+        """
+        根据股票代码获取，股票所属的所有的概念信息
+        https://datacenter.eastmoney.com/securities/api/data/v1/get?
+        reportName=RPT_F10_CORETHEME_BOARDTYPE
+        &columns=SECUCODE%2CSECURITY_CODE%2CSECURITY_NAME_ABBR%2CNEW_BOARD_CODE%2CBOARD_NAME%2CSELECTED_BOARD_REASON%2CIS_PRECISE%2CBOARD_RANK%2CBOARD_YIELD%2CDERIVE_BOARD_CODE
+        &quoteColumns=f3~05~NEW_BOARD_CODE~BOARD_YIELD
+        &filter=(SECUCODE%3D%22600138.SH%22)(IS_PRECISE%3D%221%22)
+        &pageNumber=1&pageSize=&sortTypes=1&sortColumns=BOARD_RANK&source=HSF10&client=PC&v=0029565688091059528
+        :param stock_code: 股票代码
+        :return: 概念信息
+        """
+        stock_code = compile_exchange_by_stock_code(stock_code)
+        url = f"https://datacenter.eastmoney.com/securities/api/data/v1/get?" \
+              f"reportName=RPT_F10_CORETHEME_BOARDTYPE&" \
+              f"columns=SECUCODE%2CSECURITY_CODE%2CSECURITY_NAME_ABBR%2CNEW_BOARD_CODE%2CBOARD_NAME%2CSELECTED_BOARD_REASON%2CIS_PRECISE%2CBOARD_RANK%2CBOARD_YIELD%2CDERIVE_BOARD_CODE&" \
+              f"quoteColumns=f3~05~NEW_BOARD_CODE~BOARD_YIELD&" \
+              f"filter=(SECUCODE%3D%22{stock_code}%22)(IS_PRECISE%3D%221%22)&pageNumber=1&pageSize=50&sortTypes=1&" \
+              f"sortColumns=BOARD_RANK&source=HSF10&client=PC"
+        res_json = requests.request('get', url, headers={}, proxies={}).json()
+        # 1. 返回结果判断
+        if not res_json['success']:
+            return pd.DataFrame(data=[], columns=self._CONCEPT_INFO_COLUMNS)
+
+        # 2. 正常返回数据结果封装
+        res_data = res_json['result']['data']
+        data = []
+        for _ in res_data:
+            # ['stock_code', 'short_name', 'concept_code', 'name', 'reason', 'source']
+            data.append({'stock_code': _['SECURITY_CODE'], 'concept_code': _['NEW_BOARD_CODE'],
+                         'name': _['BOARD_NAME'],
+                         'reason': _['SELECTED_BOARD_REASON'], 'source': '东方财富'})
+        result_df = pd.DataFrame(data=data, columns=self._CONCEPT_INFO_COLUMNS)
+        return result_df
+
+
+if __name__ == '__main__':
+    print(StockConceptEast().all_concept_code_east())
+    print(StockConceptEast().concept_constituent_east(concept_code="BK0637"))
+    print(StockConceptEast().get_concept_east(stock_code="600020").to_string())
```

### Comparing `adata-1.2.4/adata/stock/info/concept/stock_concept_ths.py` & `adata-2.0.0b0/adata/stock/info/concept/stock_concept_ths.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,294 +1,294 @@
-# -*- coding: utf-8 -*-
-"""
-@summary: 股票概念
-同花顺概念更及时和完整，同花顺的股票概念抓取
-
-概念，指数成分
-来源于同花顺
-http://q.10jqka.com.cn/gn
-
-https://basic.10jqka.com.cn/000002/concept.html?cid=308717#ifind
-
-https://d.10jqka.com.cn/v4/stockblock/hs_600769/last.js
-https://m.10jqka.com.cn/stockpage/hs_600769/#&atab=pankou
-
-@author: 1nchaos
-@date: 2023/3/30 16:17
-"""
-import copy
-import json
-import math
-
-import pandas as pd
-from bs4 import BeautifulSoup
-
-from adata.common.exception.exception_msg import *
-from adata.common.headers import ths_headers
-from adata.common.utils import cookie
-from adata.common.utils import requests
-from adata.stock.info.concept.stock_concept_template import StockConceptTemplate
-
-
-class StockConceptThs(StockConceptTemplate):
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def all_concept_code_ths(self):
-        """
-        获取同花顺概念列表：名称,指数代码，概念代码
-        特别注意：
-        同花顺概念指数代码是8开头
-        概念代码是3开头
-        这两个不要混淆啦，同花顺的网站获取数据需要用到这两个代码
-        :return: 概念[[name,index_code，concept_code]]
-        """
-        index_df = self.__concept_index_code_ths()
-        code_df = self.__concept_code_ths()
-        result_df_l = pd.merge(index_df, code_df, how='left', on='name')
-        result_df_r = pd.merge(index_df, code_df, how='right', on='name')
-        result_df = pd.concat([result_df_l, result_df_r]).drop_duplicates(keep='first', inplace=False,
-                                                                          ignore_index=True)
-
-        index_df.drop(index_df.index, inplace=True)
-        code_df.drop(code_df.index, inplace=True)
-        result_df_l.drop(result_df_l.index, inplace=True)
-        result_df_r.drop(result_df_r.index, inplace=True)
-        result_df['source'] = '同花顺'
-        return result_df
-
-    def __concept_code_ths(self):
-        """
-        获取同花顺的所有概念和概念代码,暂时废弃
-        web: http://q.10jqka.com.cn/gn/
-        """
-        # 1. 请求接口 url
-        api_url = f"http://q.10jqka.com.cn/gn/"
-        for i in range(3):
-            res = requests.request('get', api_url, headers=ths_headers.text_headers, proxies={})
-            # 2. 判断请求是否正确
-            text = res.text
-            if res.status_code != 200 or len(text) < 1:
-                continue
-            # 3. 解析数据
-            soup = BeautifulSoup(text, 'html.parser')
-            data = []
-            for a in soup.find_all('a'):
-                href = str(a['href'])
-                if href.startswith(api_url + 'detail/code/'):
-                    data.append([href[-7: -1], a.string, href])
-
-            # 4. 封装数据
-            data_df = pd.DataFrame(data=data, columns=['concept_code', 'name', 'href'])[['concept_code', 'name']]
-            return data_df
-
-    def __concept_index_code_ths(self):
-        """
-        获取app的概率列表，通过问财询问得到结果
-        :return: app的概念列表： concept_code，name
-        """
-        data = []
-        for i in range(1, 10):
-            api_url = f"http://search.10jqka.com.cn/gateway/urp/v7/landing/getDataList?perpage=100&page={i}&query=%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5&condition=%5B%7B%22indexName%22%3A%22%E6%8C%87%E6%95%B0%40%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22indexProperties%22%3A%5B%5D%2C%22source%22%3A%22new_parser%22%2C%22type%22%3A%22index%22%2C%22indexPropertiesMap%22%3A%7B%7D%2C%22reportType%22%3A%22null%22%2C%22chunkedResult%22%3A%22%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5%22%2C%22valueType%22%3A%22_%E6%8C%87%E6%95%B0%E7%B1%BB%E5%9E%8B%22%2C%22domain%22%3A%22abs_a%E6%8C%87%E9%A2%86%E5%9F%9F%22%2C%22uiText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22sonSize%22%3A0%2C%22queryText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22relatedSize%22%3A0%7D%5D&urp_sort_index=%E6%8C%87%E6%95%B0%E4%BB%A3%E7%A0%81&source=Ths_iwencai_Xuangu&urp_sort_way=desc&codelist=&page_id=&logid=35df00ee5ae706d0dfcd0dbfdb846e0c&ret=json_all&sessionid=35df00ee5ae706d0dfcd0dbfdb846e0c&iwc_token=0ac9667016801698001765831&user_id=Ths_iwencai_Xuangu_7fahywzhbkrh4lwwkwfw936njqbjzsly&uuids%5B0%5D=23119&query_type=zhishu&comp_id=6367801&business_cat=soniu&uuid=23119"
-            res = requests.request('get', url=api_url, headers=ths_headers.c_headers)
-            res_json = res.json()
-            if res_json['status_msg'] == 'ok':
-                data_list = res_json['answer']['components'][0]['data']['datas']
-                if len(data_list) < 1:
-                    break
-                for d in data_list:
-                    data.append([d['code'], d['指数简称']])
-        data_df = pd.DataFrame(data=data, columns=['index_code', 'name']).drop_duplicates(keep='first', inplace=False,
-                                                                                          ignore_index=True)
-        return data_df
-
-    def concept_constituent_ths(self, concept_code=None, name=None, index_code=None, wait_time=None):
-        """
-        获取同花顺概念成分
-        优先级
-        index_code >  name > concept_code: 三选其一
-        指数代码来自app，名称查询来自问财，概念代码来自网页；
-        :param wait_time: 等待时间：毫秒；表示每个请求的间隔时间，主要用于防止请求太频繁的限制。
-        :param concept_code: 概念代码，3开头
-        :param index_code: 指数代码，8开头
-        :param name: 概念名称
-        :return: 概念的成分股
-        """
-        if concept_code:
-            return self.__index_constituent_ths_by_concept_code(concept_code=concept_code, wait_time=wait_time)
-        elif name:
-            return self.__index_constituent_ths_by_name(name=name, wait_time=wait_time)
-        elif index_code:
-            return self.__index_constituent_ths_by_index_code(index_code=index_code, wait_time=wait_time)
-        else:
-            return pd.DataFrame(data=[], columns=self._CONCEPT_CONSTITUENT_COLUMNS)
-
-    def __index_constituent_ths_by_concept_code(self, concept_code=None, wait_time=None):
-        """
-        同花顺概念成分股
-        web_url :http://q.10jqka.com.cn/gn/detail/field/199112/order/desc/page/1/ajax/1/code/301539
-        answer: http://www.iwencai.com/gateway/urp/v7/landing/getDataList?query=chatgpt%20%E6%A6%82%E5%BF%B5%E6%88%90%E5%88%86&page=1&perpage=100&query_type=stock&comp_id=6734520&uuid=24087
-        :param concept_code: 概念代码： 301539
-        :param wait_time: 等待时间：表示每个请求的间隔时间，主要用于防止请求太频繁的限制。
-        :return:['concept_code', 'stock_code', 'short_name']
-        """
-        # 1. url拼接页码等参数
-        data = []
-        total_pages = 1
-        curr_page = 1
-        while curr_page <= total_pages:
-            api_url = f"http://q.10jqka.com.cn/gn/detail/field/199112/order/desc/page/" \
-                      f"{curr_page}/ajax/1/code/{concept_code}"
-            headers = copy.deepcopy(ths_headers.text_headers)
-            headers['Cookie'] = cookie.ths_cookie()
-            res = requests.request(method='get', url=api_url, headers=headers, proxies={}, wait_time=wait_time)
-            curr_page += 1
-            # 2. 判断请求是否成功
-            if res.status_code != 200:
-                continue
-            text = res.text
-            if THS_IP_LIMIT_RES in text:
-                return Exception(THS_IP_LIMIT_MSG)
-            if '暂无成份股数据' in text or '概念板块' in text or '概念时间表' in text:
-                break
-            soup = BeautifulSoup(text, 'html.parser')
-            # 3 .获取总的页数
-            if total_pages == 1:
-                page_info = soup.find('span', {'class': 'page_info'})
-                if page_info:
-                    total_pages = int(page_info.text.split("/")[1])
-            # 4. 解析数据
-            page_data = []
-            for idx, tr in enumerate(soup.find_all('tr')):
-                if idx != 0:
-                    tds = tr.find_all('td')
-                    page_data.append({'stock_code': tds[1].contents[0].text, 'short_name': tds[2].contents[0].text})
-            data.extend(page_data)
-        # 5. 封装数据
-        if not data:
-            return pd.DataFrame(data=data, columns=self._CONCEPT_CONSTITUENT_COLUMNS)
-        result_df = pd.DataFrame(data=data)
-        data.clear()
-        return result_df[self._CONCEPT_CONSTITUENT_COLUMNS]
-
-    def __index_constituent_ths_by_index_code(self, index_code=None, wait_time=None):
-        """
-        根据概念指数代码获取成分股
-        web_url： https://d.10jqka.com.cn/v2/blockrank/885338/8/d3000.js
-        :param index_code: 指数代码，ths 8开头
-        :param wait_time: 等待时间：表示每个请求的间隔时间，主要用于防止请求太频繁的限制。
-        :return: ['stock_code', 'short_name']
-        """
-        # 1.接口 url
-        api_url = f"https://d.10jqka.com.cn/v2/blockrank/{index_code}/8/d15.js"
-        headers = copy.deepcopy(ths_headers.text_headers)
-        headers['Host'] = 'd.10jqka.com.cn'
-        res = requests.request(method='get', url=api_url, headers=headers, proxies={}, wait_time=wait_time)
-        # 同花顺可能ip限制，降低请求次数
-        text = res.text
-        if THS_IP_LIMIT_RES in text:
-            return Exception(THS_IP_LIMIT_MSG)
-        # 2. 解析总数
-        result_json = json.loads(text[text.index('{'):-1])
-        total_count = float(result_json['block']['subcodeCount'])
-        if total_count < 2500:
-            total_num = math.ceil(total_count / 15) * 15
-            apis = [f"https://d.10jqka.com.cn/v2/blockrank/{index_code}/8/d{total_num}.js"]
-        else:
-            apis = [f"https://d.10jqka.com.cn/v2/blockrank/{index_code}/8/a2500.js",
-                    f"https://d.10jqka.com.cn/v2/blockrank/{index_code}/8/d2500.js"]
-        data_list = []
-
-        # 3. 请求所有数据
-        for api_url in apis:
-            res = requests.request(method='get', url=api_url, headers=headers, proxies={}, wait_time=wait_time)
-            text = res.text
-            result_json = json.loads(text[text.index('{'):-1])
-            items = result_json['items']
-            data_list.extend(items)
-
-        # 4. 数据封装，去重
-        rename = {'5': 'stock_code', '55': 'short_name'}
-        result_df = pd.DataFrame(data=data_list).rename(columns=rename)
-        result_df = result_df.drop_duplicates(subset=['stock_code'], keep='last', ignore_index=True)
-        return result_df[self._CONCEPT_CONSTITUENT_COLUMNS]
-
-    def __index_constituent_ths_by_name(self, name=None, wait_time=None):
-        """
-        同花顺概念成分股，通过问财询问
-        answer: http://www.iwencai.com/gateway/urp/v7/landing/getDataList?query=chatgpt%20%E6%A6%82%E5%BF%B5%E6%88%90%E5%88%86&page=1&perpage=100&query_type=stock&comp_id=6734520&uuid=24087
-        :param name: 概念名称
-        :param wait_time: 等待时间：表示每个请求的间隔时间，主要用于防止请求太频繁的限制。
-        :return:['concept_code', 'stock_code', 'short_name']
-        """
-        # 1. url拼接页码等参数
-        data = []
-        total_pages = 1
-        curr_page = 1
-        while curr_page <= total_pages:
-            api_url = f"https://www.iwencai.com/gateway/urp/v7/landing/getDataList?query={name} 概念成分&" \
-                      f"page={curr_page}&perpage=100&query_type=stock&comp_id=6734520&uuid=24087"
-            headers = copy.deepcopy(ths_headers.json_headers)
-            headers['Host'] = 'www.iwencai.com'
-            headers['Sec-Fetch-Mode'] = 'navigate'
-            res = requests.request(method='get', url=api_url, headers=headers, proxies={}, wait_time=wait_time)
-            curr_page += 1
-            # 2. 判断请求是否成功
-            if res.status_code != 200:
-                continue
-            text = res.text.encode('utf-8').decode('unicode escape')
-            if THS_IP_LIMIT_RES in text:
-                return Exception(THS_IP_LIMIT_MSG)
-            if name not in text:
-                break
-            res_json = res.json()
-            data_dic = res_json['answer']['components'][0]['data']
-            # 3 .获取总的页数
-            if total_pages == 1:
-                total_pages = math.ceil(data_dic['meta']['extra']['code_count'] / 100)
-            # 4. 解析数据
-            page_data = []
-            data_list = data_dic['datas']
-            for one in data_list:
-                if (name == one['所属概念']) or \
-                        ('所属指数类' in one.keys() and (name == one['所属指数类'] or f"{name};" in one['所属指数类'])):
-                    page_data.append({'stock_code': one['code'], 'short_name': one['股票简称'], '': ''})
-            data.extend(page_data)
-        # 5. 封装数据
-        if not data:
-            return pd.DataFrame(data=data, columns=self._CONCEPT_CONSTITUENT_COLUMNS)
-        result_df = pd.DataFrame(data=data)
-        data.clear()
-        return result_df[self._CONCEPT_CONSTITUENT_COLUMNS]
-
-    def get_concept_ths(self, stock_code: str = '000001'):
-        """
-        根据股票代码获取，股票所属的所有的概念信息
-        https://basic.10jqka.com.cn/300033/concept.html
-        :param stock_code: 股票代码
-        :return: 概念信息
-        """
-        url = f"https://basic.10jqka.com.cn/{stock_code}/concept.html"
-        headers = ths_headers.text_headers
-        headers['Host'] = 'basic.10jqka.com.cn'
-        res = requests.request('get', url, headers=headers, proxies={})
-        # 3. 解析数据
-        text = res.content.decode('gbk')
-        soup = BeautifulSoup(text, 'html.parser')
-        table = soup.find('table', attrs={'class': 'gnContent'})
-        trs = table.tbody.find_all('tr')
-        data = []
-        for i in range(0, len(trs), 2):
-            columns = trs[i].find_all('td')
-            data.append({'stock_code': stock_code, 'concept_code': columns[1].get('clid'),
-                         'name': columns[1].text,
-                         'reason': trs[i + 1].text, 'source': '同花顺'})
-        result_df = pd.DataFrame(data=data, columns=self._CONCEPT_INFO_COLUMNS)
-        result_df.replace(to_replace=[r'\t', r'\n', ' '], value='', regex=True, inplace=True)
-        return result_df
-
-
-if __name__ == '__main__':
-    # print(StockConceptThs().all_concept_code_ths())
-    print(StockConceptThs().get_concept_ths(stock_code='300033')[
-              ['stock_code', 'concept_code', 'name', 'source','reason']].to_string())
+# -*- coding: utf-8 -*-
+"""
+@summary: 股票概念
+同花顺概念更及时和完整，同花顺的股票概念抓取
+
+概念，指数成分
+来源于同花顺
+http://q.10jqka.com.cn/gn
+
+https://basic.10jqka.com.cn/000002/concept.html?cid=308717#ifind
+
+https://d.10jqka.com.cn/v4/stockblock/hs_600769/last.js
+https://m.10jqka.com.cn/stockpage/hs_600769/#&atab=pankou
+
+@author: 1nchaos
+@date: 2023/3/30 16:17
+"""
+import copy
+import json
+import math
+
+import pandas as pd
+from bs4 import BeautifulSoup
+
+from adata.common.exception.exception_msg import *
+from adata.common.headers import ths_headers
+from adata.common.utils import cookie
+from adata.common.utils import requests
+from adata.stock.info.concept.stock_concept_template import StockConceptTemplate
+
+
+class StockConceptThs(StockConceptTemplate):
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def all_concept_code_ths(self):
+        """
+        获取同花顺概念列表：名称,指数代码，概念代码
+        特别注意：
+        同花顺概念指数代码是8开头
+        概念代码是3开头
+        这两个不要混淆啦，同花顺的网站获取数据需要用到这两个代码
+        :return: 概念[[name,index_code，concept_code]]
+        """
+        index_df = self.__concept_index_code_ths()
+        code_df = self.__concept_code_ths()
+        result_df_l = pd.merge(index_df, code_df, how='left', on='name')
+        result_df_r = pd.merge(index_df, code_df, how='right', on='name')
+        result_df = pd.concat([result_df_l, result_df_r]).drop_duplicates(keep='first', inplace=False,
+                                                                          ignore_index=True)
+
+        index_df.drop(index_df.index, inplace=True)
+        code_df.drop(code_df.index, inplace=True)
+        result_df_l.drop(result_df_l.index, inplace=True)
+        result_df_r.drop(result_df_r.index, inplace=True)
+        result_df['source'] = '同花顺'
+        return result_df
+
+    def __concept_code_ths(self):
+        """
+        获取同花顺的所有概念和概念代码,暂时废弃
+        web: http://q.10jqka.com.cn/gn/
+        """
+        # 1. 请求接口 url
+        api_url = f"http://q.10jqka.com.cn/gn/"
+        for i in range(3):
+            res = requests.request('get', api_url, headers=ths_headers.text_headers, proxies={})
+            # 2. 判断请求是否正确
+            text = res.text
+            if res.status_code != 200 or len(text) < 1:
+                continue
+            # 3. 解析数据
+            soup = BeautifulSoup(text, 'html.parser')
+            data = []
+            for a in soup.find_all('a'):
+                href = str(a['href'])
+                if href.startswith(api_url + 'detail/code/'):
+                    data.append([href[-7: -1], a.string, href])
+
+            # 4. 封装数据
+            data_df = pd.DataFrame(data=data, columns=['concept_code', 'name', 'href'])[['concept_code', 'name']]
+            return data_df
+
+    def __concept_index_code_ths(self):
+        """
+        获取app的概率列表，通过问财询问得到结果
+        :return: app的概念列表： concept_code，name
+        """
+        data = []
+        for i in range(1, 10):
+            api_url = f"http://search.10jqka.com.cn/gateway/urp/v7/landing/getDataList?perpage=100&page={i}&query=%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5&condition=%5B%7B%22indexName%22%3A%22%E6%8C%87%E6%95%B0%40%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22indexProperties%22%3A%5B%5D%2C%22source%22%3A%22new_parser%22%2C%22type%22%3A%22index%22%2C%22indexPropertiesMap%22%3A%7B%7D%2C%22reportType%22%3A%22null%22%2C%22chunkedResult%22%3A%22%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5%22%2C%22valueType%22%3A%22_%E6%8C%87%E6%95%B0%E7%B1%BB%E5%9E%8B%22%2C%22domain%22%3A%22abs_a%E6%8C%87%E9%A2%86%E5%9F%9F%22%2C%22uiText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22sonSize%22%3A0%2C%22queryText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22relatedSize%22%3A0%7D%5D&urp_sort_index=%E6%8C%87%E6%95%B0%E4%BB%A3%E7%A0%81&source=Ths_iwencai_Xuangu&urp_sort_way=desc&codelist=&page_id=&logid=35df00ee5ae706d0dfcd0dbfdb846e0c&ret=json_all&sessionid=35df00ee5ae706d0dfcd0dbfdb846e0c&iwc_token=0ac9667016801698001765831&user_id=Ths_iwencai_Xuangu_7fahywzhbkrh4lwwkwfw936njqbjzsly&uuids%5B0%5D=23119&query_type=zhishu&comp_id=6367801&business_cat=soniu&uuid=23119"
+            res = requests.request('get', url=api_url, headers=ths_headers.c_headers)
+            res_json = res.json()
+            if res_json['status_msg'] == 'ok':
+                data_list = res_json['answer']['components'][0]['data']['datas']
+                if len(data_list) < 1:
+                    break
+                for d in data_list:
+                    data.append([d['code'], d['指数简称']])
+        data_df = pd.DataFrame(data=data, columns=['index_code', 'name']).drop_duplicates(keep='first', inplace=False,
+                                                                                          ignore_index=True)
+        return data_df
+
+    def concept_constituent_ths(self, concept_code=None, name=None, index_code=None, wait_time=None):
+        """
+        获取同花顺概念成分
+        优先级
+        index_code >  name > concept_code: 三选其一
+        指数代码来自app，名称查询来自问财，概念代码来自网页；
+        :param wait_time: 等待时间：毫秒；表示每个请求的间隔时间，主要用于防止请求太频繁的限制。
+        :param concept_code: 概念代码，3开头
+        :param index_code: 指数代码，8开头
+        :param name: 概念名称
+        :return: 概念的成分股
+        """
+        if concept_code:
+            return self.__index_constituent_ths_by_concept_code(concept_code=concept_code, wait_time=wait_time)
+        elif name:
+            return self.__index_constituent_ths_by_name(name=name, wait_time=wait_time)
+        elif index_code:
+            return self.__index_constituent_ths_by_index_code(index_code=index_code, wait_time=wait_time)
+        else:
+            return pd.DataFrame(data=[], columns=self._CONCEPT_CONSTITUENT_COLUMNS)
+
+    def __index_constituent_ths_by_concept_code(self, concept_code=None, wait_time=None):
+        """
+        同花顺概念成分股
+        web_url :http://q.10jqka.com.cn/gn/detail/field/199112/order/desc/page/1/ajax/1/code/301539
+        answer: http://www.iwencai.com/gateway/urp/v7/landing/getDataList?query=chatgpt%20%E6%A6%82%E5%BF%B5%E6%88%90%E5%88%86&page=1&perpage=100&query_type=stock&comp_id=6734520&uuid=24087
+        :param concept_code: 概念代码： 301539
+        :param wait_time: 等待时间：表示每个请求的间隔时间，主要用于防止请求太频繁的限制。
+        :return:['concept_code', 'stock_code', 'short_name']
+        """
+        # 1. url拼接页码等参数
+        data = []
+        total_pages = 1
+        curr_page = 1
+        while curr_page <= total_pages:
+            api_url = f"http://q.10jqka.com.cn/gn/detail/field/199112/order/desc/page/" \
+                      f"{curr_page}/ajax/1/code/{concept_code}"
+            headers = copy.deepcopy(ths_headers.text_headers)
+            headers['Cookie'] = cookie.ths_cookie()
+            res = requests.request(method='get', url=api_url, headers=headers, proxies={}, wait_time=wait_time)
+            curr_page += 1
+            # 2. 判断请求是否成功
+            if res.status_code != 200:
+                continue
+            text = res.text
+            if THS_IP_LIMIT_RES in text:
+                return Exception(THS_IP_LIMIT_MSG)
+            if '暂无成份股数据' in text or '概念板块' in text or '概念时间表' in text:
+                break
+            soup = BeautifulSoup(text, 'html.parser')
+            # 3 .获取总的页数
+            if total_pages == 1:
+                page_info = soup.find('span', {'class': 'page_info'})
+                if page_info:
+                    total_pages = int(page_info.text.split("/")[1])
+            # 4. 解析数据
+            page_data = []
+            for idx, tr in enumerate(soup.find_all('tr')):
+                if idx != 0:
+                    tds = tr.find_all('td')
+                    page_data.append({'stock_code': tds[1].contents[0].text, 'short_name': tds[2].contents[0].text})
+            data.extend(page_data)
+        # 5. 封装数据
+        if not data:
+            return pd.DataFrame(data=data, columns=self._CONCEPT_CONSTITUENT_COLUMNS)
+        result_df = pd.DataFrame(data=data)
+        data.clear()
+        return result_df[self._CONCEPT_CONSTITUENT_COLUMNS]
+
+    def __index_constituent_ths_by_index_code(self, index_code=None, wait_time=None):
+        """
+        根据概念指数代码获取成分股
+        web_url： https://d.10jqka.com.cn/v2/blockrank/885338/8/d3000.js
+        :param index_code: 指数代码，ths 8开头
+        :param wait_time: 等待时间：表示每个请求的间隔时间，主要用于防止请求太频繁的限制。
+        :return: ['stock_code', 'short_name']
+        """
+        # 1.接口 url
+        api_url = f"https://d.10jqka.com.cn/v2/blockrank/{index_code}/8/d15.js"
+        headers = copy.deepcopy(ths_headers.text_headers)
+        headers['Host'] = 'd.10jqka.com.cn'
+        res = requests.request(method='get', url=api_url, headers=headers, proxies={}, wait_time=wait_time)
+        # 同花顺可能ip限制，降低请求次数
+        text = res.text
+        if THS_IP_LIMIT_RES in text:
+            return Exception(THS_IP_LIMIT_MSG)
+        # 2. 解析总数
+        result_json = json.loads(text[text.index('{'):-1])
+        total_count = float(result_json['block']['subcodeCount'])
+        if total_count < 2500:
+            total_num = math.ceil(total_count / 15) * 15
+            apis = [f"https://d.10jqka.com.cn/v2/blockrank/{index_code}/8/d{total_num}.js"]
+        else:
+            apis = [f"https://d.10jqka.com.cn/v2/blockrank/{index_code}/8/a2500.js",
+                    f"https://d.10jqka.com.cn/v2/blockrank/{index_code}/8/d2500.js"]
+        data_list = []
+
+        # 3. 请求所有数据
+        for api_url in apis:
+            res = requests.request(method='get', url=api_url, headers=headers, proxies={}, wait_time=wait_time)
+            text = res.text
+            result_json = json.loads(text[text.index('{'):-1])
+            items = result_json['items']
+            data_list.extend(items)
+
+        # 4. 数据封装，去重
+        rename = {'5': 'stock_code', '55': 'short_name'}
+        result_df = pd.DataFrame(data=data_list).rename(columns=rename)
+        result_df = result_df.drop_duplicates(subset=['stock_code'], keep='last', ignore_index=True)
+        return result_df[self._CONCEPT_CONSTITUENT_COLUMNS]
+
+    def __index_constituent_ths_by_name(self, name=None, wait_time=None):
+        """
+        同花顺概念成分股，通过问财询问
+        answer: http://www.iwencai.com/gateway/urp/v7/landing/getDataList?query=chatgpt%20%E6%A6%82%E5%BF%B5%E6%88%90%E5%88%86&page=1&perpage=100&query_type=stock&comp_id=6734520&uuid=24087
+        :param name: 概念名称
+        :param wait_time: 等待时间：表示每个请求的间隔时间，主要用于防止请求太频繁的限制。
+        :return:['concept_code', 'stock_code', 'short_name']
+        """
+        # 1. url拼接页码等参数
+        data = []
+        total_pages = 1
+        curr_page = 1
+        while curr_page <= total_pages:
+            api_url = f"https://www.iwencai.com/gateway/urp/v7/landing/getDataList?query={name} 概念成分&" \
+                      f"page={curr_page}&perpage=100&query_type=stock&comp_id=6734520&uuid=24087"
+            headers = copy.deepcopy(ths_headers.json_headers)
+            headers['Host'] = 'www.iwencai.com'
+            headers['Sec-Fetch-Mode'] = 'navigate'
+            res = requests.request(method='get', url=api_url, headers=headers, proxies={}, wait_time=wait_time)
+            curr_page += 1
+            # 2. 判断请求是否成功
+            if res.status_code != 200:
+                continue
+            text = res.text.encode('utf-8').decode('unicode escape')
+            if THS_IP_LIMIT_RES in text:
+                return Exception(THS_IP_LIMIT_MSG)
+            if name not in text:
+                break
+            res_json = res.json()
+            data_dic = res_json['answer']['components'][0]['data']
+            # 3 .获取总的页数
+            if total_pages == 1:
+                total_pages = math.ceil(data_dic['meta']['extra']['code_count'] / 100)
+            # 4. 解析数据
+            page_data = []
+            data_list = data_dic['datas']
+            for one in data_list:
+                if (name == one['所属概念']) or \
+                        ('所属指数类' in one.keys() and (name == one['所属指数类'] or f"{name};" in one['所属指数类'])):
+                    page_data.append({'stock_code': one['code'], 'short_name': one['股票简称'], '': ''})
+            data.extend(page_data)
+        # 5. 封装数据
+        if not data:
+            return pd.DataFrame(data=data, columns=self._CONCEPT_CONSTITUENT_COLUMNS)
+        result_df = pd.DataFrame(data=data)
+        data.clear()
+        return result_df[self._CONCEPT_CONSTITUENT_COLUMNS]
+
+    def get_concept_ths(self, stock_code: str = '000001'):
+        """
+        根据股票代码获取，股票所属的所有的概念信息
+        https://basic.10jqka.com.cn/300033/concept.html
+        :param stock_code: 股票代码
+        :return: 概念信息
+        """
+        url = f"https://basic.10jqka.com.cn/{stock_code}/concept.html"
+        headers = ths_headers.text_headers
+        headers['Host'] = 'basic.10jqka.com.cn'
+        res = requests.request('get', url, headers=headers, proxies={})
+        # 3. 解析数据
+        text = res.content.decode('gbk')
+        soup = BeautifulSoup(text, 'html.parser')
+        table = soup.find('table', attrs={'class': 'gnContent'})
+        trs = table.tbody.find_all('tr')
+        data = []
+        for i in range(0, len(trs), 2):
+            columns = trs[i].find_all('td')
+            data.append({'stock_code': stock_code, 'concept_code': columns[1].get('clid'),
+                         'name': columns[1].text,
+                         'reason': trs[i + 1].text, 'source': '同花顺'})
+        result_df = pd.DataFrame(data=data, columns=self._CONCEPT_INFO_COLUMNS)
+        result_df.replace(to_replace=[r'\t', r'\n', ' '], value='', regex=True, inplace=True)
+        return result_df
+
+
+if __name__ == '__main__':
+    # print(StockConceptThs().all_concept_code_ths())
+    print(StockConceptThs().get_concept_ths(stock_code='300033')[
+              ['stock_code', 'concept_code', 'name', 'source','reason']].to_string())
```

### Comparing `adata-1.2.4/adata/stock/info/stock_code.py` & `adata-2.0.0b0/adata/stock/info/stock_code.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-# -*- coding: utf-8 -*-
-"""
-@desc: 股票代码，上市日期等信息
-深交所
-http://www.szse.cn/market/product/stock/list/index.html
-上海交易所
-http://www.sse.com.cn/assortment/stock/list/share/
-北交所
-https://www.bse.cn/nq/listedcompany.html
-
-东方财富：新股列表可做最新的补充
-https://data.eastmoney.com/xg/xg/
-
-@author: 1nchaos
-@time: 2023/3/28
-@log: change log
-"""
-import time
-
-import numpy as np
-import pandas as pd
-import requests
-
-from adata.common.exception.handler import handler_null
-from adata.common.headers import baidu_headers
-from adata.stock.cache import get_code_csv_path
-
-
-class StockCode(object):
-    """
-    股票代码
-    """
-    __CODE_COLUMNS = ['stock_code', 'short_name', 'exchange', 'list_date']
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def all_code(self):
-        """
-        获取所有股票的代码
-        :return: 所有股票的代码信息：  ['stock_code', 'short_name', 'exchange', 'list_date']
-        """
-        # 拼接股票上市日期
-        code = pd.read_csv(get_code_csv_path())[['stock_code', 'list_date2']]
-        res_df = self.__market_rank_baidu()
-        east = self.__new_sub_east()
-        if not east.empty:
-            res_df = pd.concat([east, res_df], axis=0, ignore_index=True)
-            res_df = res_df.drop_duplicates(subset=['stock_code'], keep='first')
-        res_df['stock_code'] = res_df['stock_code'].astype(str)
-        code['stock_code'] = code['stock_code'].astype(str).str.zfill(6)
-        df = pd.merge(res_df, code, on='stock_code', how='left')
-        df['list_date'] = df['list_date'].fillna(df['list_date2'])
-        return df.sort_values('stock_code').reset_index(drop=True)[self.__CODE_COLUMNS]
-
-    def __market_rank_baidu(self):
-        """
-        获取百度当前涨幅排名的代码
-        web： https://gushitong.baidu.com/top/ab-increase-%E6%B6%A8%E5%B9%85%E6%A6%9C
-        url：https://finance.pae.baidu.com/selfselect/getmarketrank?sort_type=1&sort_key=14&from_mid=1&pn=0&rn=200&group=pclist&type=ab&finClientType=pc
-        其中：pn 起始数 rn 翻页数，最大200
-        :return 代码列表：['stock_code','short_name','exchange']
-        """
-        # 1. 请求市场排名的 url
-        api_url = f"https://finance.pae.baidu.com/selfselect/getmarketrank" \
-                  f"?sort_type=1&sort_key=14&from_mid=1&group=pclist&type=ab&finClientType=pc"
-        max_page_size = 200
-        data = []
-
-        # 2. 一直翻页请求数据，股票目前数据5000,50页一共1w只,后续增加了可以再加
-        for page_no in range(49):
-            api_url = f"{api_url}&pn={page_no * max_page_size}&rn={max_page_size}"
-            try:
-                res = requests.get(api_url, headers=baidu_headers.json_headers, proxies={})
-                res_json = res.json()
-                if res.status_code != 200 or res_json['ResultCode'] != '0':
-                    continue
-                # 3. 解析数据
-                result = res_json['Result']['Result']
-                # 结果为空跳出循环
-                if not result:
-                    break
-                code_list = result[0]['DisplayData']['resultData']['tplData']['result']['rank']
-                data.extend(code_list)
-            except Exception as e:
-                time.sleep(2)
-                print(e)
-                continue
-        # 4. 封装数据
-        rename = {'name': 'short_name', 'code': 'stock_code'}
-        df = pd.DataFrame(data=data)[['code', 'name', 'exchange']].rename(columns=rename)
-        df['list_date'] = np.nan
-        return df[self.__CODE_COLUMNS]
-
-    @handler_null
-    def __new_sub_east(self):
-        """
-        东方财富新股申购列表
-        https://data.eastmoney.com/xg/xg/default.html
-        https://datacenter-web.eastmoney.com/api/data/v1/get?sortColumns=APPLY_DATE,SECURITY_CODE&sortTypes=-1,-1&pageSize=50&pageNumber=1&reportName=RPTA_APP_IPOAPPLY&columns=SECURITY_CODE,SECURITY_NAME&quoteType=0&filter=(APPLY_DATE>'2010-01-01')&source=WEB&client=WEB
-        """
-        data = []
-        for i in range(100):
-            url = f"https://datacenter-web.eastmoney.com/api/data/v1/get?" \
-                  f"sortColumns=APPLY_DATE,SECURITY_CODE&sortTypes=-1,-1&pageSize=50&pageNumber={i + 1}&" \
-                  f"reportName=RPTA_APP_IPOAPPLY&columns=SECURITY_CODE,SECURITY_NAME,TRADE_MARKET,LISTING_DATE&quoteType=0&" \
-                  f"filter=(APPLY_DATE>'2010-01-01')&source=WEB&client=WEB"
-            res_json = requests.request('get', url, headers={}, proxies={}).json()
-            res_data = res_json['result']['data']
-            for _ in res_data:
-                exchange = str(_['TRADE_MARKET'])
-                if exchange.startswith('上海'):
-                    exchange = 'SH'
-                elif exchange.startswith('深圳'):
-                    exchange = 'SZ'
-                elif exchange.startswith('北京'):
-                    exchange = 'BJ'
-                if _['LISTING_DATE']:
-                    data.append({'stock_code': _['SECURITY_CODE'], 'short_name': _['SECURITY_NAME'],
-                                 'exchange': exchange, 'list_date': _['LISTING_DATE']})
-            # if pd.to_datetime(data[-1]['list_date']) < pd.to_datetime('2023-10-01'):
-            if pd.to_datetime(data[-1]['list_date']) < pd.to_datetime('2020-01-01'):
-                break
-        result_df = pd.DataFrame(data=data, columns=self.__CODE_COLUMNS)
-        result_df['list_date'] = pd.to_datetime(result_df['list_date']).dt.date
-        return result_df
-
-
-if __name__ == '__main__':
-    print(StockCode().all_code())
+# -*- coding: utf-8 -*-
+"""
+@desc: 股票代码，上市日期等信息
+深交所
+http://www.szse.cn/market/product/stock/list/index.html
+上海交易所
+http://www.sse.com.cn/assortment/stock/list/share/
+北交所
+https://www.bse.cn/nq/listedcompany.html
+
+东方财富：新股列表可做最新的补充
+https://data.eastmoney.com/xg/xg/
+
+@author: 1nchaos
+@time: 2023/3/28
+@log: change log
+"""
+import time
+
+import numpy as np
+import pandas as pd
+import requests
+
+from adata.common.exception.handler import handler_null
+from adata.common.headers import baidu_headers
+from adata.stock.cache import get_code_csv_path
+
+
+class StockCode(object):
+    """
+    股票代码
+    """
+    __CODE_COLUMNS = ['stock_code', 'short_name', 'exchange', 'list_date']
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def all_code(self):
+        """
+        获取所有股票的代码
+        :return: 所有股票的代码信息：  ['stock_code', 'short_name', 'exchange', 'list_date']
+        """
+        # 拼接股票上市日期
+        code = pd.read_csv(get_code_csv_path())[['stock_code', 'list_date2']]
+        res_df = self.__market_rank_baidu()
+        east = self.__new_sub_east()
+        if not east.empty:
+            res_df = pd.concat([east, res_df], axis=0, ignore_index=True)
+            res_df = res_df.drop_duplicates(subset=['stock_code'], keep='first')
+        res_df['stock_code'] = res_df['stock_code'].astype(str)
+        code['stock_code'] = code['stock_code'].astype(str).str.zfill(6)
+        df = pd.merge(res_df, code, on='stock_code', how='left')
+        df['list_date'] = df['list_date'].fillna(df['list_date2'])
+        return df.sort_values('stock_code').reset_index(drop=True)[self.__CODE_COLUMNS]
+
+    def __market_rank_baidu(self):
+        """
+        获取百度当前涨幅排名的代码
+        web： https://gushitong.baidu.com/top/ab-increase-%E6%B6%A8%E5%B9%85%E6%A6%9C
+        url：https://finance.pae.baidu.com/selfselect/getmarketrank?sort_type=1&sort_key=14&from_mid=1&pn=0&rn=200&group=pclist&type=ab&finClientType=pc
+        其中：pn 起始数 rn 翻页数，最大200
+        :return 代码列表：['stock_code','short_name','exchange']
+        """
+        # 1. 请求市场排名的 url
+        api_url = f"https://finance.pae.baidu.com/selfselect/getmarketrank" \
+                  f"?sort_type=1&sort_key=14&from_mid=1&group=pclist&type=ab&finClientType=pc"
+        max_page_size = 200
+        data = []
+
+        # 2. 一直翻页请求数据，股票目前数据5000,50页一共1w只,后续增加了可以再加
+        for page_no in range(49):
+            api_url = f"{api_url}&pn={page_no * max_page_size}&rn={max_page_size}"
+            try:
+                res = requests.get(api_url, headers=baidu_headers.json_headers, proxies={})
+                res_json = res.json()
+                if res.status_code != 200 or res_json['ResultCode'] != '0':
+                    continue
+                # 3. 解析数据
+                result = res_json['Result']['Result']
+                # 结果为空跳出循环
+                if not result:
+                    break
+                code_list = result[0]['DisplayData']['resultData']['tplData']['result']['rank']
+                data.extend(code_list)
+            except Exception as e:
+                time.sleep(2)
+                print(e)
+                continue
+        # 4. 封装数据
+        rename = {'name': 'short_name', 'code': 'stock_code'}
+        df = pd.DataFrame(data=data)[['code', 'name', 'exchange']].rename(columns=rename)
+        df['list_date'] = np.nan
+        return df[self.__CODE_COLUMNS]
+
+    @handler_null
+    def __new_sub_east(self):
+        """
+        东方财富新股申购列表
+        https://data.eastmoney.com/xg/xg/default.html
+        https://datacenter-web.eastmoney.com/api/data/v1/get?sortColumns=APPLY_DATE,SECURITY_CODE&sortTypes=-1,-1&pageSize=50&pageNumber=1&reportName=RPTA_APP_IPOAPPLY&columns=SECURITY_CODE,SECURITY_NAME&quoteType=0&filter=(APPLY_DATE>'2010-01-01')&source=WEB&client=WEB
+        """
+        data = []
+        for i in range(100):
+            url = f"https://datacenter-web.eastmoney.com/api/data/v1/get?" \
+                  f"sortColumns=APPLY_DATE,SECURITY_CODE&sortTypes=-1,-1&pageSize=50&pageNumber={i + 1}&" \
+                  f"reportName=RPTA_APP_IPOAPPLY&columns=SECURITY_CODE,SECURITY_NAME,TRADE_MARKET,LISTING_DATE&quoteType=0&" \
+                  f"filter=(APPLY_DATE>'2010-01-01')&source=WEB&client=WEB"
+            res_json = requests.request('get', url, headers={}, proxies={}).json()
+            res_data = res_json['result']['data']
+            for _ in res_data:
+                exchange = str(_['TRADE_MARKET'])
+                if exchange.startswith('上海'):
+                    exchange = 'SH'
+                elif exchange.startswith('深圳'):
+                    exchange = 'SZ'
+                elif exchange.startswith('北京'):
+                    exchange = 'BJ'
+                if _['LISTING_DATE']:
+                    data.append({'stock_code': _['SECURITY_CODE'], 'short_name': _['SECURITY_NAME'],
+                                 'exchange': exchange, 'list_date': _['LISTING_DATE']})
+            # if pd.to_datetime(data[-1]['list_date']) < pd.to_datetime('2023-10-01'):
+            if pd.to_datetime(data[-1]['list_date']) < pd.to_datetime('2020-01-01'):
+                break
+        result_df = pd.DataFrame(data=data, columns=self.__CODE_COLUMNS)
+        result_df['list_date'] = pd.to_datetime(result_df['list_date']).dt.date
+        return result_df
+
+
+if __name__ == '__main__':
+    print(StockCode().all_code())
```

### Comparing `adata-1.2.4/adata/stock/info/stock_index.py` & `adata-2.0.0b0/adata/stock/info/stock_index.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,249 +1,249 @@
-# -*- coding: utf-8 -*-
-"""
-@desc:
-a股指数
-上交所
-http://www.sse.com.cn/market/sseindex/indexlist/
-深交所
-http://www.szse.cn/market/exponent/sample/index.html
-
-同花顺
-http://q.10jqka.com.cn/zs/
-
-东方财富
-http://quote.eastmoney.com/center/gridlist.html#index_sh
-http://quote.eastmoney.com/center/gridlist.html#index_sz
-
-指数成分：只用同花顺和东方财富，新浪和百度目前都不准确
-@author: 1nchaos
-@time: 2023/5/23
-@log: change log
-"""
-import copy
-
-import pandas as pd
-from bs4 import BeautifulSoup
-
-from adata.common.exception.exception_msg import *
-from adata.common.headers import ths_headers
-from adata.common.utils import cookie, requests
-from adata.stock.cache.index_code_rel_ths import rel
-
-
-class StockIndex(object):
-    """
-    A股指数
-    """
-    __INDEX_CONSTITUENT_COLUMN = ['index_code', 'stock_code', 'short_name']
-    __INDEX_CODE_COLUMN = ['index_code', 'concept_code', 'name', 'source']
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def all_index_code(self):
-        """
-        获取所有A股市场的指数的代码
-        目前主要来源：同花顺,
-        concept_code为同花顺的概念代码
-        :return: 指数信息[name,index_code,concept_code,source]
-        """
-        return self.__all_index_code_ths()
-
-    def __all_index_code_ths(self):
-        """
-        获取同花顺所有行情中心的指数代码
-        http://q.10jqka.com.cn/zs/
-        上面地址可不用翻页
-        :return: 指数信息[name,index_code，concept_code,source]
-        """
-        # 1. url拼接页码等参数
-        data = []
-        total_pages = 1
-        curr_page = 1
-        while curr_page <= total_pages:
-            api_url = f"http://q.10jqka.com.cn/zs/index/field/zdf/order/desc/page/{curr_page}/ajax/1/"
-            headers = copy.deepcopy(ths_headers.text_headers)
-            headers['Cookie'] = cookie.ths_cookie()
-            res = requests.request(method='get', url=api_url, headers=headers, proxies={})
-            curr_page += 1
-            # 2. 判断请求是否成功
-            if res.status_code != 200:
-                continue
-            text = res.text
-            soup = BeautifulSoup(text, 'html.parser')
-            # 3 .获取总的页数
-            if total_pages == 1:
-                page_info = soup.find('span', {'class': 'page_info'})
-                if page_info:
-                    total_pages = int(page_info.text.split("/")[1])
-            # 4. 解析数据
-            page_data = []
-            for idx, tr in enumerate(soup.find_all('tr')):
-                if idx != 0:
-                    tds = tr.find_all('td')
-                    a_href = tds[1].find('a')
-                    page_data.append({'index_code': tds[1].contents[0].text,
-                                      'concept_code': a_href['href'].split('/')[-2],
-                                      'name': tds[2].contents[0].text, 'source': '同花顺'})
-            data.extend(page_data)
-        # 5. 封装数据
-        if not data:
-            return pd.DataFrame(data=data, columns=self.__INDEX_CODE_COLUMN)
-        result_df = pd.DataFrame(data=data)
-        data.clear()
-        return result_df[self.__INDEX_CODE_COLUMN]
-
-    def index_constituent(self, index_code=None, wait_time=None):
-        """
-        获取对应指数的成分股
-        ps:百度和新浪的数据有问题，丢弃这两个数据源，优先使用同花顺
-        :param index_code: 指数代码
-        :param wait_time: 等待时间：毫秒；表示每个请求的间隔时间，主要用于防止请求太频繁的限制。
-        :return: ['index_code', 'stock_code', 'short_name']
-        """
-        # res = self.__index_constituent_sina(index_code=index_code)
-        # if not res.empty:
-        #     return res
-        return self.__index_constituent_ths(index_code=index_code, wait_time=wait_time)
-
-    def __index_constituent_ths(self, index_code=None, wait_time=None):
-        """
-        同花顺指数成分股
-        :param index_code: 指数代码 399282
-        :param wait_time: 等待时间：毫秒；表示每个请求的间隔时间，主要用于防止请求太频繁的限制。
-        :return:['index_code', 'stock_code', 'short_name']
-        """
-        # 转换抓取的code,
-        catch_code = rel[index_code] if index_code.startswith('0') and index_code in rel.keys() else index_code
-        # 转换指数代码
-        index_code = rel[index_code] if ('A' in index_code or 'B' in index_code or 'C' in index_code) and index_code in rel.keys() else index_code
-        # 1. url拼接页码等参数
-        data = []
-        total_pages = 1
-        curr_page = 1
-        while curr_page <= total_pages:
-            api_url = f"http://q.10jqka.com.cn/zs/detail/field/199112/order/desc/page/" \
-                      f"{curr_page}/ajax/1/code/{catch_code}"
-            headers = copy.deepcopy(ths_headers.text_headers)
-            headers['Cookie'] = cookie.ths_cookie()
-            res = requests.request(method='get', url=api_url, headers=headers, proxies={}, wait_time=wait_time)
-            curr_page += 1
-            # 2. 判断请求是否成功
-            if res.status_code != 200:
-                continue
-            text = res.text
-            if THS_IP_LIMIT_RES in res:
-                raise Exception(THS_IP_LIMIT_MSG)
-            if '暂无成份股数据' in text or '概念板块' in text or '概念时间表' in text:
-                break
-            soup = BeautifulSoup(text, 'html.parser')
-            # 3 .获取总的页数
-            if total_pages == 1:
-                page_info = soup.find('span', {'class': 'page_info'})
-                if page_info:
-                    total_pages = int(page_info.text.split("/")[1])
-            # 4. 解析数据
-            page_data = []
-            for idx, tr in enumerate(soup.find_all('tr')):
-                if idx != 0:
-                    tds = tr.find_all('td')
-                    page_data.append({'index_code': index_code, 'stock_code': tds[1].contents[0].text,
-                                      'short_name': tds[2].contents[0].text})
-            data.extend(page_data)
-        # 5. 封装数据
-        if not data:
-            return pd.DataFrame(data=data, columns=self.__INDEX_CONSTITUENT_COLUMN)
-        result_df = pd.DataFrame(data=data)
-        data.clear()
-        return result_df[self.__INDEX_CONSTITUENT_COLUMN]
-
-    def __index_constituent_baidu(self, index_code=None):
-        """
-        https://gushitong.baidu.com/opendata?resource_id=5352&query=000133&code=000133&market=ab&group=asyn_ranking&pn=100&rn=50&pc_web=1&finClientType=pc
-        百度指数成分股，目前接口存在bug
-        :param index_code: 指数代码 399282
-        :return:['index_code', 'stock_code', 'short_name']
-        """
-        # 1.请求接口 url
-        data = []
-        for page in range(100):
-            api_url = f"https://gushitong.baidu.com/opendata?resource_id=5352&query={index_code}&code={index_code}&" \
-                      f"market=ab&group=asyn_ranking&pn={page * 50}&rn=100&pc_web=1&finClientType=pc"
-            res = requests.request('get', api_url, headers={})
-
-            # 2. 判断结果是否正确
-            if len(res.text) < 1 or res.status_code != 200:
-                break
-            res_json = res.json()
-            if res_json['ResultCode'] != '0':
-                break
-            # 3.解析数据
-            # 3.1 空数据时返回为空
-            result = res_json['Result']
-            if not result:
-                break
-
-            # 3.2 正常解析数据
-            try:
-                result_list = result[-1]['DisplayData']['resultData']['tplData']['result']['list']
-                data.extend(result_list)
-            except KeyError:
-                break
-
-        # 4. 封装数据
-        result_df = pd.DataFrame(data=data).rename(columns={'code': 'stock_code', 'name': 'short_name'})
-        result_df['index_code'] = index_code
-        data.clear()
-        return result_df[self.__INDEX_CONSTITUENT_COLUMN]
-
-    def __index_constituent_sina(self, index_code=None, wait_time=None):
-        """
-        http://vip.stock.finance.sina.com.cn/corp/view/vII_NewestComponent.php?page=1&indexid=000099
-        新浪指数成分：目前数据不准确
-        :param index_code: 指数代码 399282
-        :return:['index_code', 'stock_code', 'short_name']
-        """
-        # 1. url拼接页码等参数
-        data = []
-        total_pages = 1
-        curr_page = 1
-        while curr_page <= total_pages:
-            api_url = f"http://vip.stock.finance.sina.com.cn/corp/view/vII_NewestComponent.php?" \
-                      f"page={curr_page}&indexid={index_code}"
-
-            res = requests.request(method='get', url=api_url, proxies={}, wait_time=wait_time)
-            curr_page += 1
-            # 2. 判断请求是否成功
-            if res.status_code != 200:
-                continue
-            text = res.text
-            if 'NewStockTable' not in text or '最新成分' not in text:
-                break
-            soup = BeautifulSoup(text, 'html.parser')
-            # 3 .获取总的页数
-            if total_pages == 1:
-                page_info = soup.find('table', {'class': 'table2'}).text
-                if page_info and '共' in page_info and '页' in page_info:
-                    # Extract the total number of pages from the page_info string
-                    total_pages = int(page_info.split('共')[1].split('页')[0])
-            # 4. 解析数据
-            page_data = []
-            table = soup.find('table', {'id': 'NewStockTable'})
-            for row in table.find_all('tr')[2:]:
-                cells = row.find_all('td')
-                if len(cells) == 3:
-                    page_data.append({'index_code': index_code, 'stock_code': cells[0].div.text.strip(),
-                                      'short_name': cells[1].div.text.strip()})
-            data.extend(page_data)
-        # 5. 封装数据
-        if not data:
-            return pd.DataFrame(data=data, columns=self.__INDEX_CONSTITUENT_COLUMN)
-        result_df = pd.DataFrame(data=data)
-        data.clear()
-        return result_df[self.__INDEX_CONSTITUENT_COLUMN]
-
-
-if __name__ == '__main__':
-    print(StockIndex().all_index_code())
-    print(StockIndex().index_constituent(index_code='000033'))
-    print(StockIndex().index_constituent(index_code='399387', wait_time=158))
+# -*- coding: utf-8 -*-
+"""
+@desc:
+a股指数
+上交所
+http://www.sse.com.cn/market/sseindex/indexlist/
+深交所
+http://www.szse.cn/market/exponent/sample/index.html
+
+同花顺
+http://q.10jqka.com.cn/zs/
+
+东方财富
+http://quote.eastmoney.com/center/gridlist.html#index_sh
+http://quote.eastmoney.com/center/gridlist.html#index_sz
+
+指数成分：只用同花顺和东方财富，新浪和百度目前都不准确
+@author: 1nchaos
+@time: 2023/5/23
+@log: change log
+"""
+import copy
+
+import pandas as pd
+from bs4 import BeautifulSoup
+
+from adata.common.exception.exception_msg import *
+from adata.common.headers import ths_headers
+from adata.common.utils import cookie, requests
+from adata.stock.cache.index_code_rel_ths import rel
+
+
+class StockIndex(object):
+    """
+    A股指数
+    """
+    __INDEX_CONSTITUENT_COLUMN = ['index_code', 'stock_code', 'short_name']
+    __INDEX_CODE_COLUMN = ['index_code', 'concept_code', 'name', 'source']
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def all_index_code(self):
+        """
+        获取所有A股市场的指数的代码
+        目前主要来源：同花顺,
+        concept_code为同花顺的概念代码
+        :return: 指数信息[name,index_code,concept_code,source]
+        """
+        return self.__all_index_code_ths()
+
+    def __all_index_code_ths(self):
+        """
+        获取同花顺所有行情中心的指数代码
+        http://q.10jqka.com.cn/zs/
+        上面地址可不用翻页
+        :return: 指数信息[name,index_code，concept_code,source]
+        """
+        # 1. url拼接页码等参数
+        data = []
+        total_pages = 1
+        curr_page = 1
+        while curr_page <= total_pages:
+            api_url = f"http://q.10jqka.com.cn/zs/index/field/zdf/order/desc/page/{curr_page}/ajax/1/"
+            headers = copy.deepcopy(ths_headers.text_headers)
+            headers['Cookie'] = cookie.ths_cookie()
+            res = requests.request(method='get', url=api_url, headers=headers, proxies={})
+            curr_page += 1
+            # 2. 判断请求是否成功
+            if res.status_code != 200:
+                continue
+            text = res.text
+            soup = BeautifulSoup(text, 'html.parser')
+            # 3 .获取总的页数
+            if total_pages == 1:
+                page_info = soup.find('span', {'class': 'page_info'})
+                if page_info:
+                    total_pages = int(page_info.text.split("/")[1])
+            # 4. 解析数据
+            page_data = []
+            for idx, tr in enumerate(soup.find_all('tr')):
+                if idx != 0:
+                    tds = tr.find_all('td')
+                    a_href = tds[1].find('a')
+                    page_data.append({'index_code': tds[1].contents[0].text,
+                                      'concept_code': a_href['href'].split('/')[-2],
+                                      'name': tds[2].contents[0].text, 'source': '同花顺'})
+            data.extend(page_data)
+        # 5. 封装数据
+        if not data:
+            return pd.DataFrame(data=data, columns=self.__INDEX_CODE_COLUMN)
+        result_df = pd.DataFrame(data=data)
+        data.clear()
+        return result_df[self.__INDEX_CODE_COLUMN]
+
+    def index_constituent(self, index_code=None, wait_time=None):
+        """
+        获取对应指数的成分股
+        ps:百度和新浪的数据有问题，丢弃这两个数据源，优先使用同花顺
+        :param index_code: 指数代码
+        :param wait_time: 等待时间：毫秒；表示每个请求的间隔时间，主要用于防止请求太频繁的限制。
+        :return: ['index_code', 'stock_code', 'short_name']
+        """
+        # res = self.__index_constituent_sina(index_code=index_code)
+        # if not res.empty:
+        #     return res
+        return self.__index_constituent_ths(index_code=index_code, wait_time=wait_time)
+
+    def __index_constituent_ths(self, index_code=None, wait_time=None):
+        """
+        同花顺指数成分股
+        :param index_code: 指数代码 399282
+        :param wait_time: 等待时间：毫秒；表示每个请求的间隔时间，主要用于防止请求太频繁的限制。
+        :return:['index_code', 'stock_code', 'short_name']
+        """
+        # 转换抓取的code,
+        catch_code = rel[index_code] if index_code.startswith('0') and index_code in rel.keys() else index_code
+        # 转换指数代码
+        index_code = rel[index_code] if ('A' in index_code or 'B' in index_code or 'C' in index_code) and index_code in rel.keys() else index_code
+        # 1. url拼接页码等参数
+        data = []
+        total_pages = 1
+        curr_page = 1
+        while curr_page <= total_pages:
+            api_url = f"http://q.10jqka.com.cn/zs/detail/field/199112/order/desc/page/" \
+                      f"{curr_page}/ajax/1/code/{catch_code}"
+            headers = copy.deepcopy(ths_headers.text_headers)
+            headers['Cookie'] = cookie.ths_cookie()
+            res = requests.request(method='get', url=api_url, headers=headers, proxies={}, wait_time=wait_time)
+            curr_page += 1
+            # 2. 判断请求是否成功
+            if res.status_code != 200:
+                continue
+            text = res.text
+            if THS_IP_LIMIT_RES in res:
+                raise Exception(THS_IP_LIMIT_MSG)
+            if '暂无成份股数据' in text or '概念板块' in text or '概念时间表' in text:
+                break
+            soup = BeautifulSoup(text, 'html.parser')
+            # 3 .获取总的页数
+            if total_pages == 1:
+                page_info = soup.find('span', {'class': 'page_info'})
+                if page_info:
+                    total_pages = int(page_info.text.split("/")[1])
+            # 4. 解析数据
+            page_data = []
+            for idx, tr in enumerate(soup.find_all('tr')):
+                if idx != 0:
+                    tds = tr.find_all('td')
+                    page_data.append({'index_code': index_code, 'stock_code': tds[1].contents[0].text,
+                                      'short_name': tds[2].contents[0].text})
+            data.extend(page_data)
+        # 5. 封装数据
+        if not data:
+            return pd.DataFrame(data=data, columns=self.__INDEX_CONSTITUENT_COLUMN)
+        result_df = pd.DataFrame(data=data)
+        data.clear()
+        return result_df[self.__INDEX_CONSTITUENT_COLUMN]
+
+    def __index_constituent_baidu(self, index_code=None):
+        """
+        https://gushitong.baidu.com/opendata?resource_id=5352&query=000133&code=000133&market=ab&group=asyn_ranking&pn=100&rn=50&pc_web=1&finClientType=pc
+        百度指数成分股，目前接口存在bug
+        :param index_code: 指数代码 399282
+        :return:['index_code', 'stock_code', 'short_name']
+        """
+        # 1.请求接口 url
+        data = []
+        for page in range(100):
+            api_url = f"https://gushitong.baidu.com/opendata?resource_id=5352&query={index_code}&code={index_code}&" \
+                      f"market=ab&group=asyn_ranking&pn={page * 50}&rn=100&pc_web=1&finClientType=pc"
+            res = requests.request('get', api_url, headers={})
+
+            # 2. 判断结果是否正确
+            if len(res.text) < 1 or res.status_code != 200:
+                break
+            res_json = res.json()
+            if res_json['ResultCode'] != '0':
+                break
+            # 3.解析数据
+            # 3.1 空数据时返回为空
+            result = res_json['Result']
+            if not result:
+                break
+
+            # 3.2 正常解析数据
+            try:
+                result_list = result[-1]['DisplayData']['resultData']['tplData']['result']['list']
+                data.extend(result_list)
+            except KeyError:
+                break
+
+        # 4. 封装数据
+        result_df = pd.DataFrame(data=data).rename(columns={'code': 'stock_code', 'name': 'short_name'})
+        result_df['index_code'] = index_code
+        data.clear()
+        return result_df[self.__INDEX_CONSTITUENT_COLUMN]
+
+    def __index_constituent_sina(self, index_code=None, wait_time=None):
+        """
+        http://vip.stock.finance.sina.com.cn/corp/view/vII_NewestComponent.php?page=1&indexid=000099
+        新浪指数成分：目前数据不准确
+        :param index_code: 指数代码 399282
+        :return:['index_code', 'stock_code', 'short_name']
+        """
+        # 1. url拼接页码等参数
+        data = []
+        total_pages = 1
+        curr_page = 1
+        while curr_page <= total_pages:
+            api_url = f"http://vip.stock.finance.sina.com.cn/corp/view/vII_NewestComponent.php?" \
+                      f"page={curr_page}&indexid={index_code}"
+
+            res = requests.request(method='get', url=api_url, proxies={}, wait_time=wait_time)
+            curr_page += 1
+            # 2. 判断请求是否成功
+            if res.status_code != 200:
+                continue
+            text = res.text
+            if 'NewStockTable' not in text or '最新成分' not in text:
+                break
+            soup = BeautifulSoup(text, 'html.parser')
+            # 3 .获取总的页数
+            if total_pages == 1:
+                page_info = soup.find('table', {'class': 'table2'}).text
+                if page_info and '共' in page_info and '页' in page_info:
+                    # Extract the total number of pages from the page_info string
+                    total_pages = int(page_info.split('共')[1].split('页')[0])
+            # 4. 解析数据
+            page_data = []
+            table = soup.find('table', {'id': 'NewStockTable'})
+            for row in table.find_all('tr')[2:]:
+                cells = row.find_all('td')
+                if len(cells) == 3:
+                    page_data.append({'index_code': index_code, 'stock_code': cells[0].div.text.strip(),
+                                      'short_name': cells[1].div.text.strip()})
+            data.extend(page_data)
+        # 5. 封装数据
+        if not data:
+            return pd.DataFrame(data=data, columns=self.__INDEX_CONSTITUENT_COLUMN)
+        result_df = pd.DataFrame(data=data)
+        data.clear()
+        return result_df[self.__INDEX_CONSTITUENT_COLUMN]
+
+
+if __name__ == '__main__':
+    print(StockIndex().all_index_code())
+    print(StockIndex().index_constituent(index_code='000033'))
+    print(StockIndex().index_constituent(index_code='399387', wait_time=158))
```

### Comparing `adata-1.2.4/adata/stock/market/concepth_market/concept_market_east.py` & `adata-2.0.0b0/adata/stock/market/concepth_market/concept_market_east.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-# -*- coding: utf-8 -*-
-"""
-@summary: 股票概念 行情
-https://quote.eastmoney.com/bk/90.BK0612.html
-TODO 概念板块当日涨跌幅排名
-https://push2.eastmoney.com/api/qt/clist/get?pn=1&pz=1000&po=1&fid=f3&fields=f1,f2,f3,f4,f12,f13,f14&fs=b:BK0900&ut=fa5fd1943c7b386f172d6893dbfba10b&cb=jQuery35109553587682356608_1691083378045&_=1691083378046
-@author: 1nchaos
-@date: 2023/08/03 23:17
-"""
-import datetime
-
-import pandas as pd
-
-from adata.common import requests
-from adata.stock.market.concepth_market.concept_market_template import ConceptMarketTemplate
-
-
-class ConceptMarketEase(ConceptMarketTemplate):
-    """
-    股票概念 行情
-    """
-
-    def get_market_concept_east(self, index_code: str = 'BK0612', k_type: int = 1):
-        """
-        获取东方财富的概念的行情
-        https://push2his.eastmoney.com/api/qt/stock/kline/get?secid=90.BK0612&fields1=f1,f2,f3,f4,f5,f6&fields2=f51,f52,f53,f54,f55,f56,f57,f58,f59,f60,f61&klt=101&fqt=1&end=20500101&lmt=1000000
-        :param index_code: 东方财富概念指数代码：BK开头
-        :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
-        :return: k线行情数据 [日期，开，高，低，收,成交量，成交额]
-         "2012-06-14,765.93,760.75,766.05,759.93,28427953,30155329024.00,0.61,-23.93,-239.25,0.12",
-        成交量：股 820953530  821万手
-        成交额：元 16959251000.000 169.6亿
-        """
-        url = f"https://push2his.eastmoney.com/api/qt/stock/kline/get?" \
-              f"secid=90.{index_code}&fields1=f1,f2,f3,f4,f5,f6&fields2=f51,f52,f53,f54,f55,f56,f57,f58,f59,f60,f61" \
-              f"&klt=10{k_type}&fqt=1&end=20500101&lmt=1000000"
-        res_json = requests.request('get', url, headers={}, proxies={}).json()
-        # 解析数据
-        code = res_json['data']['code']
-        if code != index_code:
-            return
-        res_data = res_json['data']['klines']
-        data = []
-        for _ in res_data:
-            row = str(_).split(',')
-            data.append(
-                {'trade_date': row[0], 'open': row[1], 'close': row[2], 'high': row[3], 'low': row[4], 'volume': row[5],
-                 'amount': row[6], 'change': row[9], 'change_pct': row[8], 'index_code': index_code})
-        result_df = pd.DataFrame(data=data, columns=self._MARKET_COLUMNS)
-
-        # 清洗数据
-        result_df[['open', 'high', 'low', 'close', 'volume', 'amount', 'change', 'change_pct']] = \
-            result_df[['open', 'high', 'low', 'close', 'volume', 'amount', 'change', 'change_pct']].astype(float)
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d %H:%M:%S')
-        result_df = result_df.round(2)
-        return result_df
-
-    def get_market_concept_min_east(self, index_code='BK0612'):
-        """
-        获取概念行情当日分时
-        https://quote.eastmoney.com/bk/90.BK0612.html#fullScreenChart
-        :param index_code: 概念指数代码
-        :return 时间，现价，成交额（元），均价，成交量（股） 涨跌额，涨跌幅
-        'index_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'avg_price', 'amount'
-        """
-        url = f"https://push2his.eastmoney.com/api/qt/stock/trends2/get?" \
-              f"fields2=f51,f52,f53,f54,f55,f56,f57,f58&secid=90.{index_code}&" \
-              f"ndays=1&iscr=0&fields1=f1,f2,f3,f4,f5,f6,f7,f8,f9,f10,f11,f12,f13"
-        res_json = requests.request('get', url, headers={}, proxies={}).json()
-        # 解析数据
-        code = res_json['data']['code']
-        pre_price = res_json['data']['prePrice']
-        if code != index_code:
-            return
-        res_data = res_json['data']['trends']
-        data = []
-        for _ in res_data:
-            row = str(_).split(',')
-            data.append(
-                {'trade_date': row[0], 'open': row[1], 'price': row[2], 'high': row[3], 'low': row[4],
-                 'volume': row[5], 'amount': row[6], 'avg_price': row[7], 'index_code': index_code})
-        result_df = pd.DataFrame(data=data, columns=self._MARKET_CONCEPT_MIN_COLUMNS)
-
-        # 清洗数据
-        result_df[['price', 'volume', 'amount', 'avg_price']] = \
-            result_df[['price', 'volume', 'amount', 'avg_price']].astype(float)
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d %H:%M:%S')
-        result_df['trade_date'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d')
-        result_df['change'] = result_df['price'] - pre_price
-        result_df['change_pct'] = result_df['change'] / pre_price * 100
-        result_df = result_df.round(2)
-        return result_df
-
-    def get_market_concept_current_east(self, index_code: str = 'BK0612'):
-        """
-        https://push2.eastmoney.com/api/qt/stock/get?secid=90.BK0612&fields=f57,f58,f106,f59,f43,f46,f60,f44,f45,f47,f48,f49,f113,f114,f115,f117,f85,f50,f119,f120,f121,f122,f135,f136,f137,f138,f139,f140,f141,f142,f143,f144,f145,f146,f147,f148,f149
-        :param index_code: 东方财富指数代码
-        :return: k线行情数据 [概念代码,交易时间，交易日期，开，高，低，当前价格,成交量，成交额]
-        """
-        url = f"https://push2.eastmoney.com/api/qt/stock/get?secid=90.{index_code}&" \
-              f"fields=f57,f58,f106,f59,f43,f46,f60,f44,f45,f47,f48,f49,f113,f114,f115,f117,f85,f50,f119,f120," \
-              f"f121,f122,f135,f136,f137,f138,f139,f140,f141,f142,f143,f144,f145,f146,f147,f148,f149"
-        res_json = requests.request('get', url, headers={}, proxies={}).json()
-        # 解析数据
-        j = res_json['data']
-        if not j:
-            return pd.DataFrame(data=[], columns=self._MARKET_CONCEPT_CURRENT_COLUMNS)
-        code = j['f57']
-        if code != index_code:
-            return pd.DataFrame(data=[], columns=self._MARKET_CONCEPT_CURRENT_COLUMNS)
-        pre_close = j['f60']
-        data = [{'open': j['f46'], 'high': j['f44'], 'low': j['f45'], 'price': j['f43'], 'volume': j['f47'],
-                 'amount': j['f48'], 'index_code': index_code}]
-        result_df = pd.DataFrame(data=data, columns=self._MARKET_CONCEPT_CURRENT_COLUMNS)
-
-        # 清洗数据
-        result_df[['open', 'high', 'low', 'price', 'volume', 'amount']] = \
-            result_df[['open', 'high', 'low', 'price', 'volume', 'amount']].astype(float)
-        result_df['change'] = result_df['price'] - pre_close
-        result_df['change_pct'] = result_df['change'] / pre_close * 100
-        result_df = result_df.round(2)
-        result_df['trade_time'] = datetime.datetime.now()
-        return result_df
-
-
-if __name__ == '__main__':
-    print(ConceptMarketEase().get_market_concept_east(index_code='BK0612'))
-    print(ConceptMarketEase().get_market_concept_min_east(index_code='BK0612'))
-    print(ConceptMarketEase().get_market_concept_current_east(index_code='BK0612'))
+# -*- coding: utf-8 -*-
+"""
+@summary: 股票概念 行情
+https://quote.eastmoney.com/bk/90.BK0612.html
+TODO 概念板块当日涨跌幅排名
+https://push2.eastmoney.com/api/qt/clist/get?pn=1&pz=1000&po=1&fid=f3&fields=f1,f2,f3,f4,f12,f13,f14&fs=b:BK0900&ut=fa5fd1943c7b386f172d6893dbfba10b&cb=jQuery35109553587682356608_1691083378045&_=1691083378046
+@author: 1nchaos
+@date: 2023/08/03 23:17
+"""
+import datetime
+
+import pandas as pd
+
+from adata.common import requests
+from adata.stock.market.concepth_market.concept_market_template import ConceptMarketTemplate
+
+
+class ConceptMarketEase(ConceptMarketTemplate):
+    """
+    股票概念 行情
+    """
+
+    def get_market_concept_east(self, index_code: str = 'BK0612', k_type: int = 1):
+        """
+        获取东方财富的概念的行情
+        https://push2his.eastmoney.com/api/qt/stock/kline/get?secid=90.BK0612&fields1=f1,f2,f3,f4,f5,f6&fields2=f51,f52,f53,f54,f55,f56,f57,f58,f59,f60,f61&klt=101&fqt=1&end=20500101&lmt=1000000
+        :param index_code: 东方财富概念指数代码：BK开头
+        :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
+        :return: k线行情数据 [日期，开，高，低，收,成交量，成交额]
+         "2012-06-14,765.93,760.75,766.05,759.93,28427953,30155329024.00,0.61,-23.93,-239.25,0.12",
+        成交量：股 820953530  821万手
+        成交额：元 16959251000.000 169.6亿
+        """
+        url = f"https://push2his.eastmoney.com/api/qt/stock/kline/get?" \
+              f"secid=90.{index_code}&fields1=f1,f2,f3,f4,f5,f6&fields2=f51,f52,f53,f54,f55,f56,f57,f58,f59,f60,f61" \
+              f"&klt=10{k_type}&fqt=1&end=20500101&lmt=1000000"
+        res_json = requests.request('get', url, headers={}, proxies={}).json()
+        # 解析数据
+        code = res_json['data']['code']
+        if code != index_code:
+            return
+        res_data = res_json['data']['klines']
+        data = []
+        for _ in res_data:
+            row = str(_).split(',')
+            data.append(
+                {'trade_date': row[0], 'open': row[1], 'close': row[2], 'high': row[3], 'low': row[4], 'volume': row[5],
+                 'amount': row[6], 'change': row[9], 'change_pct': row[8], 'index_code': index_code})
+        result_df = pd.DataFrame(data=data, columns=self._MARKET_COLUMNS)
+
+        # 清洗数据
+        result_df[['open', 'high', 'low', 'close', 'volume', 'amount', 'change', 'change_pct']] = \
+            result_df[['open', 'high', 'low', 'close', 'volume', 'amount', 'change', 'change_pct']].astype(float)
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d %H:%M:%S')
+        result_df = result_df.round(2)
+        return result_df
+
+    def get_market_concept_min_east(self, index_code='BK0612'):
+        """
+        获取概念行情当日分时
+        https://quote.eastmoney.com/bk/90.BK0612.html#fullScreenChart
+        :param index_code: 概念指数代码
+        :return 时间，现价，成交额（元），均价，成交量（股） 涨跌额，涨跌幅
+        'index_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'avg_price', 'amount'
+        """
+        url = f"https://push2his.eastmoney.com/api/qt/stock/trends2/get?" \
+              f"fields2=f51,f52,f53,f54,f55,f56,f57,f58&secid=90.{index_code}&" \
+              f"ndays=1&iscr=0&fields1=f1,f2,f3,f4,f5,f6,f7,f8,f9,f10,f11,f12,f13"
+        res_json = requests.request('get', url, headers={}, proxies={}).json()
+        # 解析数据
+        code = res_json['data']['code']
+        pre_price = res_json['data']['prePrice']
+        if code != index_code:
+            return
+        res_data = res_json['data']['trends']
+        data = []
+        for _ in res_data:
+            row = str(_).split(',')
+            data.append(
+                {'trade_date': row[0], 'open': row[1], 'price': row[2], 'high': row[3], 'low': row[4],
+                 'volume': row[5], 'amount': row[6], 'avg_price': row[7], 'index_code': index_code})
+        result_df = pd.DataFrame(data=data, columns=self._MARKET_CONCEPT_MIN_COLUMNS)
+
+        # 清洗数据
+        result_df[['price', 'volume', 'amount', 'avg_price']] = \
+            result_df[['price', 'volume', 'amount', 'avg_price']].astype(float)
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d %H:%M:%S')
+        result_df['trade_date'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d')
+        result_df['change'] = result_df['price'] - pre_price
+        result_df['change_pct'] = result_df['change'] / pre_price * 100
+        result_df = result_df.round(2)
+        return result_df
+
+    def get_market_concept_current_east(self, index_code: str = 'BK0612'):
+        """
+        https://push2.eastmoney.com/api/qt/stock/get?secid=90.BK0612&fields=f57,f58,f106,f59,f43,f46,f60,f44,f45,f47,f48,f49,f113,f114,f115,f117,f85,f50,f119,f120,f121,f122,f135,f136,f137,f138,f139,f140,f141,f142,f143,f144,f145,f146,f147,f148,f149
+        :param index_code: 东方财富指数代码
+        :return: k线行情数据 [概念代码,交易时间，交易日期，开，高，低，当前价格,成交量，成交额]
+        """
+        url = f"https://push2.eastmoney.com/api/qt/stock/get?secid=90.{index_code}&" \
+              f"fields=f57,f58,f106,f59,f43,f46,f60,f44,f45,f47,f48,f49,f113,f114,f115,f117,f85,f50,f119,f120," \
+              f"f121,f122,f135,f136,f137,f138,f139,f140,f141,f142,f143,f144,f145,f146,f147,f148,f149"
+        res_json = requests.request('get', url, headers={}, proxies={}).json()
+        # 解析数据
+        j = res_json['data']
+        if not j:
+            return pd.DataFrame(data=[], columns=self._MARKET_CONCEPT_CURRENT_COLUMNS)
+        code = j['f57']
+        if code != index_code:
+            return pd.DataFrame(data=[], columns=self._MARKET_CONCEPT_CURRENT_COLUMNS)
+        pre_close = j['f60']
+        data = [{'open': j['f46'], 'high': j['f44'], 'low': j['f45'], 'price': j['f43'], 'volume': j['f47'],
+                 'amount': j['f48'], 'index_code': index_code}]
+        result_df = pd.DataFrame(data=data, columns=self._MARKET_CONCEPT_CURRENT_COLUMNS)
+
+        # 清洗数据
+        result_df[['open', 'high', 'low', 'price', 'volume', 'amount']] = \
+            result_df[['open', 'high', 'low', 'price', 'volume', 'amount']].astype(float)
+        result_df['change'] = result_df['price'] - pre_close
+        result_df['change_pct'] = result_df['change'] / pre_close * 100
+        result_df = result_df.round(2)
+        result_df['trade_time'] = datetime.datetime.now()
+        return result_df
+
+
+if __name__ == '__main__':
+    print(ConceptMarketEase().get_market_concept_east(index_code='BK0612'))
+    print(ConceptMarketEase().get_market_concept_min_east(index_code='BK0612'))
+    print(ConceptMarketEase().get_market_concept_current_east(index_code='BK0612'))
```

### Comparing `adata-1.2.4/adata/stock/market/concepth_market/concept_market_template.py` & `adata-2.0.0b0/adata/stock/market/concepth_market/concept_market_template.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# -*- coding: utf-8 -*-
-"""
-@summary: 股票概念 行情
-"""
-
-
-class ConceptMarketTemplate(object):
-    """
-    股票概念 行情
-    """
-    _MARKET_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'open', 'high', 'low', 'close', 'volume',
-                       'amount', 'change', 'change_pct']
-    _MARKET_CONCEPT_MIN_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'price', 'avg_price', 'volume', 'amount',
-                                   'change', 'change_pct']
-    _MARKET_CONCEPT_CURRENT_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'open', 'high', 'low', 'price',
-                                       'volume', 'amount', 'change', 'change_pct']
+# -*- coding: utf-8 -*-
+"""
+@summary: 股票概念 行情
+"""
+
+
+class ConceptMarketTemplate(object):
+    """
+    股票概念 行情
+    """
+    _MARKET_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'open', 'high', 'low', 'close', 'volume',
+                       'amount', 'change', 'change_pct']
+    _MARKET_CONCEPT_MIN_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'price', 'avg_price', 'volume', 'amount',
+                                   'change', 'change_pct']
+    _MARKET_CONCEPT_CURRENT_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'open', 'high', 'low', 'price',
+                                       'volume', 'amount', 'change', 'change_pct']
```

### Comparing `adata-1.2.4/adata/stock/market/concepth_market/concept_market_ths.py` & `adata-2.0.0b0/adata/stock/market/concepth_market/concept_market_ths.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-# -*- coding: utf-8 -*-
-"""
-@summary: 股票概念 行情
-同花顺概念更及时和完整，所以目前暂只基于同花顺的股票概念抓取,网页数据中心和手机概念板块
-http://d.10jqka.com.cn/v6/line/48_885772/01/last1800.js
-http://search.10jqka.com.cn/gateway/urp/v7/landing/getDataList?query=%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5&condition=%5B%7B%22indexName%22%3A%22%E6%8C%87%E6%95%B0%40%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22indexProperties%22%3A%5B%5D%2C%22source%22%3A%22new_parser%22%2C%22type%22%3A%22index%22%2C%22indexPropertiesMap%22%3A%7B%7D%2C%22reportType%22%3A%22null%22%2C%22chunkedResult%22%3A%22%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5%22%2C%22valueType%22%3A%22_%E6%8C%87%E6%95%B0%E7%B1%BB%E5%9E%8B%22%2C%22domain%22%3A%22abs_a%E6%8C%87%E9%A2%86%E5%9F%9F%22%2C%22uiText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22sonSize%22%3A0%2C%22queryText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22relatedSize%22%3A0%7D%5D&urp_sort_index=%E6%8C%87%E6%95%B0%E4%BB%A3%E7%A0%81&source=Ths_iwencai_Xuangu&perpage=500&page=1&urp_sort_way=desc&codelist=&page_id=&logid=35df00ee5ae706d0dfcd0dbfdb846e0c&ret=json_all&sessionid=35df00ee5ae706d0dfcd0dbfdb846e0c&iwc_token=0ac9667016801698001765831&user_id=Ths_iwencai_Xuangu_7fahywzhbkrh4lwwkwfw936njqbjzsly&uuids%5B0%5D=23119&query_type=zhishu&comp_id=6367801&business_cat=soniu&uuid=23119
-885772 表示同花顺的概念指数的代码
-@author: 1nchaos
-@date: 2023/3/30 16:17
-"""
-import json
-
-import numpy as np
-import pandas as pd
-
-from adata.common.base.base_ths import BaseThs
-from adata.common.exception.exception_msg import *
-from adata.stock.market.concepth_market.concept_market_template import ConceptMarketTemplate
-
-
-class ConceptMarketThs(BaseThs, ConceptMarketTemplate):
-    """
-    股票概念 行情
-    """
-
-    def get_market_concept_ths(self, index_code: str = '886013', k_type: int = 1, adjust_type: int = 1):
-        """
-        获取同花顺的概念的行情
-        web: http://q.10jqka.com.cn/gn/
-        pc: http://d.10jqka.com.cn/v4/line/bk_885772/21/last.js
-        app: http://d.10jqka.com.cn/v6/line/48_886013/01/last1800.js
-        00 日k不复权；01日k前复权；02日k后复权；11周k前复权；21月k前复权
-        :param index_code: 同花顺概念指数代码
-        :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
-        :param adjust_type: k线复权类型：0.不复权；1.前复权；2.后复权 默认：1 前复权
-        :return: k线行情数据 [日期，开，高，低，收,成交量，成交额]
-        ;20230419,958.901,981.118,958.449,961.107,521143220,20442229000.000
-        成交量：股 820953530  821万手
-        成交额：元 16959251000.000 169.6亿
-        """
-        # 0.参数校验
-        if not index_code.startswith('8'):
-            raise RuntimeError('index_code错误，是8开头的指数代码,')
-        # 1.接口 url
-        api_url = f"http://d.10jqka.com.cn/v6/line/48_{index_code}/{k_type - 1}{adjust_type}/last1800.js"
-        # 同花顺可能ip限制，降低请求次数
-        text = self._get_text(api_url, index_code)
-        if THS_IP_LIMIT_RES in text:
-            return Exception(THS_IP_LIMIT_MSG)
-        result_text = text[text.index('{'):-1]
-        data_list = json.loads(result_text)['data'].split(';')
-        data = []
-        for d in data_list:
-            data.append(str(d).split(',')[0:7])
-        result_df = pd.DataFrame(data=data, columns=['trade_date', 'open', 'high', 'low', 'close', 'volume', 'amount'])
-        result_df['index_code'] = index_code
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d %H:%M:%S')
-        result_df['trade_date'] = pd.to_datetime(result_df['trade_date'], format='%Y%m%d').dt.strftime('%Y-%m-%d')
-        result_df['close'] = result_df['close'].astype(float)
-        result_df['change'] = result_df['close'] - result_df['close'].shift(1)
-        result_df['change_pct'] = result_df['change'] / result_df['close'].shift(1) * 100
-
-        # 3. 清洗数据
-        result_df = result_df.round(2)
-        result_df['close'] = result_df['close'].apply(lambda x: format(x, '.2f'))
-        result_df.replace('--', None, inplace=True)
-        result_df.replace('', None, inplace=True)
-        result_df.replace(np.nan, None, inplace=True)
-        return result_df[self._MARKET_COLUMNS]
-
-    def get_market_concept_min_ths(self, index_code='886041'):
-        """
-        获取概念行情当日分时
-        web： http://d.10jqka.com.cn/v6/time/48_886013/last.js
-        0930,958.901,74456973,36.807,2022925;  "pre": "960.374",
-        :param index_code: 概念指数代码
-        :return 时间，现价，成交额（元），均价，成交量（股） 涨跌额，涨跌幅
-        'index_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'pre_close', 'amount'
-        """
-        # 0.参数校验
-        if not index_code.startswith('8'):
-            raise RuntimeError('index_code错误，是8开头的指数代码,')
-        # 1.接口 url
-        api_url = f"http://d.10jqka.com.cn/v6/time/48_{index_code}/last.js"
-        text = self._get_text(api_url, index_code)
-        if THS_IP_LIMIT_RES in text:
-            return Exception(THS_IP_LIMIT_MSG)
-        # 2. 解析数据
-        result_json = json.loads(text[text.index('{'):-1])[f"48_{index_code}"]
-        pre_price = result_json['pre']
-        trade_date = result_json['date']
-        data_list = result_json['data'].split(';')
-        data = []
-        for d in data_list:
-            data.append(str(d).split(','))
-        # 3. 封装数据
-        result_df = pd.DataFrame(data=data, columns=['trade_time', 'price', 'amount', 'xx', 'volume'])
-        result_df['index_code'] = index_code
-        result_df['trade_time'] = trade_date + result_df['trade_time']
-        result_df['trade_date'] = pd.to_datetime(trade_date, format='%Y%m%d').strftime('%Y-%m-%d')
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_time'], format='%Y%m%d%H%M').dt.strftime(
-            '%Y-%m-%d %H:%M:%S')
-        result_df['price'] = result_df['price']
-        result_df['avg_price'] = None
-        result_df['change'] = result_df['price'].astype(float) - float(pre_price)
-        result_df['change_pct'] = result_df['change'] / float(pre_price) * 100
-        result_df.replace('--', None, inplace=True)
-        result_df.replace('', None, inplace=True)
-        result_df.replace(np.nan, None, inplace=True)
-        return result_df[self._MARKET_CONCEPT_MIN_COLUMNS]
-
-    def get_market_concept_current_ths(self, index_code: str = '886013', k_type: int = 1):
-        """
-        获取同花顺当前的概念行情
-        web: http://q.10jqka.com.cn/gn/
-        pc: http://d.10jqka.com.cn/v6/line/48_886042/01/today.js
-        quotebridge_v6_line_48_886042_01_today({"48_886042":{"1":"20230425","7":"891.344","8":"892.350","9":"853.800",
-        "11":"860.076","13":491708080,"19":"17647511000.000","74":"","1968584":"","66":"","open":1,"dt":"2244",
-        "name":"\u5b58\u50a8\u82af\u7247","marketType":""}})
-
-        :param index_code: 同花顺概念指数代码
-        :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
-        :return: k线行情数据 [概念代码,交易时间，交易日期，开，高，低，当前价格,成交量，成交额]
-        ;20230419,958.901,981.118,958.449,961.107,521143220,20442229000.000,存储芯片
-        k:   1,      7,      8,       9,      11,      13,         19,        name
-        成交量：股 820953530  821万手
-        成交额：元 16959251000.000 169.6亿
-        """
-        # 0.参数校验
-        if not index_code.startswith('8'):
-            raise RuntimeError('index_code错误，是8开头的指数代码,')
-        # 1.接口 url
-        api_url = f"http://d.10jqka.com.cn/v6/line/48_{index_code}/{k_type - 1}1/today.js"
-        # 同花顺可能ip限制，降低请求次数
-        text = self._get_text(api_url, index_code)
-        if THS_IP_LIMIT_RES in text:
-            return Exception(THS_IP_LIMIT_MSG)
-        result_text = text[text.index('{'):-1]
-        data_list = [json.loads(result_text)[f"48_{index_code}"]]
-        rename = {'1': 'trade_date', '7': 'open', '8': 'high', '9': 'low', '11': 'price', '13': 'volume',
-                  '19': 'amount', 'open': 'status'}
-        result_df = pd.DataFrame(data=data_list).rename(columns=rename)
-        result_df['trade_time'] = result_df['trade_date'] + result_df['dt']
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_time'], format='%Y%m%d%H%M').dt.strftime(
-            '%Y-%m-%d %H:%M:%S')
-        columns = ['trade_time', 'trade_date', 'open', 'high', 'low', 'price', 'volume', 'amount']
-        result_df = result_df[columns]
-        result_df['index_code'] = index_code
-        result_df['trade_date'] = pd.to_datetime(result_df['trade_date'], format='%Y%m%d').dt.strftime('%Y-%m-%d')
-        result_df['change'] = None
-        result_df['change_pct'] = None
-        return result_df[self._MARKET_CONCEPT_CURRENT_COLUMNS]
-
-
-if __name__ == '__main__':
-    print(ConceptMarketThs().get_market_concept_ths(index_code='886041'))
-    print(ConceptMarketThs().get_market_concept_min_ths(index_code='886041'))
-    print(ConceptMarketThs().get_market_concept_current_ths(index_code='886041'))
+# -*- coding: utf-8 -*-
+"""
+@summary: 股票概念 行情
+同花顺概念更及时和完整，所以目前暂只基于同花顺的股票概念抓取,网页数据中心和手机概念板块
+http://d.10jqka.com.cn/v6/line/48_885772/01/last1800.js
+http://search.10jqka.com.cn/gateway/urp/v7/landing/getDataList?query=%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5&condition=%5B%7B%22indexName%22%3A%22%E6%8C%87%E6%95%B0%40%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22indexProperties%22%3A%5B%5D%2C%22source%22%3A%22new_parser%22%2C%22type%22%3A%22index%22%2C%22indexPropertiesMap%22%3A%7B%7D%2C%22reportType%22%3A%22null%22%2C%22chunkedResult%22%3A%22%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5%22%2C%22valueType%22%3A%22_%E6%8C%87%E6%95%B0%E7%B1%BB%E5%9E%8B%22%2C%22domain%22%3A%22abs_a%E6%8C%87%E9%A2%86%E5%9F%9F%22%2C%22uiText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22sonSize%22%3A0%2C%22queryText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22relatedSize%22%3A0%7D%5D&urp_sort_index=%E6%8C%87%E6%95%B0%E4%BB%A3%E7%A0%81&source=Ths_iwencai_Xuangu&perpage=500&page=1&urp_sort_way=desc&codelist=&page_id=&logid=35df00ee5ae706d0dfcd0dbfdb846e0c&ret=json_all&sessionid=35df00ee5ae706d0dfcd0dbfdb846e0c&iwc_token=0ac9667016801698001765831&user_id=Ths_iwencai_Xuangu_7fahywzhbkrh4lwwkwfw936njqbjzsly&uuids%5B0%5D=23119&query_type=zhishu&comp_id=6367801&business_cat=soniu&uuid=23119
+885772 表示同花顺的概念指数的代码
+@author: 1nchaos
+@date: 2023/3/30 16:17
+"""
+import json
+
+import numpy as np
+import pandas as pd
+
+from adata.common.base.base_ths import BaseThs
+from adata.common.exception.exception_msg import *
+from adata.stock.market.concepth_market.concept_market_template import ConceptMarketTemplate
+
+
+class ConceptMarketThs(BaseThs, ConceptMarketTemplate):
+    """
+    股票概念 行情
+    """
+
+    def get_market_concept_ths(self, index_code: str = '886013', k_type: int = 1, adjust_type: int = 1):
+        """
+        获取同花顺的概念的行情
+        web: http://q.10jqka.com.cn/gn/
+        pc: http://d.10jqka.com.cn/v4/line/bk_885772/21/last.js
+        app: http://d.10jqka.com.cn/v6/line/48_886013/01/last1800.js
+        00 日k不复权；01日k前复权；02日k后复权；11周k前复权；21月k前复权
+        :param index_code: 同花顺概念指数代码
+        :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
+        :param adjust_type: k线复权类型：0.不复权；1.前复权；2.后复权 默认：1 前复权
+        :return: k线行情数据 [日期，开，高，低，收,成交量，成交额]
+        ;20230419,958.901,981.118,958.449,961.107,521143220,20442229000.000
+        成交量：股 820953530  821万手
+        成交额：元 16959251000.000 169.6亿
+        """
+        # 0.参数校验
+        if not index_code.startswith('8'):
+            raise RuntimeError('index_code错误，是8开头的指数代码,')
+        # 1.接口 url
+        api_url = f"http://d.10jqka.com.cn/v6/line/48_{index_code}/{k_type - 1}{adjust_type}/last1800.js"
+        # 同花顺可能ip限制，降低请求次数
+        text = self._get_text(api_url, index_code)
+        if THS_IP_LIMIT_RES in text:
+            return Exception(THS_IP_LIMIT_MSG)
+        result_text = text[text.index('{'):-1]
+        data_list = json.loads(result_text)['data'].split(';')
+        data = []
+        for d in data_list:
+            data.append(str(d).split(',')[0:7])
+        result_df = pd.DataFrame(data=data, columns=['trade_date', 'open', 'high', 'low', 'close', 'volume', 'amount'])
+        result_df['index_code'] = index_code
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d %H:%M:%S')
+        result_df['trade_date'] = pd.to_datetime(result_df['trade_date'], format='%Y%m%d').dt.strftime('%Y-%m-%d')
+        result_df['close'] = result_df['close'].astype(float)
+        result_df['change'] = result_df['close'] - result_df['close'].shift(1)
+        result_df['change_pct'] = result_df['change'] / result_df['close'].shift(1) * 100
+
+        # 3. 清洗数据
+        result_df = result_df.round(2)
+        result_df['close'] = result_df['close'].apply(lambda x: format(x, '.2f'))
+        result_df.replace('--', None, inplace=True)
+        result_df.replace('', None, inplace=True)
+        result_df.replace(np.nan, None, inplace=True)
+        return result_df[self._MARKET_COLUMNS]
+
+    def get_market_concept_min_ths(self, index_code='886041'):
+        """
+        获取概念行情当日分时
+        web： http://d.10jqka.com.cn/v6/time/48_886013/last.js
+        0930,958.901,74456973,36.807,2022925;  "pre": "960.374",
+        :param index_code: 概念指数代码
+        :return 时间，现价，成交额（元），均价，成交量（股） 涨跌额，涨跌幅
+        'index_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'pre_close', 'amount'
+        """
+        # 0.参数校验
+        if not index_code.startswith('8'):
+            raise RuntimeError('index_code错误，是8开头的指数代码,')
+        # 1.接口 url
+        api_url = f"http://d.10jqka.com.cn/v6/time/48_{index_code}/last.js"
+        text = self._get_text(api_url, index_code)
+        if THS_IP_LIMIT_RES in text:
+            return Exception(THS_IP_LIMIT_MSG)
+        # 2. 解析数据
+        result_json = json.loads(text[text.index('{'):-1])[f"48_{index_code}"]
+        pre_price = result_json['pre']
+        trade_date = result_json['date']
+        data_list = result_json['data'].split(';')
+        data = []
+        for d in data_list:
+            data.append(str(d).split(','))
+        # 3. 封装数据
+        result_df = pd.DataFrame(data=data, columns=['trade_time', 'price', 'amount', 'xx', 'volume'])
+        result_df['index_code'] = index_code
+        result_df['trade_time'] = trade_date + result_df['trade_time']
+        result_df['trade_date'] = pd.to_datetime(trade_date, format='%Y%m%d').strftime('%Y-%m-%d')
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_time'], format='%Y%m%d%H%M').dt.strftime(
+            '%Y-%m-%d %H:%M:%S')
+        result_df['price'] = result_df['price']
+        result_df['avg_price'] = None
+        result_df['change'] = result_df['price'].astype(float) - float(pre_price)
+        result_df['change_pct'] = result_df['change'] / float(pre_price) * 100
+        result_df.replace('--', None, inplace=True)
+        result_df.replace('', None, inplace=True)
+        result_df.replace(np.nan, None, inplace=True)
+        return result_df[self._MARKET_CONCEPT_MIN_COLUMNS]
+
+    def get_market_concept_current_ths(self, index_code: str = '886013', k_type: int = 1):
+        """
+        获取同花顺当前的概念行情
+        web: http://q.10jqka.com.cn/gn/
+        pc: http://d.10jqka.com.cn/v6/line/48_886042/01/today.js
+        quotebridge_v6_line_48_886042_01_today({"48_886042":{"1":"20230425","7":"891.344","8":"892.350","9":"853.800",
+        "11":"860.076","13":491708080,"19":"17647511000.000","74":"","1968584":"","66":"","open":1,"dt":"2244",
+        "name":"\u5b58\u50a8\u82af\u7247","marketType":""}})
+
+        :param index_code: 同花顺概念指数代码
+        :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
+        :return: k线行情数据 [概念代码,交易时间，交易日期，开，高，低，当前价格,成交量，成交额]
+        ;20230419,958.901,981.118,958.449,961.107,521143220,20442229000.000,存储芯片
+        k:   1,      7,      8,       9,      11,      13,         19,        name
+        成交量：股 820953530  821万手
+        成交额：元 16959251000.000 169.6亿
+        """
+        # 0.参数校验
+        if not index_code.startswith('8'):
+            raise RuntimeError('index_code错误，是8开头的指数代码,')
+        # 1.接口 url
+        api_url = f"http://d.10jqka.com.cn/v6/line/48_{index_code}/{k_type - 1}1/today.js"
+        # 同花顺可能ip限制，降低请求次数
+        text = self._get_text(api_url, index_code)
+        if THS_IP_LIMIT_RES in text:
+            return Exception(THS_IP_LIMIT_MSG)
+        result_text = text[text.index('{'):-1]
+        data_list = [json.loads(result_text)[f"48_{index_code}"]]
+        rename = {'1': 'trade_date', '7': 'open', '8': 'high', '9': 'low', '11': 'price', '13': 'volume',
+                  '19': 'amount', 'open': 'status'}
+        result_df = pd.DataFrame(data=data_list).rename(columns=rename)
+        result_df['trade_time'] = result_df['trade_date'] + result_df['dt']
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_time'], format='%Y%m%d%H%M').dt.strftime(
+            '%Y-%m-%d %H:%M:%S')
+        columns = ['trade_time', 'trade_date', 'open', 'high', 'low', 'price', 'volume', 'amount']
+        result_df = result_df[columns]
+        result_df['index_code'] = index_code
+        result_df['trade_date'] = pd.to_datetime(result_df['trade_date'], format='%Y%m%d').dt.strftime('%Y-%m-%d')
+        result_df['change'] = None
+        result_df['change_pct'] = None
+        return result_df[self._MARKET_CONCEPT_CURRENT_COLUMNS]
+
+
+if __name__ == '__main__':
+    print(ConceptMarketThs().get_market_concept_ths(index_code='886041'))
+    print(ConceptMarketThs().get_market_concept_min_ths(index_code='886041'))
+    print(ConceptMarketThs().get_market_concept_current_ths(index_code='886041'))
```

### Comparing `adata-1.2.4/adata/stock/market/index_market/market_index_east.py` & `adata-2.0.0b0/adata/stock/market/index_market/market_index_east.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-# -*- coding: utf-8 -*-
-"""
-@summary: 股票指数 行情
-@author: 1nchaos
-@date: 2023/06/01 16:17
-"""
-import datetime
-
-import pandas as pd
-
-from adata.common import requests
-from adata.common.exception.handler import handler_null
-from adata.stock.market.index_market.market_index_template import StockMarketIndexTemplate
-
-
-class StockMarketIndexEast(StockMarketIndexTemplate):
-    def __init__(self) -> None:
-        super().__init__()
-
-    @handler_null
-    def get_market_index(self, index_code: str = '000001', start_date='2020-01-01', k_type: int = 1):
-        """
-        获取指数行情
-        http://77.push2his.eastmoney.com/api/qt/stock/kline/get?secid=1.000300&fields1=f1,f2,f3,f4,f5,f6&fields2=f51,f52,f53,f54,f55,f56,f57,f58,f59,f60,f61&klt=102&fqt=1&beg=0&end=20500101&smplmt=1247.73&lmt=1000000
-        :param start_date: 开始时间
-        :param index_code: 指数代码
-        :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
-        :return: k线行情数据 [日期，开，高，低，收,成交量，成交额]
-        """
-        url = f"https://push2his.eastmoney.com/api/qt/stock/kline/get?" \
-              f"secid=1.{index_code}&fields1=f1,f2,f3,f4,f5,f6&fields2=f51,f52,f53,f54,f55,f56,f57,f58,f59,f60,f61&" \
-              f"klt=10{k_type}&fqt=1&end=20500101&lmt=1000000"
-        res_json = requests.request('get', url, headers={}, proxies={}).json()
-        # 解析数据
-        code = res_json['data']['code']
-        if code != index_code:
-            return
-        res_data = res_json['data']['klines']
-        data = []
-        for _ in res_data:
-            row = str(_).split(',')
-            data.append(
-                {'trade_date': row[0], 'open': row[1], 'close': row[2], 'high': row[3], 'low': row[4], 'volume': row[5],
-                 'amount': row[6], 'change': row[9], 'change_pct': row[8], 'index_code': index_code})
-        result_df = pd.DataFrame(data=data, columns=self._MARKET_INDEX_COLUMNS)
-
-        # 清洗数据
-        result_df[['open', 'high', 'low', 'close', 'volume', 'amount', 'change', 'change_pct']] = \
-            result_df[['open', 'high', 'low', 'close', 'volume', 'amount', 'change', 'change_pct']].astype(float)
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d %H:%M:%S')
-        result_df = result_df.round(2)
-        if start_date:
-            result_df = result_df[result_df['trade_date'] >= start_date]
-        return result_df[self._MARKET_INDEX_COLUMNS]
-
-    @handler_null
-    def get_market_index_min(self, index_code='000001'):
-        """
-        获取指数当日的分时行情
-        http://push2his.eastmoney.com/api/qt/stock/trends2/get?fields1=f1,f2,f3,f4,f5,f6,f7,f8,f9,f10,f11,f12,f13&fields2=f51,f52,f53,f54,f55,f56,f57,f58&iscr=0&ndays=1&secid=1.000300
-        :param index_code: 指数代码
-        :return 时间，现价，成交额（元），均价，成交量（股） 涨跌额，涨跌幅
-        ['index_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'avg_price', 'amount']
-        """
-        url = f"http://push2his.eastmoney.com/api/qt/stock/trends2/get?" \
-              f"fields1=f1,f2,f3,f4,f5,f6,f7,f8,f9,f10,f11,f12,f13&fields2=f51,f52,f53,f54,f55,f56,f57,f58&" \
-              f"iscr=0&ndays=1&secid=1.{index_code}"
-        res_json = requests.request('get', url, headers={}, proxies={}).json()
-        # 解析数据
-        code = res_json['data']['code']
-        pre_price = res_json['data']['prePrice']
-        if code != index_code:
-            return
-        res_data = res_json['data']['trends']
-        data = []
-        for _ in res_data:
-            row = str(_).split(',')
-            data.append(
-                {'trade_date': row[0], 'open': row[1], 'price': row[2], 'high': row[3], 'low': row[4],
-                 'volume': row[5], 'amount': row[6], 'avg_price': row[7], 'index_code': index_code})
-        result_df = pd.DataFrame(data=data, columns=self._MARKET_INDEX_MIN_COLUMNS)
-
-        # 清洗数据
-        result_df[['price', 'volume', 'amount', 'avg_price']] = \
-            result_df[['price', 'volume', 'amount', 'avg_price']].astype(float)
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d %H:%M:%S')
-        result_df['trade_date'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d')
-        result_df['change'] = result_df['price'] - pre_price
-        result_df['change_pct'] = result_df['change'] / pre_price * 100
-        result_df = result_df.round(2)
-        return result_df
-
-    @handler_null
-    def get_market_index_current(self, index_code: str = '000001'):
-        """
-        获取当前的指数行情
-        :param index_code: 指数代码
-        :return: [指数代码,交易时间，交易日期，开，高，低，当前价格,成交量，成交额]
-        ['trade_time', 'trade_date', 'open', 'high', 'low', 'price', 'volume', 'amount']
-        """
-        url = f"http://push2.eastmoney.com/api/qt/stock/get?" \
-              f"invt=2&fltt=1&fields=f58,f107,f57,f43,f59,f169,f170,f152,f46,f60,f44,f45,f47,f48,f19,f532,f39,f161,f49," \
-              f"f171,f50,f86,f600,f601,f154,f84,f85,f168,f108,f116,f167,f164,f92,f71,f117,f292,f113,f114,f115,f119," \
-              f"f120,f121,f122,f296&secid=1.{index_code}&wbp2u=|0|0|0|web"
-        res_json = requests.request('get', url, headers={}, proxies={}).json()
-        # 解析数据
-        j = res_json['data']
-        if not j:
-            return pd.DataFrame(data=[], columns=self._MARKET_INDEX_CURRENT_COLUMNS)
-        code = j['f57']
-        if code != index_code:
-            return pd.DataFrame(data=[], columns=self._MARKET_INDEX_CURRENT_COLUMNS)
-        pre_close = j['f60']
-        data = [{'open': j['f46'], 'high': j['f44'], 'low': j['f45'], 'price': j['f43'], 'volume': j['f47'],
-                 'amount': j['f48'], 'index_code': index_code}]
-        result_df = pd.DataFrame(data=data, columns=self._MARKET_INDEX_CURRENT_COLUMNS)
-
-        # 清洗数据
-        result_df[['open', 'high', 'low', 'price', 'volume', 'amount']] = \
-            result_df[['open', 'high', 'low', 'price', 'volume', 'amount']].astype(float)
-        result_df['change'] = result_df['price'] - pre_close
-        result_df['change_pct'] = result_df['change'] / pre_close * 100
-        result_df = result_df.round(2)
-        result_df['trade_time'] = datetime.datetime.now()
-        return result_df
-
-
-if __name__ == '__main__':
-    print(StockMarketIndexEast().get_market_index(index_code='000001', start_date='2022-12-01'))
-    print(StockMarketIndexEast().get_market_index_min(index_code='000001'))
-    print(StockMarketIndexEast().get_market_index_current(index_code='000001'))
+# -*- coding: utf-8 -*-
+"""
+@summary: 股票指数 行情
+@author: 1nchaos
+@date: 2023/06/01 16:17
+"""
+import datetime
+
+import pandas as pd
+
+from adata.common import requests
+from adata.common.exception.handler import handler_null
+from adata.stock.market.index_market.market_index_template import StockMarketIndexTemplate
+
+
+class StockMarketIndexEast(StockMarketIndexTemplate):
+    def __init__(self) -> None:
+        super().__init__()
+
+    @handler_null
+    def get_market_index(self, index_code: str = '000001', start_date='2020-01-01', k_type: int = 1):
+        """
+        获取指数行情
+        http://77.push2his.eastmoney.com/api/qt/stock/kline/get?secid=1.000300&fields1=f1,f2,f3,f4,f5,f6&fields2=f51,f52,f53,f54,f55,f56,f57,f58,f59,f60,f61&klt=102&fqt=1&beg=0&end=20500101&smplmt=1247.73&lmt=1000000
+        :param start_date: 开始时间
+        :param index_code: 指数代码
+        :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
+        :return: k线行情数据 [日期，开，高，低，收,成交量，成交额]
+        """
+        url = f"https://push2his.eastmoney.com/api/qt/stock/kline/get?" \
+              f"secid=1.{index_code}&fields1=f1,f2,f3,f4,f5,f6&fields2=f51,f52,f53,f54,f55,f56,f57,f58,f59,f60,f61&" \
+              f"klt=10{k_type}&fqt=1&end=20500101&lmt=1000000"
+        res_json = requests.request('get', url, headers={}, proxies={}).json()
+        # 解析数据
+        code = res_json['data']['code']
+        if code != index_code:
+            return
+        res_data = res_json['data']['klines']
+        data = []
+        for _ in res_data:
+            row = str(_).split(',')
+            data.append(
+                {'trade_date': row[0], 'open': row[1], 'close': row[2], 'high': row[3], 'low': row[4], 'volume': row[5],
+                 'amount': row[6], 'change': row[9], 'change_pct': row[8], 'index_code': index_code})
+        result_df = pd.DataFrame(data=data, columns=self._MARKET_INDEX_COLUMNS)
+
+        # 清洗数据
+        result_df[['open', 'high', 'low', 'close', 'volume', 'amount', 'change', 'change_pct']] = \
+            result_df[['open', 'high', 'low', 'close', 'volume', 'amount', 'change', 'change_pct']].astype(float)
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d %H:%M:%S')
+        result_df = result_df.round(2)
+        if start_date:
+            result_df = result_df[result_df['trade_date'] >= start_date]
+        return result_df[self._MARKET_INDEX_COLUMNS]
+
+    @handler_null
+    def get_market_index_min(self, index_code='000001'):
+        """
+        获取指数当日的分时行情
+        http://push2his.eastmoney.com/api/qt/stock/trends2/get?fields1=f1,f2,f3,f4,f5,f6,f7,f8,f9,f10,f11,f12,f13&fields2=f51,f52,f53,f54,f55,f56,f57,f58&iscr=0&ndays=1&secid=1.000300
+        :param index_code: 指数代码
+        :return 时间，现价，成交额（元），均价，成交量（股） 涨跌额，涨跌幅
+        ['index_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'avg_price', 'amount']
+        """
+        url = f"http://push2his.eastmoney.com/api/qt/stock/trends2/get?" \
+              f"fields1=f1,f2,f3,f4,f5,f6,f7,f8,f9,f10,f11,f12,f13&fields2=f51,f52,f53,f54,f55,f56,f57,f58&" \
+              f"iscr=0&ndays=1&secid=1.{index_code}"
+        res_json = requests.request('get', url, headers={}, proxies={}).json()
+        # 解析数据
+        code = res_json['data']['code']
+        pre_price = res_json['data']['prePrice']
+        if code != index_code:
+            return
+        res_data = res_json['data']['trends']
+        data = []
+        for _ in res_data:
+            row = str(_).split(',')
+            data.append(
+                {'trade_date': row[0], 'open': row[1], 'price': row[2], 'high': row[3], 'low': row[4],
+                 'volume': row[5], 'amount': row[6], 'avg_price': row[7], 'index_code': index_code})
+        result_df = pd.DataFrame(data=data, columns=self._MARKET_INDEX_MIN_COLUMNS)
+
+        # 清洗数据
+        result_df[['price', 'volume', 'amount', 'avg_price']] = \
+            result_df[['price', 'volume', 'amount', 'avg_price']].astype(float)
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d %H:%M:%S')
+        result_df['trade_date'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d')
+        result_df['change'] = result_df['price'] - pre_price
+        result_df['change_pct'] = result_df['change'] / pre_price * 100
+        result_df = result_df.round(2)
+        return result_df
+
+    @handler_null
+    def get_market_index_current(self, index_code: str = '000001'):
+        """
+        获取当前的指数行情
+        :param index_code: 指数代码
+        :return: [指数代码,交易时间，交易日期，开，高，低，当前价格,成交量，成交额]
+        ['trade_time', 'trade_date', 'open', 'high', 'low', 'price', 'volume', 'amount']
+        """
+        url = f"http://push2.eastmoney.com/api/qt/stock/get?" \
+              f"invt=2&fltt=1&fields=f58,f107,f57,f43,f59,f169,f170,f152,f46,f60,f44,f45,f47,f48,f19,f532,f39,f161,f49," \
+              f"f171,f50,f86,f600,f601,f154,f84,f85,f168,f108,f116,f167,f164,f92,f71,f117,f292,f113,f114,f115,f119," \
+              f"f120,f121,f122,f296&secid=1.{index_code}&wbp2u=|0|0|0|web"
+        res_json = requests.request('get', url, headers={}, proxies={}).json()
+        # 解析数据
+        j = res_json['data']
+        if not j:
+            return pd.DataFrame(data=[], columns=self._MARKET_INDEX_CURRENT_COLUMNS)
+        code = j['f57']
+        if code != index_code:
+            return pd.DataFrame(data=[], columns=self._MARKET_INDEX_CURRENT_COLUMNS)
+        pre_close = j['f60']
+        data = [{'open': j['f46'], 'high': j['f44'], 'low': j['f45'], 'price': j['f43'], 'volume': j['f47'],
+                 'amount': j['f48'], 'index_code': index_code}]
+        result_df = pd.DataFrame(data=data, columns=self._MARKET_INDEX_CURRENT_COLUMNS)
+
+        # 清洗数据
+        result_df[['open', 'high', 'low', 'price', 'volume', 'amount']] = \
+            result_df[['open', 'high', 'low', 'price', 'volume', 'amount']].astype(float)
+        result_df['change'] = result_df['price'] - pre_close
+        result_df['change_pct'] = result_df['change'] / pre_close * 100
+        result_df = result_df.round(2)
+        result_df['trade_time'] = datetime.datetime.now()
+        return result_df
+
+
+if __name__ == '__main__':
+    print(StockMarketIndexEast().get_market_index(index_code='000001', start_date='2022-12-01'))
+    print(StockMarketIndexEast().get_market_index_min(index_code='000001'))
+    print(StockMarketIndexEast().get_market_index_current(index_code='000001'))
```

### Comparing `adata-1.2.4/adata/stock/market/index_market/market_index_template.py` & `adata-2.0.0b0/adata/stock/market/index_market/market_index_template.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# -*- coding: utf-8 -*-
-"""
-@summary: 股票指数 行情
-@author: 1nchaos
-@date: 2023/06/01 16:17
-"""
-
-
-class StockMarketIndexTemplate(object):
-    """
-    股票指数 行情
-    """
-    _MARKET_INDEX_COLUMNS = ['index_code', 'trade_date', 'trade_time', 'open', 'high', 'low', 'close', 'volume',
-                             'amount', 'change', 'change_pct']
-    _MARKET_INDEX_MIN_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'price', 'avg_price', 'volume', 'amount',
-                                 'change', 'change_pct']
-    _MARKET_INDEX_CURRENT_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'open', 'high', 'low', 'price',
-                                     'volume', 'amount']
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def get_market_index(self, index_code: str = '000001', start_date='2020-01-01', k_type: int = 1):
-        """
-        获取指数行情
-        """
-        pass
-
-    def get_market_index_min(self, index_code='000001'):
-        """
-        获取指数当日的分时行情
-        :param index_code: 指数代码
-        :return 时间，现价，成交额（元），均价，成交量（股） 涨跌额，涨跌幅
-        ['index_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'avg_price', 'amount']
-        """
-        pass
-
-    def get_market_index_current(self, index_code: str = '000001'):
-        """
-        获取当前的指数行情
-        :param index_code: 指数代码
-        :return: [指数代码,交易时间，交易日期，开，高，低，当前价格,成交量，成交额]
-        ['trade_time', 'trade_date', 'open', 'high', 'low', 'price', 'volume', 'amount']
-        """
-        pass
+# -*- coding: utf-8 -*-
+"""
+@summary: 股票指数 行情
+@author: 1nchaos
+@date: 2023/06/01 16:17
+"""
+
+
+class StockMarketIndexTemplate(object):
+    """
+    股票指数 行情
+    """
+    _MARKET_INDEX_COLUMNS = ['index_code', 'trade_date', 'trade_time', 'open', 'high', 'low', 'close', 'volume',
+                             'amount', 'change', 'change_pct']
+    _MARKET_INDEX_MIN_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'price', 'avg_price', 'volume', 'amount',
+                                 'change', 'change_pct']
+    _MARKET_INDEX_CURRENT_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'open', 'high', 'low', 'price',
+                                     'volume', 'amount']
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def get_market_index(self, index_code: str = '000001', start_date='2020-01-01', k_type: int = 1):
+        """
+        获取指数行情
+        """
+        pass
+
+    def get_market_index_min(self, index_code='000001'):
+        """
+        获取指数当日的分时行情
+        :param index_code: 指数代码
+        :return 时间，现价，成交额（元），均价，成交量（股） 涨跌额，涨跌幅
+        ['index_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'avg_price', 'amount']
+        """
+        pass
+
+    def get_market_index_current(self, index_code: str = '000001'):
+        """
+        获取当前的指数行情
+        :param index_code: 指数代码
+        :return: [指数代码,交易时间，交易日期，开，高，低，当前价格,成交量，成交额]
+        ['trade_time', 'trade_date', 'open', 'high', 'low', 'price', 'volume', 'amount']
+        """
+        pass
```

### Comparing `adata-1.2.4/adata/stock/market/index_market/market_index_ths.py` & `adata-2.0.0b0/adata/fund/market/etf_market_ths.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,161 +1,155 @@
-# -*- coding: utf-8 -*-
-"""
-@summary: 股票指数 行情
-@author: 1nchaos
-@date: 2023/06/01 16:17
-"""
-import copy
-import json
-
-import numpy as np
-import pandas as pd
-
-from adata.common.base.base_ths import BaseThs
-from adata.common.exception.exception_msg import *
-from adata.common.headers import ths_headers
-from adata.stock.cache.index_code_rel_ths import rel
-from adata.stock.market.index_market.market_index_template import StockMarketIndexTemplate
-
-
-class StockMarketIndexThs(BaseThs, StockMarketIndexTemplate):
-    """
-    股票指数 行情
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def get_market_index(self, index_code: str = '000001', start_date='2020-01-01', k_type: int = 1):
-        """
-        获取指数行情数据
-        http://d.10jqka.com.cn/v4/line/zs_1A0001/01/2022.js
-        :param start_date: 开始时间
-        :param index_code: 指数代码
-        :param k_type:  k线类型：1.日；2.周；3.月 默认：1 日k
-        :return: ['trade_date', 'open', 'high', 'low', 'close', 'volume', 'amount']
-        """
-        # 0. 时间范围处理
-        years = self._get_years_by_start_date(start_date)
-        concept_code = rel[index_code] if index_code in rel.keys() else index_code
-        data = []
-        for year in years:
-            # 1.接口 url
-            api_url = f"http://d.10jqka.com.cn/v4/line/zs_{concept_code}/{k_type - 1}1/{year}.js"
-            # 同花顺可能ip限制，降低请求次数
-            text = self._get_text(api_url, concept_code)
-            if THS_IP_LIMIT_RES in text:
-                return Exception(THS_IP_LIMIT_MSG)
-            # 为空继续
-            if not text:
-                continue
-            # 2. 解析数据
-            result_text = text[text.index('{'):-1]
-            data_list = json.loads(result_text)['data'].split(';')
-            for d in data_list:
-                data.append(str(d).split(',')[0:7])
-        # 3. 数据etl
-        result_df = pd.DataFrame(data=data, columns=['trade_date', 'open', 'high', 'low', 'close', 'volume', 'amount'])
-        result_df.drop_duplicates(subset=['trade_date'], inplace=True)
-        result_df = result_df.sort_values(by='trade_date', ascending=True)
-        # 去重，日期升序
-        result_df['index_code'] = index_code
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d %H:%M:%S')
-        result_df['trade_date'] = pd.to_datetime(result_df['trade_date'], format='%Y%m%d').dt.strftime('%Y-%m-%d')
-        result_df['close'] = result_df['close'].astype(float)
-        result_df['change'] = result_df['close'] - result_df['close'].shift(1)
-        result_df['change_pct'] = result_df['change'] / result_df['close'].shift(1) * 100
-        result_df = result_df.round(2)
-        result_df['close'] = result_df['close'].apply(lambda x: format(x, '.2f'))
-        result_df.replace('--', None, inplace=True)
-        result_df.replace('', None, inplace=True)
-        result_df.replace(np.nan, None, inplace=True)
-        # 4. 筛选时间范围
-        if start_date:
-            result_df = result_df[result_df['trade_date'] >= start_date]
-        return result_df[self._MARKET_INDEX_COLUMNS]
-
-    def get_market_index_min(self, index_code='000001'):
-        """
-        获取概念行情当日分时
-        web： http://d.10jqka.com.cn/v4/time/zs_1A0001/last.js
-        0930,958.901,74456973,36.807,2022925;  "pre": "960.374",
-        :param index_code: 概念指数代码
-        :return 时间，现价，成交额（元），均价，成交量（股） 涨跌额，涨跌幅
-        ['index_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'avg_price', 'amount']
-        """
-        # 0. 指数代码转换
-        concept_code = rel[index_code] if index_code in rel.keys() else index_code
-        # 1.接口 url
-        api_url = f"http://d.10jqka.com.cn/v4/time/zs_{concept_code}/last.js"
-        text = self._get_text(api_url, concept_code)
-        if THS_IP_LIMIT_RES in text:
-            return Exception(THS_IP_LIMIT_MSG)
-        if not text:
-            return pd.DataFrame(data=[], columns=self._MARKET_INDEX_MIN_COLUMNS)
-        # 2. 解析数据
-        result_json = json.loads(text[text.index('{'):-1])[f"zs_{concept_code}"]
-        pre_price = result_json['pre']
-        trade_date = result_json['date']
-        data_list = result_json['data'].split(';')
-        data = []
-        for d in data_list:
-            data.append(str(d).split(','))
-        # 3. 封装数据
-        result_df = pd.DataFrame(data=data, columns=['trade_time', 'price', 'amount', 'avg_price', 'volume'])
-        result_df['index_code'] = index_code
-        result_df['trade_time'] = trade_date + result_df['trade_time']
-        result_df['trade_date'] = pd.to_datetime(trade_date, format='%Y%m%d').strftime('%Y-%m-%d')
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_time'], format='%Y%m%d%H%M').dt.strftime(
-            '%Y-%m-%d %H:%M:%S')
-        result_df['price'] = result_df['price']
-        result_df['change'] = result_df['price'].astype(float) - float(pre_price)
-        result_df['change_pct'] = result_df['change'] / float(pre_price) * 100
-
-        result_df['change'] = result_df['change'].apply(lambda x: format(x, '.2f'))
-        result_df['change_pct'] = result_df['change_pct'].apply(lambda x: format(x, '.2f'))
-        result_df.replace('--', None, inplace=True)
-        result_df.replace('', None, inplace=True)
-        result_df.replace(np.nan, None, inplace=True)
-        return result_df[self._MARKET_INDEX_MIN_COLUMNS]
-
-    def get_market_index_current(self, index_code: str = '000001'):
-        """
-        获取当前的指数行情
-        web: http://q.10jqka.com.cn/gn/
-        pc: http://d.10jqka.com.cn/v4/line/zs_1A0001/21/today.js
-        quotebridge_v4_line_zs_1A0001_21_today({"zs_1A0001":{"1":"20230602","7":"3196.15","8":"3233.99","9":"3189.52",
-        "11":"3230.07","13":60699786000,"19":"778489410000.00","74":"","1968584":"1.428","66":null,"open":1,"dt":"1755",
-        "name":"\u4e0a\u8bc1\u6307\u6570","marketType":""}})
-        :param index_code: 指数代码
-        :return: [指数代码,交易时间，交易日期，开，高，低，当前价格,成交量，成交额]
-        ['trade_time', 'trade_date', 'open', 'high', 'low', 'price', 'volume', 'amount']
-        """
-        # 0. 指数代码转换
-        concept_code = rel[index_code] if index_code in rel.keys() else index_code
-        # 1.接口 url
-        api_url = f"http://d.10jqka.com.cn/v4/line/zs_{concept_code}/01/today.js"
-        headers = copy.deepcopy(ths_headers.text_headers)
-        headers['Host'] = 'd.10jqka.com.cn'
-        # 同花顺可能ip限制，降低请求次数
-        text = self._get_text(api_url, concept_code)
-        if THS_IP_LIMIT_RES in text:
-            return Exception(THS_IP_LIMIT_MSG)
-        result_text = text[text.index('{'):-1]
-        data_list = [json.loads(result_text)[f"zs_{concept_code}"]]
-        rename = {'1': 'trade_date', '7': 'open', '8': 'high', '9': 'low', '11': 'price', '13': 'volume',
-                  '19': 'amount', 'open': 'status'}
-        result_df = pd.DataFrame(data=data_list).rename(columns=rename)
-        result_df['trade_time'] = result_df['trade_date'] + result_df['dt']
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_time'], format='%Y%m%d%H%M').dt.strftime(
-            '%Y-%m-%d %H:%M:%S')
-        columns = ['trade_time', 'trade_date', 'open', 'high', 'low', 'price', 'volume', 'amount']
-        result_df = result_df[columns]
-        result_df['index_code'] = index_code
-        result_df['trade_date'] = pd.to_datetime(result_df['trade_date'], format='%Y%m%d').dt.strftime('%Y-%m-%d')
-        return result_df[self._MARKET_INDEX_CURRENT_COLUMNS]
-
-
-if __name__ == '__main__':
-    print(StockMarketIndexThs().get_market_index(index_code='000001', start_date='2022-12-01'))
-    print(StockMarketIndexThs().get_market_index_min(index_code='000001'))
-    print(StockMarketIndexThs().get_market_index_current(index_code='000001'))
+# -*- coding: utf-8 -*-
+"""
+@summary: ETF 行情
+https://d.10jqka.com.cn/v6/line/hs_512880/11/last360.js
+
+@author: 1nchaos
+@date: 2023/3/30 16:17
+"""
+import json
+
+import numpy as np
+import pandas as pd
+
+from adata.common.base.base_ths import BaseThs
+from adata.common.exception.exception_msg import *
+from adata.fund.market.etf_market_template import ETFMarketTemplate
+
+
+class ETFMarketThs(BaseThs, ETFMarketTemplate):
+    """
+    股票概念 行情
+    """
+
+    def get_market_etf_ths(self, fund_code: str = '512880', k_type: int = 1, start_date='', end_date=''):
+        """
+        获取同花顺的ETF的行情
+        app: https://d.10jqka.com.cn/v6/line/hs_512880/01/last36000.js
+        00 日k不复权；01日k前复权；02日k后复权；11周k前复权；21月k前复权
+        :param start_date: 开始时间
+        :param end_date: 结束时间
+        :param fund_code: ETF代码
+        :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
+        :return: k线行情数据 [日期，开，高，低，收,成交量，成交额]
+        ;20230419,958.901,981.118,958.449,961.107,521143220,20442229000.000
+        成交量：股 820953530  821万手
+        成交额：元 16959251000.000 169.6亿
+        """
+        # 0.参数校验
+        # 1.接口 url
+        api_url = f"http://d.10jqka.com.cn/v6/line/hs_{fund_code}/{k_type - 1}1/last36000.js"
+        # 同花顺可能ip限制，降低请求次数
+        text = self._get_text(api_url, fund_code)
+        if THS_IP_LIMIT_RES in text:
+            return Exception(THS_IP_LIMIT_MSG)
+        result_text = text[text.index('{'):-1]
+        data_list = json.loads(result_text)['data'].split(';')
+        data = []
+        for d in data_list:
+            data.append(str(d).split(',')[0:7])
+        result_df = pd.DataFrame(data=data, columns=['trade_date', 'open', 'high', 'low', 'close', 'volume', 'amount'])
+        result_df['index_code'] = fund_code
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d %H:%M:%S')
+        result_df['trade_date'] = pd.to_datetime(result_df['trade_date'], format='%Y%m%d').dt.strftime('%Y-%m-%d')
+        result_df['close'] = result_df['close'].astype(float)
+        result_df['change'] = result_df['close'] - result_df['close'].shift(1)
+        result_df['change_pct'] = result_df['change'] / result_df['close'].shift(1) * 100
+
+        # 3. 清洗数据
+        result_df = result_df.round(3)
+        result_df['close'] = result_df['close'].apply(lambda x: format(x, '.3f'))
+        result_df.replace('--', None, inplace=True)
+        result_df.replace('', None, inplace=True)
+        result_df.replace(np.nan, None, inplace=True)
+        # 4. 时间范围
+        start_date = start_date if start_date else '1990-01-01'
+        end_date = end_date if end_date else '2099-01-01'
+        result_df = result_df[(result_df['trade_date'] >= start_date) & (result_df['trade_date'] <= end_date)]
+        return result_df[self._MARKET_COLUMNS]
+
+    def get_market_etf_min_ths(self, fund_code='512880'):
+        """
+        获取etf行情当日分时
+        web： https://d.10jqka.com.cn/v6/time/hs_512880/last.js
+        0930,958.901,74456973,36.807,2022925;  "pre": "960.374",
+        :param fund_code: ETF代码
+        :return 时间，现价，成交额（元），均价，成交量（股） 涨跌额，涨跌幅
+        'index_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'pre_close', 'amount'
+        """
+        # 0.参数校验
+        # 1.接口 url
+        api_url = f"http://d.10jqka.com.cn/v6/time/hs_{fund_code}/last.js"
+        text = self._get_text(api_url, fund_code)
+        if THS_IP_LIMIT_RES in text:
+            return Exception(THS_IP_LIMIT_MSG)
+        # 2. 解析数据
+        result_json = json.loads(text[text.index('{'):-1])[f"hs_{fund_code}"]
+        pre_price = result_json['pre']
+        trade_date = result_json['date']
+        data_list = result_json['data'].split(';')
+        data = []
+        for d in data_list:
+            data.append(str(d).split(','))
+        # 3. 封装数据
+        result_df = pd.DataFrame(data=data, columns=['trade_time', 'price', 'amount', 'avg_price', 'volume'])
+        result_df['index_code'] = fund_code
+        result_df['trade_time'] = trade_date + result_df['trade_time']
+        result_df['trade_date'] = pd.to_datetime(trade_date, format='%Y%m%d').strftime('%Y-%m-%d')
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_time'], format='%Y%m%d%H%M').dt.strftime(
+            '%Y-%m-%d %H:%M:%S')
+        result_df['price'] = result_df['price']
+        result_df['change'] = result_df['price'].astype(float) - float(pre_price)
+        result_df['change_pct'] = result_df['change'] / float(pre_price) * 100
+        result_df.replace('--', None, inplace=True)
+        result_df.replace('', None, inplace=True)
+        result_df.replace(np.nan, None, inplace=True)
+        return result_df[self._MARKET_ETF_MIN_COLUMNS]
+
+    def get_market_etf_current_ths(self, fund_code: str = '512880', k_type: int = 1):
+        """
+        获取同花顺当前的概念行情
+        web: https://d.10jqka.com.cn/v6/line/hs_512880/01/today.js
+        quotebridge_v6_line_hs_512880_01_today({
+        "hs_512880": { "1": "20240417", "7": "0.810", "8": "0.827", "9": "0.806","11": "0.825", "13": 1336243640,
+        "19": "1092886150.000", "74": "","1968584": "3.727","66": "","open": 1,"dt": "1751","name": "\u8bc1\u5238ETF",
+        "marketType": "" }})
+
+        :param fund_code: ETF代码
+        :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
+        :return: k线行情数据 [ETF代码,交易时间，交易日期，开，高，低，当前价格,成交量，成交额]
+        ;20230419,958.901,981.118,958.449,961.107,521143220,20442229000.000,存储芯片
+        k:   1,      7,      8,       9,      11,      13,         19,        name
+        成交量：股 820953530  821万手
+        成交额：元 16959251000.000 169.6亿
+        """
+        # 0.参数校验
+        # 1.接口 url
+        api_url = f"http://d.10jqka.com.cn/v6/line/hs_{fund_code}/{k_type - 1}1/today.js"
+        # 同花顺可能ip限制，降低请求次数
+        text = self._get_text(api_url, fund_code)
+        if THS_IP_LIMIT_RES in text:
+            return Exception(THS_IP_LIMIT_MSG)
+        result_text = text[text.index('{'):-1]
+        data_list = [json.loads(result_text)[f"hs_{fund_code}"]]
+        rename = {'1': 'trade_date', '7': 'open', '8': 'high', '9': 'low', '11': 'price', '13': 'volume',
+                  '19': 'amount', 'open': 'status'}
+        result_df = pd.DataFrame(data=data_list).rename(columns=rename)
+        result_df['trade_time'] = result_df['trade_date'] + result_df['dt']
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_time'], format='%Y%m%d%H%M').dt.strftime(
+            '%Y-%m-%d %H:%M:%S')
+        columns = ['trade_time', 'trade_date', 'open', 'high', 'low', 'price', 'volume', 'amount']
+        result_df = result_df[columns]
+        result_df['index_code'] = fund_code
+        result_df['trade_date'] = pd.to_datetime(result_df['trade_date'], format='%Y%m%d').dt.strftime('%Y-%m-%d')
+        result_df['change'] = None
+        result_df['change_pct'] = None
+        return result_df[self._MARKET_ETF_CURRENT_COLUMNS]
+
+
+if __name__ == '__main__':
+    print(ETFMarketThs().get_market_etf_ths(fund_code='512880', start_date='2024-01-01'))
+    print(ETFMarketThs().get_market_etf_ths(fund_code='159841', start_date='2024-01-01'))
+    print(ETFMarketThs().get_market_etf_min_ths(fund_code='512880'))
+    print(ETFMarketThs().get_market_etf_min_ths(fund_code='159841'))
+    print(ETFMarketThs().get_market_etf_current_ths(fund_code='512880'))
+    print(ETFMarketThs().get_market_etf_current_ths(fund_code='513800'))
```

### Comparing `adata-1.2.4/adata/stock/market/stock_dividend.py` & `adata-2.0.0b0/adata/stock/market/stock_dividend.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-# -*- coding: utf-8 -*-
-"""
-@desc: 股票分红信息
-数据来源：1. 百度
-
-@author: 1nchaos
-@time: 2023/3/29
-@log: change log
-"""
-
-import pandas as pd
-import numpy as np
-
-from adata.common.headers import baidu_headers
-from adata.common.utils import requests
-
-
-class StockDividend(object):
-    """
-    股票分红
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def get_dividend(self, stock_code='000001'):
-        """
-        获取当个股票的分红信息
-        :param stock_code: 股票代码
-        :return: 股票分红信息
-        """
-        return self.__dividend_baidu(stock_code)
-
-    def __dividend_baidu(self, stock_code):
-        """
-        获取百度的股票分红数据：公告日；分红方案；除权除息日
-        web： https://gushitong.baidu.com/stock/ab-300033
-        url： https://gushitong.baidu.com/opendata?openapi=1&dspName=iphone&tn=tangram&
-        client=app&query=300033&code=300033&word=300033&resource_id=5429&ma_ver=4&finClientType=pc
-        :param stock_code: 6位股票代码
-        :return: 股票分红信息
-        """
-        columns = ['report_date', 'dividend_plan', 'ex_dividend_date']
-        null_df = pd.DataFrame(data=[], columns=columns)
-        # 1.请求接口 url
-        api_url = f"https://gushitong.baidu.com/opendata?openapi=1&dspName=iphone&tn=tangram&client=app&" \
-                  f"query={stock_code}&code={stock_code}&word={stock_code}&resource_id=5429&ma_ver=4&finClientType=pc"
-        res = requests.request('get', api_url, headers=baidu_headers.text_headers)
-
-        # 2. 判断结果是否正确
-        if len(res.text) < 1 or res.status_code != 200:
-            return pd.DataFrame()
-        res_json = res.json()
-        if res_json['ResultCode'] != '0':
-            return null_df
-        # 3.解析数据
-        # 3.1 空数据时返回为空
-        result = res_json['Result']
-        if not result:
-            return null_df
-
-        # 3.2 正常解析数据 basicInfo,shareholderEquity,organRating,executiveInfo,bonusTransfer
-        try:
-            new_company = result[-1]['DisplayData']['resultData']['tplData']['result']['tabs'][-1]['content'][
-                'newCompany']
-            bonus_transfer = new_company['bonusTransfer']
-            header = bonus_transfer['header']
-            body = bonus_transfer['body']
-        except KeyError:
-            # TODO logger
-            return null_df
-
-        # 4. 封装数据
-        result_df = pd.DataFrame(data=body, columns=header)[['公告日', '分红方案', '除权除息日']]
-        result_df['stock_code'] = stock_code
-        rename_columns = {'公告日': 'report_date', '分红方案': 'dividend_plan', '除权除息日': 'ex_dividend_date'}
-        result_df = result_df.rename(columns=rename_columns)
-        # 5. 数据清洗
-        result_df = result_df[result_df.dividend_plan != '利润不分配']
-        result_df['ex_dividend_date'] = result_df['ex_dividend_date'].replace('--', np.nan)
-        return result_df
-
-
-if __name__ == '__main__':
-    print(StockDividend().get_dividend(stock_code='600781'))
+# -*- coding: utf-8 -*-
+"""
+@desc: 股票分红信息
+数据来源：1. 百度
+
+@author: 1nchaos
+@time: 2023/3/29
+@log: change log
+"""
+
+import pandas as pd
+import numpy as np
+
+from adata.common.headers import baidu_headers
+from adata.common.utils import requests
+
+
+class StockDividend(object):
+    """
+    股票分红
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def get_dividend(self, stock_code='000001'):
+        """
+        获取当个股票的分红信息
+        :param stock_code: 股票代码
+        :return: 股票分红信息
+        """
+        return self.__dividend_baidu(stock_code)
+
+    def __dividend_baidu(self, stock_code):
+        """
+        获取百度的股票分红数据：公告日；分红方案；除权除息日
+        web： https://gushitong.baidu.com/stock/ab-300033
+        url： https://gushitong.baidu.com/opendata?openapi=1&dspName=iphone&tn=tangram&
+        client=app&query=300033&code=300033&word=300033&resource_id=5429&ma_ver=4&finClientType=pc
+        :param stock_code: 6位股票代码
+        :return: 股票分红信息
+        """
+        columns = ['report_date', 'dividend_plan', 'ex_dividend_date']
+        null_df = pd.DataFrame(data=[], columns=columns)
+        # 1.请求接口 url
+        api_url = f"https://gushitong.baidu.com/opendata?openapi=1&dspName=iphone&tn=tangram&client=app&" \
+                  f"query={stock_code}&code={stock_code}&word={stock_code}&resource_id=5429&ma_ver=4&finClientType=pc"
+        res = requests.request('get', api_url, headers=baidu_headers.text_headers)
+
+        # 2. 判断结果是否正确
+        if len(res.text) < 1 or res.status_code != 200:
+            return pd.DataFrame()
+        res_json = res.json()
+        if res_json['ResultCode'] != '0':
+            return null_df
+        # 3.解析数据
+        # 3.1 空数据时返回为空
+        result = res_json['Result']
+        if not result:
+            return null_df
+
+        # 3.2 正常解析数据 basicInfo,shareholderEquity,organRating,executiveInfo,bonusTransfer
+        try:
+            new_company = result[-1]['DisplayData']['resultData']['tplData']['result']['tabs'][-1]['content'][
+                'newCompany']
+            bonus_transfer = new_company['bonusTransfer']
+            header = bonus_transfer['header']
+            body = bonus_transfer['body']
+        except KeyError:
+            # TODO logger
+            return null_df
+
+        # 4. 封装数据
+        result_df = pd.DataFrame(data=body, columns=header)[['公告日', '分红方案', '除权除息日']]
+        result_df['stock_code'] = stock_code
+        rename_columns = {'公告日': 'report_date', '分红方案': 'dividend_plan', '除权除息日': 'ex_dividend_date'}
+        result_df = result_df.rename(columns=rename_columns)
+        # 5. 数据清洗
+        result_df = result_df[result_df.dividend_plan != '利润不分配']
+        result_df['ex_dividend_date'] = result_df['ex_dividend_date'].replace('--', np.nan)
+        return result_df
+
+
+if __name__ == '__main__':
+    print(StockDividend().get_dividend(stock_code='600781'))
```

### Comparing `adata-1.2.4/adata/stock/market/stock_market/stock_market.py` & `adata-2.0.0b0/adata/stock/market/stock_market/stock_market.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-# -*- coding: utf-8 -*-
-"""
-@desc: 股票行情
-@author: 1nchaos
-@time: 2023/3/29
-@log: change log
-TODO 数据返回类型转换
-"""
-
-import pandas as pd
-
-from adata.stock.market.stock_market.stock_market_baidu import StockMarketBaiDu
-from adata.stock.market.stock_market.stock_market_qq import StockMarketQQ
-from adata.stock.market.stock_market.stock_market_sina import StockMarketSina
-
-
-class StockMarket(object):
-    """
-    股票行情
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.sina = StockMarketSina()
-        self.qq = StockMarketQQ()
-        self.baidu = StockMarketBaiDu()
-
-    def get_market(self, stock_code: str = '000001', start_date='1990-01-01', k_type=1, adjust_type: int = 1):
-        """
-        获取单个股票的行情
-        :param stock_code: 股票代码
-        :param start_date: 开始时间
-        :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
-        :param adjust_type: k线复权类型：0.不复权；1.前复权；2.后复权 默认：1 前复权 （目前：只有前复权,作为股票交易已经可用）
-        :return: k线行情数据
-        """
-        return self.baidu.get_market(stock_code=stock_code, start_date=start_date, k_type=k_type)
-
-    def get_market_min(self, stock_code: str = '000001'):
-        """
-        获取单个股票的今日分时行情
-        :param stock_code: 股票代码
-        :return: 当日分钟行情数据
-        """
-        return self.baidu.get_market_min(stock_code=stock_code)
-
-    def list_market_current(self, code_list=None):
-        """
-        获取多个股票最新行情信息
-        :param code_list: 股票代码
-        :return: 当前最新的行情价格信息
-        stock_code: 股票代码
-        short_name: 股票简称
-        price: 当前价格（元）
-        change: 涨跌额（元）
-        change_pct: 涨跌幅（%）
-        volume: 成交量（股）
-        amount: 成交金额（元）
-        """
-        if code_list is None:
-            return pd.DataFrame()
-        # 1. 先查询新浪
-        df = self.sina.list_market_current(code_list=code_list)
-        # 2. 然后腾讯
-        if df.empty:
-            df = self.qq.list_market_current(code_list=code_list)
-        return df
-
-    def get_market_five(self, stock_code: str = '000001'):
-        """
-        获取单个股票的5档行情
-        其中：百度的接口数据更精准，精确到了股。腾讯的精确到手
-        :param stock_code: 股票代码
-        :return: 最新的五档行情
-        """
-        res_df = self.qq.get_market_five(stock_code=stock_code)
-        if res_df.empty:
-            res_df = self.baidu.get_market_five(stock_code=stock_code)
-        return res_df
-
-    def get_market_bar(self, stock_code: str = '000001'):
-        """
-        获取单个股票的分时成交
-        :param stock_code: 股票代码
-        :return: 最新当天的分时成交
-        """
-        return self.baidu.get_market_bar(stock_code=stock_code)
-
-
-if __name__ == '__main__':
-    print(StockMarket().get_market(stock_code='000001', start_date='2021-01-01', k_type=3))
-    print(StockMarket().get_market_min(stock_code='000001'))
-    print(StockMarket().list_market_current(code_list=['000001', '600001', '000795', '872925']))
-    print(StockMarket().get_market_five(stock_code='000001'))
-    print(StockMarket().get_market_bar(stock_code='872925'))
+# -*- coding: utf-8 -*-
+"""
+@desc: 股票行情
+@author: 1nchaos
+@time: 2023/3/29
+@log: change log
+TODO 数据返回类型转换
+"""
+
+import pandas as pd
+
+from adata.stock.market.stock_market.stock_market_baidu import StockMarketBaiDu
+from adata.stock.market.stock_market.stock_market_qq import StockMarketQQ
+from adata.stock.market.stock_market.stock_market_sina import StockMarketSina
+
+
+class StockMarket(object):
+    """
+    股票行情
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.sina = StockMarketSina()
+        self.qq = StockMarketQQ()
+        self.baidu = StockMarketBaiDu()
+
+    def get_market(self, stock_code: str = '000001', start_date='1990-01-01', k_type=1, adjust_type: int = 1):
+        """
+        获取单个股票的行情
+        :param stock_code: 股票代码
+        :param start_date: 开始时间
+        :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
+        :param adjust_type: k线复权类型：0.不复权；1.前复权；2.后复权 默认：1 前复权 （目前：只有前复权,作为股票交易已经可用）
+        :return: k线行情数据
+        """
+        return self.baidu.get_market(stock_code=stock_code, start_date=start_date, k_type=k_type)
+
+    def get_market_min(self, stock_code: str = '000001'):
+        """
+        获取单个股票的今日分时行情
+        :param stock_code: 股票代码
+        :return: 当日分钟行情数据
+        """
+        return self.baidu.get_market_min(stock_code=stock_code)
+
+    def list_market_current(self, code_list=None):
+        """
+        获取多个股票最新行情信息
+        :param code_list: 股票代码
+        :return: 当前最新的行情价格信息
+        stock_code: 股票代码
+        short_name: 股票简称
+        price: 当前价格（元）
+        change: 涨跌额（元）
+        change_pct: 涨跌幅（%）
+        volume: 成交量（股）
+        amount: 成交金额（元）
+        """
+        if code_list is None:
+            return pd.DataFrame()
+        # 1. 先查询新浪
+        df = self.sina.list_market_current(code_list=code_list)
+        # 2. 然后腾讯
+        if df.empty:
+            df = self.qq.list_market_current(code_list=code_list)
+        return df
+
+    def get_market_five(self, stock_code: str = '000001'):
+        """
+        获取单个股票的5档行情
+        其中：百度的接口数据更精准，精确到了股。腾讯的精确到手
+        :param stock_code: 股票代码
+        :return: 最新的五档行情
+        """
+        res_df = self.qq.get_market_five(stock_code=stock_code)
+        if res_df.empty:
+            res_df = self.baidu.get_market_five(stock_code=stock_code)
+        return res_df
+
+    def get_market_bar(self, stock_code: str = '000001'):
+        """
+        获取单个股票的分时成交
+        :param stock_code: 股票代码
+        :return: 最新当天的分时成交
+        """
+        return self.baidu.get_market_bar(stock_code=stock_code)
+
+
+if __name__ == '__main__':
+    print(StockMarket().get_market(stock_code='000001', start_date='2021-01-01', k_type=1))
+    print(StockMarket().get_market_min(stock_code='000001'))
+    print(StockMarket().list_market_current(code_list=['000001', '600001', '000795', '872925']))
+    print(StockMarket().get_market_five(stock_code='000001'))
+    print(StockMarket().get_market_bar(stock_code='872925'))
```

### Comparing `adata-1.2.4/adata/stock/market/stock_market/stock_market_baidu.py` & `adata-2.0.0b0/adata/stock/market/stock_market/stock_market_baidu.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,224 +1,224 @@
-# -*- coding: utf-8 -*-
-"""
-@desc: 百度股市通
-https://gushitong.baidu.com/
-
-@author: 1nchaos
-@time: 2023/06/19
-@log: change log
-"""
-
-import time
-
-import pandas as pd
-
-from adata.common.exception.handler import handler_null
-from adata.common.headers import baidu_headers
-from adata.common.utils import requests
-from adata.stock.market.stock_market.stock_market_template import StockMarketTemplate
-
-
-class StockMarketBaiDu(StockMarketTemplate):
-    """
-    百度股票行情
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def get_market(self, stock_code: str = '000001', start_date='1990-01-01', k_type=1, adjust_type: int = 1):
-        """
-        获取百度的股票行情数据
-        web： https://gushitong.baidu.com/stock/ab-002926
-        url：quotation_fiveday_ab 5日分时，quotation_kline_ab K线， quotation_minute_ab 当日分钟
-        k线
-        https://finance.pae.baidu.com/selfselect/getstockquotation?all=1&isIndex=false&isBk=false&isBlock=false&
-        isFutures=false&isStock=true&newFormat=1&group=quotation_kline_ab&finClientType=pc&
-        code=002926&start_time=2018-02-05 00:00:00&ktype=1
-        分钟
-        https://finance.pae.baidu.com/selfselect/getstockquotation?
-        all=1&code=601318&isIndex=false&isBk=false&isBlock=false&isFutures=false&isStock=true&newFormat=1&
-        group=quotation_minute_ab&finClientType=pc
-        "ma5均价","ma5成交量","ma10均价","ma10成交量","ma20均价","ma20成交量"
-        :param stock_code: 6位股票代码
-        :param start_date: 开始时间
-        :param k_type: k线类型：1.日；2.周；3.月
-        # :param adjust_type: k线复权类型：0.不复权；1.前复权；2.后复权 默认：1 前复权 TODO
-        :return: k线行情数据:"时间戳", "时间","开盘","收盘","成交量","最高","最低","成交额","涨跌额","涨跌幅","换手率","昨收"
-        """
-        # 1. 请求接口 url
-        api_url = f"https://finance.pae.baidu.com/selfselect/getstockquotation?all=1&isIndex=false&isBk=false&" \
-                  f"isBlock=false&isFutures=false&isStock=true&newFormat=1&group=quotation_kline_ab&finClientType=pc&" \
-                  f"code={stock_code}&start_time={start_date} 00:00:00&ktype={k_type}"
-
-        res_json = None
-        for i in range(3):
-            res = requests.request('get', api_url, headers=baidu_headers.json_headers, proxies={})
-            # 2. 校验请求结果数据
-            res_json = res.json()
-            if res_json['ResultCode'] == '0':
-                break
-            time.sleep(2)
-        # 3.解析数据
-        # 3.1 空数据时返回为空
-        result = res_json['Result']
-        if not result:
-            return pd.DataFrame(data=[], columns=self._MARKET_COLUMNS)
-
-        # 3.2. 正常解析数据
-        keys = res_json['Result']['newMarketData']['keys']
-        market_data = res_json['Result']['newMarketData']['marketData']
-        market_data_list = str(market_data).split(';')
-        data = []
-        for one in market_data_list:
-            data.append(one.split(','))
-
-        # 4. 封装数据
-        rename_columns = {'turnoverratio': 'turnover_ratio', 'preClose': 'pre_close', 'range': 'change',
-                          'ratio': 'change_pct', 'time': 'trade_time'}
-        result_df = pd.DataFrame(data=data, columns=keys).rename(columns=rename_columns)[self._MARKET_COLUMNS]
-        if result_df.empty:
-            return pd.DataFrame(data=[], columns=self._MARKET_COLUMNS)
-        result_df['stock_code'] = stock_code
-        result_df['trade_date'] = result_df['trade_time']
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_time']).dt.strftime('%Y-%m-%d %H:%M:%S')
-        # 5. 数据清洗，剔除成交量为0的异常数据
-        result_df.replace('--', None, inplace=True)
-        result_df.replace('', None, inplace=True)
-        result_df['amount'] = result_df['amount'].astype(float)
-        result_df = result_df[result_df['amount'] > 0]
-        result_df['change'] = result_df['change'].str.replace('+', '').astype(float)
-        result_df['change_pct'] = result_df['change_pct'].str.replace('+', '').astype(float)
-        return result_df
-
-    def get_market_min(self, stock_code: str = '000001'):
-        """
-        获取百度的股票行情数据
-        web： https://gushitong.baidu.com/stock/ab-002926
-        url: https://finance.pae.baidu.com/selfselect/getstockquotation?
-        all=1&code=601318&isIndex=false&isBk=false&isBlock=false&isFutures=false&isStock=true&newFormat=1
-        &group=quotation_minute_ab&finClientType=pc
-        time, price, ratio, increase, volume, avgPrice, amount, timeKey, datetime, oriAmount
-        :param stock_code: 6位股票代码
-        :return: k线行情数据:"时间","价格","涨跌率","涨幅","均价","成交量", "成交额"
-        """
-        # 1. 请求接口 url
-        api_url = f"https://finance.pae.baidu.com/selfselect/getstockquotation?all=1&isIndex=false&isBk=false&" \
-                  f"isBlock=false&isFutures=false&isStock=true&newFormat=1&group=quotation_minute_ab&" \
-                  f"finClientType=pc&code={stock_code}"
-
-        res_json = None
-        for i in range(3):
-            res = requests.request('get', api_url, headers=baidu_headers.json_headers, proxies={})
-            # 2. 校验请求结果数据
-            res_json = res.json()
-            if res_json['ResultCode'] == '0':
-                break
-            time.sleep(2)
-        # 3.解析数据
-        # 3.1 空数据时返回为空
-        result = res_json['Result']
-        if not result:
-            return pd.DataFrame(data=[], columns=self._MARKET_MIN_COLUMNS)
-
-        # 3.2. 正常解析数据
-        market_data_list = res_json['Result']['priceinfo']
-
-        # 4. 封装数据
-        field = ['time', 'price', 'ratio', 'increase', 'volume', 'avgPrice', 'amount', 'timeKey', 'datetime',
-                 'oriAmount']
-        rename_columns = {'avgPrice': 'avg_price', 'oriAmount': 'ori_amount', 'ratio': 'change_pct',
-                          'increase': 'change'}
-        result_df = pd.DataFrame(data=market_data_list, columns=field).rename(columns=rename_columns)
-        result_df['amount'] = result_df['ori_amount']
-        result_df['stock_code'] = stock_code
-        # 这里是分钟均价，数据存在四舍五入的情况
-        result_df['volume'] = result_df['volume'].astype(int) * 100
-        result_df['trade_time'] = pd.to_datetime(result_df['time'], unit='s', utc=True).dt.tz_convert('Asia/Shanghai')
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_time']).dt.strftime("%Y-%m-%d %H:%M:%S")
-        result_df['trade_date'] = result_df['trade_time'].str[:10]
-        result_df['change'] = result_df['change'].str.replace('+', '').astype(float)
-        result_df['change_pct'] = result_df['change_pct'].str.replace('+', '').str.replace('%', '').astype(float)
-        return result_df[self._MARKET_MIN_COLUMNS]
-
-    @handler_null
-    def get_market_five(self, stock_code: str = '000001'):
-        """
-        https://finance.pae.baidu.com/vapi/v1/getquotation?srcid=5353&all=1&pointType=string&group=quotation_minute_ab&query=872925&code=872925&market_type=ab&newFormat=1&name=锦好医疗&finClientType=pc
-        :param stock_code: 股票代码
-        :return:
-        """
-        # 1. 请求接口 url
-        api_url = f" https://finance.pae.baidu.com/vapi/v1/getquotation?srcid=5353&all=1&pointType=string&" \
-                  f"group=quotation_minute_ab&query={stock_code}&code={stock_code}&market_type=ab&newFormat=1&finClientType=pc"
-
-        res = requests.request('get', api_url, headers=baidu_headers.json_headers, proxies={})
-        # 2. 校验请求结果数据
-        res_json = res.json()
-        # 3.解析数据
-        # 3.1 空数据时返回为空
-        result = res_json['Result']
-        if not result:
-            return pd.DataFrame(data=[], columns=self._MARKET_FIVE_COLUMNS)
-
-        # 3.2. 正常解析数据
-        sell = result['askinfos']
-        buy = result['buyinfos']
-        short_name = result["basicinfos"]["name"]
-        # 4. 封装数据
-        data = {'stock_code': stock_code, 'short_name': short_name,
-                's5': sell[0]['askprice'], 'sv5': sell[0]['askvolume'],
-                's4': sell[1]['askprice'], 'sv4': sell[1]['askvolume'],
-                's3': sell[2]['askprice'], 'sv3': sell[2]['askvolume'],
-                's2': sell[3]['askprice'], 'sv2': sell[3]['askvolume'],
-                's1': sell[4]['askprice'], 'sv1': sell[4]['askvolume'],
-                'b1': buy[0]['bidprice'], 'bv1': buy[0]['bidvolume'],
-                'b2': buy[1]['bidprice'], 'bv2': buy[1]['bidvolume'],
-                'b3': buy[2]['bidprice'], 'bv3': buy[2]['bidvolume'],
-                'b4': buy[3]['bidprice'], 'bv4': buy[3]['bidvolume'],
-                'b5': buy[4]['bidprice'], 'bv5': buy[4]['bidvolume']}
-        result_df = pd.DataFrame(data=[data], columns=self._MARKET_FIVE_COLUMNS)
-        return result_df[self._MARKET_FIVE_COLUMNS]
-
-    def get_market_bar(self, stock_code: str = '000001'):
-        """
-        https://finance.pae.baidu.com/vapi/v1/getquotation?srcid=5353&all=1&pointType=string&group=quotation_minute_ab&query=872925&code=872925&market_type=ab&newFormat=1&name=锦好医疗&finClientType=pc
-        :param stock_code: 股票代码
-        :return:
-        """
-        # 1. 请求接口 url
-        api_url = f" https://finance.pae.baidu.com/vapi/v1/getquotation?srcid=5353&all=1&pointType=string&" \
-                  f"group=quotation_minute_ab&query={stock_code}&code={stock_code}&market_type=ab&newFormat=1&finClientType=pc"
-
-        res_json = None
-        for i in range(3):
-            res = requests.request('get', api_url, headers=baidu_headers.json_headers, proxies={})
-            # 2. 校验请求结果数据
-            res_json = res.json()
-            if res_json['ResultCode'] == '0':
-                break
-            time.sleep(1)
-        # 3.解析数据
-        # 3.1 空数据时返回为空
-        result = res_json['Result']
-        if not result:
-            return pd.DataFrame(data=[], columns=self._MARKET_MIN_COLUMNS)
-
-        # 3.2. 正常解析数据
-        market_data_list = res_json['Result']['detailinfos']
-
-        # 4. 封装数据
-        field = ['time', 'volume', 'price', 'type', 'bsFlag', 'formatTime']
-        rename_columns = {'time': 'trade_time', 'bsFlag': 'bs_type'}
-        result_df = pd.DataFrame(data=market_data_list, columns=field).rename(columns=rename_columns)
-        result_df['stock_code'] = stock_code
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_time'], unit='s', utc=True).dt.tz_convert(
-            'Asia/Shanghai')
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_time']).dt.strftime("%Y-%m-%d %H:%M:%S")
-        return result_df[self._MARKET_BAR_COLUMNS]
-
-
-if __name__ == '__main__':
-    print(StockMarketBaiDu().get_market(stock_code='000001', start_date='2021-01-01', k_type=1))
-    print(StockMarketBaiDu().get_market_min(stock_code='000001'))
-    print(StockMarketBaiDu().get_market_bar(stock_code='000001'))
+# -*- coding: utf-8 -*-
+"""
+@desc: 百度股市通
+https://gushitong.baidu.com/
+
+@author: 1nchaos
+@time: 2023/06/19
+@log: change log
+"""
+
+import time
+
+import pandas as pd
+
+from adata.common.exception.handler import handler_null
+from adata.common.headers import baidu_headers
+from adata.common.utils import requests
+from adata.stock.market.stock_market.stock_market_template import StockMarketTemplate
+
+
+class StockMarketBaiDu(StockMarketTemplate):
+    """
+    百度股票行情
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def get_market(self, stock_code: str = '000001', start_date='1990-01-01', k_type=1, adjust_type: int = 1):
+        """
+        获取百度的股票行情数据
+        web： https://gushitong.baidu.com/stock/ab-002926
+        url：quotation_fiveday_ab 5日分时，quotation_kline_ab K线， quotation_minute_ab 当日分钟
+        k线
+        https://finance.pae.baidu.com/selfselect/getstockquotation?all=1&isIndex=false&isBk=false&isBlock=false&
+        isFutures=false&isStock=true&newFormat=1&group=quotation_kline_ab&finClientType=pc&
+        code=002926&start_time=2018-02-05 00:00:00&ktype=1
+        分钟
+        https://finance.pae.baidu.com/selfselect/getstockquotation?
+        all=1&code=601318&isIndex=false&isBk=false&isBlock=false&isFutures=false&isStock=true&newFormat=1&
+        group=quotation_minute_ab&finClientType=pc
+        "ma5均价","ma5成交量","ma10均价","ma10成交量","ma20均价","ma20成交量"
+        :param stock_code: 6位股票代码
+        :param start_date: 开始时间
+        :param k_type: k线类型：1.日；2.周；3.月
+        # :param adjust_type: k线复权类型：0.不复权；1.前复权；2.后复权 默认：1 前复权 TODO
+        :return: k线行情数据:"时间戳", "时间","开盘","收盘","成交量","最高","最低","成交额","涨跌额","涨跌幅","换手率","昨收"
+        """
+        # 1. 请求接口 url
+        api_url = f"https://finance.pae.baidu.com/selfselect/getstockquotation?all=1&isIndex=false&isBk=false&" \
+                  f"isBlock=false&isFutures=false&isStock=true&newFormat=1&group=quotation_kline_ab&finClientType=pc&" \
+                  f"code={stock_code}&start_time={start_date} 00:00:00&ktype={k_type}"
+
+        res_json = None
+        for i in range(3):
+            res = requests.request('get', api_url, headers=baidu_headers.json_headers, proxies={})
+            # 2. 校验请求结果数据
+            res_json = res.json()
+            if res_json['ResultCode'] == '0':
+                break
+            time.sleep(2)
+        # 3.解析数据
+        # 3.1 空数据时返回为空
+        result = res_json['Result']
+        if not result:
+            return pd.DataFrame(data=[], columns=self._MARKET_COLUMNS)
+
+        # 3.2. 正常解析数据
+        keys = res_json['Result']['newMarketData']['keys']
+        market_data = res_json['Result']['newMarketData']['marketData']
+        market_data_list = str(market_data).split(';')
+        data = []
+        for one in market_data_list:
+            data.append(one.split(','))
+
+        # 4. 封装数据
+        rename_columns = {'turnoverratio': 'turnover_ratio', 'preClose': 'pre_close', 'range': 'change',
+                          'ratio': 'change_pct', 'time': 'trade_time'}
+        result_df = pd.DataFrame(data=data, columns=keys).rename(columns=rename_columns)[self._MARKET_COLUMNS]
+        if result_df.empty:
+            return pd.DataFrame(data=[], columns=self._MARKET_COLUMNS)
+        result_df['stock_code'] = stock_code
+        result_df['trade_date'] = result_df['trade_time']
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_time']).dt.strftime('%Y-%m-%d %H:%M:%S')
+        # 5. 数据清洗，剔除成交量为0的异常数据
+        result_df.replace('--', None, inplace=True)
+        result_df.replace('', None, inplace=True)
+        result_df['amount'] = result_df['amount'].astype(float)
+        result_df = result_df[result_df['amount'] > 0]
+        result_df['change'] = result_df['change'].str.replace('+', '').astype(float)
+        result_df['change_pct'] = result_df['change_pct'].str.replace('+', '').astype(float)
+        return result_df
+
+    def get_market_min(self, stock_code: str = '000001'):
+        """
+        获取百度的股票行情数据
+        web： https://gushitong.baidu.com/stock/ab-002926
+        url: https://finance.pae.baidu.com/selfselect/getstockquotation?
+        all=1&code=601318&isIndex=false&isBk=false&isBlock=false&isFutures=false&isStock=true&newFormat=1
+        &group=quotation_minute_ab&finClientType=pc
+        time, price, ratio, increase, volume, avgPrice, amount, timeKey, datetime, oriAmount
+        :param stock_code: 6位股票代码
+        :return: k线行情数据:"时间","价格","涨跌率","涨幅","均价","成交量", "成交额"
+        """
+        # 1. 请求接口 url
+        api_url = f"https://finance.pae.baidu.com/selfselect/getstockquotation?all=1&isIndex=false&isBk=false&" \
+                  f"isBlock=false&isFutures=false&isStock=true&newFormat=1&group=quotation_minute_ab&" \
+                  f"finClientType=pc&code={stock_code}"
+
+        res_json = None
+        for i in range(3):
+            res = requests.request('get', api_url, headers=baidu_headers.json_headers, proxies={})
+            # 2. 校验请求结果数据
+            res_json = res.json()
+            if res_json['ResultCode'] == '0':
+                break
+            time.sleep(2)
+        # 3.解析数据
+        # 3.1 空数据时返回为空
+        result = res_json['Result']
+        if not result:
+            return pd.DataFrame(data=[], columns=self._MARKET_MIN_COLUMNS)
+
+        # 3.2. 正常解析数据
+        market_data_list = res_json['Result']['priceinfo']
+
+        # 4. 封装数据
+        field = ['time', 'price', 'ratio', 'increase', 'volume', 'avgPrice', 'amount', 'timeKey', 'datetime',
+                 'oriAmount']
+        rename_columns = {'avgPrice': 'avg_price', 'oriAmount': 'ori_amount', 'ratio': 'change_pct',
+                          'increase': 'change'}
+        result_df = pd.DataFrame(data=market_data_list, columns=field).rename(columns=rename_columns)
+        result_df['amount'] = result_df['ori_amount']
+        result_df['stock_code'] = stock_code
+        # 这里是分钟均价，数据存在四舍五入的情况
+        result_df['volume'] = result_df['volume'].astype(int) * 100
+        result_df['trade_time'] = pd.to_datetime(result_df['time'], unit='s', utc=True).dt.tz_convert('Asia/Shanghai')
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_time']).dt.strftime("%Y-%m-%d %H:%M:%S")
+        result_df['trade_date'] = result_df['trade_time'].str[:10]
+        result_df['change'] = result_df['change'].str.replace('+', '').astype(float)
+        result_df['change_pct'] = result_df['change_pct'].str.replace('+', '').str.replace('%', '').astype(float)
+        return result_df[self._MARKET_MIN_COLUMNS]
+
+    @handler_null
+    def get_market_five(self, stock_code: str = '000001'):
+        """
+        https://finance.pae.baidu.com/vapi/v1/getquotation?srcid=5353&all=1&pointType=string&group=quotation_minute_ab&query=872925&code=872925&market_type=ab&newFormat=1&name=锦好医疗&finClientType=pc
+        :param stock_code: 股票代码
+        :return:
+        """
+        # 1. 请求接口 url
+        api_url = f" https://finance.pae.baidu.com/vapi/v1/getquotation?srcid=5353&all=1&pointType=string&" \
+                  f"group=quotation_minute_ab&query={stock_code}&code={stock_code}&market_type=ab&newFormat=1&finClientType=pc"
+
+        res = requests.request('get', api_url, headers=baidu_headers.json_headers, proxies={})
+        # 2. 校验请求结果数据
+        res_json = res.json()
+        # 3.解析数据
+        # 3.1 空数据时返回为空
+        result = res_json['Result']
+        if not result:
+            return pd.DataFrame(data=[], columns=self._MARKET_FIVE_COLUMNS)
+
+        # 3.2. 正常解析数据
+        sell = result['askinfos']
+        buy = result['buyinfos']
+        short_name = result["basicinfos"]["name"]
+        # 4. 封装数据
+        data = {'stock_code': stock_code, 'short_name': short_name,
+                's5': sell[0]['askprice'], 'sv5': sell[0]['askvolume'],
+                's4': sell[1]['askprice'], 'sv4': sell[1]['askvolume'],
+                's3': sell[2]['askprice'], 'sv3': sell[2]['askvolume'],
+                's2': sell[3]['askprice'], 'sv2': sell[3]['askvolume'],
+                's1': sell[4]['askprice'], 'sv1': sell[4]['askvolume'],
+                'b1': buy[0]['bidprice'], 'bv1': buy[0]['bidvolume'],
+                'b2': buy[1]['bidprice'], 'bv2': buy[1]['bidvolume'],
+                'b3': buy[2]['bidprice'], 'bv3': buy[2]['bidvolume'],
+                'b4': buy[3]['bidprice'], 'bv4': buy[3]['bidvolume'],
+                'b5': buy[4]['bidprice'], 'bv5': buy[4]['bidvolume']}
+        result_df = pd.DataFrame(data=[data], columns=self._MARKET_FIVE_COLUMNS)
+        return result_df[self._MARKET_FIVE_COLUMNS]
+
+    def get_market_bar(self, stock_code: str = '000001'):
+        """
+        https://finance.pae.baidu.com/vapi/v1/getquotation?srcid=5353&all=1&pointType=string&group=quotation_minute_ab&query=872925&code=872925&market_type=ab&newFormat=1&name=锦好医疗&finClientType=pc
+        :param stock_code: 股票代码
+        :return:
+        """
+        # 1. 请求接口 url
+        api_url = f" https://finance.pae.baidu.com/vapi/v1/getquotation?srcid=5353&all=1&pointType=string&" \
+                  f"group=quotation_minute_ab&query={stock_code}&code={stock_code}&market_type=ab&newFormat=1&finClientType=pc"
+
+        res_json = None
+        for i in range(3):
+            res = requests.request('get', api_url, headers=baidu_headers.json_headers, proxies={})
+            # 2. 校验请求结果数据
+            res_json = res.json()
+            if res_json['ResultCode'] == '0':
+                break
+            time.sleep(1)
+        # 3.解析数据
+        # 3.1 空数据时返回为空
+        result = res_json['Result']
+        if not result:
+            return pd.DataFrame(data=[], columns=self._MARKET_MIN_COLUMNS)
+
+        # 3.2. 正常解析数据
+        market_data_list = res_json['Result']['detailinfos']
+
+        # 4. 封装数据
+        field = ['time', 'volume', 'price', 'type', 'bsFlag', 'formatTime']
+        rename_columns = {'time': 'trade_time', 'bsFlag': 'bs_type'}
+        result_df = pd.DataFrame(data=market_data_list, columns=field).rename(columns=rename_columns)
+        result_df['stock_code'] = stock_code
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_time'], unit='s', utc=True).dt.tz_convert(
+            'Asia/Shanghai')
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_time']).dt.strftime("%Y-%m-%d %H:%M:%S")
+        return result_df[self._MARKET_BAR_COLUMNS]
+
+
+if __name__ == '__main__':
+    print(StockMarketBaiDu().get_market(stock_code='000001', start_date='2021-01-01', k_type=1))
+    print(StockMarketBaiDu().get_market_min(stock_code='000001'))
+    print(StockMarketBaiDu().get_market_bar(stock_code='000001'))
```

### Comparing `adata-1.2.4/adata/stock/market/stock_market/stock_market_qq.py` & `adata-2.0.0b0/adata/stock/market/stock_market/stock_market_qq.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-# -*- coding: utf-8 -*-
-"""
-@desc: 腾讯股票行情中心
-https://stockapp.finance.qq.com/mstats/#
-
-@author: 1nchaos
-@time: 2023/6/19
-@log: change log
-"""
-import pandas as pd
-
-from adata.common import requests
-from adata.stock.market.stock_market.stock_market_template import StockMarketTemplate
-
-
-class StockMarketQQ(StockMarketTemplate):
-    """
-    腾讯股票行情
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def list_market_current(self, code_list=None):
-        """
-        获取多个股票最新行情信息
-        https://qt.gtimg.cn/r=0.5979076524724433&q=s_sh600011,s_r_hk00902,s_sh600012,s_r_hk00995,s_sh600016,whHKDCNY
-        :param code_list: 股票代码
-        :return: 当前最新的行情价格信息
-        """
-        api_url = f"https://qt.gtimg.cn/r=0.5979076524724433&q="
-        for code in code_list:
-            if code.startswith('0') or code.startswith('3'):
-                api_url += 's_sz' + code + ','
-            elif code.startswith('6') or code.startswith('9'):
-                api_url += 's_sh' + code + ','
-            elif code.startswith('4') or code.startswith('8'):
-                api_url += 's_bj' + code + ','
-
-        # 1.请求接口
-        res = requests.request('get', api_url, headers={})
-
-        # 2. 判断结果是否正确
-        if len(res.text) < 1 or res.status_code != 200:
-            return pd.DataFrame(data=[], columns=self._MARKET_CURRENT_COLUMNS)
-        # 3.解析数据
-
-        # 正常解析数据 v_s_sz000936="51~华西股份~000936~12.60~1.15~10.04~69137~8711~~111.64~GP-A";
-        data_list = res.text.split(';')
-        data = []
-        for data_str in data_list:
-            if len(data_str) < 8:
-                continue
-            code = data_str.split('~')
-            if len(code) == 11:
-                data.append(code[1:8])
-
-        # 4. 封装数据
-        data_columns = ['short_name', 'stock_code', 'price', 'change', 'change_pct', 'volume', 'amount']
-        result_df = pd.DataFrame(data=data, columns=data_columns)
-        # 单位：手，万元
-        mask = result_df['stock_code'].str.startswith(('0', '3', '6', '9'))
-        result_df.loc[mask, 'volume'] = result_df['volume'].astype(int) * 100
-        result_df.loc[mask, 'amount'] = result_df['amount'].astype(float) * 10000
-        return result_df[self._MARKET_CURRENT_COLUMNS]
-
-    def get_market_five(self, stock_code: str = '000001'):
-        """
-         https://web.sqt.gtimg.cn/q=sh601666,sh600691
-        :param stock_code: 股票代码
-        :return:
-        """
-        return self.list_market_five([stock_code])
-
-    def list_market_five(self, code_list=None):
-        """
-         https://web.sqt.gtimg.cn/q=sh601666,sh600691
-        :param code_list: 股票代码列表
-        :return:
-        """
-        if code_list is None or len(code_list) == 0:
-            return pd.DataFrame(data=[], columns=self._MARKET_FIVE_COLUMNS)
-        api_url = f"https://web.sqt.gtimg.cn/q="
-        for code in code_list:
-            if code.startswith('0') or code.startswith('3'):
-                api_url += 'sz' + code + ','
-            elif code.startswith('6') or code.startswith('9'):
-                api_url += 'sh' + code + ','
-            elif code.startswith('4') or code.startswith('8'):
-                api_url += 'bj' + code + ','
-
-        # 1.请求接口
-        res = requests.request('get', api_url, headers={})
-
-        # 2. 判断结果是否正确
-        if len(res.text) < 1 or res.status_code != 200:
-            return pd.DataFrame(data=[], columns=self._MARKET_FIVE_COLUMNS)
-        # 3.解析数据
-
-        # 正常解析数据 _sh601666="1~平煤股份~601666~10.13~9.82~9.82~545608~302942~242666~10.12~1000~10.11~471~10.10~2083~10.09
-        # ~989~10.08~632~10.13~2544~10.14~2794~10.15~3149~10.16~2103~10.17~1430~~20230913155915~0.31~3.16~10.23~9.82
-        # ~10.13/545608/551678149~545608~55168~2.37~5.10~~10.23~9.82~4.18~233.15~234.39~1.08~10.80~8.84~1.05~-6845~10
-        # .11~5.25~4.09~~~1.16~55167.8149~0.0000~0~
-        # ~GP-A~1.91~1.81~8.59~19.02~6.34~13.52~7.21~19.60~31.56~34.53~2301581075~2313866675~-39.81~-4.70~2301581075
-        # ~~~-22.43~0.10~~CNY~0~___D__F__N";
-        data_list = res.text.split(';')
-        data = []
-        for data_str in data_list:
-            if len(data_str) < 8:
-                continue
-            code = data_str.split('~')
-
-            if len(code) == 85:
-                row = code[2:3]
-                row.append(code[1])
-                row.extend(code[27:29])
-                row.extend(code[25:27])
-                row.extend(code[23:25])
-                row.extend(code[21:23])
-                row.extend(code[19:21])
-                row.extend(code[9:19])
-                data.append(row)
-
-        # 4. 封装数据
-        result_df = pd.DataFrame(data=data, columns=self._MARKET_FIVE_COLUMNS)
-        columns_to_multiply = ['sv5', 'sv4', 'sv3', 'sv2', 'sv1', 'bv1', 'bv2', 'bv3', 'bv4', 'bv5']
-        result_df[columns_to_multiply] = result_df[columns_to_multiply].astype(int) * 100
-        return result_df
-
-
-if __name__ == '__main__':
-    print(StockMarketQQ().list_market_current(code_list=['000001', '600001', '000795', '872925']))
-    print(StockMarketQQ().get_market_five(stock_code='000001'))
+# -*- coding: utf-8 -*-
+"""
+@desc: 腾讯股票行情中心
+https://stockapp.finance.qq.com/mstats/#
+
+@author: 1nchaos
+@time: 2023/6/19
+@log: change log
+"""
+import pandas as pd
+
+from adata.common import requests
+from adata.stock.market.stock_market.stock_market_template import StockMarketTemplate
+
+
+class StockMarketQQ(StockMarketTemplate):
+    """
+    腾讯股票行情
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def list_market_current(self, code_list=None):
+        """
+        获取多个股票最新行情信息
+        https://qt.gtimg.cn/r=0.5979076524724433&q=s_sh600011,s_r_hk00902,s_sh600012,s_r_hk00995,s_sh600016,whHKDCNY
+        :param code_list: 股票代码
+        :return: 当前最新的行情价格信息
+        """
+        api_url = f"https://qt.gtimg.cn/r=0.5979076524724433&q="
+        for code in code_list:
+            if code.startswith('0') or code.startswith('3'):
+                api_url += 's_sz' + code + ','
+            elif code.startswith('6') or code.startswith('9'):
+                api_url += 's_sh' + code + ','
+            elif code.startswith('4') or code.startswith('8'):
+                api_url += 's_bj' + code + ','
+
+        # 1.请求接口
+        res = requests.request('get', api_url, headers={})
+
+        # 2. 判断结果是否正确
+        if len(res.text) < 1 or res.status_code != 200:
+            return pd.DataFrame(data=[], columns=self._MARKET_CURRENT_COLUMNS)
+        # 3.解析数据
+
+        # 正常解析数据 v_s_sz000936="51~华西股份~000936~12.60~1.15~10.04~69137~8711~~111.64~GP-A";
+        data_list = res.text.split(';')
+        data = []
+        for data_str in data_list:
+            if len(data_str) < 8:
+                continue
+            code = data_str.split('~')
+            if len(code) == 11:
+                data.append(code[1:8])
+
+        # 4. 封装数据
+        data_columns = ['short_name', 'stock_code', 'price', 'change', 'change_pct', 'volume', 'amount']
+        result_df = pd.DataFrame(data=data, columns=data_columns)
+        # 单位：手，万元
+        mask = result_df['stock_code'].str.startswith(('0', '3', '6', '9'))
+        result_df.loc[mask, 'volume'] = result_df['volume'].astype(int) * 100
+        result_df.loc[mask, 'amount'] = result_df['amount'].astype(float) * 10000
+        return result_df[self._MARKET_CURRENT_COLUMNS]
+
+    def get_market_five(self, stock_code: str = '000001'):
+        """
+         https://web.sqt.gtimg.cn/q=sh601666,sh600691
+        :param stock_code: 股票代码
+        :return:
+        """
+        return self.list_market_five([stock_code])
+
+    def list_market_five(self, code_list=None):
+        """
+         https://web.sqt.gtimg.cn/q=sh601666,sh600691
+        :param code_list: 股票代码列表
+        :return:
+        """
+        if code_list is None or len(code_list) == 0:
+            return pd.DataFrame(data=[], columns=self._MARKET_FIVE_COLUMNS)
+        api_url = f"https://web.sqt.gtimg.cn/q="
+        for code in code_list:
+            if code.startswith('0') or code.startswith('3'):
+                api_url += 'sz' + code + ','
+            elif code.startswith('6') or code.startswith('9'):
+                api_url += 'sh' + code + ','
+            elif code.startswith('4') or code.startswith('8'):
+                api_url += 'bj' + code + ','
+
+        # 1.请求接口
+        res = requests.request('get', api_url, headers={})
+
+        # 2. 判断结果是否正确
+        if len(res.text) < 1 or res.status_code != 200:
+            return pd.DataFrame(data=[], columns=self._MARKET_FIVE_COLUMNS)
+        # 3.解析数据
+
+        # 正常解析数据 _sh601666="1~平煤股份~601666~10.13~9.82~9.82~545608~302942~242666~10.12~1000~10.11~471~10.10~2083~10.09
+        # ~989~10.08~632~10.13~2544~10.14~2794~10.15~3149~10.16~2103~10.17~1430~~20230913155915~0.31~3.16~10.23~9.82
+        # ~10.13/545608/551678149~545608~55168~2.37~5.10~~10.23~9.82~4.18~233.15~234.39~1.08~10.80~8.84~1.05~-6845~10
+        # .11~5.25~4.09~~~1.16~55167.8149~0.0000~0~
+        # ~GP-A~1.91~1.81~8.59~19.02~6.34~13.52~7.21~19.60~31.56~34.53~2301581075~2313866675~-39.81~-4.70~2301581075
+        # ~~~-22.43~0.10~~CNY~0~___D__F__N";
+        data_list = res.text.split(';')
+        data = []
+        for data_str in data_list:
+            if len(data_str) < 8:
+                continue
+            code = data_str.split('~')
+
+            if len(code) == 85:
+                row = code[2:3]
+                row.append(code[1])
+                row.extend(code[27:29])
+                row.extend(code[25:27])
+                row.extend(code[23:25])
+                row.extend(code[21:23])
+                row.extend(code[19:21])
+                row.extend(code[9:19])
+                data.append(row)
+
+        # 4. 封装数据
+        result_df = pd.DataFrame(data=data, columns=self._MARKET_FIVE_COLUMNS)
+        columns_to_multiply = ['sv5', 'sv4', 'sv3', 'sv2', 'sv1', 'bv1', 'bv2', 'bv3', 'bv4', 'bv5']
+        result_df[columns_to_multiply] = result_df[columns_to_multiply].astype(int) * 100
+        return result_df
+
+
+if __name__ == '__main__':
+    print(StockMarketQQ().list_market_current(code_list=['000001', '600001', '000795', '872925']))
+    print(StockMarketQQ().get_market_five(stock_code='000001'))
```

### Comparing `adata-1.2.4/adata/stock/market/stock_market/stock_market_sina.py` & `adata-2.0.0b0/adata/stock/market/stock_market/stock_market_sina.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-# -*- coding: utf-8 -*-
-"""
-@desc: 新浪
-https://finance.sina.com.cn/stock/
-
-@author: 1nchaos
-@time: 2023/06/19
-@log: change log
-"""
-
-import pandas as pd
-
-from adata.common.headers import sina_headers
-from adata.common.utils import requests
-from adata.stock.market.stock_market.stock_market_template import StockMarketTemplate
-
-
-class StockMarketSina(StockMarketTemplate):
-    """
-    新浪股票行情
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def list_market_current(self, code_list=None):
-        """
-        获取新浪的最新股票行情
-        url : https://hq.sinajs.cn/list=s_sh600905,s_sz000725,s_sz000100,s_sh601919
-        :param code_list:  代码列表
-        :return: 最新行情数据：代码,简称,当前价格(元),涨跌额(元),涨跌幅(%),成交量(股),成交额(元)
-        """
-        # 0.进行参数拼接处理
-        api_url = f"https://hq.sinajs.cn/list="
-        for code in code_list:
-            if code.startswith('0') or code.startswith('3'):
-                api_url += 's_sz' + code + ','
-            elif code.startswith('6') or code.startswith('9'):
-                api_url += 's_sh' + code + ','
-            elif code.startswith('4') or code.startswith('8'):
-                api_url += 's_bj' + code + ','
-
-        # 1.请求接口
-        res = requests.request('get', api_url, headers=sina_headers.c_headers)
-
-        # 2. 判断结果是否正确
-        if len(res.text) < 1 or res.status_code != 200:
-            return pd.DataFrame(data=[], columns=self._MARKET_CURRENT_COLUMNS)
-        # 3.解析数据
-
-        # 正常解析数据 var hq_str_s_bj872925="平安银行,14.840,0.480,3.343,374847,5483780.180";
-        data_list = res.text.split(';')
-        data = []
-        for data_str in data_list:
-            if len(data_str) < 8:
-                continue
-            idx = data_str.index('=')
-            code = [data_str[idx - 6:idx]]
-            code.extend(data_str[idx + 2:-1].split(','))
-            if len(code) == 7:
-                data.append(code)
-
-        # 4. 封装数据
-        result_df = pd.DataFrame(data=data, columns=self._MARKET_CURRENT_COLUMNS)
-        # 北京的单位是股和万元
-        mask = result_df['stock_code'].str.startswith(('0', '3', '6', '9'))
-        result_df.loc[mask, 'volume'] = result_df['volume'].astype(int) * 100
-        result_df.loc[mask, 'amount'] = result_df['amount'].astype(float) * 10000
-        return result_df
-
-
-if __name__ == '__main__':
-    print(StockMarketSina().list_market_current(code_list=['000001', '600001', '000795', '872925']))
+# -*- coding: utf-8 -*-
+"""
+@desc: 新浪
+https://finance.sina.com.cn/stock/
+
+@author: 1nchaos
+@time: 2023/06/19
+@log: change log
+"""
+
+import pandas as pd
+
+from adata.common.headers import sina_headers
+from adata.common.utils import requests
+from adata.stock.market.stock_market.stock_market_template import StockMarketTemplate
+
+
+class StockMarketSina(StockMarketTemplate):
+    """
+    新浪股票行情
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def list_market_current(self, code_list=None):
+        """
+        获取新浪的最新股票行情
+        url : https://hq.sinajs.cn/list=s_sh600905,s_sz000725,s_sz000100,s_sh601919
+        :param code_list:  代码列表
+        :return: 最新行情数据：代码,简称,当前价格(元),涨跌额(元),涨跌幅(%),成交量(股),成交额(元)
+        """
+        # 0.进行参数拼接处理
+        api_url = f"https://hq.sinajs.cn/list="
+        for code in code_list:
+            if code.startswith('0') or code.startswith('3'):
+                api_url += 's_sz' + code + ','
+            elif code.startswith('6') or code.startswith('9'):
+                api_url += 's_sh' + code + ','
+            elif code.startswith('4') or code.startswith('8'):
+                api_url += 's_bj' + code + ','
+
+        # 1.请求接口
+        res = requests.request('get', api_url, headers=sina_headers.c_headers)
+
+        # 2. 判断结果是否正确
+        if len(res.text) < 1 or res.status_code != 200:
+            return pd.DataFrame(data=[], columns=self._MARKET_CURRENT_COLUMNS)
+        # 3.解析数据
+
+        # 正常解析数据 var hq_str_s_bj872925="平安银行,14.840,0.480,3.343,374847,5483780.180";
+        data_list = res.text.split(';')
+        data = []
+        for data_str in data_list:
+            if len(data_str) < 8:
+                continue
+            idx = data_str.index('=')
+            code = [data_str[idx - 6:idx]]
+            code.extend(data_str[idx + 2:-1].split(','))
+            if len(code) == 7:
+                data.append(code)
+
+        # 4. 封装数据
+        result_df = pd.DataFrame(data=data, columns=self._MARKET_CURRENT_COLUMNS)
+        # 北京的单位是股和万元
+        mask = result_df['stock_code'].str.startswith(('0', '3', '6', '9'))
+        result_df.loc[mask, 'volume'] = result_df['volume'].astype(int) * 100
+        result_df.loc[mask, 'amount'] = result_df['amount'].astype(float) * 10000
+        return result_df
+
+
+if __name__ == '__main__':
+    print(StockMarketSina().list_market_current(code_list=['000001', '600001', '000795', '872925']))
```

### Comparing `adata-1.2.4/adata/stock/market/stock_market/stock_market_template.py` & `adata-2.0.0b0/adata/stock/market/stock_market/stock_market_template.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-# -*- coding: utf-8 -*-
-"""
-@desc: readme
-@author: 1nchaos
-@time: 2023/3/29
-@log: change log
-"""
-
-
-class StockMarketTemplate(object):
-    """
-    股票行情
-    """
-    _MARKET_COLUMNS = ['trade_time', 'open', 'close', 'volume', 'high', 'low', 'amount', 'change', 'change_pct',
-                       'turnover_ratio', 'pre_close']
-    _MARKET_MIN_COLUMNS = ['stock_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'avg_price', 'amount']
-    _MARKET_CURRENT_COLUMNS = ['stock_code', 'short_name', 'price', 'change', 'change_pct', 'volume', 'amount']
-    _MARKET_FIVE_COLUMNS = ['stock_code', 'short_name', 's5', 'sv5', 's4', 'sv4', 's3', 'sv3', 's2', 'sv2', 's1', 'sv1',
-                            'b1', 'bv1', 'b2', 'bv2', 'b3', 'bv3', 'b4', 'bv4', 'b5', 'bv5']
-    _MARKET_BAR_COLUMNS = ['stock_code', 'trade_time', 'price', 'volume', 'bs_type']
-
-    def get_market(self, stock_code: str = '000001', start_date='1990-01-01', k_type=1, adjust_type: int = 1):
-        """
-        获取单个股票的行情
-        :param stock_code: 股票代码
-        :param start_date: 开始时间
-        :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
-        :param adjust_type: k线复权类型：0.不复权；1.前复权；2.后复权 默认：1 前复权 （目前：只有前复权,作为股票交易已经可用）
-        :return: k线行情数据
-        _MARKET_COLUMNS
-        """
-        pass
-
-    def get_market_min(self, stock_code: str = '000001'):
-        """
-        获取单个股票的今日分时行情
-        :param stock_code: 股票代码
-        :return: 当日分钟行情数据
-        _MARKET_MIN_COLUMNS
-        """
-        pass
-
-    def list_market_current(self, code_list=None):
-        """
-        获取多个股票最新行情信息
-        :param code_list: 股票代码
-        :return: 当前最新的行情价格信息
-        _MARKET_CURRENT_COLUMNS
-        """
-        pass
-
-    def get_market_five(self, stock_code: str = '000001'):
-        """
-        获取单个股票的5档行情
-        :param stock_code: 股票代码
-        :return: 最新的五档行情
-        """
-        pass
-
-    def list_market_five(self, code_list=None):
-        """
-         https://web.sqt.gtimg.cn/q=sh601666,sh600691
-        :param code_list: 股票代码列表
-        :return:
-        """
-        pass
-
-    def get_market_bar(self, stock_code: str = '000001'):
-        """
-        获取单个股票的分时成交
-        :param stock_code: 股票代码
-        :return: 最新当天的分时成交
-        """
-        pass
+# -*- coding: utf-8 -*-
+"""
+@desc: readme
+@author: 1nchaos
+@time: 2023/3/29
+@log: change log
+"""
+
+
+class StockMarketTemplate(object):
+    """
+    股票行情
+    """
+    _MARKET_COLUMNS = ['trade_time', 'open', 'close', 'volume', 'high', 'low', 'amount', 'change', 'change_pct',
+                       'turnover_ratio', 'pre_close']
+    _MARKET_MIN_COLUMNS = ['stock_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'avg_price', 'amount']
+    _MARKET_CURRENT_COLUMNS = ['stock_code', 'short_name', 'price', 'change', 'change_pct', 'volume', 'amount']
+    _MARKET_FIVE_COLUMNS = ['stock_code', 'short_name', 's5', 'sv5', 's4', 'sv4', 's3', 'sv3', 's2', 'sv2', 's1', 'sv1',
+                            'b1', 'bv1', 'b2', 'bv2', 'b3', 'bv3', 'b4', 'bv4', 'b5', 'bv5']
+    _MARKET_BAR_COLUMNS = ['stock_code', 'trade_time', 'price', 'volume', 'bs_type']
+
+    def get_market(self, stock_code: str = '000001', start_date='1990-01-01', k_type=1, adjust_type: int = 1):
+        """
+        获取单个股票的行情
+        :param stock_code: 股票代码
+        :param start_date: 开始时间
+        :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
+        :param adjust_type: k线复权类型：0.不复权；1.前复权；2.后复权 默认：1 前复权 （目前：只有前复权,作为股票交易已经可用）
+        :return: k线行情数据
+        _MARKET_COLUMNS
+        """
+        pass
+
+    def get_market_min(self, stock_code: str = '000001'):
+        """
+        获取单个股票的今日分时行情
+        :param stock_code: 股票代码
+        :return: 当日分钟行情数据
+        _MARKET_MIN_COLUMNS
+        """
+        pass
+
+    def list_market_current(self, code_list=None):
+        """
+        获取多个股票最新行情信息
+        :param code_list: 股票代码
+        :return: 当前最新的行情价格信息
+        _MARKET_CURRENT_COLUMNS
+        """
+        pass
+
+    def get_market_five(self, stock_code: str = '000001'):
+        """
+        获取单个股票的5档行情
+        :param stock_code: 股票代码
+        :return: 最新的五档行情
+        """
+        pass
+
+    def list_market_five(self, code_list=None):
+        """
+         https://web.sqt.gtimg.cn/q=sh601666,sh600691
+        :param code_list: 股票代码列表
+        :return:
+        """
+        pass
+
+    def get_market_bar(self, stock_code: str = '000001'):
+        """
+        获取单个股票的分时成交
+        :param stock_code: 股票代码
+        :return: 最新当天的分时成交
+        """
+        pass
```

### Comparing `adata-1.2.4/adata.egg-info/PKG-INFO` & `adata-2.0.0b0/adata.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,289 +1,304 @@
-Metadata-Version: 2.1
-Name: adata
-Version: 1.2.4
-Summary: A Data,A Stock,ETF,Bond,Quant,Stock Market,K Line
-Home-page: https://github.com/1nchaos/adata
-Author: 1nchaos
-Author-email: 9527@1nchaos.com
-License: Apache License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.16.0
-Requires-Dist: pandas>=0.22.0
-Requires-Dist: beautifulsoup4>=4.0.2
-Requires-Dist: py_mini_racer>=0.6.0
-
-# [AData](https://adata.1nchaos.com)
-
-<p align="center">
-  <a href="https://adata.1nchaos.com/" target="_blank">
-    <img width="180" src="./docs/AData200x200.png" alt="logo">
-  </a>
-</p>
-
-![GitHub language count](https://img.shields.io/github/languages/count/1nchaos/adata)![GitHub top language](https://img.shields.io/github/languages/top/1nchaos/adata)[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/adata?color=d)](https://pypi.org/project/adata/)[![Licence](https://img.shields.io/hexpm/l/apa?color=d)](https://gitee.com/inchaos/adata/blob/main/LICENSE)[![Downloads](https://static.pepy.tech/badge/adata/week)](https://pepy.tech/project/adata)![GitHub Repo stars](https://img.shields.io/github/stars/1nchaos/adata)![GitHub issues](https://img.shields.io/github/issues/1nchaos/adata)![GitHub contributors](https://img.shields.io/github/contributors/1nchaos/adata)![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/1nchaos/adata)[![Downloads](https://static.pepy.tech/badge/adata)](https://pepy.tech/project/adata)![PyPI - Version](https://img.shields.io/pypi/v/adata)
-
-
-
-## 0、[介绍](https://adata.1nchaos.com/idea.html)
-> 专注A股，专注量化，向阳而生；开放、纯净、持续、为Ai(爱)发电。
->
-> 专注股票行情数据，为了保证数据的高可用性，采用多数据源融合切换。
->
-> 目标：支持个人量化行情的需要；众人拾柴火焰高，欢迎加入。
-
-**市场寒冷，发热不易，坚持更难；如有帮助到你，右上角点 ⭐Star 一键三连，谢谢支持和收藏^_^**
-
-## 一、[快速开始](https://adata.1nchaos.com/quickStart.html)
-
-### （1）安装sdk
-
-~~~python
-# 首次安装
-pip install adata
-# 指定镜像源
-pip install adata -i http://mirrors.aliyun.com/pypi/simple/
-
-# 升级版本
-pip install -U adata
-# 指定镜像源
-pip install -U adata -i http://mirrors.aliyun.com/pypi/simple/
-~~~
-
-**注：国内镜像可能存在同步延迟，可使用官方镜像源，以下是镜像源**
-
-阿里云【推荐】：http://mirrors.aliyun.com/pypi/simple/  
-
-清华大学：https://pypi.tuna.tsinghua.edu.cn/simple  
-
-官方镜像源：https://pypi.org/simple
-
-### （2）使用示例
-
-#### 1. 获取股票代码
-
-获取所有的股票代码
-
-~~~python
-import adata
-
-res_df = adata.stock.info.all_code()
-print(res_df)
-~~~
-
-示例结果：
-
-~~~python
-  stock_code short_name exchange
-0        001324       N长青科       SZ
-1        301361       众智科技       SZ
-2        300514        友讯达       SZ
-...         ...        ...      ...
-5490     300367        网力退       SZ
-5491     300372        欣泰退       SZ
-5492     300431        暴风退       SZ
-
-[5493 rows x 3 columns]
-~~~
-
-#### 2. 获取股票的行情
-
-获取到股票代码后，传入对应的stock_code参数，查询对应股票的行情信息。
-
-```python
-import adata
-
-# k_type: k线类型：1.日；2.周；3.月 默认：1 日k
-res_df = adata.stock.market.get_market(stock_code='000001', k_type=1, start_date='2021-01-01')
-print(res_df)
-```
-
-示例结果：
-
-~~~python
-            trade_time   open  close  ... pre_close stock_code  trade_date
-0    2021-01-04 00:00:00  18.69  18.19  ...     18.93     000001  2021-01-04
-1    2021-01-05 00:00:00  17.99  17.76  ...     18.19     000001  2021-01-05
-2    2021-01-06 00:00:00  17.67  19.15  ...     17.76     000001  2021-01-06
-..                   ...    ...    ...  ...       ...        ...         ...
-573  2023-05-18 00:00:00  12.57  12.49  ...     12.49     000001  2023-05-18
-574  2023-05-19 00:00:00  12.43  12.34  ...     12.49     000001  2023-05-19
-575  2023-05-22 00:00:00  12.31  12.38  ...     12.34     000001  2023-05-22
-
-[576 rows :x 13 columns]
-~~~
-
-#### 3. 其它数据使用
-
-请参考下面数据列表和相关字典文档，找到对应的函数并查看对应的函数注释，进行正确使用。
-
-- [数据字典](https://adata.1nchaos.com/dic/stockInfo.html) 
-
-####  4. 代理设置
-
-项目是基于公开接口，可能存在限制等，因此增加代理设置功能
-
-~~~
-import adata
-
-# 设置代理,代理是全局设置,代理失效后可重新设置。参数:ip,proxy_url
-adata.proxy(is_proxy=True, ip='60.167.21.27:1133')
-res_df = adata.stock.info.all_code()
-print(res_df)
-~~~
-
-**注：**
-
-- v0.0.027b0 及以上版本支持；
-- proxy_url: 获取代理Ip的链接；ip和proxy_url方式选择其一；
-- 每次请求获取一次，为节省ip资源建议使用自建的代理池。
-
-## 二、[数据列表](https://adata.1nchaos.com/dic/dataList.html)
-
-整理了最新版本的数据列表和相关使用Api，详细内容和相关使用参数，请参考数据字典文档。
-
-- [数据列表](https://adata.1nchaos.com/dic/dataList.html) 
-- [数据字典](https://adata.1nchaos.com/dic/stockInfo.html)
-
-### （1）股票-Stock
-
-#### 	1. 基本信息
-
-| 数据             | API                                   | 说明                                   | 备注                                                         |
-| ---------------- | ------------------------------------- | -------------------------------------- | ------------------------------------------------------------ |
-| A股代码          | stock.info.all_code()                 | 所有A股代码信息                        |                                                              |
-| **概念**         |                                       |                                        |                                                              |
-| 来源：同花顺     |                                       |                                        |                                                              |
-| 概念代码         | stock.info.all_concept_code_ths()     | 所有A股概念代码信息（同花顺）          | 来源：同花顺公开数据                                         |
-| 概念成分列表     | stock.info.concept_constituent_ths()  | 获取同花顺概念指数的成分股（同花顺）   | 注意：返回结果只有股票代码和股票简称，可根据概念名称查询     |
-| 股票所属概念     | stock.info.get_concept_ths()          | 获取单只股票所属的概念板块             | [F10](https://basic.10jqka.com.cn/300033/concept.html)       |
-| 来源：东方财富   |                                       |                                        |                                                              |
-| 概念代码         | stock.info.all_concept_code_east()    | 所有A股概念代码信息（东方财富）        | 来源：[东方财富](https://data.eastmoney.com/bkzj/gn.html)    |
-| 概念成分列表     | stock.info.concept_constituent_east() | 获取同花顺概念指数的成分股（东方财富） | 注意：返回结果只有股票代码和股票简称，可根据概念名称查询     |
-| 股票所属概念     | stock.info.get_concept_east()         | 获取单只股票所属的概念板块             | [核心题材](https://emweb.securities.eastmoney.com/pc_hsf10/pages/index.html?type=web&code=SZ300059&color=b#/hxtc) |
-| **指数**         |                                       |                                        |                                                              |
-| 指数代码         | stock.info.all_index_code()           | 获取所有A股市场的指数代码              | 来源同花顺，可能存在同花顺对代码重新编码的情况               |
-| 指数对应的成分股 | stock.info.index_constituent()        | 获取对应指数的成分股列表               |                                                              |
-| **其它**         |                                       |                                        |                                                              |
-| 股票交易日历     | stock.info.trade_calendar()           | 获取股票交易日信息                     | 来源：深交所                                                 |
-
-#### 	2. 行情信息
-
-
-| 数据                | API                                            | 说明                                  | 备注                                                         |
-| ------------------- | ---------------------------------------------- | ------------------------------------- | ------------------------------------------------------------ |
-| 分红信息            | stock.market.get_dividend()                    | 获取单只股票的分红信息                |                                                              |
-| 股票行情            | stock.market.get_market()                      | 获取单只股票的行情信息-日、周、月 k线 |                                                              |
-|                     | stock.market.get_market_min()                  | 获取单个股票的今日分时行情            | 只能获取当天                                                 |
-| <u>**实时行情**</u> | stock.market.list_market_current()             | 获取多个股票最新行情信息              | 实时行情<br />数据源：2个，新浪和腾讯                        |
-|                     | stock.market.get_market_five()                 | 获取单个股票的5档行情信息             | 实时行情<br />数据源：2个，腾讯和百度                        |
-|                     | stock.market.get_market_bar()                  | 获取单个股票的分笔成交行情            | 实时行情<br />[股市通](https://gushitong.baidu.com/stock/ab-872925) |
-| 概念行情-同花顺     | stock.market.get_market_concept_ths()          | 获取单个概念的行情信息-日、周、月 k线 | 获取同花顺概念行情时，<br />请注意传入参数是指数代码还是概念代码，<br />指数代码8开头，index_code |
-|                     | stock.market.get_market_concept_min_ths()      | 获取同花顺概念行情-当日分时           | 只能获取当天                                                 |
-|                     | stock.market.get_market_concept_current_ths()  | 获取同花顺当前的概念行情              | 实时行情                                                     |
-| 概念行情-东方财富   | stock.market.get_market_concept_east()         | 获取单个概念的行情信息-日、周、月 k线 | 获取东方财富概念行情时，<br />指数代码BK开头，index_code     |
-|                     | stock.market.get_market_concept_min_east()     | 获取同花顺概念行情-当日分时           | 只能获取当天                                                 |
-|                     | stock.market.get_market_concept_current_east() | 获取同花顺当前的概念行情              | 实时行情                                                     |
-| 指数行情            | stock.market.get_market_index()                | 获取指数的行情信息-日、周、月 k线     |                                                              |
-|                     | stock.market.get_market_index_min()            | 获取指数的行情-当日分时               |                                                              |
-|                     | stock.market.get_market_index_current()        | 获取当前的指数行情                    | 实时行情                                                     |
-
-**注：概念和指数从本质来看是一样的，所以相关的接口和返回结果是一致的，概念是各个厂商自定义的指数，指数是官方或者权威机构定义的，都是一揽子股票的组合。**
-
-### （2）基金-ETF
-
-| 数据           | API                                      | 说明                           | 备注                                                         |
-| -------------- | ---------------------------------------- | ------------------------------ | ------------------------------------------------------------ |
-| ETF（场内）    | fund.info.all_etf_exchange_traded_info() | 获取所有A股市场的ETF信息       | 来源：1. [东方财富](http://quote.eastmoney.com/center/gridlist.html#fund_etf) |
-| 其它数据排期中 | TODO                                     | 若您有相关资源可以一起参与贡献 |                                                              |
-
-### （3）债券-Bond
-
-| 数据           | API                          | 说明                                | 备注                                                   |
-| -------------- | ---------------------------- | ----------------------------------- | ------------------------------------------------------ |
-| 可转债代码     | bond.info.all_convert_code() | 获取所有A股市场的可转换债券代码信息 | 来源：1. [同花顺](http://data.10jqka.com.cn/ipo/bond/) |
-| 其它数据排期中 | TODO                         | 若您有相关资源可以一起参与贡献      |                                                        |
-
-### （4）舆情
-
-| 数据                     | API                                  | 说明                                       | 备注                                                         |
-| ------------------------ | ------------------------------------ | ------------------------------------------ | ------------------------------------------------------------ |
-| 最近一个月的股票解禁列表 | sentiment.stock_lifting_last_month() | 查询最近一个月的股票解禁列表               | 来源：1. [同花顺](http://data.10jqka.com.cn/market/xsjj/)    |
-| 全市场融资融券余额列表   | sentiment.securities_margin()        | 查询全市场融资融券余额列表                 | 来源：1. [东方财富](https://data.eastmoney.com/rzrq/)        |
-| **北向资金-行情**        |                                      |                                            |                                                              |
-|                          | sentiment.north.north_flow_current() | 获取北向资金（沪深港通）当前流入资金的行情 | 来源：1.[东方财富](https://data.eastmoney.com/hsgt/index.html) |
-|                          | sentiment.north.north_flow_min()     | 获取北向资金分时行情                       |                                                              |
-|                          | sentiment.north.north_flow()         | 获取北向资金历史流入行情                   |                                                              |
-| 其它数据排期中           | TODO                                 | 若您有相关资源可以一起参与贡献             |                                                              |
-
-## 三、[数据源](https://adata.1nchaos.com/dataSource.html)
-
-| 数据源     | 板块                                                         | 描述             |
-| ---------- | ------------------------------------------------------------ | ---------------- |
-| 同花顺     | [数据中心](http://data.10jqka.com.cn/)，[行情中心](http://q.10jqka.com.cn/)，[问财](http://www.iwencai.com/unifiedwap/home/index) | 让投资变的更简单 |
-| 百度股市通 | [股市通](https://gushitong.baidu.com/)                       | 科技让投资更简单 |
-| 东方财富   | [数据中心](https://data.eastmoney.com/center/)，[行情中心](http://quote.eastmoney.com/center/) | 财经门户         |
-| 腾讯理财   | [行情中心](https://stockapp.finance.qq.com/mstats/#)         |                  |
-| 新浪财经   | [新浪财经](https://finance.sina.com.cn/stock/)               | 门户网站         |
-
-***--------------------------------------------感谢各位大厂提供的数据----------------------------------------------***
-
-## 四、 其它参考
-
-主要记录查阅过的项目和相关平台，并对此项目产生了深远印象，特此鸣谢。
-
-| [akshare](https://gitee.com/mirrors/akshare) | [聚宽量化](https://www.joinquant.com/) | [baostock](http://baostock.com/baostock/index.php/Python%E5%BC%80%E5%8F%91%E8%B5%84%E6%BA%90) | [MyData](http://api.mairui.club/hsdata.html) |
-| -------------------------------------------- | -------------------------------------- | ------------------------------------------------------------ | -------------------------------------------- |
-
-## 五、发布计划
-
-|      | 版本号 | 内容 | 发布日期     | 备注                           |
-| ---- | ------ | ---- | ------------ | ------------------------------ |
-| ✅    | 0.x.x  | 股票 | 2023-04-05 ~ | 预览版本                       |
-| ✅ ️    | 1.x.x  | 股票 | 2023-10-01   | 中国Ai股                       |
-| ☑️    | 2.x.x  | 基金、债券 | 2024-01-01 | 场内可交易基金：ETF、可转债        |
-| ☑️    | 3.x.x | xxx        | 排期中       |  |
-
-## 六、理念
-
-1. 关于AData，我们只关注交易产生的数据。在A股只有交易数据是真实的，对于量化和AI训练，也只需要关心交易相关的行情数据，做到真正的专注。当然，你可能会说财务数据等也非常有用，但财务数据相对滞后，而且可能ZJ，甚至有XL可能，最终对于普通交易者可能就成了接盘侠。财务数据在我们这里，只做股票池筛选作用，不做实时交易指标推荐。
-
-2. 根据多年的数据治理经验，函数和字典在设计上面，符合标准的数据存储，可根据数据字典建表落地到数据库。
-
-3. 距离15年已过8年，时光匆匆，**抓住底部机会**。
-
-**注：**
-
-- 永久免费开源A股数据库，只有交易相关的数据，专注量化交易。
-- 送给A股的各位朋友一首歌：[谢天笑-向阳花](https://adata.1nchaos.com/向阳花.html)，愿你我向阳而生。
-
-## 参与贡献
-
-1.  Fork 本仓库
-2.  新建 Feat_xxx 分支
-3.  提交代码（注意代码风格和本项目一致即可）
-4.  新建 Pull Request
-
-
-## 特别鸣谢
-
-> 对于项目有支持，包括但不仅限：内容贡献，bug提交，思想交流等等，对项目有影响的个人和机构
-
-| Simon                                         | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https://github.com/LuneZ99) | 匿名用户 | thue | [Triones009](https://github.com/Triones009) |
-| --------------------------------------------- | ------------------------------------------------- | ------------------------------------- | -------- | ---- | ------------------------------------------- |
-| [LeslieWuboy](https://github.com/LeslieWuboy) |                                                   |                                       |          |      |                                             |
-
-----------------------------------------------------------------------
-
-> 
-## Star History
-
-[![Star History Chart](https://api.star-history.com/svg?repos=1nchaos/adata&type=Date)](https://star-history.com/#1nchaos/adata&Date)
+Metadata-Version: 2.1
+Name: adata
+Version: 2.0.0b0
+Summary: A Data,A Stock,ETF,Bond,Quant,Stock Market,K Line
+Home-page: https://github.com/1nchaos/adata
+Author: 1nchaos
+Author-email: 9527@1nchaos.com
+License: Apache License
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# [AData](https://adata.30006124.xyz)
+
+<p align="center">
+  <a href="https://adata.30006124.xyz/" target="_blank">
+    <img width="180" src="./docs/AData200x200.png" alt="logo">
+  </a>
+</p>
+
+![GitHub language count](https://img.shields.io/github/languages/count/1nchaos/adata)![GitHub top language](https://img.shields.io/github/languages/top/1nchaos/adata)[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/adata?color=d)](https://pypi.org/project/adata/)[![Licence](https://img.shields.io/hexpm/l/apa?color=d)](https://gitee.com/inchaos/adata/blob/main/LICENSE)[![Downloads](https://static.pepy.tech/badge/adata/week)](https://pepy.tech/project/adata)![GitHub Repo stars](https://img.shields.io/github/stars/1nchaos/adata)![GitHub issues](https://img.shields.io/github/issues/1nchaos/adata)![GitHub contributors](https://img.shields.io/github/contributors/1nchaos/adata)![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/1nchaos/adata)[![Downloads](https://static.pepy.tech/badge/adata)](https://pepy.tech/project/adata)![PyPI - Version](https://img.shields.io/pypi/v/adata)
+
+
+
+## 0、[介绍](https://adata.30006124.xyz/idea.html)
+> 专注A股，专注量化，向阳而生；开放、纯净、持续、为Ai(爱)发电。
+>
+> 专注股票行情数据，为了保证数据的高可用性，采用多数据源融合切换。
+>
+> 目标：支持个人量化行情的需要；众人拾柴火焰高，欢迎加入。
+
+**市场寒冷，发热不易，坚持更难；如有帮助到你，右上角点 ⭐Star 一键三连，谢谢支持和收藏^_^**
+
+## 一、[快速开始](https://adata.30006124.xyz/quickStart.html)
+
+### （1）安装sdk
+
+~~~python
+# 首次安装
+pip install adata
+# 指定镜像源
+pip install adata -i http://mirrors.aliyun.com/pypi/simple/
+
+# 升级版本
+pip install -U adata
+# 指定镜像源
+pip install -U adata -i http://mirrors.aliyun.com/pypi/simple/
+~~~
+
+**注：国内镜像可能存在同步延迟，可使用官方镜像源，以下是镜像源**
+
+阿里云【推荐】：http://mirrors.aliyun.com/pypi/simple/  
+
+清华大学：https://pypi.tuna.tsinghua.edu.cn/simple  
+
+官方镜像源：https://pypi.org/simple
+
+### （2）使用示例
+
+#### 1. 获取股票代码
+
+获取所有的股票代码
+
+~~~python
+import adata
+
+res_df = adata.stock.info.all_code()
+print(res_df)
+~~~
+
+示例结果：
+
+~~~python
+  stock_code short_name exchange
+0        001324       N长青科       SZ
+1        301361       众智科技       SZ
+2        300514        友讯达       SZ
+...         ...        ...      ...
+5490     300367        网力退       SZ
+5491     300372        欣泰退       SZ
+5492     300431        暴风退       SZ
+
+[5493 rows x 3 columns]
+~~~
+
+#### 2. 获取股票的行情
+
+获取到股票代码后，传入对应的stock_code参数，查询对应股票的行情信息。
+
+```python
+import adata
+
+# k_type: k线类型：1.日；2.周；3.月 默认：1 日k
+res_df = adata.stock.market.get_market(stock_code='000001', k_type=1, start_date='2021-01-01')
+print(res_df)
+```
+
+示例结果：
+
+~~~python
+            trade_time   open  close  ... pre_close stock_code  trade_date
+0    2021-01-04 00:00:00  18.69  18.19  ...     18.93     000001  2021-01-04
+1    2021-01-05 00:00:00  17.99  17.76  ...     18.19     000001  2021-01-05
+2    2021-01-06 00:00:00  17.67  19.15  ...     17.76     000001  2021-01-06
+..                   ...    ...    ...  ...       ...        ...         ...
+573  2023-05-18 00:00:00  12.57  12.49  ...     12.49     000001  2023-05-18
+574  2023-05-19 00:00:00  12.43  12.34  ...     12.49     000001  2023-05-19
+575  2023-05-22 00:00:00  12.31  12.38  ...     12.34     000001  2023-05-22
+
+[576 rows :x 13 columns]
+~~~
+
+#### 3. 其它数据使用
+
+请参考下面数据列表和相关字典文档，找到对应的函数并查看对应的函数注释，进行正确使用。
+
+- [数据字典](https://adata.30006124.xyz/dic/stockInfo.html) 
+
+####  4. 代理设置
+
+项目是基于公开接口，可能存在限制等，因此增加代理设置功能
+
+~~~
+import adata
+
+# 设置代理,代理是全局设置,代理失效后可重新设置。参数:ip,proxy_url
+adata.proxy(is_proxy=True, ip='60.167.21.27:1133')
+res_df = adata.stock.info.all_code()
+print(res_df)
+~~~
+
+**注：**
+
+- proxy_url: 获取代理Ip的链接；ip和proxy_url方式选择其一；
+- 每次请求获取一次，为节省ip资源建议使用自建的代理池。
+
+## 二、[数据列表](https://adata.30006124.xyz/dic/dataList.html)
+
+整理了最新版本的数据列表和相关使用Api，详细内容和相关使用参数，请参考数据字典文档。
+
+- [数据列表](https://adata.30006124.xyz/dic/dataList.html) 
+- [数据字典](https://adata.30006124.xyz/dic/stockInfo.html)
+
+### （1）股票-Stock
+
+#### 	1. 基本信息
+
+| 数据             | API                                   | 说明                                   | 备注                                                         |
+| ---------------- | ------------------------------------- | -------------------------------------- | ------------------------------------------------------------ |
+| A股代码          | stock.info.all_code()                 | 所有A股代码信息                        |                                                              |
+| **概念**         |                                       |                                        |                                                              |
+| 来源：同花顺     |                                       |                                        |                                                              |
+| 概念代码         | stock.info.all_concept_code_ths()     | 所有A股概念代码信息（同花顺）          | 来源：同花顺公开数据                                         |
+| 概念成分列表     | stock.info.concept_constituent_ths()  | 获取同花顺概念指数的成分股（同花顺）   | 注意：返回结果只有股票代码和股票简称，可根据概念名称查询     |
+| 股票所属概念     | stock.info.get_concept_ths()          | 获取单只股票所属的概念板块             | [F10](https://basic.10jqka.com.cn/300033/concept.html)       |
+| 来源：东方财富   |                                       |                                        |                                                              |
+| 概念代码         | stock.info.all_concept_code_east()    | 所有A股概念代码信息（东方财富）        | 来源：[东方财富](https://data.eastmoney.com/bkzj/gn.html)    |
+| 概念成分列表     | stock.info.concept_constituent_east() | 获取同花顺概念指数的成分股（东方财富） | 注意：返回结果只有股票代码和股票简称，可根据概念名称查询     |
+| 股票所属概念     | stock.info.get_concept_east()         | 获取单只股票所属的概念板块             | [核心题材](https://emweb.securities.eastmoney.com/pc_hsf10/pages/index.html?type=web&code=SZ300059&color=b#/hxtc) |
+| **指数**         |                                       |                                        |                                                              |
+| 指数代码         | stock.info.all_index_code()           | 获取所有A股市场的指数代码              | 来源同花顺，可能存在同花顺对代码重新编码的情况               |
+| 指数对应的成分股 | stock.info.index_constituent()        | 获取对应指数的成分股列表               |                                                              |
+| **其它**         |                                       |                                        |                                                              |
+| 股票交易日历     | stock.info.trade_calendar()           | 获取股票交易日信息                     | 来源：深交所                                                 |
+
+#### 	2. 行情信息
+
+
+| 数据                | API                                            | 说明                                  | 备注                                                         |
+| ------------------- | ---------------------------------------------- | ------------------------------------- | ------------------------------------------------------------ |
+| 分红信息            | stock.market.get_dividend()                    | 获取单只股票的分红信息                |                                                              |
+| 股票行情            | stock.market.get_market()                      | 获取单只股票的行情信息-日、周、月 k线 |                                                              |
+|                     | stock.market.get_market_min()                  | 获取单个股票的今日分时行情            | 只能获取当天                                                 |
+| <u>**实时行情**</u> | stock.market.list_market_current()             | 获取多个股票最新行情信息              | 实时行情<br />数据源：2个，新浪和腾讯                        |
+|                     | stock.market.get_market_five()                 | 获取单个股票的5档行情信息             | 实时行情<br />数据源：2个，腾讯和百度                        |
+|                     | stock.market.get_market_bar()                  | 获取单个股票的分笔成交行情            | 实时行情<br />[股市通](https://gushitong.baidu.com/stock/ab-872925) |
+| 概念行情-同花顺     | stock.market.get_market_concept_ths()          | 获取单个概念的行情信息-日、周、月 k线 | 获取同花顺概念行情时，<br />请注意传入参数是指数代码还是概念代码，<br />指数代码8开头，index_code |
+|                     | stock.market.get_market_concept_min_ths()      | 获取同花顺概念行情-当日分时           | 只能获取当天                                                 |
+|                     | stock.market.get_market_concept_current_ths()  | 获取同花顺当前的概念行情              | 实时行情                                                     |
+| 概念行情-东方财富   | stock.market.get_market_concept_east()         | 获取单个概念的行情信息-日、周、月 k线 | 获取东方财富概念行情时，<br />指数代码BK开头，index_code     |
+|                     | stock.market.get_market_concept_min_east()     | 获取同花顺概念行情-当日分时           | 只能获取当天                                                 |
+|                     | stock.market.get_market_concept_current_east() | 获取同花顺当前的概念行情              | 实时行情                                                     |
+| 指数行情            | stock.market.get_market_index()                | 获取指数的行情信息-日、周、月 k线     |                                                              |
+|                     | stock.market.get_market_index_min()            | 获取指数的行情-当日分时               |                                                              |
+|                     | stock.market.get_market_index_current()        | 获取当前的指数行情                    | 实时行情                                                     |
+
+**注：概念和指数从本质来看是一样的，所以相关的接口和返回结果是一致的，概念是各个厂商自定义的指数，指数是官方或者权威机构定义的，都是一揽子股票的组合。**
+
+### （2）基金-ETF
+
+#### 1. 基本信息
+
+| 数据        | API                                      | 说明                     | 备注                                                         |
+| ----------- | ---------------------------------------- | ------------------------ | ------------------------------------------------------------ |
+| ETF（场内） | fund.info.all_etf_exchange_traded_info() | 获取所有A股市场的ETF信息 | 来源：1. [东方财富](http://quote.eastmoney.com/center/gridlist.html#fund_etf) |
+
+#### 2. 行情信息
+
+| 数据    | API                                  | 说明                             | 备注                                     |
+| ------- | ------------------------------------ | -------------------------------- | ---------------------------------------- |
+| ETF行情 | fund.market.get_market_etf()         | 获取ETF的行情信息-日、周、月 k线 | 来源：[同花顺](https://m.10jqka.com.cn/) |
+|         | fund.market.get_market_etf_min()     | 获取ETF的行情-当日分时           |                                          |
+|         | fund.market.get_market_etf_current() | 获取当前的ETF行情                | 实时行情                                 |
+
+### （3）债券-Bond
+
+| 数据           | API                          | 说明                                | 备注                                                   |
+| -------------- | ---------------------------- | ----------------------------------- | ------------------------------------------------------ |
+| 可转债代码     | bond.info.all_convert_code() | 获取所有A股市场的可转换债券代码信息 | 来源：1. [同花顺](http://data.10jqka.com.cn/ipo/bond/) |
+| 其它数据排期中 | TODO                         | 若您有相关资源可以一起参与贡献      |                                                        |
+
+### （4）舆情
+
+| 数据                     | API                                  | 说明                                       | 备注                                                         |
+| ------------------------ | ------------------------------------ | ------------------------------------------ | ------------------------------------------------------------ |
+| 最近一个月的股票解禁列表 | sentiment.stock_lifting_last_month() | 查询最近一个月的股票解禁列表               | 来源：1. [同花顺](http://data.10jqka.com.cn/market/xsjj/)    |
+| 全市场融资融券余额列表   | sentiment.securities_margin()        | 查询全市场融资融券余额列表                 | 来源：1. [东方财富](https://data.eastmoney.com/rzrq/)        |
+| **北向资金-行情**        |                                      |                                            |                                                              |
+|                          | sentiment.north.north_flow_current() | 获取北向资金（沪深港通）当前流入资金的行情 | 来源：1.[东方财富](https://data.eastmoney.com/hsgt/index.html) |
+|                          | sentiment.north.north_flow_min()     | 获取北向资金分时行情                       |                                                              |
+|                          | sentiment.north.north_flow()         | 获取北向资金历史流入行情                   |                                                              |
+| 其它数据排期中           | TODO                                 | 若您有相关资源可以一起参与贡献             |                                                              |
+
+## 三、[数据源](https://adata.30006124.xyz/dataSource.html)
+
+| 数据源     | 板块                                                         | 描述             |
+| ---------- | ------------------------------------------------------------ | ---------------- |
+| 同花顺     | [数据中心](http://data.10jqka.com.cn/)，[行情中心](http://q.10jqka.com.cn/)，[问财](http://www.iwencai.com/unifiedwap/home/index) | 让投资变的更简单 |
+| 百度股市通 | [股市通](https://gushitong.baidu.com/)                       | 科技让投资更简单 |
+| 东方财富   | [数据中心](https://data.eastmoney.com/center/)，[行情中心](http://quote.eastmoney.com/center/) | 财经门户         |
+| 腾讯理财   | [行情中心](https://stockapp.finance.qq.com/mstats/#)         |                  |
+| 新浪财经   | [新浪财经](https://finance.sina.com.cn/stock/)               | 门户网站         |
+
+***--------------------------------------------感谢各位大厂提供的数据----------------------------------------------***
+
+## 四、 其它参考
+
+主要记录查阅过的项目和相关平台，并对此项目产生了深远印象，特此鸣谢。
+
+| [akshare](https://gitee.com/mirrors/akshare) | [聚宽量化](https://www.joinquant.com/) | [baostock](http://baostock.com/baostock/index.php/Python%E5%BC%80%E5%8F%91%E8%B5%84%E6%BA%90) | [MyData](http://api.mairui.club/hsdata.html) |
+| -------------------------------------------- | -------------------------------------- | ------------------------------------------------------------ | -------------------------------------------- |
+
+## 五、发布计划
+
+|      | 版本号 | 内容 | 发布日期     | 备注                           |
+| ---- | ------ | ---- | ------------ | ------------------------------ |
+| ✅    | 0.x.x  | 股票 | 2023-04-05 ~ | 预览版本                       |
+| ✅ ️    | 1.x.x  | 股票 | 2023-10-01   | 中国Ai股                       |
+| ☑️    | 2.x.x  | 基金、债券 | 开发中 | 场内可交易基金：ETF、可转债        |
+| ☑️    | 3.x.x | xxx        | 排期中       |  |
+
+## 六、理念
+
+1. 关于AData，我们只关注交易产生的数据。在A股只有交易数据是真实的，对于量化和AI训练，也只需要关心交易相关的行情数据，做到真正的专注。当然，你可能会说财务数据等也非常有用，但财务数据相对滞后，而且可能ZJ，甚至有XL可能，最终对于普通交易者可能就成了接盘侠。财务数据在我们这里，只做股票池筛选作用，不做实时交易指标推荐。
+
+2. 根据多年的数据治理经验，函数和字典在设计上面，符合标准的数据存储，可根据数据字典建表落地到数据库。
+
+3. 距离15年已过8年，时光匆匆，**抓住底部机会**。
+
+**注：**
+
+- 永久免费开源A股数据库，只有交易相关的数据，专注量化交易。
+- 送给A股的各位朋友一首歌：[谢天笑-向阳花](https://adata.30006124.xyz/向阳花.html)，愿你我向阳而生。
+
+## 参与贡献
+
+1.  Fork 本仓库
+2.  新建 Feat_xxx 分支
+3.  提交代码（注意代码风格和本项目一致即可）
+4.  新建 Pull Request
+
+
+## 特别鸣谢
+
+> 对于项目有支持，包括但不仅限：内容贡献，bug提交，思想交流等等，对项目有影响的个人和机构
+
+| Simon | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https://github.com/LuneZ99) | 匿名用户 | thue | [Triones009](https://github.com/Triones009) | **[adaaaaaa](https://github.com/adaaaaaa)** | **[LeslieWuboy](https://github.com/LeslieWuboy)** |
+| ----- | ------------------------------------------------- | ------------------------------------- | -------- | ---- | ------------------------------------------- | ------------------------------------------- | ------------------------------------------------- |
+|       |                                                   |                                       |          |      |                                             |                                             |                                                   |
+
+----------------------------------------------------------------------
+
+> 
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=1nchaos/adata&type=Date)](https://star-history.com/#1nchaos/adata&Date)
+
+## 欢迎进行交流
+<p align="center">
+  <a href="https://adata.30006124.xyz/" target="_blank">
+    <img width="180" src="./docs/wx.jpg" alt="logo">
+  </a>
+</p>
+
+- 添加wx好友，备注：Adata量化进交流群；
+- 群最近建立，意在提供一个交流的平台，欢迎讨论交流；
+- 一起保卫3000点直到突破6124点。
```

#### html2text {}

```diff
@@ -1,42 +1,40 @@
-Metadata-Version: 2.1 Name: adata Version: 1.2.4 Summary: A Data,A
+Metadata-Version: 2.1 Name: adata Version: 2.0.0b0 Summary: A Data,A
 Stock,ETF,Bond,Quant,Stock Market,K Line Home-page: https://github.com/1nchaos/
 adata Author: 1nchaos Author-email: 9527@1nchaos.com License: Apache License
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: requests>=2.16.0 Requires-Dist: pandas>=0.22.0
-Requires-Dist: beautifulsoup4>=4.0.2 Requires-Dist: py_mini_racer>=0.6.0 #
-[AData](https://adata.1nchaos.com)
+File: LICENSE # [AData](https://adata.30006124.xyz)
                                     _[_l_o_g_o_]
 ![GitHub language count](https://img.shields.io/github/languages/count/1nchaos/
 adata)![GitHub top language](https://img.shields.io/github/languages/top/
 1nchaos/adata)[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 adata?color=d)](https://pypi.org/project/adata/)[![Licence](https://
 img.shields.io/hexpm/l/apa?color=d)](https://gitee.com/inchaos/adata/blob/main/
 LICENSE)[![Downloads](https://static.pepy.tech/badge/adata/week)](https://
 pepy.tech/project/adata)![GitHub Repo stars](https://img.shields.io/github/
 stars/1nchaos/adata)![GitHub issues](https://img.shields.io/github/issues/
 1nchaos/adata)![GitHub contributors](https://img.shields.io/github/
 contributors/1nchaos/adata)![GitHub (Pre-)Release Date](https://img.shields.io/
 github/release-date-pre/1nchaos/adata)[![Downloads](https://static.pepy.tech/
 badge/adata)](https://pepy.tech/project/adata)![PyPI - Version](https://
-img.shields.io/pypi/v/adata) ## 0ã[ä»ç»](https://adata.1nchaos.com/
+img.shields.io/pypi/v/adata) ## 0ã[ä»ç»](https://adata.30006124.xyz/
 idea.html) >
 ä¸æ³¨Aè¡ï¼ä¸æ³¨éåï¼åé³èçï¼å¼æ¾ãçº¯åãæç»­ãä¸ºAi
 (ç±)åçµã > >
 ä¸æ³¨è¡ç¥¨è¡ææ°æ®ï¼ä¸ºäºä¿è¯æ°æ®çé«å¯ç¨æ§ï¼éç¨å¤æ°æ®æºèååæ¢ã
 > >
 ç®æ ï¼æ¯æä¸ªäººéåè¡æçéè¦ï¼ä¼äººæ¾æ´ç«ç°é«ï¼æ¬¢è¿å å¥ã
 **å¸åºå¯å·ï¼åç­ä¸æï¼åææ´é¾ï¼å¦æå¸®å©å°ä½ ï¼å³ä¸è§ç¹
 â­Star ä¸é®ä¸è¿ï¼è°¢è°¢æ¯æåæ¶è^_^** ## ä¸ã[å¿«éå¼å§]
-(https://adata.1nchaos.com/quickStart.html) ### ï¼1ï¼å®è£sdk ~~~python #
+(https://adata.30006124.xyz/quickStart.html) ### ï¼1ï¼å®è£sdk ~~~python #
 é¦æ¬¡å®è£ pip install adata # æå®éåæº pip install adata -i http://
 mirrors.aliyun.com/pypi/simple/ # åçº§çæ¬ pip install -U adata #
 æå®éåæº pip install -U adata -i http://mirrors.aliyun.com/pypi/simple/
 ~~~
 **æ³¨ï¼å½åéåå¯è½å­å¨åæ­¥å»¶è¿ï¼å¯ä½¿ç¨å®æ¹éåæºï¼ä»¥ä¸æ¯éåæº**
 é¿éäºãæ¨èãï¼http://mirrors.aliyun.com/pypi/simple/
 æ¸åå¤§å­¦ï¼https://pypi.tuna.tsinghua.edu.cn/simple
@@ -55,28 +53,27 @@
 18.19 ... 18.93 000001 2021-01-04 1 2021-01-05 00:00:00 17.99 17.76 ... 18.19
 000001 2021-01-05 2 2021-01-06 00:00:00 17.67 19.15 ... 17.76 000001 2021-01-06
 .. ... ... ... ... ... ... ... 573 2023-05-18 00:00:00 12.57 12.49 ... 12.49
 000001 2023-05-18 574 2023-05-19 00:00:00 12.43 12.34 ... 12.49 000001 2023-05-
 19 575 2023-05-22 00:00:00 12.31 12.38 ... 12.34 000001 2023-05-22 [576 rows :
 x 13 columns] ~~~ #### 3. å¶å®æ°æ®ä½¿ç¨
 è¯·åèä¸é¢æ°æ®åè¡¨åç¸å³å­å¸ææ¡£ï¼æ¾å°å¯¹åºçå½æ°å¹¶æ¥çå¯¹åºçå½æ°æ³¨éï¼è¿è¡æ­£ç¡®ä½¿ç¨ã
-- [æ°æ®å­å¸](https://adata.1nchaos.com/dic/stockInfo.html) #### 4.
+- [æ°æ®å­å¸](https://adata.30006124.xyz/dic/stockInfo.html) #### 4.
 ä»£çè®¾ç½®
 é¡¹ç®æ¯åºäºå¬å¼æ¥å£ï¼å¯è½å­å¨éå¶ç­ï¼å æ­¤å¢å ä»£çè®¾ç½®åè½
 ~~~ import adata #
 è®¾ç½®ä»£ç,ä»£çæ¯å¨å±è®¾ç½®,ä»£çå¤±æåå¯éæ°è®¾ç½®ãåæ°:
 ip,proxy_url adata.proxy(is_proxy=True, ip='60.167.21.27:1133') res_df =
-adata.stock.info.all_code() print(res_df) ~~~ **æ³¨ï¼** - v0.0.027b0
-åä»¥ä¸çæ¬æ¯æï¼ - proxy_url:
+adata.stock.info.all_code() print(res_df) ~~~ **æ³¨ï¼** - proxy_url:
 è·åä»£çIpçé¾æ¥ï¼ipåproxy_urlæ¹å¼éæ©å¶ä¸ï¼ -
 æ¯æ¬¡è¯·æ±è·åä¸æ¬¡ï¼ä¸ºèçipèµæºå»ºè®®ä½¿ç¨èªå»ºçä»£çæ± ã
-## äºã[æ°æ®åè¡¨](https://adata.1nchaos.com/dic/dataList.html)
+## äºã[æ°æ®åè¡¨](https://adata.30006124.xyz/dic/dataList.html)
 æ´çäºææ°çæ¬çæ°æ®åè¡¨åç¸å³ä½¿ç¨Apiï¼è¯¦ç»åå®¹åç¸å³ä½¿ç¨åæ°ï¼è¯·åèæ°æ®å­å¸ææ¡£ã
-- [æ°æ®åè¡¨](https://adata.1nchaos.com/dic/dataList.html) - [æ°æ®å­å¸]
-(https://adata.1nchaos.com/dic/stockInfo.html) ### ï¼1ï¼è¡ç¥¨-Stock #### 1.
+- [æ°æ®åè¡¨](https://adata.30006124.xyz/dic/dataList.html) - [æ°æ®å­å¸]
+(https://adata.30006124.xyz/dic/stockInfo.html) ### ï¼1ï¼è¡ç¥¨-Stock #### 1.
 åºæ¬ä¿¡æ¯ | æ°æ® | API | è¯´æ | å¤æ³¨ | | ---------------- | ----------
 --------------------------- | -------------------------------------- | --------
 ---------------------------------------------------- | | Aè¡ä»£ç  |
 stock.info.all_code() | ææAè¡ä»£ç ä¿¡æ¯ | | | **æ¦å¿µ** | | | | |
 æ¥æºï¼åè±é¡º | | | | | æ¦å¿µä»£ç  | stock.info.all_concept_code_ths() |
 ææAè¡æ¦å¿µä»£ç ä¿¡æ¯ï¼åè±é¡ºï¼ | æ¥æºï¼åè±é¡ºå¬å¼æ°æ® |
 | æ¦å¿µæååè¡¨ | stock.info.concept_constituent_ths() |
@@ -132,24 +129,30 @@
 stock.market.get_market_concept_current_east() |
 è·ååè±é¡ºå½åçæ¦å¿µè¡æ | å®æ¶è¡æ | | ææ°è¡æ |
 stock.market.get_market_index() | è·åææ°çè¡æä¿¡æ¯-æ¥ãå¨ãæ
 kçº¿ | | | | stock.market.get_market_index_min() | è·åææ°çè¡æ-
 å½æ¥åæ¶ | | | | stock.market.get_market_index_current() |
 è·åå½åçææ°è¡æ | å®æ¶è¡æ |
 **æ³¨ï¼æ¦å¿µåææ°ä»æ¬è´¨æ¥çæ¯ä¸æ ·çï¼æä»¥ç¸å³çæ¥å£åè¿åç»ææ¯ä¸è´çï¼æ¦å¿µæ¯åä¸ªååèªå®ä¹çææ°ï¼ææ°æ¯å®æ¹æèæå¨æºæå®ä¹çï¼é½æ¯ä¸æ½å­è¡ç¥¨çç»åã**
-### ï¼2ï¼åºé-ETF | æ°æ® | API | è¯´æ | å¤æ³¨ | | -------------- | ---
-------------------------------------- | ------------------------------ | ------
------------------------------------------------------- | | ETFï¼åºåï¼ |
-fund.info.all_etf_exchange_traded_info() | è·åææAè¡å¸åºçETFä¿¡æ¯ |
-æ¥æºï¼1. [ä¸æ¹è´¢å¯](http://quote.eastmoney.com/center/
-gridlist.html#fund_etf) | | å¶å®æ°æ®ææä¸­ | TODO |
-è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® | | ### ï¼3ï¼åºå¸-Bond |
-æ°æ® | API | è¯´æ | å¤æ³¨ | | -------------- | ---------------------------
-- | ----------------------------------- | -------------------------------------
------------------ | | å¯è½¬åºä»£ç  | bond.info.all_convert_code() |
+### ï¼2ï¼åºé-ETF #### 1. åºæ¬ä¿¡æ¯ | æ°æ® | API | è¯´æ | å¤æ³¨ | |
+----------- | ---------------------------------------- | ----------------------
+-- | ------------------------------------------------------------ | |
+ETFï¼åºåï¼ | fund.info.all_etf_exchange_traded_info() |
+è·åææAè¡å¸åºçETFä¿¡æ¯ | æ¥æºï¼1. [ä¸æ¹è´¢å¯](http://
+quote.eastmoney.com/center/gridlist.html#fund_etf) | #### 2. è¡æä¿¡æ¯ |
+æ°æ® | API | è¯´æ | å¤æ³¨ | | ------- | ----------------------------------
+-- | -------------------------------- | ---------------------------------------
+- | | ETFè¡æ | fund.market.get_market_etf() | è·åETFçè¡æä¿¡æ¯-
+æ¥ãå¨ãæ kçº¿ | æ¥æºï¼[åè±é¡º](https://m.10jqka.com.cn/) | | |
+fund.market.get_market_etf_min() | è·åETFçè¡æ-å½æ¥åæ¶ | | | |
+fund.market.get_market_etf_current() | è·åå½åçETFè¡æ | å®æ¶è¡æ
+| ### ï¼3ï¼åºå¸-Bond | æ°æ® | API | è¯´æ | å¤æ³¨ | | -------------- |
+---------------------------- | ----------------------------------- | ----------
+-------------------------------------------- | | å¯è½¬åºä»£ç  |
+bond.info.all_convert_code() |
 è·åææAè¡å¸åºçå¯è½¬æ¢åºå¸ä»£ç ä¿¡æ¯ | æ¥æºï¼1. [åè±é¡º]
 (http://data.10jqka.com.cn/ipo/bond/) | | å¶å®æ°æ®ææä¸­ | TODO |
 è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® | | ### ï¼4ï¼èæ | æ°æ® |
 API | è¯´æ | å¤æ³¨ | | ------------------------ | --------------------------
 ---------- | ------------------------------------------ | ---------------------
 --------------------------------------- | |
 æè¿ä¸ä¸ªæçè¡ç¥¨è§£ç¦åè¡¨ | sentiment.stock_lifting_last_month() |
@@ -159,17 +162,17 @@
 æ¥æºï¼1. [ä¸æ¹è´¢å¯](https://data.eastmoney.com/rzrq/) | |
 **ååèµé-è¡æ** | | | | | | sentiment.north.north_flow_current() |
 è·åååèµéï¼æ²ªæ·±æ¸¯éï¼å½åæµå¥èµéçè¡æ | æ¥æºï¼1.
 [ä¸æ¹è´¢å¯](https://data.eastmoney.com/hsgt/index.html) | | |
 sentiment.north.north_flow_min() | è·åååèµéåæ¶è¡æ | | | |
 sentiment.north.north_flow() | è·åååèµéåå²æµå¥è¡æ | | |
 å¶å®æ°æ®ææä¸­ | TODO | è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® |
-| ## ä¸ã[æ°æ®æº](https://adata.1nchaos.com/dataSource.html) | æ°æ®æº |
-æ¿å | æè¿° | | ---------- | ----------------------------------------------
--------------- | ---------------- | | åè±é¡º | [æ°æ®ä¸­å¿](http://
+| ## ä¸ã[æ°æ®æº](https://adata.30006124.xyz/dataSource.html) | æ°æ®æº
+| æ¿å | æè¿° | | ---------- | --------------------------------------------
+---------------- | ---------------- | | åè±é¡º | [æ°æ®ä¸­å¿](http://
 data.10jqka.com.cn/)ï¼[è¡æä¸­å¿](http://q.10jqka.com.cn/)ï¼[é®è´¢](http:
 //www.iwencai.com/unifiedwap/home/index) | è®©æèµåçæ´ç®å | |
 ç¾åº¦è¡å¸é | [è¡å¸é](https://gushitong.baidu.com/) |
 ç§æè®©æèµæ´ç®å | | ä¸æ¹è´¢å¯ | [æ°æ®ä¸­å¿](https://
 data.eastmoney.com/center/)ï¼[è¡æä¸­å¿](http://quote.eastmoney.com/center/
 ) | è´¢ç»é¨æ· | | è¾è®¯çè´¢ | [è¡æä¸­å¿](https://
 stockapp.finance.qq.com/mstats/#) | | | æ°æµªè´¢ç» | [æ°æµªè´¢ç»](https://
@@ -182,31 +185,37 @@
 Python%E5%BC%80%E5%8F%91%E8%B5%84%E6%BA%90) | [MyData](http://api.mairui.club/
 hsdata.html) | | -------------------------------------------- | ---------------
 ----------------------- | -----------------------------------------------------
 ------- | -------------------------------------------- | ## äºãåå¸è®¡å
 | | çæ¬å· | åå®¹ | åå¸æ¥æ | å¤æ³¨ | | ---- | ------ | ---- | -----
 ------- | ------------------------------ | | â | 0.x.x | è¡ç¥¨ | 2023-04-05
 ~ | é¢è§çæ¬ | | â ï¸ | 1.x.x | è¡ç¥¨ | 2023-10-01 | ä¸­å½Aiè¡ | |
-âï¸ | 2.x.x | åºéãåºå¸ | 2024-01-01 |
+âï¸ | 2.x.x | åºéãåºå¸ | å¼åä¸­ |
 åºåå¯äº¤æåºéï¼ETFãå¯è½¬åº | | âï¸ | 3.x.x | xxx | ææä¸­ |
 | ## å­ãçå¿µ 1.
 å³äºADataï¼æä»¬åªå³æ³¨äº¤æäº§ççæ°æ®ãå¨Aè¡åªæäº¤ææ°æ®æ¯çå®çï¼å¯¹äºéååAIè®­ç»ï¼ä¹åªéè¦å³å¿äº¤æç¸å³çè¡ææ°æ®ï¼åå°çæ­£çä¸æ³¨ãå½ç¶ï¼ä½ å¯è½ä¼è¯´è´¢å¡æ°æ®ç­ä¹éå¸¸æç¨ï¼ä½è´¢å¡æ°æ®ç¸å¯¹æ»åï¼èä¸å¯è½ZJï¼çè³æXLå¯è½ï¼æç»å¯¹äºæ®éäº¤æèå¯è½å°±æäºæ¥çä¾ ãè´¢å¡æ°æ®å¨æä»¬è¿éï¼åªåè¡ç¥¨æ± ç­éä½ç¨ï¼ä¸åå®æ¶äº¤æææ æ¨èã
 2.
 æ ¹æ®å¤å¹´çæ°æ®æ²»çç»éªï¼å½æ°åå­å¸å¨è®¾è®¡ä¸é¢ï¼ç¬¦åæ åçæ°æ®å­å¨ï¼å¯æ ¹æ®æ°æ®å­å¸å»ºè¡¨è½å°å°æ°æ®åºã
 3. è·ç¦»15å¹´å·²è¿8å¹´ï¼æ¶åååï¼**æä½åºé¨æºä¼**ã **æ³¨ï¼**
 -
 æ°¸ä¹åè´¹å¼æºAè¡æ°æ®åºï¼åªæäº¤æç¸å³çæ°æ®ï¼ä¸æ³¨éåäº¤æã
 - éç»Aè¡çåä½æåä¸é¦æ­ï¼[è°¢å¤©ç¬-åé³è±](https://
-adata.1nchaos.com/åé³è±.html)ï¼æ¿ä½ æåé³èçã ## åä¸è´¡ç® 1.
-Fork æ¬ä»åº 2. æ°å»º Feat_xxx åæ¯ 3.
+adata.30006124.xyz/åé³è±.html)ï¼æ¿ä½ æåé³èçã ## åä¸è´¡ç®
+1. Fork æ¬ä»åº 2. æ°å»º Feat_xxx åæ¯ 3.
 æäº¤ä»£ç ï¼æ³¨æä»£ç é£æ ¼åæ¬é¡¹ç®ä¸è´å³å¯ï¼ 4. æ°å»º Pull
 Request ## ç¹å«é¸£è°¢ >
 å¯¹äºé¡¹ç®ææ¯æï¼åæ¬ä½ä¸ä»éï¼åå®¹è´¡ç®ï¼bugæäº¤ï¼ææ³äº¤æµç­ç­ï¼å¯¹é¡¹ç®æå½±åçä¸ªäººåæºæ
 | Simon | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https:/
 /github.com/LuneZ99) | å¿åç¨æ· | thue | [Triones009](https://github.com/
-Triones009) | | --------------------------------------------- | ---------------
----------------------------------- | ------------------------------------- | --
------- | ---- | ------------------------------------------- | | [LeslieWuboy]
-(https://github.com/LeslieWuboy) | | | | | | ----------------------------------
------------------------------------- > ## Star History [![Star History Chart]
-(https://api.star-history.com/svg?repos=1nchaos/adata&type=Date)](https://star-
-history.com/#1nchaos/adata&Date)
+Triones009) | **[adaaaaaa](https://github.com/adaaaaaa)** | **[LeslieWuboy]
+(https://github.com/LeslieWuboy)** | | ----- | --------------------------------
+----------------- | ------------------------------------- | -------- | ---- | -
+------------------------------------------ | ----------------------------------
+--------- | ------------------------------------------------- | | | | | | | | |
+| ---------------------------------------------------------------------- > ##
+Star History [![Star History Chart](https://api.star-history.com/
+svg?repos=1nchaos/adata&type=Date)](https://star-history.com/#1nchaos/
+adata&Date) ## æ¬¢è¿è¿è¡äº¤æµ
+                                    _[_l_o_g_o_]
+- æ·»å wxå¥½åï¼å¤æ³¨ï¼Adataéåè¿äº¤æµç¾¤ï¼ -
+ç¾¤æè¿å»ºç«ï¼æå¨æä¾ä¸ä¸ªäº¤æµçå¹³å°ï¼æ¬¢è¿è®¨è®ºäº¤æµï¼ -
+ä¸èµ·ä¿å«3000ç¹ç´å°çªç ´6124ç¹ã
```

### Comparing `adata-1.2.4/adata.egg-info/SOURCES.txt` & `adata-2.0.0b0/adata.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 adata/common/utils/sunrequests.py
 adata/fund/__init__.py
 adata/fund/cache/__init__.py
 adata/fund/info/__init__.py
 adata/fund/info/fund_info.py
 adata/fund/market/__init__.py
 adata/fund/market/etf_market.py
+adata/fund/market/etf_market_template.py
+adata/fund/market/etf_market_ths.py
 adata/message/__init__.py
 adata/sentiment/__init__.py
 adata/sentiment/north_flow.py
 adata/sentiment/securities_margin.py
 adata/sentiment/stock_lifting.py
 adata/sentiment/cache/__init__.py
 adata/stock/__init__.py
@@ -96,11 +98,8 @@
 adata/stock/market/index_market/market_index_template.py
 adata/stock/market/index_market/market_index_ths.py
 adata/stock/market/stock_market/__init__.py
 adata/stock/market/stock_market/stock_market.py
 adata/stock/market/stock_market/stock_market_baidu.py
 adata/stock/market/stock_market/stock_market_qq.py
 adata/stock/market/stock_market/stock_market_sina.py
-adata/stock/market/stock_market/stock_market_template.py
-tests/other/__init__.py
-tests/other/bs4_test.py
-tests/other/year_test.py
+adata/stock/market/stock_market/stock_market_template.py
```

