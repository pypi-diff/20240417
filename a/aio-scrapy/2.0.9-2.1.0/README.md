# Comparing `tmp/aio-scrapy-2.0.9.tar.gz` & `tmp/aio-scrapy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio-scrapy-2.0.9.tar", last modified: Wed Apr  3 06:32:05 2024, max compression
+gzip compressed data, was "aio-scrapy-2.1.0.tar", last modified: Wed Apr 17 06:38:12 2024, max compression
```

## Comparing `aio-scrapy-2.0.9.tar` & `aio-scrapy-2.1.0.tar`

### file list

```diff
@@ -1,169 +1,170 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.429945 aio-scrapy-2.0.9/
--rw-rw-rw-   0        0        0     1088 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/LICENSE
--rw-rw-rw-   0        0        0      182 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     6337 2024-04-03 06:32:05.428956 aio-scrapy-2.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3855 2023-12-25 01:05:41.000000 aio-scrapy-2.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.425913 aio-scrapy-2.0.9/aio_scrapy.egg-info/
--rw-rw-rw-   0        0        0     6337 2024-04-03 06:32:04.000000 aio-scrapy-2.0.9/aio_scrapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4366 2024-04-03 06:32:04.000000 aio-scrapy-2.0.9/aio_scrapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 06:32:04.000000 aio-scrapy-2.0.9/aio_scrapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-03 06:32:04.000000 aio-scrapy-2.0.9/aio_scrapy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-03 06:32:04.000000 aio-scrapy-2.0.9/aio_scrapy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      574 2024-04-03 06:32:04.000000 aio-scrapy-2.0.9/aio_scrapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-03 06:32:04.000000 aio-scrapy-2.0.9/aio_scrapy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:04.875668 aio-scrapy-2.0.9/aioscrapy/
--rw-rw-rw-   0        0        0        5 2024-04-03 06:26:17.000000 aio-scrapy-2.0.9/aioscrapy/VERSION
--rw-rw-rw-   0        0        0      858 2023-09-28 01:34:29.000000 aio-scrapy-2.0.9/aioscrapy/__init__.py
--rw-rw-rw-   0        0        0       80 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/__main__.py
--rw-rw-rw-   0        0        0     5159 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/cmdline.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:04.918480 aio-scrapy-2.0.9/aioscrapy/commands/
--rw-rw-rw-   0        0        0     4769 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/__init__.py
--rw-rw-rw-   0        0        0     1020 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/crawl.py
--rw-rw-rw-   0        0        0     5426 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/genspider.py
--rw-rw-rw-   0        0        0      346 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/list.py
--rw-rw-rw-   0        0        0     2067 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/runspider.py
--rw-rw-rw-   0        0        0     1798 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/settings.py
--rw-rw-rw-   0        0        0     4001 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/startproject.py
--rw-rw-rw-   0        0        0      485 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/version.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:04.923810 aio-scrapy-2.0.9/aioscrapy/core/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:04.938965 aio-scrapy-2.0.9/aioscrapy/core/downloader/
--rw-rw-rw-   0        0        0     9465 2024-01-15 09:49:33.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:04.995130 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/
--rw-rw-rw-   0        0        0     3198 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/__init__.py
--rw-rw-rw-   0        0        0     3942 2023-12-25 07:35:12.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/aiohttp.py
--rw-rw-rw-   0        0        0     3041 2023-09-27 08:43:17.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/httpx.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.006182 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/playwright/
--rw-rw-rw-   0        0        0     4160 2023-10-12 09:22:48.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/playwright/__init__.py
--rw-rw-rw-   0        0        0     1374 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/playwright/driverpool.py
--rw-rw-rw-   0        0        0     3530 2023-10-12 09:38:59.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/playwright/webdriver.py
--rw-rw-rw-   0        0        0     2228 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/pyhttpx.py
--rw-rw-rw-   0        0        0     1996 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/requests.py
--rw-rw-rw-   0        0        0    10925 2024-01-15 09:37:22.000000 aio-scrapy-2.0.9/aioscrapy/core/engine.py
--rw-rw-rw-   0        0        0     5737 2023-09-27 09:13:11.000000 aio-scrapy-2.0.9/aioscrapy/core/scheduler.py
--rw-rw-rw-   0        0        0    10304 2023-10-12 09:32:46.000000 aio-scrapy-2.0.9/aioscrapy/core/scraper.py
--rw-rw-rw-   0        0        0    10109 2023-12-22 04:04:27.000000 aio-scrapy-2.0.9/aioscrapy/crawler.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.014768 aio-scrapy-2.0.9/aioscrapy/db/
--rw-rw-rw-   0        0        0     2456 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/db/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/db/absmanager.py
--rw-rw-rw-   0        0        0     2745 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/db/aiomongo.py
--rw-rw-rw-   0        0        0     3799 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/db/aiomysql.py
--rw-rw-rw-   0        0        0     3213 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/db/aiopg.py
--rw-rw-rw-   0        0        0     5583 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/db/aiorabbitmq.py
--rw-rw-rw-   0        0        0     2966 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/db/aioredis.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.030116 aio-scrapy-2.0.9/aioscrapy/dupefilters/
--rw-rw-rw-   0        0        0     1498 2024-04-03 06:24:20.000000 aio-scrapy-2.0.9/aioscrapy/dupefilters/__init__.py
--rw-rw-rw-   0        0        0     1551 2024-04-03 06:24:20.000000 aio-scrapy-2.0.9/aioscrapy/dupefilters/disk.py
--rw-rw-rw-   0        0        0     4723 2024-04-03 06:24:20.000000 aio-scrapy-2.0.9/aioscrapy/dupefilters/redis.py
--rw-rw-rw-   0        0        0     2027 2024-01-15 09:43:42.000000 aio-scrapy-2.0.9/aioscrapy/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.033116 aio-scrapy-2.0.9/aioscrapy/http/
--rw-rw-rw-   0        0        0      597 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/__init__.py
--rw-rw-rw-   0        0        0     1573 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/headers.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.057981 aio-scrapy-2.0.9/aioscrapy/http/request/
--rw-rw-rw-   0        0        0     7121 2023-09-26 06:37:06.000000 aio-scrapy-2.0.9/aioscrapy/http/request/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/request/form.py
--rw-rw-rw-   0        0        0     2051 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/request/json_request.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.091989 aio-scrapy-2.0.9/aioscrapy/http/response/
--rw-rw-rw-   0        0        0     6731 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/response/__init__.py
--rw-rw-rw-   0        0        0      303 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/response/html.py
--rw-rw-rw-   0        0        0     1051 2023-10-12 09:29:08.000000 aio-scrapy-2.0.9/aioscrapy/http/response/playwright.py
--rw-rw-rw-   0        0        0     9844 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/response/text.py
--rw-rw-rw-   0        0        0      300 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/response/xml.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.092988 aio-scrapy-2.0.9/aioscrapy/libs/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.119955 aio-scrapy-2.0.9/aioscrapy/libs/downloader/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/libs/downloader/__init__.py
--rw-rw-rw-   0        0        0      563 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/libs/downloader/defaultheaders.py
--rw-rw-rw-   0        0        0      704 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/libs/downloader/downloadtimeout.py
--rw-rw-rw-   0        0        0     1058 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/libs/downloader/ja3fingerprint.py
--rw-rw-rw-   0        0        0     5191 2024-03-01 06:49:55.000000 aio-scrapy-2.0.9/aioscrapy/libs/downloader/retry.py
--rw-rw-rw-   0        0        0     1376 2023-09-26 09:41:57.000000 aio-scrapy-2.0.9/aioscrapy/libs/downloader/stats.py
--rw-rw-rw-   0        0        0      743 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/libs/downloader/useragent.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.137091 aio-scrapy-2.0.9/aioscrapy/libs/extensions/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/libs/extensions/__init__.py
--rw-rw-rw-   0        0        0     2734 2023-09-22 10:41:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/extensions/closespider.py
--rw-rw-rw-   0        0        0     1820 2023-09-26 08:56:09.000000 aio-scrapy-2.0.9/aioscrapy/libs/extensions/corestats.py
--rw-rw-rw-   0        0        0     1844 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/extensions/logstats.py
--rw-rw-rw-   0        0        0     5479 2023-10-20 01:51:59.000000 aio-scrapy-2.0.9/aioscrapy/libs/extensions/metric.py
--rw-rw-rw-   0        0        0     3512 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/extensions/throttle.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.145175 aio-scrapy-2.0.9/aioscrapy/libs/pipelines/
--rw-rw-rw-   0        0        0     5709 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/pipelines/__init__.py
--rw-rw-rw-   0        0        0     2454 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/pipelines/csv.py
--rw-rw-rw-   0        0        0     6284 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/pipelines/execl.py
--rw-rw-rw-   0        0        0     2001 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/pipelines/mongo.py
--rw-rw-rw-   0        0        0     1022 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/pipelines/mysql.py
--rw-rw-rw-   0        0        0      990 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/pipelines/pg.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.163841 aio-scrapy-2.0.9/aioscrapy/libs/spider/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/libs/spider/__init__.py
--rw-rw-rw-   0        0        0     1938 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/spider/depth.py
--rw-rw-rw-   0        0        0     1857 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/spider/httperror.py
--rw-rw-rw-   0        0        0     2941 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/spider/offsite.py
--rw-rw-rw-   0        0        0    13768 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/libs/spider/referer.py
--rw-rw-rw-   0        0        0     1151 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/spider/urllength.py
--rw-rw-rw-   0        0        0     1867 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/link.py
--rw-rw-rw-   0        0        0     3028 2023-10-12 09:32:03.000000 aio-scrapy-2.0.9/aioscrapy/logformatter.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.170852 aio-scrapy-2.0.9/aioscrapy/middleware/
--rw-rw-rw-   0        0        0      396 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/middleware/__init__.py
--rw-rw-rw-   0        0        0     3410 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/middleware/absmanager.py
--rw-rw-rw-   0        0        0     3199 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/middleware/downloader.py
--rw-rw-rw-   0        0        0      420 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/middleware/extension.py
--rw-rw-rw-   0        0        0      674 2023-09-19 03:48:43.000000 aio-scrapy-2.0.9/aioscrapy/middleware/itempipeline.py
--rw-rw-rw-   0        0        0     6361 2023-12-05 08:01:00.000000 aio-scrapy-2.0.9/aioscrapy/middleware/spider.py
--rw-rw-rw-   0        0        0     1603 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/process.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.199809 aio-scrapy-2.0.9/aioscrapy/proxy/
--rw-rw-rw-   0        0        0     1807 2024-01-15 08:08:24.000000 aio-scrapy-2.0.9/aioscrapy/proxy/__init__.py
--rw-rw-rw-   0        0        0     2711 2024-01-15 09:59:00.000000 aio-scrapy-2.0.9/aioscrapy/proxy/redis.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.224959 aio-scrapy-2.0.9/aioscrapy/queue/
--rw-rw-rw-   0        0        0     2037 2024-01-17 07:10:58.000000 aio-scrapy-2.0.9/aioscrapy/queue/__init__.py
--rw-rw-rw-   0        0        0     3140 2024-01-17 07:10:58.000000 aio-scrapy-2.0.9/aioscrapy/queue/memory.py
--rw-rw-rw-   0        0        0     2516 2024-01-17 07:10:58.000000 aio-scrapy-2.0.9/aioscrapy/queue/rabbitmq.py
--rw-rw-rw-   0        0        0     4788 2024-01-17 07:10:58.000000 aio-scrapy-2.0.9/aioscrapy/queue/redis.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.240616 aio-scrapy-2.0.9/aioscrapy/scrapyd/
--rw-rw-rw-   0        0        0       68 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/scrapyd/__init__.py
--rw-rw-rw-   0        0        0     1777 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/scrapyd/runner.py
--rw-rw-rw-   0        0        0      734 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/serializer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.258422 aio-scrapy-2.0.9/aioscrapy/settings/
--rw-rw-rw-   0        0        0    15781 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/settings/__init__.py
--rw-rw-rw-   0        0        0     5432 2023-09-27 08:43:18.000000 aio-scrapy-2.0.9/aioscrapy/settings/default_settings.py
--rw-rw-rw-   0        0        0     2402 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/signalmanager.py
--rw-rw-rw-   0        0        0      610 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/signals.py
--rw-rw-rw-   0        0        0     3426 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/spiderloader.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.268995 aio-scrapy-2.0.9/aioscrapy/spiders/
--rw-rw-rw-   0        0        0     3934 2024-01-17 07:10:58.000000 aio-scrapy-2.0.9/aioscrapy/spiders/__init__.py
--rw-rw-rw-   0        0        0     2036 2023-12-05 07:56:11.000000 aio-scrapy-2.0.9/aioscrapy/statscollectors.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:04.778530 aio-scrapy-2.0.9/aioscrapy/templates/
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.270997 aio-scrapy-2.0.9/aioscrapy/templates/project/
--rw-rw-rw-   0        0        0      112 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/templates/project/aioscrapy.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.285303 aio-scrapy-2.0.9/aioscrapy/templates/project/module/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/templates/project/module/__init__.py
--rw-rw-rw-   0        0        0     3469 2023-12-05 07:04:56.000000 aio-scrapy-2.0.9/aioscrapy/templates/project/module/middlewares.py.tmpl
--rw-rw-rw-   0        0        0      164 2023-12-05 07:04:56.000000 aio-scrapy-2.0.9/aioscrapy/templates/project/module/pipelines.py.tmpl
--rw-rw-rw-   0        0        0     1421 2023-12-05 07:11:48.000000 aio-scrapy-2.0.9/aioscrapy/templates/project/module/settings.py.tmpl
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.303577 aio-scrapy-2.0.9/aioscrapy/templates/project/module/spiders/
--rw-rw-rw-   0        0        0      164 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/templates/project/module/spiders/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.306579 aio-scrapy-2.0.9/aioscrapy/templates/spiders/
--rw-rw-rw-   0        0        0      375 2023-12-05 07:11:48.000000 aio-scrapy-2.0.9/aioscrapy/templates/spiders/basic.tmpl
--rw-rw-rw-   0        0        0      942 2023-12-05 07:11:48.000000 aio-scrapy-2.0.9/aioscrapy/templates/spiders/single.tmpl
-drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.414993 aio-scrapy-2.0.9/aioscrapy/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/utils/__init__.py
--rw-rw-rw-   0        0        0     7208 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/conf.py
--rw-rw-rw-   0        0        0     3295 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/curl.py
--rw-rw-rw-   0        0        0      794 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/decorators.py
--rw-rw-rw-   0        0        0     5467 2023-09-28 01:34:29.000000 aio-scrapy-2.0.9/aioscrapy/utils/deprecate.py
--rw-rw-rw-   0        0        0      708 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/httpobj.py
--rw-rw-rw-   0        0        0     1697 2024-04-03 06:24:20.000000 aio-scrapy-2.0.9/aioscrapy/utils/log.py
--rw-rw-rw-   0        0        0     3509 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/misc.py
--rw-rw-rw-   0        0        0      896 2023-09-26 07:33:08.000000 aio-scrapy-2.0.9/aioscrapy/utils/ossignal.py
--rw-rw-rw-   0        0        0     2905 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/project.py
--rw-rw-rw-   0        0        0     4577 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/python.py
--rw-rw-rw-   0        0        0      487 2024-01-17 07:10:58.000000 aio-scrapy-2.0.9/aioscrapy/utils/reqser.py
--rw-rw-rw-   0        0        0     2418 2024-01-17 07:10:58.000000 aio-scrapy-2.0.9/aioscrapy/utils/request.py
--rw-rw-rw-   0        0        0     1341 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/response.py
--rw-rw-rw-   0        0        0     2282 2023-09-26 06:57:24.000000 aio-scrapy-2.0.9/aioscrapy/utils/signal.py
--rw-rw-rw-   0        0        0      610 2023-09-26 06:57:24.000000 aio-scrapy-2.0.9/aioscrapy/utils/spider.py
--rw-rw-rw-   0        0        0      833 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/template.py
--rw-rw-rw-   0        0        0     2319 2023-09-22 09:42:23.000000 aio-scrapy-2.0.9/aioscrapy/utils/tools.py
--rw-rw-rw-   0        0        0     2019 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/trackref.py
--rw-rw-rw-   0        0        0     5464 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/url.py
--rw-rw-rw-   0        0        0       42 2024-04-03 06:32:05.430945 aio-scrapy-2.0.9/setup.cfg
--rw-rw-rw-   0        0        0     2444 2023-10-07 03:17:40.000000 aio-scrapy-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.802206 aio-scrapy-2.1.0/
+-rw-rw-rw-   0        0        0     1088 2023-04-10 08:42:04.000000 aio-scrapy-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0      182 2023-04-10 08:42:04.000000 aio-scrapy-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6461 2024-04-17 06:38:12.801208 aio-scrapy-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3855 2023-12-25 01:05:41.000000 aio-scrapy-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.798212 aio-scrapy-2.1.0/aio_scrapy.egg-info/
+-rw-rw-rw-   0        0        0     6461 2024-04-17 06:38:11.000000 aio-scrapy-2.1.0/aio_scrapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4414 2024-04-17 06:38:11.000000 aio-scrapy-2.1.0/aio_scrapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 06:38:11.000000 aio-scrapy-2.1.0/aio_scrapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-17 06:38:11.000000 aio-scrapy-2.1.0/aio_scrapy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 03:59:03.000000 aio-scrapy-2.1.0/aio_scrapy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      614 2024-04-17 06:38:11.000000 aio-scrapy-2.1.0/aio_scrapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-17 06:38:11.000000 aio-scrapy-2.1.0/aio_scrapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:11.852183 aio-scrapy-2.1.0/aioscrapy/
+-rw-rw-rw-   0        0        0        5 2024-04-17 03:57:53.000000 aio-scrapy-2.1.0/aioscrapy/VERSION
+-rw-rw-rw-   0        0        0      858 2023-09-28 01:34:29.000000 aio-scrapy-2.1.0/aioscrapy/__init__.py
+-rw-rw-rw-   0        0        0       80 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/__main__.py
+-rw-rw-rw-   0        0        0     5159 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/cmdline.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:11.913090 aio-scrapy-2.1.0/aioscrapy/commands/
+-rw-rw-rw-   0        0        0     4769 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/commands/__init__.py
+-rw-rw-rw-   0        0        0     1020 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/commands/crawl.py
+-rw-rw-rw-   0        0        0     5426 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/commands/genspider.py
+-rw-rw-rw-   0        0        0      346 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/commands/list.py
+-rw-rw-rw-   0        0        0     2067 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/commands/runspider.py
+-rw-rw-rw-   0        0        0     1798 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/commands/settings.py
+-rw-rw-rw-   0        0        0     4001 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/commands/startproject.py
+-rw-rw-rw-   0        0        0      485 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/commands/version.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:11.919088 aio-scrapy-2.1.0/aioscrapy/core/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.1.0/aioscrapy/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:11.927264 aio-scrapy-2.1.0/aioscrapy/core/downloader/
+-rw-rw-rw-   0        0        0     9574 2024-04-08 07:38:05.000000 aio-scrapy-2.1.0/aioscrapy/core/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.016907 aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/
+-rw-rw-rw-   0        0        0     3198 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/__init__.py
+-rw-rw-rw-   0        0        0     3942 2023-12-25 07:35:12.000000 aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/aiohttp.py
+-rw-rw-rw-   0        0        0     2250 2024-04-17 03:38:29.000000 aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/curl_cffi.py
+-rw-rw-rw-   0        0        0     3041 2023-09-27 08:43:17.000000 aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/httpx.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.036908 aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/playwright/
+-rw-rw-rw-   0        0        0     4160 2023-10-12 09:22:48.000000 aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/playwright/__init__.py
+-rw-rw-rw-   0        0        0     1374 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/playwright/driverpool.py
+-rw-rw-rw-   0        0        0     3530 2023-10-12 09:38:59.000000 aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/playwright/webdriver.py
+-rw-rw-rw-   0        0        0     2228 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/pyhttpx.py
+-rw-rw-rw-   0        0        0     1996 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/requests.py
+-rw-rw-rw-   0        0        0     9843 2024-04-08 03:15:09.000000 aio-scrapy-2.1.0/aioscrapy/core/engine.py
+-rw-rw-rw-   0        0        0     7408 2024-04-08 08:48:10.000000 aio-scrapy-2.1.0/aioscrapy/core/scheduler.py
+-rw-rw-rw-   0        0        0    10304 2023-10-12 09:32:46.000000 aio-scrapy-2.1.0/aioscrapy/core/scraper.py
+-rw-rw-rw-   0        0        0    10330 2024-04-17 03:49:10.000000 aio-scrapy-2.1.0/aioscrapy/crawler.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.070940 aio-scrapy-2.1.0/aioscrapy/db/
+-rw-rw-rw-   0        0        0     2456 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/db/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/db/absmanager.py
+-rw-rw-rw-   0        0        0     2745 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/db/aiomongo.py
+-rw-rw-rw-   0        0        0     3799 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/db/aiomysql.py
+-rw-rw-rw-   0        0        0     3213 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/db/aiopg.py
+-rw-rw-rw-   0        0        0     5583 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/db/aiorabbitmq.py
+-rw-rw-rw-   0        0        0     2966 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/db/aioredis.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.095282 aio-scrapy-2.1.0/aioscrapy/dupefilters/
+-rw-rw-rw-   0        0        0     1498 2024-04-03 06:24:20.000000 aio-scrapy-2.1.0/aioscrapy/dupefilters/__init__.py
+-rw-rw-rw-   0        0        0     1551 2024-04-03 06:24:20.000000 aio-scrapy-2.1.0/aioscrapy/dupefilters/disk.py
+-rw-rw-rw-   0        0        0     4812 2024-04-03 09:56:31.000000 aio-scrapy-2.1.0/aioscrapy/dupefilters/redis.py
+-rw-rw-rw-   0        0        0     2027 2024-01-15 09:43:42.000000 aio-scrapy-2.1.0/aioscrapy/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.108296 aio-scrapy-2.1.0/aioscrapy/http/
+-rw-rw-rw-   0        0        0      597 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/http/__init__.py
+-rw-rw-rw-   0        0        0     1573 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/http/headers.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.147393 aio-scrapy-2.1.0/aioscrapy/http/request/
+-rw-rw-rw-   0        0        0     7121 2023-09-26 06:37:06.000000 aio-scrapy-2.1.0/aioscrapy/http/request/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/http/request/form.py
+-rw-rw-rw-   0        0        0     2051 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/http/request/json_request.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.197595 aio-scrapy-2.1.0/aioscrapy/http/response/
+-rw-rw-rw-   0        0        0     6731 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/http/response/__init__.py
+-rw-rw-rw-   0        0        0      303 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/http/response/html.py
+-rw-rw-rw-   0        0        0     1051 2023-10-12 09:29:08.000000 aio-scrapy-2.1.0/aioscrapy/http/response/playwright.py
+-rw-rw-rw-   0        0        0     9844 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/http/response/text.py
+-rw-rw-rw-   0        0        0      300 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/http/response/xml.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.198578 aio-scrapy-2.1.0/aioscrapy/libs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.1.0/aioscrapy/libs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.225384 aio-scrapy-2.1.0/aioscrapy/libs/downloader/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.1.0/aioscrapy/libs/downloader/__init__.py
+-rw-rw-rw-   0        0        0      563 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/libs/downloader/defaultheaders.py
+-rw-rw-rw-   0        0        0      704 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/libs/downloader/downloadtimeout.py
+-rw-rw-rw-   0        0        0     1058 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/libs/downloader/ja3fingerprint.py
+-rw-rw-rw-   0        0        0     5306 2024-04-17 04:14:02.000000 aio-scrapy-2.1.0/aioscrapy/libs/downloader/retry.py
+-rw-rw-rw-   0        0        0     1376 2023-09-26 09:41:57.000000 aio-scrapy-2.1.0/aioscrapy/libs/downloader/stats.py
+-rw-rw-rw-   0        0        0      743 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/libs/downloader/useragent.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.283034 aio-scrapy-2.1.0/aioscrapy/libs/extensions/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.1.0/aioscrapy/libs/extensions/__init__.py
+-rw-rw-rw-   0        0        0     2734 2023-09-22 10:41:29.000000 aio-scrapy-2.1.0/aioscrapy/libs/extensions/closespider.py
+-rw-rw-rw-   0        0        0     1820 2023-09-26 08:56:09.000000 aio-scrapy-2.1.0/aioscrapy/libs/extensions/corestats.py
+-rw-rw-rw-   0        0        0     1844 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/libs/extensions/logstats.py
+-rw-rw-rw-   0        0        0     5479 2023-10-20 01:51:59.000000 aio-scrapy-2.1.0/aioscrapy/libs/extensions/metric.py
+-rw-rw-rw-   0        0        0     3512 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/libs/extensions/throttle.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.315043 aio-scrapy-2.1.0/aioscrapy/libs/pipelines/
+-rw-rw-rw-   0        0        0     5642 2024-04-17 02:17:45.000000 aio-scrapy-2.1.0/aioscrapy/libs/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     2454 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/libs/pipelines/csv.py
+-rw-rw-rw-   0        0        0     6284 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/libs/pipelines/execl.py
+-rw-rw-rw-   0        0        0     2001 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/libs/pipelines/mongo.py
+-rw-rw-rw-   0        0        0     1022 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/libs/pipelines/mysql.py
+-rw-rw-rw-   0        0        0      990 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/libs/pipelines/pg.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.344285 aio-scrapy-2.1.0/aioscrapy/libs/spider/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.1.0/aioscrapy/libs/spider/__init__.py
+-rw-rw-rw-   0        0        0     1938 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/libs/spider/depth.py
+-rw-rw-rw-   0        0        0     1857 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/libs/spider/httperror.py
+-rw-rw-rw-   0        0        0     2941 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/libs/spider/offsite.py
+-rw-rw-rw-   0        0        0    13768 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/libs/spider/referer.py
+-rw-rw-rw-   0        0        0     1151 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/libs/spider/urllength.py
+-rw-rw-rw-   0        0        0     1867 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/link.py
+-rw-rw-rw-   0        0        0     3028 2023-10-12 09:32:03.000000 aio-scrapy-2.1.0/aioscrapy/logformatter.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.355285 aio-scrapy-2.1.0/aioscrapy/middleware/
+-rw-rw-rw-   0        0        0      396 2023-04-10 08:42:04.000000 aio-scrapy-2.1.0/aioscrapy/middleware/__init__.py
+-rw-rw-rw-   0        0        0     3410 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/middleware/absmanager.py
+-rw-rw-rw-   0        0        0     3199 2023-09-26 06:48:29.000000 aio-scrapy-2.1.0/aioscrapy/middleware/downloader.py
+-rw-rw-rw-   0        0        0      420 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/middleware/extension.py
+-rw-rw-rw-   0        0        0      674 2023-09-19 03:48:43.000000 aio-scrapy-2.1.0/aioscrapy/middleware/itempipeline.py
+-rw-rw-rw-   0        0        0     6361 2023-12-05 08:01:00.000000 aio-scrapy-2.1.0/aioscrapy/middleware/spider.py
+-rw-rw-rw-   0        0        0     1603 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/process.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.377836 aio-scrapy-2.1.0/aioscrapy/proxy/
+-rw-rw-rw-   0        0        0     1807 2024-01-15 08:08:24.000000 aio-scrapy-2.1.0/aioscrapy/proxy/__init__.py
+-rw-rw-rw-   0        0        0     2711 2024-01-15 09:59:00.000000 aio-scrapy-2.1.0/aioscrapy/proxy/redis.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.398893 aio-scrapy-2.1.0/aioscrapy/queue/
+-rw-rw-rw-   0        0        0     2037 2024-01-17 07:10:58.000000 aio-scrapy-2.1.0/aioscrapy/queue/__init__.py
+-rw-rw-rw-   0        0        0     3140 2024-01-17 07:10:58.000000 aio-scrapy-2.1.0/aioscrapy/queue/memory.py
+-rw-rw-rw-   0        0        0     2516 2024-01-17 07:10:58.000000 aio-scrapy-2.1.0/aioscrapy/queue/rabbitmq.py
+-rw-rw-rw-   0        0        0     4788 2024-01-17 07:10:58.000000 aio-scrapy-2.1.0/aioscrapy/queue/redis.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.411907 aio-scrapy-2.1.0/aioscrapy/scrapyd/
+-rw-rw-rw-   0        0        0       68 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/scrapyd/__init__.py
+-rw-rw-rw-   0        0        0     1777 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/scrapyd/runner.py
+-rw-rw-rw-   0        0        0      734 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.429907 aio-scrapy-2.1.0/aioscrapy/settings/
+-rw-rw-rw-   0        0        0    15781 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/settings/__init__.py
+-rw-rw-rw-   0        0        0     5639 2024-04-17 03:35:35.000000 aio-scrapy-2.1.0/aioscrapy/settings/default_settings.py
+-rw-rw-rw-   0        0        0     2402 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/signalmanager.py
+-rw-rw-rw-   0        0        0      610 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/signals.py
+-rw-rw-rw-   0        0        0     3426 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/spiderloader.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.451471 aio-scrapy-2.1.0/aioscrapy/spiders/
+-rw-rw-rw-   0        0        0     4010 2024-04-17 03:49:10.000000 aio-scrapy-2.1.0/aioscrapy/spiders/__init__.py
+-rw-rw-rw-   0        0        0     2036 2023-12-05 07:56:11.000000 aio-scrapy-2.1.0/aioscrapy/statscollectors.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:11.715463 aio-scrapy-2.1.0/aioscrapy/templates/
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.452473 aio-scrapy-2.1.0/aioscrapy/templates/project/
+-rw-rw-rw-   0        0        0      112 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/templates/project/aioscrapy.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.474785 aio-scrapy-2.1.0/aioscrapy/templates/project/module/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.1.0/aioscrapy/templates/project/module/__init__.py
+-rw-rw-rw-   0        0        0     3469 2023-12-05 07:04:56.000000 aio-scrapy-2.1.0/aioscrapy/templates/project/module/middlewares.py.tmpl
+-rw-rw-rw-   0        0        0      164 2023-12-05 07:04:56.000000 aio-scrapy-2.1.0/aioscrapy/templates/project/module/pipelines.py.tmpl
+-rw-rw-rw-   0        0        0     1421 2023-12-05 07:11:48.000000 aio-scrapy-2.1.0/aioscrapy/templates/project/module/settings.py.tmpl
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.491788 aio-scrapy-2.1.0/aioscrapy/templates/project/module/spiders/
+-rw-rw-rw-   0        0        0      164 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/templates/project/module/spiders/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.495776 aio-scrapy-2.1.0/aioscrapy/templates/spiders/
+-rw-rw-rw-   0        0        0      375 2023-12-05 07:11:48.000000 aio-scrapy-2.1.0/aioscrapy/templates/spiders/basic.tmpl
+-rw-rw-rw-   0        0        0      942 2023-12-05 07:11:48.000000 aio-scrapy-2.1.0/aioscrapy/templates/spiders/single.tmpl
+drwxrwxrwx   0        0        0        0 2024-04-17 06:38:12.785941 aio-scrapy-2.1.0/aioscrapy/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.1.0/aioscrapy/utils/__init__.py
+-rw-rw-rw-   0        0        0     7208 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/utils/conf.py
+-rw-rw-rw-   0        0        0     3295 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/utils/curl.py
+-rw-rw-rw-   0        0        0      794 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/utils/decorators.py
+-rw-rw-rw-   0        0        0     5467 2023-09-28 01:34:29.000000 aio-scrapy-2.1.0/aioscrapy/utils/deprecate.py
+-rw-rw-rw-   0        0        0      708 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/utils/httpobj.py
+-rw-rw-rw-   0        0        0     1697 2024-04-03 06:24:20.000000 aio-scrapy-2.1.0/aioscrapy/utils/log.py
+-rw-rw-rw-   0        0        0     3509 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/utils/misc.py
+-rw-rw-rw-   0        0        0      896 2023-09-26 07:33:08.000000 aio-scrapy-2.1.0/aioscrapy/utils/ossignal.py
+-rw-rw-rw-   0        0        0     2905 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/utils/project.py
+-rw-rw-rw-   0        0        0     4577 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/utils/python.py
+-rw-rw-rw-   0        0        0      487 2024-01-17 07:10:58.000000 aio-scrapy-2.1.0/aioscrapy/utils/reqser.py
+-rw-rw-rw-   0        0        0     2418 2024-01-17 07:10:58.000000 aio-scrapy-2.1.0/aioscrapy/utils/request.py
+-rw-rw-rw-   0        0        0     1341 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/utils/response.py
+-rw-rw-rw-   0        0        0     2282 2023-09-26 06:57:24.000000 aio-scrapy-2.1.0/aioscrapy/utils/signal.py
+-rw-rw-rw-   0        0        0      610 2023-09-26 06:57:24.000000 aio-scrapy-2.1.0/aioscrapy/utils/spider.py
+-rw-rw-rw-   0        0        0      833 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/utils/template.py
+-rw-rw-rw-   0        0        0     2319 2023-09-22 09:42:23.000000 aio-scrapy-2.1.0/aioscrapy/utils/tools.py
+-rw-rw-rw-   0        0        0     2019 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/utils/trackref.py
+-rw-rw-rw-   0        0        0     5464 2023-09-21 06:43:51.000000 aio-scrapy-2.1.0/aioscrapy/utils/url.py
+-rw-rw-rw-   0        0        0       42 2024-04-17 06:38:12.802206 aio-scrapy-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2497 2024-04-17 04:16:34.000000 aio-scrapy-2.1.0/setup.py
```

### Comparing `aio-scrapy-2.0.9/LICENSE` & `aio-scrapy-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/PKG-INFO` & `aio-scrapy-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-scrapy
-Version: 2.0.9
+Version: 2.1.0
 Summary: A high-level Web Crawling and Web Scraping framework based on Asyncio
 Home-page: https://github.com/conlin-huang/aio-scrapy.git
 Author: conlin
 Author-email: 995018884@qq.com
 License: MIT
 Keywords: aio-scrapy,scrapy,aioscrapy,scrapy redis,asyncio,spider
 Classifier: License :: OSI Approved :: MIT License
@@ -35,27 +35,30 @@
 Requires-Dist: cryptography; extra == "all"
 Requires-Dist: motor>=3.1.1; extra == "all"
 Requires-Dist: pyhttpx>=2.10.1; extra == "all"
 Requires-Dist: asyncpg>=0.27.0; extra == "all"
 Requires-Dist: XlsxWriter>=3.1.2; extra == "all"
 Requires-Dist: pillow>=9.4.0; extra == "all"
 Requires-Dist: requests>=2.28.2; extra == "all"
+Requires-Dist: curl_cffi; extra == "all"
 Provides-Extra: aiomysql
 Requires-Dist: aiomysql>=0.1.1; extra == "aiomysql"
 Requires-Dist: cryptography; extra == "aiomysql"
 Provides-Extra: httpx
 Requires-Dist: httpx[http2]>=0.23.0; extra == "httpx"
 Provides-Extra: aio-pika
 Requires-Dist: aio-pika>=8.1.1; extra == "aio-pika"
 Provides-Extra: mongo
 Requires-Dist: motor>=3.1.1; extra == "mongo"
 Provides-Extra: playwright
 Requires-Dist: playwright>=1.31.1; extra == "playwright"
 Provides-Extra: pyhttpx
 Requires-Dist: pyhttpx>=2.10.4; extra == "pyhttpx"
+Provides-Extra: curl-cffi
+Requires-Dist: curl_cffi>=0.6.1; extra == "curl-cffi"
 Provides-Extra: requests
 Requires-Dist: requests>=2.28.2; extra == "requests"
 Provides-Extra: pg
 Requires-Dist: asyncpg>=0.27.0; extra == "pg"
 Provides-Extra: execl
 Requires-Dist: XlsxWriter>=3.1.2; extra == "execl"
 Requires-Dist: pillow>=9.4.0; extra == "execl"
```

### Comparing `aio-scrapy-2.0.9/README.md` & `aio-scrapy-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aio_scrapy.egg-info/PKG-INFO` & `aio-scrapy-2.1.0/aio_scrapy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-scrapy
-Version: 2.0.9
+Version: 2.1.0
 Summary: A high-level Web Crawling and Web Scraping framework based on Asyncio
 Home-page: https://github.com/conlin-huang/aio-scrapy.git
 Author: conlin
 Author-email: 995018884@qq.com
 License: MIT
 Keywords: aio-scrapy,scrapy,aioscrapy,scrapy redis,asyncio,spider
 Classifier: License :: OSI Approved :: MIT License
@@ -35,27 +35,30 @@
 Requires-Dist: cryptography; extra == "all"
 Requires-Dist: motor>=3.1.1; extra == "all"
 Requires-Dist: pyhttpx>=2.10.1; extra == "all"
 Requires-Dist: asyncpg>=0.27.0; extra == "all"
 Requires-Dist: XlsxWriter>=3.1.2; extra == "all"
 Requires-Dist: pillow>=9.4.0; extra == "all"
 Requires-Dist: requests>=2.28.2; extra == "all"
+Requires-Dist: curl_cffi; extra == "all"
 Provides-Extra: aiomysql
 Requires-Dist: aiomysql>=0.1.1; extra == "aiomysql"
 Requires-Dist: cryptography; extra == "aiomysql"
 Provides-Extra: httpx
 Requires-Dist: httpx[http2]>=0.23.0; extra == "httpx"
 Provides-Extra: aio-pika
 Requires-Dist: aio-pika>=8.1.1; extra == "aio-pika"
 Provides-Extra: mongo
 Requires-Dist: motor>=3.1.1; extra == "mongo"
 Provides-Extra: playwright
 Requires-Dist: playwright>=1.31.1; extra == "playwright"
 Provides-Extra: pyhttpx
 Requires-Dist: pyhttpx>=2.10.4; extra == "pyhttpx"
+Provides-Extra: curl-cffi
+Requires-Dist: curl_cffi>=0.6.1; extra == "curl-cffi"
 Provides-Extra: requests
 Requires-Dist: requests>=2.28.2; extra == "requests"
 Provides-Extra: pg
 Requires-Dist: asyncpg>=0.27.0; extra == "pg"
 Provides-Extra: execl
 Requires-Dist: XlsxWriter>=3.1.2; extra == "execl"
 Requires-Dist: pillow>=9.4.0; extra == "execl"
```

### Comparing `aio-scrapy-2.0.9/aio_scrapy.egg-info/SOURCES.txt` & `aio-scrapy-2.1.0/aio_scrapy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 aioscrapy/core/__init__.py
 aioscrapy/core/engine.py
 aioscrapy/core/scheduler.py
 aioscrapy/core/scraper.py
 aioscrapy/core/downloader/__init__.py
 aioscrapy/core/downloader/handlers/__init__.py
 aioscrapy/core/downloader/handlers/aiohttp.py
+aioscrapy/core/downloader/handlers/curl_cffi.py
 aioscrapy/core/downloader/handlers/httpx.py
 aioscrapy/core/downloader/handlers/pyhttpx.py
 aioscrapy/core/downloader/handlers/requests.py
 aioscrapy/core/downloader/handlers/playwright/__init__.py
 aioscrapy/core/downloader/handlers/playwright/driverpool.py
 aioscrapy/core/downloader/handlers/playwright/webdriver.py
 aioscrapy/db/__init__.py
```

### Comparing `aio-scrapy-2.0.9/aio_scrapy.egg-info/requires.txt` & `aio-scrapy-2.1.0/aio_scrapy.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 cryptography
 motor>=3.1.1
 pyhttpx>=2.10.1
 asyncpg>=0.27.0
 XlsxWriter>=3.1.2
 pillow>=9.4.0
 requests>=2.28.2
+curl_cffi
+
+[curl_cffi]
+curl_cffi>=0.6.1
 
 [execl]
 XlsxWriter>=3.1.2
 pillow>=9.4.0
 
 [httpx]
 httpx[http2]>=0.23.0
```

### Comparing `aio-scrapy-2.0.9/aioscrapy/__init__.py` & `aio-scrapy-2.1.0/aioscrapy/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/cmdline.py` & `aio-scrapy-2.1.0/aioscrapy/cmdline.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/commands/__init__.py` & `aio-scrapy-2.1.0/aioscrapy/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/commands/crawl.py` & `aio-scrapy-2.1.0/aioscrapy/commands/crawl.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/commands/genspider.py` & `aio-scrapy-2.1.0/aioscrapy/commands/genspider.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/commands/runspider.py` & `aio-scrapy-2.1.0/aioscrapy/commands/runspider.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/commands/settings.py` & `aio-scrapy-2.1.0/aioscrapy/commands/settings.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/commands/startproject.py` & `aio-scrapy-2.1.0/aioscrapy/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/core/downloader/__init__.py` & `aio-scrapy-2.1.0/aioscrapy/core/downloader/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 
         self.middleware = middleware
         self.handler = handler
         self.proxy = proxy
         self.dupefilter = dupefilter
 
         self.total_concurrency: int = self.settings.getint('CONCURRENT_REQUESTS')
+        self.get_requests_count: int = self.settings.getint('GET_REQUESTS_COUNT') or self.total_concurrency
         self.domain_concurrency: int = self.settings.getint('CONCURRENT_REQUESTS_PER_DOMAIN')
         self.ip_concurrency: int = self.settings.getint('CONCURRENT_REQUESTS_PER_IP')
         self.randomize_delay: bool = self.settings.getbool('RANDOMIZE_DOWNLOAD_DELAY')
 
         self.active: Set[Request] = set()
         self.slots: dict = {}
         self.running: bool = True
```

### Comparing `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/__init__.py` & `aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/aiohttp.py` & `aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/aiohttp.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/httpx.py` & `aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/httpx.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/playwright/__init__.py` & `aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/playwright/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/playwright/driverpool.py` & `aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/playwright/driverpool.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/playwright/webdriver.py` & `aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/playwright/webdriver.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/pyhttpx.py` & `aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/pyhttpx.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/requests.py` & `aio-scrapy-2.1.0/aioscrapy/core/downloader/handlers/requests.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/core/engine.py` & `aio-scrapy-2.1.0/aioscrapy/core/engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,26 +38,23 @@
 
     def __init__(self, crawler: "aioscrapy.Crawler") -> None:
         self.crawler = crawler
         self.settings = crawler.settings
         self.signals = crawler.signals
         self.logformatter = crawler.logformatter
 
-        self.enqueue_cache_num = self.settings.getint("ENQUEUE_CACHE_NUM")
-        self.enqueue_cache: Queue = Queue(self.enqueue_cache_num)
         self.slot: Optional[Slot] = None
         self.spider: Optional[Spider] = None
         self.downloader: Optional[DownloaderTV] = None
         self.scraper: Optional[Scraper] = None
         self.scheduler: Optional[BaseScheduler] = None
 
         self.running: bool = False
         self.unlock: bool = True
         self.finish: bool = False
-        self.enqueue_unlock: bool = True
 
     async def start(
             self,
             spider: Spider,
             start_requests: Optional[AsyncGenerator] = None
     ) -> None:
         """Start the execution engine"""
@@ -66,26 +63,24 @@
 
         self.running = True
         await self.signals.send_catch_log_deferred(signal=signals.engine_started)
         await self.open(spider, start_requests)
         while not self.finish:
             self.running and await self._next_request()
             await asyncio.sleep(1)
-            self.enqueue_cache_num != 1 and create_task(self._crawl())
             self.running and await self._spider_idle(self.spider)
 
     async def stop(self, reason: str = 'shutdown') -> None:
         """Stop the execution engine gracefully"""
         if not self.running:
             raise RuntimeError("Engine not running")
         self.running = False
 
         while not self.is_idle():
             await asyncio.sleep(0.2)
-            self.enqueue_cache_num != 1 and create_task(self._crawl())
         await self.close_spider(self.spider, reason=reason)
         await self.signals.send_catch_log_deferred(signal=signals.engine_stopped)
         self.finish = True
 
     async def open(
             self,
             spider: Spider,
@@ -134,15 +129,15 @@
             if self.spider.pause_time and self.spider.pause_time <= now:
                 self.spider.pause = False
             return
 
         while self.unlock and not self._needs_backout() and self.unlock:
             self.unlock = False
             try:
-                async for request in self.scheduler.next_request(self.downloader.total_concurrency):
+                async for request in self.scheduler.next_request(self.downloader.get_requests_count):
                     if request:
                         self.slot.add_request(request)
                         await self.downloader.fetch(request)
                 break
             finally:
                 self.unlock = True
 
@@ -208,35 +203,16 @@
         if not self.scraper.is_idle():
             # scraper is not idle
             return False
 
         return True
 
     async def crawl(self, request: Request) -> None:
-        if self.enqueue_cache_num == 1:
-            await self.scheduler.enqueue_request(request)
-            create_task(self._next_request())
-        else:
-            await self.enqueue_cache.put(request)
-
-    async def _crawl(self) -> None:
-        if not self.enqueue_unlock:
-            return
-        self.enqueue_unlock = False
-        requests = []
-        for _ in range(self.enqueue_cache.qsize()):
-            try:
-                request = self.enqueue_cache.get_nowait()
-                requests.append(request)
-            except QueueEmpty:
-                break
-        if requests:
-            await call_helper(self.scheduler.enqueue_request_batch, requests)
-            create_task(self._next_request())
-        self.enqueue_unlock = True
+        await self.scheduler.enqueue_request(request)
+        # create_task(self._next_request())
 
     async def close_spider(self, spider: Spider, reason: str = 'cancelled') -> None:
         """Close (cancel) spider and clear all its outstanding requests"""
 
         logger.info(f"Closing spider ({reason})")
 
         async def close_handler(
@@ -272,11 +248,10 @@
         res = await self.signals.send_catch_log(signals.spider_idle, spider=spider, dont_log=DontCloseSpider)
         if any(isinstance(x, DontCloseSpider) for _, x in res):
             return
 
         # method of 'has_pending_requests' has IO, so method of 'is_idle' execute twice
         if self.is_idle() \
                 and self.slot.start_requests is None \
-                and self.enqueue_unlock and self.enqueue_cache.empty() \
                 and not await self.scheduler.has_pending_requests() \
                 and self.is_idle():
             await self.stop(reason='finished')
```

### Comparing `aio-scrapy-2.0.9/aioscrapy/core/scheduler.py` & `aio-scrapy-2.1.0/aioscrapy/core/scheduler.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 class BaseScheduler(metaclass=BaseSchedulerMeta):
 
     @classmethod
     async def from_crawler(cls, crawler: "aioscrapy.Crawler") -> "BaseScheduler":
         """
-        Factory method which receives the current :class:`~scrapy.crawler.Crawler` object as argument.
+        Factory method which receives the current :class:`~aioscrapy.crawler.Crawler` object as argument.
         """
         return cls()
 
     async def close(self, reason: str) -> None:
         """
         Called when the spider is closed by the engine. It receives the reason why the crawl
         finished as argument and it's useful to execute cleaning code.
@@ -99,58 +99,99 @@
 class Scheduler(BaseScheduler):
 
     def __init__(
             self,
             queue: AbsQueue,
             spider: aioscrapy.Spider,
             stats=Optional[StatsCollector],
-            persist: bool = True
+            persist: bool = True,
+            cache_queue: Optional[AbsQueue] = None
     ):
+
         self.queue = queue
+        self.cache_queue = cache_queue
         self.spider = spider
         self.stats = stats
         self.persist = persist
 
     @classmethod
     async def from_crawler(cls: Type[SchedulerTV], crawler: "aioscrapy.Crawler") -> SchedulerTV:
+        cache_queue = None
+        if crawler.settings.getbool('USE_SCHEDULER_QUEUE_CACHE', False):
+            cache_queue = await load_instance('aioscrapy.queue.memory.SpiderPriorityQueue', spider=crawler.spider)
         instance = cls(
             await load_instance(crawler.settings['SCHEDULER_QUEUE_CLASS'], spider=crawler.spider),
             crawler.spider,
             stats=crawler.stats,
-            persist=crawler.settings.getbool('SCHEDULER_PERSIST', True)
+            persist=crawler.settings.getbool('SCHEDULER_PERSIST', True),
+            cache_queue=cache_queue
         )
 
         if crawler.settings.getbool('SCHEDULER_FLUSH_ON_START', False):
             await instance.flush()
 
         count = await call_helper(instance.queue.len)
         count and logger.info("Resuming crawl (%d requests scheduled)" % count)
 
         return instance
 
     async def close(self, reason: str) -> None:
+
         if not self.persist:
             await self.flush()
+            return
+
+        # 如果持久化，将缓存中的任务放回到redis等分布式队列中
+        if self.cache_queue is not None:
+            while True:
+                temp = []
+                async for request in self.cache_queue.pop(2000):
+                    temp.append(request)
+                temp and await self.queue.push_batch(temp)
+                if len(temp) < 2000:
+                    break
 
     async def flush(self) -> None:
         await call_helper(self.queue.clear)
 
     async def enqueue_request_batch(self, requests: List[aioscrapy.Request]) -> bool:
         await call_helper(self.queue.push_batch, requests)
         if self.stats:
             self.stats.inc_value(self.queue.inc_key, count=len(requests), spider=self.spider)
         return True
 
     async def enqueue_request(self, request: aioscrapy.Request) -> bool:
-        await call_helper(self.queue.push, request)
+        """
+        如果启用了缓存队列(USE_SCHEDULER_QUEUE_CACHE)，则优先将任务放到缓存队列中
+        """
+        if self.cache_queue is not None:
+            await call_helper(self.cache_queue.push, request)
+        else:
+            await call_helper(self.queue.push, request)
         if self.stats:
             self.stats.inc_value(self.queue.inc_key, spider=self.spider)
         return True
 
     async def next_request(self, count: int = 1) -> Optional[aioscrapy.Request]:
+        """
+        如果启用了缓存队列(USE_SCHEDULER_QUEUE_CACHE)，则优先从缓存队列中获取任务，然后从redis等分布式队列中获取任务
+        """
+        flag = False
+        if self.cache_queue is not None:
+            async for request in self.cache_queue.pop(count):
+                if request and self.stats:
+                    self.stats.inc_value(self.queue.inc_key, spider=self.spider)
+                yield request
+                flag = True
+
+        if flag:
+            return
+
         async for request in self.queue.pop(count):
             if request and self.stats:
                 self.stats.inc_value(self.queue.inc_key, spider=self.spider)
             yield request
 
+
     async def has_pending_requests(self) -> bool:
-        return await call_helper(self.queue.len) > 0
+        return await call_helper(self.queue.len) if self.cache_queue is None \
+            else (await call_helper(self.queue.len) + await call_helper(self.cache_queue.len)) > 0
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aio-scrapy-2.0.9/aioscrapy/core/scraper.py` & `aio-scrapy-2.1.0/aioscrapy/core/scraper.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/crawler.py` & `aio-scrapy-2.1.0/aioscrapy/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,17 +230,20 @@
             for crawler, (args, kwargs) in self.crawlers.items():
                 self.active_crawler(crawler, *args, **kwargs)
             while self._active:
                 await asyncio.gather(*self._active)
         finally:
             await self.recycle_db_connect()
 
-    def start(self) -> None:
+    def start(self, use_windows_selector_eventLoop: bool = False) -> None:
         if sys.platform.startswith('win'):
-            asyncio.set_event_loop(asyncio.windows_events.ProactorEventLoop())
+            if use_windows_selector_eventLoop:
+                asyncio.set_event_loop_policy(asyncio.windows_events.WindowsSelectorEventLoopPolicy())
+            else:
+                asyncio.set_event_loop(asyncio.windows_events.ProactorEventLoop())
         else:
             try:
                 import uvloop
                 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
             except ImportError:
                 pass
         asyncio.run(self.run())
```

### Comparing `aio-scrapy-2.0.9/aioscrapy/db/__init__.py` & `aio-scrapy-2.1.0/aioscrapy/db/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/db/absmanager.py` & `aio-scrapy-2.1.0/aioscrapy/db/absmanager.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/db/aiomongo.py` & `aio-scrapy-2.1.0/aioscrapy/db/aiomongo.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/db/aiomysql.py` & `aio-scrapy-2.1.0/aioscrapy/db/aiomysql.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/db/aiopg.py` & `aio-scrapy-2.1.0/aioscrapy/db/aiopg.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/db/aiorabbitmq.py` & `aio-scrapy-2.1.0/aioscrapy/db/aiorabbitmq.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/db/aioredis.py` & `aio-scrapy-2.1.0/aioscrapy/db/aioredis.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/dupefilters/__init__.py` & `aio-scrapy-2.1.0/aioscrapy/dupefilters/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/dupefilters/disk.py` & `aio-scrapy-2.1.0/aioscrapy/dupefilters/disk.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/dupefilters/redis.py` & `aio-scrapy-2.1.0/aioscrapy/dupefilters/redis.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     @classmethod
     def from_crawler(cls, crawler: "aioscrapy.crawler.Crawler"):
         server = db_manager.redis.queue
         dupefilter_key = crawler.settings.get("SCHEDULER_DUPEFILTER_KEY", '%(spider)s:dupefilter')
         keep_on_close = crawler.settings.getbool("KEEP_DUPEFILTER_DATA_ON_CLOSE", True)
         key = dupefilter_key % {'spider': crawler.spider.name}
         debug = crawler.settings.getbool('DUPEFILTER_DEBUG', False)
-        info = crawler.settings.getbool('DUPEFILTER_DEBUG', False)
+        info = crawler.settings.getbool('DUPEFILTER_INFO', False)
         instance = cls(server, key=key, debug=debug, keep_on_close=keep_on_close, info=info)
         return instance
 
     async def request_seen(self, request: Request):
         return await self.server.sadd(self.key, request.fingerprint) == 0
 
     async def close(self, reason=''):
@@ -98,30 +98,31 @@
                 pipe.setbit(self.key, offset, 1)
             await pipe.execute()
 
 
 class RedisBloomDupeFilter(RedisRFPDupeFilter):
     """Bloom filter built with the bitis bitmap of redis"""
 
-    def __init__(self, server, key, debug, bit, hash_number, keep_on_close):
-        super().__init__(server, key, debug, keep_on_close)
+    def __init__(self, server, key, debug, bit, hash_number, keep_on_close, info):
+        super().__init__(server, key, debug, keep_on_close, info)
         self.bit = bit
         self.hash_number = hash_number
         self.bf = BloomFilter(server, self.key, bit, hash_number)
 
     @classmethod
     async def from_crawler(cls, crawler: "aioscrapy.crawler.Crawler"):
         server = db_manager.redis.queue
         dupefilter_key = crawler.settings.get("SCHEDULER_DUPEFILTER_KEY", '%(spider)s:bloomfilter')
         keep_on_close = crawler.settings.getbool("KEEP_DUPEFILTER_DATA_ON_CLOSE", True)
         key = dupefilter_key % {'spider': crawler.spider.name}
         debug = crawler.settings.getbool('DUPEFILTER_DEBUG', False)
+        info = crawler.settings.getbool('DUPEFILTER_INFO', False)
         bit = crawler.settings.getint('BLOOMFILTER_BIT', 30)
         hash_number = crawler.settings.getint('BLOOMFILTER_HASH_NUMBER', 6)
-        return cls(server, key=key, debug=debug, bit=bit, hash_number=hash_number, keep_on_close=keep_on_close)
+        return cls(server, key=key, debug=debug, bit=bit, hash_number=hash_number, keep_on_close=keep_on_close, info=info)
 
     async def request_seen(self, request: Request) -> bool:
         fp = await self.bf.exists(request.fingerprint)
         if fp:
             return True
         await self.bf.insert(request.fingerprint)
         return False
```

### Comparing `aio-scrapy-2.0.9/aioscrapy/exceptions.py` & `aio-scrapy-2.1.0/aioscrapy/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/http/__init__.py` & `aio-scrapy-2.1.0/aioscrapy/http/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/http/headers.py` & `aio-scrapy-2.1.0/aioscrapy/http/headers.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/http/request/__init__.py` & `aio-scrapy-2.1.0/aioscrapy/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/http/request/form.py` & `aio-scrapy-2.1.0/aioscrapy/http/request/form.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/http/request/json_request.py` & `aio-scrapy-2.1.0/aioscrapy/http/request/json_request.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/http/response/__init__.py` & `aio-scrapy-2.1.0/aioscrapy/http/response/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/http/response/playwright.py` & `aio-scrapy-2.1.0/aioscrapy/http/response/playwright.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/http/response/text.py` & `aio-scrapy-2.1.0/aioscrapy/http/response/text.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/downloader/defaultheaders.py` & `aio-scrapy-2.1.0/aioscrapy/libs/downloader/defaultheaders.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/downloader/downloadtimeout.py` & `aio-scrapy-2.1.0/aioscrapy/libs/downloader/downloadtimeout.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/downloader/ja3fingerprint.py` & `aio-scrapy-2.1.0/aioscrapy/libs/downloader/ja3fingerprint.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/downloader/retry.py` & `aio-scrapy-2.1.0/aioscrapy/libs/downloader/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,22 @@
 try:
     from playwright._impl._api_types import Error as PlaywrightError
 
     NEED_RETRY_ERROR += (PlaywrightError,)
 except ImportError:
     pass
 
+
+try:
+    from curl_cffi.curl import CurlError
+
+    NEED_RETRY_ERROR += (CurlError,)
+except ImportError:
+    pass
+
 from aioscrapy.exceptions import NotConfigured
 from aioscrapy.http.request import Request
 from aioscrapy.spiders import Spider
 from aioscrapy.utils.python import global_object_name
 from aioscrapy.utils.log import logger as retry_logger
```

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/downloader/stats.py` & `aio-scrapy-2.1.0/aioscrapy/libs/downloader/stats.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/downloader/useragent.py` & `aio-scrapy-2.1.0/aioscrapy/libs/downloader/useragent.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/extensions/closespider.py` & `aio-scrapy-2.1.0/aioscrapy/libs/extensions/closespider.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/extensions/corestats.py` & `aio-scrapy-2.1.0/aioscrapy/libs/extensions/corestats.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/extensions/logstats.py` & `aio-scrapy-2.1.0/aioscrapy/libs/extensions/logstats.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/extensions/metric.py` & `aio-scrapy-2.1.0/aioscrapy/libs/extensions/metric.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/extensions/throttle.py` & `aio-scrapy-2.1.0/aioscrapy/libs/extensions/throttle.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/pipelines/__init__.py` & `aio-scrapy-2.1.0/aioscrapy/libs/pipelines/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,33 +4,30 @@
 from aioscrapy.utils.tools import create_task
 
 
 class SqlFormat:
 
     @staticmethod
     def pg_insert(table: str, fields: list, *args) -> str:
-        fields = ','.join(fields)
         placeholder = ','.join([f'${i + 1}' for i in range(len(fields))])
-        return f'''INSERT INTO {table} ({fields}) VALUES ({placeholder})'''
+        return f'''INSERT INTO {table} ({",".join(fields)}) VALUES ({placeholder})'''
 
     @staticmethod
     def pg_ignore_insert(table: str, fields: list, *args) -> str:
         placeholder = ','.join([f'${i + 1}' for i in range(len(fields))])
-        fields = ','.join(fields)
-        return f'INSERT INTO {table} ({fields}) VALUES ({placeholder}) ON CONFLICT DO NOTHING'
+        return f'''INSERT INTO {table} ({",".join(fields)}) VALUES ({placeholder}) ON CONFLICT DO NOTHING'''
 
     @staticmethod
     def pg_update_insert(table: str, fields: list, update_fields: list, on_conflict: str, *args) -> str:
         assert on_conflict is not None, "on_conflict must be str, eg: 'id'"
         placeholder = ','.join([f'${i + 1}' for i in range(len(fields))])
         if not update_fields:
             update_fields = fields
         update_fields = ','.join([f"{key} = excluded.{key}" for key in update_fields])
-        fields = ','.join(fields)
-        return f'INSERT INTO {table} ({fields}) VALUES ({placeholder}) ON CONFLICT({on_conflict}) DO UPDATE SET {update_fields}'
+        return f'''INSERT INTO {table} ({",".join(fields)}) VALUES ({placeholder}) ON CONFLICT({on_conflict}) DO UPDATE SET {update_fields}'''
 
     @staticmethod
     def mysql_insert(table: str, fields: list, *args) -> str:
         placeholder = ','.join(['%s'] * len(fields))
         fields = ','.join(fields)
         return f'''INSERT INTO {table} ({fields}) VALUES ({placeholder})'''
```

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/pipelines/csv.py` & `aio-scrapy-2.1.0/aioscrapy/libs/pipelines/csv.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/pipelines/execl.py` & `aio-scrapy-2.1.0/aioscrapy/libs/pipelines/execl.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/pipelines/mongo.py` & `aio-scrapy-2.1.0/aioscrapy/libs/pipelines/mongo.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/pipelines/mysql.py` & `aio-scrapy-2.1.0/aioscrapy/libs/pipelines/mysql.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/pipelines/pg.py` & `aio-scrapy-2.1.0/aioscrapy/libs/pipelines/pg.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/spider/depth.py` & `aio-scrapy-2.1.0/aioscrapy/libs/spider/depth.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/spider/httperror.py` & `aio-scrapy-2.1.0/aioscrapy/libs/spider/httperror.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/spider/offsite.py` & `aio-scrapy-2.1.0/aioscrapy/libs/spider/offsite.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/spider/referer.py` & `aio-scrapy-2.1.0/aioscrapy/libs/spider/referer.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/libs/spider/urllength.py` & `aio-scrapy-2.1.0/aioscrapy/libs/spider/urllength.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/link.py` & `aio-scrapy-2.1.0/aioscrapy/link.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/logformatter.py` & `aio-scrapy-2.1.0/aioscrapy/logformatter.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/middleware/absmanager.py` & `aio-scrapy-2.1.0/aioscrapy/middleware/absmanager.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/middleware/downloader.py` & `aio-scrapy-2.1.0/aioscrapy/middleware/downloader.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/middleware/itempipeline.py` & `aio-scrapy-2.1.0/aioscrapy/middleware/itempipeline.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/middleware/spider.py` & `aio-scrapy-2.1.0/aioscrapy/middleware/spider.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/process.py` & `aio-scrapy-2.1.0/aioscrapy/process.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/proxy/__init__.py` & `aio-scrapy-2.1.0/aioscrapy/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/proxy/redis.py` & `aio-scrapy-2.1.0/aioscrapy/proxy/redis.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/queue/__init__.py` & `aio-scrapy-2.1.0/aioscrapy/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/queue/memory.py` & `aio-scrapy-2.1.0/aioscrapy/queue/memory.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/queue/rabbitmq.py` & `aio-scrapy-2.1.0/aioscrapy/queue/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/queue/redis.py` & `aio-scrapy-2.1.0/aioscrapy/queue/redis.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/scrapyd/runner.py` & `aio-scrapy-2.1.0/aioscrapy/scrapyd/runner.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/serializer.py` & `aio-scrapy-2.1.0/aioscrapy/serializer.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/settings/__init__.py` & `aio-scrapy-2.1.0/aioscrapy/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/settings/default_settings.py` & `aio-scrapy-2.1.0/aioscrapy/settings/default_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,18 @@
         'http': 'aioscrapy.core.downloader.handlers.pyhttpx.PyhttpxDownloadHandler',
         'https': 'aioscrapy.core.downloader.handlers.pyhttpx.PyhttpxDownloadHandler',
     },
     'playwright': {
         'http': 'aioscrapy.core.downloader.handlers.playwright.PlaywrightHandler',
         'https': 'aioscrapy.core.downloader.handlers.playwright.PlaywrightHandler',
     },
+    'curl_cffi': {
+        'http': 'aioscrapy.core.downloader.handlers.curl_cffi.CurlCffiDownloadHandler',
+        'https': 'aioscrapy.core.downloader.handlers.curl_cffi.CurlCffiDownloadHandler',
+    },
 }
 
 DOWNLOAD_TIMEOUT = 180  # 3mins
 
 DOWNLOADER = 'aioscrapy.core.downloader.Downloader'
 
 DOWNLOADER_MIDDLEWARES = {}
```

### Comparing `aio-scrapy-2.0.9/aioscrapy/signalmanager.py` & `aio-scrapy-2.1.0/aioscrapy/signalmanager.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/signals.py` & `aio-scrapy-2.1.0/aioscrapy/signals.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/spiderloader.py` & `aio-scrapy-2.1.0/aioscrapy/spiderloader.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/spiders/__init__.py` & `aio-scrapy-2.1.0/aioscrapy/spiders/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,21 +102,21 @@
 
     def __str__(self):
         return f"<{type(self).__name__} {self.name!r} at 0x{id(self):0x}>"
 
     __repr__ = __str__
 
     @classmethod
-    def start(cls, setting_path=None):
+    def start(cls, setting_path=None, use_windows_selector_eventLoop: bool = False):
         from aioscrapy.crawler import CrawlerProcess
         from aioscrapy.utils.project import get_project_settings
 
         settings = get_project_settings()
         if setting_path is not None:
             settings.setmodule(setting_path)
         cp = CrawlerProcess(settings)
         cp.crawl(cls)
-        cp.start()
+        cp.start(use_windows_selector_eventLoop)
 
     def spider_idle(self):
         if not self.close_on_idle:
             raise DontCloseSpider
```

### Comparing `aio-scrapy-2.0.9/aioscrapy/statscollectors.py` & `aio-scrapy-2.1.0/aioscrapy/statscollectors.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/templates/project/module/middlewares.py.tmpl` & `aio-scrapy-2.1.0/aioscrapy/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/templates/project/module/settings.py.tmpl` & `aio-scrapy-2.1.0/aioscrapy/templates/project/module/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/templates/spiders/single.tmpl` & `aio-scrapy-2.1.0/aioscrapy/templates/spiders/single.tmpl`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/conf.py` & `aio-scrapy-2.1.0/aioscrapy/utils/conf.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/curl.py` & `aio-scrapy-2.1.0/aioscrapy/utils/curl.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/decorators.py` & `aio-scrapy-2.1.0/aioscrapy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/deprecate.py` & `aio-scrapy-2.1.0/aioscrapy/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/httpobj.py` & `aio-scrapy-2.1.0/aioscrapy/utils/httpobj.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/log.py` & `aio-scrapy-2.1.0/aioscrapy/utils/log.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/misc.py` & `aio-scrapy-2.1.0/aioscrapy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/ossignal.py` & `aio-scrapy-2.1.0/aioscrapy/utils/ossignal.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/project.py` & `aio-scrapy-2.1.0/aioscrapy/utils/project.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/python.py` & `aio-scrapy-2.1.0/aioscrapy/utils/python.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/request.py` & `aio-scrapy-2.1.0/aioscrapy/utils/request.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/response.py` & `aio-scrapy-2.1.0/aioscrapy/utils/response.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/signal.py` & `aio-scrapy-2.1.0/aioscrapy/utils/signal.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/spider.py` & `aio-scrapy-2.1.0/aioscrapy/utils/spider.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/template.py` & `aio-scrapy-2.1.0/aioscrapy/utils/template.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/tools.py` & `aio-scrapy-2.1.0/aioscrapy/utils/tools.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/trackref.py` & `aio-scrapy-2.1.0/aioscrapy/utils/trackref.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/aioscrapy/utils/url.py` & `aio-scrapy-2.1.0/aioscrapy/utils/url.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.9/setup.py` & `aio-scrapy-2.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,23 @@
     "aiomultiprocess>=0.9.0",
     "loguru>=0.7.0",
 ]
 extras_require = {
     "all": [
         "aiomysql>=0.1.1", "httpx[http2]>=0.23.0", "aio-pika>=8.1.1",
         "cryptography", "motor>=3.1.1", "pyhttpx>=2.10.1", "asyncpg>=0.27.0",
-        "XlsxWriter>=3.1.2", "pillow>=9.4.0", "requests>=2.28.2"
+        "XlsxWriter>=3.1.2", "pillow>=9.4.0", "requests>=2.28.2", "curl_cffi"
     ],
     "aiomysql": ["aiomysql>=0.1.1", "cryptography"],
     "httpx": ["httpx[http2]>=0.23.0"],
     "aio-pika": ["aio-pika>=8.1.1"],
     "mongo": ["motor>=3.1.1"],
     "playwright": ["playwright>=1.31.1"],
     "pyhttpx": ["pyhttpx>=2.10.4"],
+    "curl_cffi": ["curl_cffi>=0.6.1"],
     "requests": ["requests>=2.28.2"],
     "pg": ["asyncpg>=0.27.0"],
     "execl": ["XlsxWriter>=3.1.2", "pillow>=9.4.0"],
 }
 
 setup(
     name='aio-scrapy',
```

