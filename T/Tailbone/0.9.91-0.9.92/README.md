# Comparing `tmp/tailbone-0.9.91.tar.gz` & `tmp/tailbone-0.9.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailbone-0.9.91.tar", last modified: Mon Apr 15 15:57:40 2024, max compression
+gzip compressed data, was "tailbone-0.9.92.tar", last modified: Tue Apr 16 15:44:49 2024, max compression
```

## Comparing `tailbone-0.9.91.tar` & `tailbone-0.9.92.tar`

### file list

```diff
@@ -1,513 +1,513 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.276757 tailbone-0.9.91/
--rw-r--r--   0 lance     (1000) lance     (1000)   160360 2024-04-15 15:56:22.000000 tailbone-0.9.91/CHANGES.rst
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2018-03-01 00:58:49.000000 tailbone-0.9.91/COPYING.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      489 2022-01-13 00:06:52.000000 tailbone-0.9.91/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     2573 2024-04-15 15:57:40.276757 tailbone-0.9.91/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      269 2014-04-22 17:10:45.000000 tailbone-0.9.91/README.rst
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.276757 tailbone-0.9.91/Tailbone.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     2573 2024-04-15 15:57:40.000000 tailbone-0.9.91/Tailbone.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)    14749 2024-04-15 15:57:40.000000 tailbone-0.9.91/Tailbone.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2024-04-15 15:57:40.000000 tailbone-0.9.91/Tailbone.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      272 2024-04-15 15:57:40.000000 tailbone-0.9.91/Tailbone.egg-info/entry_points.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2024-04-15 15:57:40.000000 tailbone-0.9.91/Tailbone.egg-info/not-zip-safe
--rw-r--r--   0 lance     (1000) lance     (1000)      448 2024-04-15 15:57:40.000000 tailbone-0.9.91/Tailbone.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        9 2024-04-15 15:57:40.000000 tailbone-0.9.91/Tailbone.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)     2128 2024-04-15 15:57:40.276757 tailbone-0.9.91/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     1008 2023-05-16 20:02:32.000000 tailbone-0.9.91/setup.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/
--rw-r--r--   0 lance     (1000) lance     (1000)     1161 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       49 2024-04-15 15:56:39.000000 tailbone-0.9.91/tailbone/_version.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/api/
--rw-r--r--   0 lance     (1000) lance     (1000)     1389 2022-08-14 05:48:55.000000 tailbone-0.9.91/tailbone/api/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7865 2023-05-17 04:11:43.000000 tailbone-0.9.91/tailbone/api/auth.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/api/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)     1097 2019-11-11 20:08:35.000000 tailbone-0.9.91/tailbone/api/batch/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    12760 2023-11-02 00:42:53.000000 tailbone-0.9.91/tailbone/api/batch/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7150 2023-11-15 15:46:15.000000 tailbone-0.9.91/tailbone/api/batch/inventory.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2688 2022-08-14 05:59:35.000000 tailbone-0.9.91/tailbone/api/batch/labels.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11993 2024-04-11 18:51:54.000000 tailbone-0.9.91/tailbone/api/batch/ordering.py
--rw-r--r--   0 lance     (1000) lance     (1000)    20740 2024-04-11 19:12:25.000000 tailbone-0.9.91/tailbone/api/batch/receiving.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5099 2023-05-17 04:34:48.000000 tailbone-0.9.91/tailbone/api/common.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4643 2023-06-17 03:15:35.000000 tailbone-0.9.91/tailbone/api/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1833 2022-08-14 05:48:19.000000 tailbone-0.9.91/tailbone/api/customers.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1202 2023-05-20 00:29:29.000000 tailbone-0.9.91/tailbone/api/essentials.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1547 2023-01-30 00:46:27.000000 tailbone-0.9.91/tailbone/api/labels.py
--rw-r--r--   0 lance     (1000) lance     (1000)    21938 2023-10-08 17:24:00.000000 tailbone-0.9.91/tailbone/api/master.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1489 2022-08-14 05:42:00.000000 tailbone-0.9.91/tailbone/api/master2.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1802 2022-08-14 05:49:24.000000 tailbone-0.9.91/tailbone/api/people.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7461 2023-09-02 15:55:47.000000 tailbone-0.9.91/tailbone/api/products.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2126 2022-08-14 05:50:11.000000 tailbone-0.9.91/tailbone/api/upgrades.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2181 2023-05-03 00:13:09.000000 tailbone-0.9.91/tailbone/api/users.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1719 2022-08-14 05:51:19.000000 tailbone-0.9.91/tailbone/api/vendors.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8607 2022-08-31 02:51:40.000000 tailbone-0.9.91/tailbone/api/workorders.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11334 2023-10-24 01:35:10.000000 tailbone-0.9.91/tailbone/app.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3290 2022-08-17 00:32:35.000000 tailbone-0.9.91/tailbone/asgi.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6324 2023-05-15 13:10:42.000000 tailbone-0.9.91/tailbone/auth.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5418 2022-12-07 20:00:13.000000 tailbone-0.9.91/tailbone/beaker.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2691 2022-12-24 05:29:45.000000 tailbone-0.9.91/tailbone/cleanup.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2366 2024-04-13 14:19:43.000000 tailbone-0.9.91/tailbone/config.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8274 2023-02-07 18:19:37.000000 tailbone-0.9.91/tailbone/db.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9796 2023-12-01 00:13:00.000000 tailbone-0.9.91/tailbone/diffs.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1696 2020-02-28 23:40:40.000000 tailbone-0.9.91/tailbone/exceptions.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/forms/
--rw-r--r--   0 lance     (1000) lance     (1000)     1107 2023-09-17 00:47:36.000000 tailbone-0.9.91/tailbone/forms/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1995 2023-02-12 04:03:46.000000 tailbone-0.9.91/tailbone/forms/common.py
--rw-r--r--   0 lance     (1000) lance     (1000)    49572 2024-04-15 01:24:25.000000 tailbone-0.9.91/tailbone/forms/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2361 2023-08-29 21:08:45.000000 tailbone-0.9.91/tailbone/forms/receiving.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7041 2023-10-09 20:50:24.000000 tailbone-0.9.91/tailbone/forms/types.py
--rw-r--r--   0 lance     (1000) lance     (1000)    20432 2024-04-15 01:23:41.000000 tailbone-0.9.91/tailbone/forms/widgets.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/grids/
--rw-r--r--   0 lance     (1000) lance     (1000)     1077 2021-01-30 20:30:05.000000 tailbone-0.9.91/tailbone/grids/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    70674 2024-04-15 01:45:42.000000 tailbone-0.9.91/tailbone/grids/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)    40585 2023-12-11 19:49:51.000000 tailbone-0.9.91/tailbone/grids/filters.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2730 2023-01-16 18:44:24.000000 tailbone-0.9.91/tailbone/handler.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1883 2023-05-05 02:26:43.000000 tailbone-0.9.91/tailbone/helpers.py
--rw-r--r--   0 lance     (1000) lance     (1000)    29626 2023-10-29 20:45:59.000000 tailbone-0.9.91/tailbone/menus.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3466 2022-08-20 22:12:54.000000 tailbone-0.9.91/tailbone/progress.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1901 2023-01-15 00:47:07.000000 tailbone-0.9.91/tailbone/providers.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/reports/
--rw-rw-r--   0 lance     (1000) lance     (1000)     2481 2016-12-17 08:48:19.000000 tailbone-0.9.91/tailbone/reports/inventory_worksheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3577 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/reports/ordering_worksheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1632 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/scaffolds.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/static/
--rw-r--r--   0 lance     (1000) lance     (1000)     1152 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/static/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/static/css/
--rw-r--r--   0 lance     (1000) lance     (1000)      440 2021-01-30 19:10:34.000000 tailbone-0.9.91/tailbone/static/css/base.css
--rw-r--r--   0 lance     (1000) lance     (1000)     4880 2021-01-17 02:38:15.000000 tailbone-0.9.91/tailbone/static/css/codehilite.css
--rw-r--r--   0 lance     (1000) lance     (1000)      789 2020-08-02 03:09:36.000000 tailbone-0.9.91/tailbone/static/css/diffs.css
--rw-r--r--   0 lance     (1000) lance     (1000)      390 2023-02-02 22:24:46.000000 tailbone-0.9.91/tailbone/static/css/filters.css
--rw-r--r--   0 lance     (1000) lance     (1000)     1439 2023-02-02 22:24:46.000000 tailbone-0.9.91/tailbone/static/css/forms.css
--rw-r--r--   0 lance     (1000) lance     (1000)     5542 2023-02-03 23:02:02.000000 tailbone-0.9.91/tailbone/static/css/grids.css
--rw-r--r--   0 lance     (1000) lance     (1000)     1167 2024-04-15 01:28:38.000000 tailbone-0.9.91/tailbone/static/css/grids.rowstatus.css
--rw-r--r--   0 lance     (1000) lance     (1000)     2671 2023-10-25 15:44:50.000000 tailbone-0.9.91/tailbone/static/css/layout.css
--rw-r--r--   0 lance     (1000) lance     (1000)     7346 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/css/normalize.css
--rw-r--r--   0 lance     (1000) lance     (1000)      575 2019-06-05 00:52:33.000000 tailbone-0.9.91/tailbone/static/css/perms.css
--rw-r--r--   0 lance     (1000) lance     (1000)      965 2023-02-02 22:24:46.000000 tailbone-0.9.91/tailbone/static/css/progress.css
--rw-r--r--   0 lance     (1000) lance     (1000)      208 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/static/css/purchases.css
--rw-rw-r--   0 lance     (1000) lance     (1000)      225 2016-12-17 08:48:19.000000 tailbone-0.9.91/tailbone/static/css/schedule_print.css
--rw-rw-r--   0 lance     (1000) lance     (1000)     1664 2017-07-18 18:57:10.000000 tailbone-0.9.91/tailbone/static/css/timesheet.css
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/static/files/
--rw-r--r--   0 lance     (1000) lance     (1000)     5041 2022-08-30 13:52:10.000000 tailbone-0.9.91/tailbone/static/files/newproduct_template.xlsx
--rw-r--r--   0 lance     (1000) lance     (1000)     7593 2022-01-06 18:40:01.000000 tailbone-0.9.91/tailbone/static/files/vendor_catalog_template.xlsx
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.256757 tailbone-0.9.91/tailbone/static/img/
--rw-r--r--   0 lance     (1000) lance     (1000)   107339 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/Hymenocephalus_italicus.jpg
--rw-r--r--   0 lance     (1000) lance     (1000)      641 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/delete.png
--rw-r--r--   0 lance     (1000) lance     (1000)      533 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/edit.png
--rw-r--r--   0 lance     (1000) lance     (1000)    20687 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/home_logo.png
--rw-r--r--   0 lance     (1000) lance     (1000)      771 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/loading.gif
--rw-rw-r--   0 lance     (1000) lance     (1000)     2077 2016-12-17 08:48:19.000000 tailbone-0.9.91/tailbone/static/img/product.png
--rw-r--r--   0 lance     (1000) lance     (1000)     5694 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/rattail.ico
--rw-r--r--   0 lance     (1000) lance     (1000)      542 2015-03-10 02:10:41.000000 tailbone-0.9.91/tailbone/static/img/save.png
--rw-r--r--   0 lance     (1000) lance     (1000)      158 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/sort_arrow_down.png
--rw-r--r--   0 lance     (1000) lance     (1000)      169 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/sort_arrow_up.png
--rw-rw-r--   0 lance     (1000) lance     (1000)    10375 2022-11-21 03:00:53.000000 tailbone-0.9.91/tailbone/static/img/testing.png
--rw-r--r--   0 lance     (1000) lance     (1000)      616 2013-09-10 19:45:39.000000 tailbone-0.9.91/tailbone/static/img/view.png
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/static/js/
--rw-r--r--   0 lance     (1000) lance     (1000)      813 2021-10-12 18:14:50.000000 tailbone-0.9.91/tailbone/static/js/debounce.js
--rw-r--r--   0 lance     (1000) lance     (1000)     2380 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/static/js/numeric.js
--rw-r--r--   0 lance     (1000) lance     (1000)     9498 2023-10-26 01:03:48.000000 tailbone-0.9.91/tailbone/static/js/tailbone.buefy.autocomplete.js
--rw-r--r--   0 lance     (1000) lance     (1000)     1634 2020-11-25 22:42:00.000000 tailbone-0.9.91/tailbone/static/js/tailbone.buefy.datepicker.js
--rw-r--r--   0 lance     (1000) lance     (1000)     4561 2023-06-16 17:21:44.000000 tailbone-0.9.91/tailbone/static/js/tailbone.buefy.grid.js
--rw-r--r--   0 lance     (1000) lance     (1000)     3407 2019-11-05 01:06:58.000000 tailbone-0.9.91/tailbone/static/js/tailbone.buefy.message_recipients.js
--rw-r--r--   0 lance     (1000) lance     (1000)     1514 2022-07-26 20:56:38.000000 tailbone-0.9.91/tailbone/static/js/tailbone.buefy.numericinput.js
--rw-r--r--   0 lance     (1000) lance     (1000)     1637 2019-06-24 23:30:10.000000 tailbone-0.9.91/tailbone/static/js/tailbone.buefy.oncebutton.js
--rw-r--r--   0 lance     (1000) lance     (1000)     1403 2023-09-17 00:42:09.000000 tailbone-0.9.91/tailbone/static/js/tailbone.buefy.timepicker.js
--rw-r--r--   0 lance     (1000) lance     (1000)     1427 2023-06-06 16:53:17.000000 tailbone-0.9.91/tailbone/static/js/tailbone.feedback.js
--rw-r--r--   0 lance     (1000) lance     (1000)       26 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/static/robots.txt
--rw-r--r--   0 lance     (1000) lance     (1000)    10220 2024-04-15 01:55:42.000000 tailbone-0.9.91/tailbone/subscribers.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/
--rw-r--r--   0 lance     (1000) lance     (1000)      471 2019-08-03 00:53:47.000000 tailbone-0.9.91/tailbone/templates/about.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/appinfo/
--rw-r--r--   0 lance     (1000) lance     (1000)     7318 2023-02-02 00:31:53.000000 tailbone-0.9.91/tailbone/templates/appinfo/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3270 2023-10-24 14:53:32.000000 tailbone-0.9.91/tailbone/templates/appinfo/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     6317 2024-04-14 23:27:37.000000 tailbone-0.9.91/tailbone/templates/appsettings.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      899 2023-02-03 22:40:11.000000 tailbone-0.9.91/tailbone/templates/autocomplete.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    33683 2023-11-17 23:00:34.000000 tailbone-0.9.91/tailbone/templates/base.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      772 2021-11-04 22:56:35.000000 tailbone-0.9.91/tailbone/templates/base_meta.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)       84 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/batch/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       81 2019-06-08 19:26:19.000000 tailbone-0.9.91/tailbone/templates/batch/edit.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/batch/importer/
--rw-r--r--   0 lance     (1000) lance     (1000)     2381 2024-04-15 00:15:19.000000 tailbone-0.9.91/tailbone/templates/batch/importer/view_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     4716 2023-02-03 05:51:09.000000 tailbone-0.9.91/tailbone/templates/batch/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/batch/inventory/
--rw-r--r--   0 lance     (1000) lance     (1000)    10321 2024-04-15 00:11:34.000000 tailbone-0.9.91/tailbone/templates/batch/inventory/desktop_form.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/batch/newproduct/
--rw-r--r--   0 lance     (1000) lance     (1000)      160 2022-08-30 15:56:25.000000 tailbone-0.9.91/tailbone/templates/batch/newproduct/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/batch/pos/
--rw-r--r--   0 lance     (1000) lance     (1000)      285 2023-10-07 04:17:54.000000 tailbone-0.9.91/tailbone/templates/batch/pos/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/batch/pricing/
--rw-r--r--   0 lance     (1000) lance     (1000)      536 2022-06-14 18:18:31.000000 tailbone-0.9.91/tailbone/templates/batch/pricing/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/batch/vendorcatalog/
--rw-r--r--   0 lance     (1000) lance     (1000)     1388 2022-01-08 19:35:47.000000 tailbone-0.9.91/tailbone/templates/batch/vendorcatalog/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1288 2023-02-03 05:42:10.000000 tailbone-0.9.91/tailbone/templates/batch/vendorcatalog/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      309 2022-01-06 18:52:39.000000 tailbone-0.9.91/tailbone/templates/batch/vendorcatalog/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      241 2024-04-15 00:15:22.000000 tailbone-0.9.91/tailbone/templates/batch/vendorcatalog/view_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    11890 2024-04-15 00:15:17.000000 tailbone-0.9.91/tailbone/templates/batch/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      509 2023-02-03 05:50:25.000000 tailbone-0.9.91/tailbone/templates/batch/worksheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      121 2020-03-24 00:26:09.000000 tailbone-0.9.91/tailbone/templates/change_password.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    13008 2023-01-17 03:55:16.000000 tailbone-0.9.91/tailbone/templates/configure-menus.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     9425 2023-01-16 17:56:04.000000 tailbone-0.9.91/tailbone/templates/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/customers/
--rw-r--r--   0 lance     (1000) lance     (1000)     3775 2023-06-11 18:38:46.000000 tailbone-0.9.91/tailbone/templates/customers/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/customers/pending/
--rw-r--r--   0 lance     (1000) lance     (1000)     5021 2021-12-24 01:59:01.000000 tailbone-0.9.91/tailbone/templates/customers/pending/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1096 2024-04-15 01:26:15.000000 tailbone-0.9.91/tailbone/templates/customers/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/custorders/
--rw-r--r--   0 lance     (1000) lance     (1000)     6522 2023-10-25 00:29:26.000000 tailbone-0.9.91/tailbone/templates/custorders/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    92495 2023-10-26 14:28:39.000000 tailbone-0.9.91/tailbone/templates/custorders/create.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/custorders/items/
--rw-r--r--   0 lance     (1000) lance     (1000)    16040 2024-04-15 00:15:26.000000 tailbone-0.9.91/tailbone/templates/custorders/items/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       81 2023-09-10 19:59:06.000000 tailbone-0.9.91/tailbone/templates/custorders/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/datasync/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.260757 tailbone-0.9.91/tailbone/templates/datasync/changes/
--rw-r--r--   0 lance     (1000) lance     (1000)     2125 2023-02-03 05:54:34.000000 tailbone-0.9.91/tailbone/templates/datasync/changes/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    31019 2023-02-02 00:43:40.000000 tailbone-0.9.91/tailbone/templates/datasync/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     5964 2023-02-02 00:35:51.000000 tailbone-0.9.91/tailbone/templates/datasync/status.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/deform/
--rw-r--r--   0 lance     (1000) lance     (1000)      918 2023-02-03 05:52:17.000000 tailbone-0.9.91/tailbone/templates/deform/autocomplete_jquery.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      943 2023-02-03 05:53:06.000000 tailbone-0.9.91/tailbone/templates/deform/cases_units.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      492 2023-02-03 05:54:15.000000 tailbone-0.9.91/tailbone/templates/deform/checkbox.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      545 2021-01-06 00:19:12.000000 tailbone-0.9.91/tailbone/templates/deform/checkbox_dynamic.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     1213 2023-02-03 05:51:23.000000 tailbone-0.9.91/tailbone/templates/deform/checked_password.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      597 2023-02-03 05:53:42.000000 tailbone-0.9.91/tailbone/templates/deform/date_jquery.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      581 2019-02-23 02:44:18.000000 tailbone-0.9.91/tailbone/templates/deform/date_plain.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      543 2023-09-17 01:00:05.000000 tailbone-0.9.91/tailbone/templates/deform/datetime_falafel.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      758 2023-02-03 05:52:34.000000 tailbone-0.9.91/tailbone/templates/deform/file_upload.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      601 2019-11-04 23:21:16.000000 tailbone-0.9.91/tailbone/templates/deform/message_recipients.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      257 2023-01-29 16:59:23.000000 tailbone-0.9.91/tailbone/templates/deform/multi_file_upload.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      963 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/deform/numberinput.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      509 2019-06-28 17:09:23.000000 tailbone-0.9.91/tailbone/templates/deform/numericinput.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      616 2023-02-07 22:10:56.000000 tailbone-0.9.91/tailbone/templates/deform/password.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      710 2023-02-03 05:52:00.000000 tailbone-0.9.91/tailbone/templates/deform/percentinput.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     2102 2023-02-03 05:54:03.000000 tailbone-0.9.91/tailbone/templates/deform/permissions.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      875 2022-11-19 23:40:01.000000 tailbone-0.9.91/tailbone/templates/deform/problem_report_days.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     2164 2023-02-03 05:51:49.000000 tailbone-0.9.91/tailbone/templates/deform/select.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     1177 2023-08-08 19:10:04.000000 tailbone-0.9.91/tailbone/templates/deform/select_dynamic.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     1979 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/deform/select_jquery.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     1718 2019-09-06 22:13:34.000000 tailbone-0.9.91/tailbone/templates/deform/select_plain.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      550 2023-03-23 15:17:29.000000 tailbone-0.9.91/tailbone/templates/deform/textarea.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      894 2023-02-04 01:42:19.000000 tailbone-0.9.91/tailbone/templates/deform/textinput.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      230 2023-09-26 00:21:51.000000 tailbone-0.9.91/tailbone/templates/deform/time_falafel.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      655 2023-02-03 05:53:32.000000 tailbone-0.9.91/tailbone/templates/deform/time_jquery.pt
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/departments/
--rw-rw-r--   0 lance     (1000) lance     (1000)      294 2023-02-03 05:31:15.000000 tailbone-0.9.91/tailbone/templates/departments/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      551 2023-10-09 05:16:53.000000 tailbone-0.9.91/tailbone/templates/diff.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/email-bounces/
--rw-r--r--   0 lance     (1000) lance     (1000)     1659 2023-09-08 15:46:55.000000 tailbone-0.9.91/tailbone/templates/email-bounces/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/employees/
--rw-r--r--   0 lance     (1000) lance     (1000)      626 2023-06-11 04:11:26.000000 tailbone-0.9.91/tailbone/templates/employees/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      259 2019-04-12 19:47:07.000000 tailbone-0.9.91/tailbone/templates/employees/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1170 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/exception.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1506 2024-04-15 00:15:12.000000 tailbone-0.9.91/tailbone/templates/form.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2779 2023-06-17 19:13:31.000000 tailbone-0.9.91/tailbone/templates/formposter.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/forms/
--rw-r--r--   0 lance     (1000) lance     (1000)     7053 2024-04-15 00:03:36.000000 tailbone-0.9.91/tailbone/templates/forms/deform.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    12583 2023-02-02 00:37:54.000000 tailbone-0.9.91/tailbone/templates/generate_feature.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/generated-projects/
--rw-r--r--   0 lance     (1000) lance     (1000)      582 2023-05-04 18:51:55.000000 tailbone-0.9.91/tailbone/templates/generated-projects/create.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/grids/
--rw-r--r--   0 lance     (1000) lance     (1000)     3024 2023-02-02 00:24:21.000000 tailbone-0.9.91/tailbone/templates/grids/b-table.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    28542 2024-04-15 01:40:53.000000 tailbone-0.9.91/tailbone/templates/grids/complete.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1898 2023-10-11 03:10:01.000000 tailbone-0.9.91/tailbone/templates/grids/filters.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      755 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/grids/nav.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      672 2019-08-24 02:39:03.000000 tailbone-0.9.91/tailbone/templates/home.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/ifps-plu-codes/
--rw-r--r--   0 lance     (1000) lance     (1000)      281 2020-12-07 01:28:53.000000 tailbone-0.9.91/tailbone/templates/ifps-plu-codes/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)     6187 2023-02-02 00:43:01.000000 tailbone-0.9.91/tailbone/templates/importing/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      294 2021-12-06 18:34:10.000000 tailbone-0.9.91/tailbone/templates/importing/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2643 2021-12-07 03:29:19.000000 tailbone-0.9.91/tailbone/templates/importing/runjob.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      671 2021-12-07 03:21:19.000000 tailbone-0.9.91/tailbone/templates/importing/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.248757 tailbone-0.9.91/tailbone/templates/labels/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/labels/profiles/
--rw-rw-r--   0 lance     (1000) lance     (1000)      314 2016-12-17 08:48:19.000000 tailbone-0.9.91/tailbone/templates/labels/profiles/create.mako
--rw-rw-r--   0 lance     (1000) lance     (1000)      620 2016-12-17 08:48:19.000000 tailbone-0.9.91/tailbone/templates/labels/profiles/edit.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      432 2019-05-23 22:57:42.000000 tailbone-0.9.91/tailbone/templates/labels/profiles/printer.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1232 2023-02-09 02:19:12.000000 tailbone-0.9.91/tailbone/templates/labels/profiles/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1649 2023-02-07 22:11:44.000000 tailbone-0.9.91/tailbone/templates/login.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/luigi/
--rw-r--r--   0 lance     (1000) lance     (1000)    14033 2023-02-02 00:30:45.000000 tailbone-0.9.91/tailbone/templates/luigi/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    12842 2023-02-02 00:29:33.000000 tailbone-0.9.91/tailbone/templates/luigi/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/master/
--rw-r--r--   0 lance     (1000) lance     (1000)     1364 2024-04-15 00:15:10.000000 tailbone-0.9.91/tailbone/templates/master/clone.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      893 2021-12-14 03:26:58.000000 tailbone-0.9.91/tailbone/templates/master/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      174 2019-05-22 20:24:53.000000 tailbone-0.9.91/tailbone/templates/master/create.mako
--rw-rw-r--   0 lance     (1000) lance     (1000)      248 2016-12-17 08:48:19.000000 tailbone-0.9.91/tailbone/templates/master/create_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1389 2024-04-15 00:15:05.000000 tailbone-0.9.91/tailbone/templates/master/delete.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      226 2023-10-10 02:06:31.000000 tailbone-0.9.91/tailbone/templates/master/edit.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      879 2021-12-13 19:43:47.000000 tailbone-0.9.91/tailbone/templates/master/edit_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      584 2023-02-03 18:10:14.000000 tailbone-0.9.91/tailbone/templates/master/form.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      170 2018-11-23 00:24:59.000000 tailbone-0.9.91/tailbone/templates/master/import_file.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    25086 2024-04-13 15:01:04.000000 tailbone-0.9.91/tailbone/templates/master/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     5560 2023-06-19 02:20:45.000000 tailbone-0.9.91/tailbone/templates/master/merge.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1036 2024-04-13 15:00:59.000000 tailbone-0.9.91/tailbone/templates/master/versions.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    11305 2024-04-13 15:00:53.000000 tailbone-0.9.91/tailbone/templates/master/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      709 2023-02-03 05:26:29.000000 tailbone-0.9.91/tailbone/templates/master/view_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1413 2023-10-10 15:07:41.000000 tailbone-0.9.91/tailbone/templates/master/view_version.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/members/
--rw-r--r--   0 lance     (1000) lance     (1000)     2342 2023-08-26 14:11:45.000000 tailbone-0.9.91/tailbone/templates/members/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      262 2023-06-14 19:01:14.000000 tailbone-0.9.91/tailbone/templates/members/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1686 2023-02-02 22:24:46.000000 tailbone-0.9.91/tailbone/templates/menu.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/messages/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/messages/archive/
--rw-r--r--   0 lance     (1000) lance     (1000)      353 2023-02-03 05:34:09.000000 tailbone-0.9.91/tailbone/templates/messages/archive/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1777 2023-03-23 15:22:59.000000 tailbone-0.9.91/tailbone/templates/messages/create.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/messages/inbox/
--rw-r--r--   0 lance     (1000) lance     (1000)      355 2023-02-03 05:35:57.000000 tailbone-0.9.91/tailbone/templates/messages/inbox/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1761 2023-02-03 05:35:48.000000 tailbone-0.9.91/tailbone/templates/messages/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1101 2019-11-05 01:03:51.000000 tailbone-0.9.91/tailbone/templates/messages/recipients.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/messages/sent/
--rw-rw-r--   0 lance     (1000) lance     (1000)      354 2016-12-17 08:48:19.000000 tailbone-0.9.91/tailbone/templates/messages/sent/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3206 2023-02-03 05:35:31.000000 tailbone-0.9.91/tailbone/templates/messages/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1509 2023-01-29 17:00:34.000000 tailbone-0.9.91/tailbone/templates/multi_file_upload.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/ordering/
--rw-r--r--   0 lance     (1000) lance     (1000)      112 2023-02-03 05:36:48.000000 tailbone-0.9.91/tailbone/templates/ordering/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    16377 2021-02-01 03:51:46.000000 tailbone-0.9.91/tailbone/templates/ordering/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    11560 2023-02-03 05:37:47.000000 tailbone-0.9.91/tailbone/templates/ordering/worksheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1813 2023-08-28 02:36:03.000000 tailbone-0.9.91/tailbone/templates/page.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     7512 2022-12-28 04:29:27.000000 tailbone-0.9.91/tailbone/templates/page_help.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/people/
--rw-r--r--   0 lance     (1000) lance     (1000)     1296 2023-06-17 19:36:29.000000 tailbone-0.9.91/tailbone/templates/people/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3654 2023-02-03 05:40:07.000000 tailbone-0.9.91/tailbone/templates/people/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/people/merge-requests/
--rw-r--r--   0 lance     (1000) lance     (1000)     1183 2023-02-03 05:39:54.000000 tailbone-0.9.91/tailbone/templates/people/merge-requests/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1100 2024-04-15 00:14:52.000000 tailbone-0.9.91/tailbone/templates/people/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    84948 2024-04-15 00:33:25.000000 tailbone-0.9.91/tailbone/templates/people/view_profile.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/poser/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/poser/reports/
--rw-r--r--   0 lance     (1000) lance     (1000)     2382 2022-03-04 00:35:18.000000 tailbone-0.9.91/tailbone/templates/poser/reports/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3917 2022-03-21 22:32:51.000000 tailbone-0.9.91/tailbone/templates/poser/setup.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/poser/views/
--rw-r--r--   0 lance     (1000) lance     (1000)     1120 2022-03-21 22:32:51.000000 tailbone-0.9.91/tailbone/templates/poser/views/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/principal/
--rw-r--r--   0 lance     (1000) lance     (1000)     7971 2024-04-14 23:38:53.000000 tailbone-0.9.91/tailbone/templates/principal/find_by_perm.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      319 2023-10-18 21:45:40.000000 tailbone-0.9.91/tailbone/templates/principal/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/products/
--rw-r--r--   0 lance     (1000) lance     (1000)     3763 2024-04-15 00:12:29.000000 tailbone-0.9.91/tailbone/templates/products/batch.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     4184 2023-08-25 13:40:55.000000 tailbone-0.9.91/tailbone/templates/products/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2929 2023-02-03 05:58:51.000000 tailbone-0.9.91/tailbone/templates/products/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    11948 2023-10-26 15:05:27.000000 tailbone-0.9.91/tailbone/templates/products/lookup.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/products/pending/
--rw-r--r--   0 lance     (1000) lance     (1000)     4913 2023-10-27 01:41:10.000000 tailbone-0.9.91/tailbone/templates/products/pending/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    13263 2024-04-15 00:33:50.000000 tailbone-0.9.91/tailbone/templates/products/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     6614 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/templates/progress.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/purchases/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/purchases/batches/
--rw-r--r--   0 lance     (1000) lance     (1000)      117 2023-02-03 22:16:48.000000 tailbone-0.9.91/tailbone/templates/purchases/batches/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      278 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/purchases/batches/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/purchases/credits/
--rw-r--r--   0 lance     (1000) lance     (1000)     2469 2023-02-03 23:08:13.000000 tailbone-0.9.91/tailbone/templates/purchases/credits/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2630 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/purchases/receiving_worksheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      555 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/purchases/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/receiving/
--rw-r--r--   0 lance     (1000) lance     (1000)     7668 2023-09-17 23:19:14.000000 tailbone-0.9.91/tailbone/templates/receiving/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      117 2023-02-03 05:32:11.000000 tailbone-0.9.91/tailbone/templates/receiving/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1415 2024-04-15 00:18:30.000000 tailbone-0.9.91/tailbone/templates/receiving/declare_credit.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1320 2024-04-15 00:18:40.000000 tailbone-0.9.91/tailbone/templates/receiving/receive_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      305 2018-10-24 22:53:24.000000 tailbone-0.9.91/tailbone/templates/receiving/transform_unit_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    13336 2023-11-02 01:52:57.000000 tailbone-0.9.91/tailbone/templates/receiving/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    21718 2023-07-07 22:11:23.000000 tailbone-0.9.91/tailbone/templates/receiving/view_row.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.264757 tailbone-0.9.91/tailbone/templates/reports/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/reports/generated/
--rw-r--r--   0 lance     (1000) lance     (1000)     1811 2024-04-15 00:15:00.000000 tailbone-0.9.91/tailbone/templates/reports/generated/choose.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      635 2022-01-08 19:00:03.000000 tailbone-0.9.91/tailbone/templates/reports/generated/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      346 2021-12-15 01:04:51.000000 tailbone-0.9.91/tailbone/templates/reports/generated/delete.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      685 2024-04-15 00:14:55.000000 tailbone-0.9.91/tailbone/templates/reports/generated/generate.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1082 2022-11-28 23:53:29.000000 tailbone-0.9.91/tailbone/templates/reports/generated/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1365 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/templates/reports/inventory.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3202 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/templates/reports/ordering.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/reports/problems/
--rw-r--r--   0 lance     (1000) lance     (1000)     2397 2022-11-19 18:52:15.000000 tailbone-0.9.91/tailbone/templates/reports/problems/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/roles/
--rw-r--r--   0 lance     (1000) lance     (1000)      536 2020-07-17 00:43:21.000000 tailbone-0.9.91/tailbone/templates/roles/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      541 2020-06-22 19:53:23.000000 tailbone-0.9.91/tailbone/templates/roles/edit.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      407 2023-03-25 18:02:44.000000 tailbone-0.9.91/tailbone/templates/roles/find_by_perm.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      330 2020-06-22 20:36:16.000000 tailbone-0.9.91/tailbone/templates/roles/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      754 2024-04-15 01:27:32.000000 tailbone-0.9.91/tailbone/templates/roles/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.252757 tailbone-0.9.91/tailbone/templates/settings/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/settings/email/
--rw-r--r--   0 lance     (1000) lance     (1000)     4605 2023-08-31 04:30:54.000000 tailbone-0.9.91/tailbone/templates/settings/email/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1923 2022-08-06 23:37:28.000000 tailbone-0.9.91/tailbone/templates/settings/email/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2993 2024-04-15 00:15:31.000000 tailbone-0.9.91/tailbone/templates/settings/email/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/shifts/
--rw-r--r--   0 lance     (1000) lance     (1000)     6116 2023-02-03 22:43:25.000000 tailbone-0.9.91/tailbone/templates/shifts/base.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1025 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/shifts/schedule.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2538 2023-02-03 22:44:07.000000 tailbone-0.9.91/tailbone/templates/shifts/schedule_edit.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      900 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/shifts/schedule_print.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      813 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/shifts/schedule_print_employee.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      833 2023-02-03 22:45:27.000000 tailbone-0.9.91/tailbone/templates/shifts/timesheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1463 2023-02-03 22:42:48.000000 tailbone-0.9.91/tailbone/templates/shifts/timesheet_edit.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/tables/
--rw-r--r--   0 lance     (1000) lance     (1000)    31927 2023-05-13 02:23:37.000000 tailbone-0.9.91/tailbone/templates/tables/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      307 2023-05-13 01:29:02.000000 tailbone-0.9.91/tailbone/templates/tables/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      245 2023-05-13 01:31:53.000000 tailbone-0.9.91/tailbone/templates/tables/migrations.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/tempmon/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/tempmon/appliances/
--rw-r--r--   0 lance     (1000) lance     (1000)      736 2020-04-05 00:31:41.000000 tailbone-0.9.91/tailbone/templates/tempmon/appliances/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      510 2023-01-14 00:38:46.000000 tailbone-0.9.91/tailbone/templates/tempmon/appliances/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/tempmon/clients/
--rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:17:35.000000 tailbone-0.9.91/tailbone/templates/tempmon/clients/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1044 2023-10-05 17:49:24.000000 tailbone-0.9.91/tailbone/templates/tempmon/clients/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3718 2023-02-03 05:40:48.000000 tailbone-0.9.91/tailbone/templates/tempmon/dashboard.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/tempmon/probes/
--rw-r--r--   0 lance     (1000) lance     (1000)     3664 2023-07-07 22:38:34.000000 tailbone-0.9.91/tailbone/templates/tempmon/probes/graph.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:18:44.000000 tailbone-0.9.91/tailbone/templates/tempmon/probes/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2738 2023-10-05 17:29:42.000000 tailbone-0.9.91/tailbone/templates/tempmon/probes/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/tempmon/readings/
--rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:17:35.000000 tailbone-0.9.91/tailbone/templates/tempmon/readings/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.252757 tailbone-0.9.91/tailbone/templates/themes/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/themes/falafel/
--rw-r--r--   0 lance     (1000) lance     (1000)       93 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/templates/themes/falafel/base.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       97 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/templates/themes/falafel/progress.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       96 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/templates/themes/falafel/upgrade.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.252757 tailbone-0.9.91/tailbone/templates/trainwreck/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/trainwreck/transactions/
--rw-r--r--   0 lance     (1000) lance     (1000)     1862 2023-01-02 18:38:43.000000 tailbone-0.9.91/tailbone/templates/trainwreck/transactions/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      295 2022-01-01 22:14:16.000000 tailbone-0.9.91/tailbone/templates/trainwreck/transactions/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1625 2023-02-02 00:39:56.000000 tailbone-0.9.91/tailbone/templates/trainwreck/transactions/rollover.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      389 2022-03-17 21:59:40.000000 tailbone-0.9.91/tailbone/templates/trainwreck/transactions/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      357 2022-02-19 22:34:34.000000 tailbone-0.9.91/tailbone/templates/trainwreck/transactions/view_row.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/units-of-measure/
--rw-r--r--   0 lance     (1000) lance     (1000)     1899 2021-01-27 14:56:25.000000 tailbone-0.9.91/tailbone/templates/units-of-measure/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1736 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/templates/upgrade.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/upgrades/
--rw-r--r--   0 lance     (1000) lance     (1000)     5196 2023-02-02 00:32:20.000000 tailbone-0.9.91/tailbone/templates/upgrades/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     9408 2024-04-15 00:15:24.000000 tailbone-0.9.91/tailbone/templates/upgrades/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/users/
--rw-r--r--   0 lance     (1000) lance     (1000)      481 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/templates/users/find_by_perm.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1320 2024-04-14 23:56:36.000000 tailbone-0.9.91/tailbone/templates/users/preferences.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     4517 2023-05-15 13:10:42.000000 tailbone-0.9.91/tailbone/templates/users/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      797 2023-02-03 05:38:48.000000 tailbone-0.9.91/tailbone/templates/util.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/vendors/
--rw-r--r--   0 lance     (1000) lance     (1000)     1850 2022-05-15 21:04:06.000000 tailbone-0.9.91/tailbone/templates/vendors/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.252757 tailbone-0.9.91/tailbone/templates/views/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/views/model/
--rw-r--r--   0 lance     (1000) lance     (1000)     9427 2023-01-16 19:50:05.000000 tailbone-0.9.91/tailbone/templates/views/model/create.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.268757 tailbone-0.9.91/tailbone/templates/workorders/
--rw-r--r--   0 lance     (1000) lance     (1000)     7838 2022-08-10 02:05:11.000000 tailbone-0.9.91/tailbone/templates/workorders/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2637 2019-02-26 03:11:49.000000 tailbone-0.9.91/tailbone/tweens.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13431 2023-11-12 03:25:41.000000 tailbone-0.9.91/tailbone/util.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/
--rw-r--r--   0 lance     (1000) lance     (1000)     2797 2022-12-10 15:46:54.000000 tailbone-0.9.91/tailbone/views/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/asgi/
--rw-r--r--   0 lance     (1000) lance     (1000)     4315 2023-06-09 19:22:50.000000 tailbone-0.9.91/tailbone/views/asgi/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2654 2022-08-20 22:38:06.000000 tailbone-0.9.91/tailbone/views/asgi/datasync.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7840 2022-08-21 03:39:57.000000 tailbone-0.9.91/tailbone/views/asgi/upgrades.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9533 2023-12-13 18:05:29.000000 tailbone-0.9.91/tailbone/views/auth.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)     1075 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/views/batch/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    59664 2024-04-15 01:48:34.000000 tailbone-0.9.91/tailbone/views/batch/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3698 2021-10-31 02:25:39.000000 tailbone-0.9.91/tailbone/views/batch/delproduct.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6098 2024-04-14 23:51:02.000000 tailbone-0.9.91/tailbone/views/batch/handheld.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9880 2024-04-15 01:55:22.000000 tailbone-0.9.91/tailbone/views/batch/importer.py
--rw-r--r--   0 lance     (1000) lance     (1000)    19323 2023-10-06 20:52:44.000000 tailbone-0.9.91/tailbone/views/batch/inventory.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7101 2022-01-10 20:54:44.000000 tailbone-0.9.91/tailbone/views/batch/labels.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6695 2023-08-31 01:01:47.000000 tailbone-0.9.91/tailbone/views/batch/newproduct.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9505 2024-04-15 00:34:44.000000 tailbone-0.9.91/tailbone/views/batch/pos.py
--rw-r--r--   0 lance     (1000) lance     (1000)    12439 2024-03-26 17:53:16.000000 tailbone-0.9.91/tailbone/views/batch/pricing.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9258 2024-04-14 23:44:49.000000 tailbone-0.9.91/tailbone/views/batch/product.py
--rw-r--r--   0 lance     (1000) lance     (1000)    15017 2023-05-30 18:24:14.000000 tailbone-0.9.91/tailbone/views/batch/vendorcatalog.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6644 2022-08-14 04:58:46.000000 tailbone-0.9.91/tailbone/views/batch/vendorinvoice.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7059 2023-10-18 23:04:31.000000 tailbone-0.9.91/tailbone/views/bouncer.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3974 2022-07-19 19:48:52.000000 tailbone-0.9.91/tailbone/views/brands.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3712 2022-11-23 17:57:17.000000 tailbone-0.9.91/tailbone/views/categories.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13198 2023-06-17 21:09:24.000000 tailbone-0.9.91/tailbone/views/common.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6188 2023-06-17 20:49:58.000000 tailbone-0.9.91/tailbone/views/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2502 2022-11-23 18:19:27.000000 tailbone-0.9.91/tailbone/views/customergroups.py
--rw-r--r--   0 lance     (1000) lance     (1000)    31934 2024-04-15 01:54:49.000000 tailbone-0.9.91/tailbone/views/customers.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/custorders/
--rw-r--r--   0 lance     (1000) lance     (1000)     1213 2020-08-02 04:53:28.000000 tailbone-0.9.91/tailbone/views/custorders/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7676 2023-02-12 15:33:23.000000 tailbone-0.9.91/tailbone/views/custorders/batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1948 2022-11-23 18:19:21.000000 tailbone-0.9.91/tailbone/views/custorders/creating.py
--rw-r--r--   0 lance     (1000) lance     (1000)    26148 2024-04-15 00:35:12.000000 tailbone-0.9.91/tailbone/views/custorders/items.py
--rw-r--r--   0 lance     (1000) lance     (1000)    45521 2023-10-25 19:05:36.000000 tailbone-0.9.91/tailbone/views/custorders/orders.py
--rw-r--r--   0 lance     (1000) lance     (1000)    16525 2023-06-01 16:37:13.000000 tailbone-0.9.91/tailbone/views/datasync.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7781 2024-04-15 00:32:55.000000 tailbone-0.9.91/tailbone/views/departments.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2065 2022-11-23 18:19:03.000000 tailbone-0.9.91/tailbone/views/depositlinks.py
--rw-r--r--   0 lance     (1000) lance     (1000)    19409 2023-10-30 03:22:01.000000 tailbone-0.9.91/tailbone/views/email.py
--rw-r--r--   0 lance     (1000) lance     (1000)    14156 2023-10-18 22:53:40.000000 tailbone-0.9.91/tailbone/views/employees.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2229 2023-05-05 15:39:16.000000 tailbone-0.9.91/tailbone/views/essentials.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6163 2022-12-25 18:44:17.000000 tailbone-0.9.91/tailbone/views/exports.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3231 2022-11-23 18:00:03.000000 tailbone-0.9.91/tailbone/views/families.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4000 2023-05-15 13:10:42.000000 tailbone-0.9.91/tailbone/views/features.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2483 2022-11-23 18:18:45.000000 tailbone-0.9.91/tailbone/views/filemon.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1384 2023-09-10 18:50:16.000000 tailbone-0.9.91/tailbone/views/handheld.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2778 2022-11-23 18:18:37.000000 tailbone-0.9.91/tailbone/views/ifps.py
--rw-r--r--   0 lance     (1000) lance     (1000)    21962 2023-05-10 01:24:53.000000 tailbone-0.9.91/tailbone/views/importing.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2566 2022-11-23 18:18:26.000000 tailbone-0.9.91/tailbone/views/inventory.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/labels/
--rw-r--r--   0 lance     (1000) lance     (1000)     1155 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/views/labels/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1326 2023-09-10 18:50:26.000000 tailbone-0.9.91/tailbone/views/labels/batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6330 2023-02-09 02:19:03.000000 tailbone-0.9.91/tailbone/views/labels/profiles.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11286 2023-02-03 06:49:24.000000 tailbone-0.9.91/tailbone/views/luigi.py
--rw-r--r--   0 lance     (1000) lance     (1000)   228233 2024-04-14 23:07:56.000000 tailbone-0.9.91/tailbone/views/master.py
--rw-r--r--   0 lance     (1000) lance     (1000)    18131 2023-12-01 00:19:11.000000 tailbone-0.9.91/tailbone/views/members.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6801 2023-02-03 06:44:00.000000 tailbone-0.9.91/tailbone/views/menus.py
--rw-r--r--   0 lance     (1000) lance     (1000)    20417 2024-04-15 01:47:46.000000 tailbone-0.9.91/tailbone/views/messages.py
--rw-r--r--   0 lance     (1000) lance     (1000)    75831 2024-04-15 01:45:58.000000 tailbone-0.9.91/tailbone/views/people.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1816 2022-11-23 18:18:05.000000 tailbone-0.9.91/tailbone/views/permissions.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/poser/
--rw-r--r--   0 lance     (1000) lance     (1000)     1138 2022-03-05 00:03:03.000000 tailbone-0.9.91/tailbone/views/poser/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2470 2022-05-11 01:00:46.000000 tailbone-0.9.91/tailbone/views/poser/master.py
--rw-r--r--   0 lance     (1000) lance     (1000)    10063 2022-05-11 01:00:44.000000 tailbone-0.9.91/tailbone/views/poser/reports.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11220 2022-07-26 17:01:09.000000 tailbone-0.9.91/tailbone/views/poser/views.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6454 2024-04-14 23:38:57.000000 tailbone-0.9.91/tailbone/views/principal.py
--rw-r--r--   0 lance     (1000) lance     (1000)   102892 2024-04-15 01:46:20.000000 tailbone-0.9.91/tailbone/views/products.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2491 2022-11-23 18:17:55.000000 tailbone-0.9.91/tailbone/views/progress.py
--rw-r--r--   0 lance     (1000) lance     (1000)    15358 2023-05-20 00:45:29.000000 tailbone-0.9.91/tailbone/views/projects.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/purchases/
--rw-r--r--   0 lance     (1000) lance     (1000)     1159 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/views/purchases/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13572 2023-10-18 23:17:47.000000 tailbone-0.9.91/tailbone/views/purchases/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6915 2023-09-17 23:22:43.000000 tailbone-0.9.91/tailbone/views/purchases/credits.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/purchasing/
--rw-r--r--   0 lance     (1000) lance     (1000)     1266 2021-09-29 15:13:18.000000 tailbone-0.9.91/tailbone/views/purchasing/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    34167 2024-04-15 00:36:07.000000 tailbone-0.9.91/tailbone/views/purchasing/batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)    12698 2023-06-27 23:18:35.000000 tailbone-0.9.91/tailbone/views/purchasing/costing.py
--rw-r--r--   0 lance     (1000) lance     (1000)    19673 2024-04-14 23:29:26.000000 tailbone-0.9.91/tailbone/views/purchasing/ordering.py
--rw-r--r--   0 lance     (1000) lance     (1000)    89356 2024-04-15 00:37:38.000000 tailbone-0.9.91/tailbone/views/purchasing/receiving.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3197 2022-11-23 18:17:10.000000 tailbone-0.9.91/tailbone/views/reportcodes.py
--rw-r--r--   0 lance     (1000) lance     (1000)    29907 2024-04-15 00:32:35.000000 tailbone-0.9.91/tailbone/views/reports.py
--rw-r--r--   0 lance     (1000) lance     (1000)    20099 2024-04-15 00:39:14.000000 tailbone-0.9.91/tailbone/views/roles.py
--rw-r--r--   0 lance     (1000) lance     (1000)    16580 2024-04-15 01:25:01.000000 tailbone-0.9.91/tailbone/views/settings.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/shifts/
--rw-r--r--   0 lance     (1000) lance     (1000)     1207 2018-03-01 00:58:49.000000 tailbone-0.9.91/tailbone/views/shifts/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6797 2023-10-18 23:14:40.000000 tailbone-0.9.91/tailbone/views/shifts/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)    22006 2024-04-14 23:49:25.000000 tailbone-0.9.91/tailbone/views/shifts/lib.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9975 2023-02-12 03:56:46.000000 tailbone-0.9.91/tailbone/views/shifts/schedule.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5387 2023-02-12 03:56:32.000000 tailbone-0.9.91/tailbone/views/shifts/timesheet.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3726 2022-11-23 18:16:15.000000 tailbone-0.9.91/tailbone/views/stores.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5677 2023-02-03 22:10:08.000000 tailbone-0.9.91/tailbone/views/subdepartments.py
--rw-r--r--   0 lance     (1000) lance     (1000)    15898 2024-04-14 23:09:45.000000 tailbone-0.9.91/tailbone/views/tables.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2103 2023-10-07 02:23:35.000000 tailbone-0.9.91/tailbone/views/taxes.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/tempmon/
--rw-r--r--   0 lance     (1000) lance     (1000)     1344 2020-04-04 20:42:25.000000 tailbone-0.9.91/tailbone/views/tempmon/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6526 2023-01-14 02:16:48.000000 tailbone-0.9.91/tailbone/views/tempmon/appliances.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9593 2023-10-05 18:08:20.000000 tailbone-0.9.91/tailbone/views/tempmon/clients.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3480 2024-04-15 00:40:07.000000 tailbone-0.9.91/tailbone/views/tempmon/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6056 2023-02-12 15:31:40.000000 tailbone-0.9.91/tailbone/views/tempmon/dashboard.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11672 2023-10-18 23:08:32.000000 tailbone-0.9.91/tailbone/views/tempmon/probes.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4062 2023-10-18 23:16:37.000000 tailbone-0.9.91/tailbone/views/tempmon/readings.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2076 2023-10-19 22:38:32.000000 tailbone-0.9.91/tailbone/views/tenders.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/trainwreck/
--rw-r--r--   0 lance     (1000) lance     (1000)     1135 2023-01-19 01:57:13.000000 tailbone-0.9.91/tailbone/views/trainwreck/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    14860 2024-04-15 00:40:27.000000 tailbone-0.9.91/tailbone/views/trainwreck/base.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1582 2022-11-23 18:15:06.000000 tailbone-0.9.91/tailbone/views/trainwreck/defaults.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2409 2023-10-07 01:55:59.000000 tailbone-0.9.91/tailbone/views/typical.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4350 2022-11-23 18:14:52.000000 tailbone-0.9.91/tailbone/views/uoms.py
--rw-r--r--   0 lance     (1000) lance     (1000)    24918 2024-04-15 01:52:07.000000 tailbone-0.9.91/tailbone/views/upgrades.py
--rw-r--r--   0 lance     (1000) lance     (1000)    27763 2024-04-15 00:33:08.000000 tailbone-0.9.91/tailbone/views/users.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tailbone/views/vendors/
--rw-r--r--   0 lance     (1000) lance     (1000)     1236 2023-02-23 01:01:50.000000 tailbone-0.9.91/tailbone/views/vendors/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1363 2023-09-10 18:50:49.000000 tailbone-0.9.91/tailbone/views/vendors/catalogs.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7783 2023-10-24 22:43:48.000000 tailbone-0.9.91/tailbone/views/vendors/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1363 2023-09-10 18:50:41.000000 tailbone-0.9.91/tailbone/views/vendors/invoices.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4738 2023-02-23 04:40:20.000000 tailbone-0.9.91/tailbone/views/vendors/samplefiles.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2951 2021-11-09 23:17:17.000000 tailbone-0.9.91/tailbone/views/versions.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6966 2023-10-18 23:16:11.000000 tailbone-0.9.91/tailbone/views/views.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13863 2023-09-02 20:50:35.000000 tailbone-0.9.91/tailbone/views/workorders.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3747 2023-05-17 02:25:47.000000 tailbone-0.9.91/tailbone/webapi.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1445 2024-04-15 15:57:32.000000 tailbone-0.9.91/tasks.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-15 15:57:40.272757 tailbone-0.9.91/tests/
--rw-rw-r--   0 lance     (1000) lance     (1000)     1057 2023-05-25 19:55:35.000000 tailbone-0.9.91/tests/test_app.py
--rw-r--r--   0 lance     (1000) lance     (1000)      191 2013-09-10 19:45:40.000000 tailbone-0.9.91/tests/test_helpers.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.536640 tailbone-0.9.92/
+-rw-r--r--   0 lance     (1000) lance     (1000)   160548 2024-04-16 15:44:18.000000 tailbone-0.9.92/CHANGES.rst
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2018-03-01 00:58:49.000000 tailbone-0.9.92/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      489 2022-01-13 00:06:52.000000 tailbone-0.9.92/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     2571 2024-04-16 15:44:49.536640 tailbone-0.9.92/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      269 2014-04-22 17:10:45.000000 tailbone-0.9.92/README.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.536640 tailbone-0.9.92/Tailbone.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2571 2024-04-16 15:44:49.000000 tailbone-0.9.92/Tailbone.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)    14749 2024-04-16 15:44:49.000000 tailbone-0.9.92/Tailbone.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2024-04-16 15:44:49.000000 tailbone-0.9.92/Tailbone.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      272 2024-04-16 15:44:49.000000 tailbone-0.9.92/Tailbone.egg-info/entry_points.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2024-04-16 15:44:49.000000 tailbone-0.9.92/Tailbone.egg-info/not-zip-safe
+-rw-r--r--   0 lance     (1000) lance     (1000)      446 2024-04-16 15:44:49.000000 tailbone-0.9.92/Tailbone.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        9 2024-04-16 15:44:49.000000 tailbone-0.9.92/Tailbone.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     2124 2024-04-16 15:44:49.536640 tailbone-0.9.92/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)     1008 2023-05-16 20:02:32.000000 tailbone-0.9.92/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.512639 tailbone-0.9.92/tailbone/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1161 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       49 2024-04-16 15:44:08.000000 tailbone-0.9.92/tailbone/_version.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.516639 tailbone-0.9.92/tailbone/api/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1389 2022-08-14 05:48:55.000000 tailbone-0.9.92/tailbone/api/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7865 2023-05-17 04:11:43.000000 tailbone-0.9.92/tailbone/api/auth.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.516639 tailbone-0.9.92/tailbone/api/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1097 2019-11-11 20:08:35.000000 tailbone-0.9.92/tailbone/api/batch/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    12760 2023-11-02 00:42:53.000000 tailbone-0.9.92/tailbone/api/batch/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7150 2023-11-15 15:46:15.000000 tailbone-0.9.92/tailbone/api/batch/inventory.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2688 2022-08-14 05:59:35.000000 tailbone-0.9.92/tailbone/api/batch/labels.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11993 2024-04-11 18:51:54.000000 tailbone-0.9.92/tailbone/api/batch/ordering.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    20740 2024-04-11 19:12:25.000000 tailbone-0.9.92/tailbone/api/batch/receiving.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5099 2023-05-17 04:34:48.000000 tailbone-0.9.92/tailbone/api/common.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4643 2023-06-17 03:15:35.000000 tailbone-0.9.92/tailbone/api/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1833 2022-08-14 05:48:19.000000 tailbone-0.9.92/tailbone/api/customers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1202 2023-05-20 00:29:29.000000 tailbone-0.9.92/tailbone/api/essentials.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1547 2023-01-30 00:46:27.000000 tailbone-0.9.92/tailbone/api/labels.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    21938 2023-10-08 17:24:00.000000 tailbone-0.9.92/tailbone/api/master.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1489 2022-08-14 05:42:00.000000 tailbone-0.9.92/tailbone/api/master2.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1802 2022-08-14 05:49:24.000000 tailbone-0.9.92/tailbone/api/people.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7461 2023-09-02 15:55:47.000000 tailbone-0.9.92/tailbone/api/products.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2126 2022-08-14 05:50:11.000000 tailbone-0.9.92/tailbone/api/upgrades.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2181 2023-05-03 00:13:09.000000 tailbone-0.9.92/tailbone/api/users.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1719 2022-08-14 05:51:19.000000 tailbone-0.9.92/tailbone/api/vendors.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8607 2022-08-31 02:51:40.000000 tailbone-0.9.92/tailbone/api/workorders.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11673 2024-04-16 02:52:40.000000 tailbone-0.9.92/tailbone/app.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3290 2022-08-17 00:32:35.000000 tailbone-0.9.92/tailbone/asgi.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8543 2024-04-16 14:44:23.000000 tailbone-0.9.92/tailbone/auth.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5418 2022-12-07 20:00:13.000000 tailbone-0.9.92/tailbone/beaker.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2691 2022-12-24 05:29:45.000000 tailbone-0.9.92/tailbone/cleanup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2366 2024-04-13 14:19:43.000000 tailbone-0.9.92/tailbone/config.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8274 2023-02-07 18:19:37.000000 tailbone-0.9.92/tailbone/db.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9796 2023-12-01 00:13:00.000000 tailbone-0.9.92/tailbone/diffs.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1696 2020-02-28 23:40:40.000000 tailbone-0.9.92/tailbone/exceptions.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.516639 tailbone-0.9.92/tailbone/forms/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1107 2023-09-17 00:47:36.000000 tailbone-0.9.92/tailbone/forms/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1995 2023-02-12 04:03:46.000000 tailbone-0.9.92/tailbone/forms/common.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    49572 2024-04-15 01:24:25.000000 tailbone-0.9.92/tailbone/forms/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2361 2023-08-29 21:08:45.000000 tailbone-0.9.92/tailbone/forms/receiving.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7041 2023-10-09 20:50:24.000000 tailbone-0.9.92/tailbone/forms/types.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    20432 2024-04-15 01:23:41.000000 tailbone-0.9.92/tailbone/forms/widgets.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.516639 tailbone-0.9.92/tailbone/grids/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1077 2021-01-30 20:30:05.000000 tailbone-0.9.92/tailbone/grids/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    70674 2024-04-15 01:45:42.000000 tailbone-0.9.92/tailbone/grids/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    41091 2024-04-15 17:43:57.000000 tailbone-0.9.92/tailbone/grids/filters.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2730 2023-01-16 18:44:24.000000 tailbone-0.9.92/tailbone/handler.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1883 2023-05-05 02:26:43.000000 tailbone-0.9.92/tailbone/helpers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    29626 2023-10-29 20:45:59.000000 tailbone-0.9.92/tailbone/menus.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3466 2022-08-20 22:12:54.000000 tailbone-0.9.92/tailbone/progress.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1901 2023-01-15 00:47:07.000000 tailbone-0.9.92/tailbone/providers.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.516639 tailbone-0.9.92/tailbone/reports/
+-rw-rw-r--   0 lance     (1000) lance     (1000)     2481 2016-12-17 08:48:19.000000 tailbone-0.9.92/tailbone/reports/inventory_worksheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3577 2023-02-03 22:10:08.000000 tailbone-0.9.92/tailbone/reports/ordering_worksheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1632 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/scaffolds.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.516639 tailbone-0.9.92/tailbone/static/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1152 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/static/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.516639 tailbone-0.9.92/tailbone/static/css/
+-rw-r--r--   0 lance     (1000) lance     (1000)      440 2021-01-30 19:10:34.000000 tailbone-0.9.92/tailbone/static/css/base.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     4880 2021-01-17 02:38:15.000000 tailbone-0.9.92/tailbone/static/css/codehilite.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      789 2020-08-02 03:09:36.000000 tailbone-0.9.92/tailbone/static/css/diffs.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      390 2023-02-02 22:24:46.000000 tailbone-0.9.92/tailbone/static/css/filters.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     1439 2023-02-02 22:24:46.000000 tailbone-0.9.92/tailbone/static/css/forms.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     5542 2023-02-03 23:02:02.000000 tailbone-0.9.92/tailbone/static/css/grids.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     1167 2024-04-15 01:28:38.000000 tailbone-0.9.92/tailbone/static/css/grids.rowstatus.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     2869 2024-04-15 18:31:42.000000 tailbone-0.9.92/tailbone/static/css/layout.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     7346 2013-09-10 19:45:39.000000 tailbone-0.9.92/tailbone/static/css/normalize.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      575 2019-06-05 00:52:33.000000 tailbone-0.9.92/tailbone/static/css/perms.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      965 2023-02-02 22:24:46.000000 tailbone-0.9.92/tailbone/static/css/progress.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      208 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/static/css/purchases.css
+-rw-rw-r--   0 lance     (1000) lance     (1000)      225 2016-12-17 08:48:19.000000 tailbone-0.9.92/tailbone/static/css/schedule_print.css
+-rw-rw-r--   0 lance     (1000) lance     (1000)     1664 2017-07-18 18:57:10.000000 tailbone-0.9.92/tailbone/static/css/timesheet.css
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.516639 tailbone-0.9.92/tailbone/static/files/
+-rw-r--r--   0 lance     (1000) lance     (1000)     5041 2022-08-30 13:52:10.000000 tailbone-0.9.92/tailbone/static/files/newproduct_template.xlsx
+-rw-r--r--   0 lance     (1000) lance     (1000)     7593 2022-01-06 18:40:01.000000 tailbone-0.9.92/tailbone/static/files/vendor_catalog_template.xlsx
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.516639 tailbone-0.9.92/tailbone/static/img/
+-rw-r--r--   0 lance     (1000) lance     (1000)   107339 2013-09-10 19:45:39.000000 tailbone-0.9.92/tailbone/static/img/Hymenocephalus_italicus.jpg
+-rw-r--r--   0 lance     (1000) lance     (1000)      641 2013-09-10 19:45:39.000000 tailbone-0.9.92/tailbone/static/img/delete.png
+-rw-r--r--   0 lance     (1000) lance     (1000)      533 2013-09-10 19:45:39.000000 tailbone-0.9.92/tailbone/static/img/edit.png
+-rw-r--r--   0 lance     (1000) lance     (1000)    20687 2013-09-10 19:45:39.000000 tailbone-0.9.92/tailbone/static/img/home_logo.png
+-rw-r--r--   0 lance     (1000) lance     (1000)      771 2013-09-10 19:45:39.000000 tailbone-0.9.92/tailbone/static/img/loading.gif
+-rw-rw-r--   0 lance     (1000) lance     (1000)     2077 2016-12-17 08:48:19.000000 tailbone-0.9.92/tailbone/static/img/product.png
+-rw-r--r--   0 lance     (1000) lance     (1000)     5694 2013-09-10 19:45:39.000000 tailbone-0.9.92/tailbone/static/img/rattail.ico
+-rw-r--r--   0 lance     (1000) lance     (1000)      542 2015-03-10 02:10:41.000000 tailbone-0.9.92/tailbone/static/img/save.png
+-rw-r--r--   0 lance     (1000) lance     (1000)      158 2013-09-10 19:45:39.000000 tailbone-0.9.92/tailbone/static/img/sort_arrow_down.png
+-rw-r--r--   0 lance     (1000) lance     (1000)      169 2013-09-10 19:45:39.000000 tailbone-0.9.92/tailbone/static/img/sort_arrow_up.png
+-rw-rw-r--   0 lance     (1000) lance     (1000)    10375 2022-11-21 03:00:53.000000 tailbone-0.9.92/tailbone/static/img/testing.png
+-rw-r--r--   0 lance     (1000) lance     (1000)      616 2013-09-10 19:45:39.000000 tailbone-0.9.92/tailbone/static/img/view.png
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.516639 tailbone-0.9.92/tailbone/static/js/
+-rw-r--r--   0 lance     (1000) lance     (1000)      813 2021-10-12 18:14:50.000000 tailbone-0.9.92/tailbone/static/js/debounce.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     2380 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/static/js/numeric.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     9498 2023-10-26 01:03:48.000000 tailbone-0.9.92/tailbone/static/js/tailbone.buefy.autocomplete.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     1634 2020-11-25 22:42:00.000000 tailbone-0.9.92/tailbone/static/js/tailbone.buefy.datepicker.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     4561 2023-06-16 17:21:44.000000 tailbone-0.9.92/tailbone/static/js/tailbone.buefy.grid.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     3407 2019-11-05 01:06:58.000000 tailbone-0.9.92/tailbone/static/js/tailbone.buefy.message_recipients.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     1514 2022-07-26 20:56:38.000000 tailbone-0.9.92/tailbone/static/js/tailbone.buefy.numericinput.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     1637 2019-06-24 23:30:10.000000 tailbone-0.9.92/tailbone/static/js/tailbone.buefy.oncebutton.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     1403 2023-09-17 00:42:09.000000 tailbone-0.9.92/tailbone/static/js/tailbone.buefy.timepicker.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     1427 2023-06-06 16:53:17.000000 tailbone-0.9.92/tailbone/static/js/tailbone.feedback.js
+-rw-r--r--   0 lance     (1000) lance     (1000)       26 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/static/robots.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)    10115 2024-04-16 14:47:26.000000 tailbone-0.9.92/tailbone/subscribers.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.520639 tailbone-0.9.92/tailbone/templates/
+-rw-r--r--   0 lance     (1000) lance     (1000)      471 2019-08-03 00:53:47.000000 tailbone-0.9.92/tailbone/templates/about.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.520639 tailbone-0.9.92/tailbone/templates/appinfo/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7318 2023-02-02 00:31:53.000000 tailbone-0.9.92/tailbone/templates/appinfo/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3270 2024-04-16 14:47:29.000000 tailbone-0.9.92/tailbone/templates/appinfo/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     6317 2024-04-14 23:27:37.000000 tailbone-0.9.92/tailbone/templates/appsettings.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      899 2023-02-03 22:40:11.000000 tailbone-0.9.92/tailbone/templates/autocomplete.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    33655 2024-04-15 18:01:50.000000 tailbone-0.9.92/tailbone/templates/base.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      772 2021-11-04 22:56:35.000000 tailbone-0.9.92/tailbone/templates/base_meta.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.520639 tailbone-0.9.92/tailbone/templates/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)       84 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/templates/batch/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       81 2019-06-08 19:26:19.000000 tailbone-0.9.92/tailbone/templates/batch/edit.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.520639 tailbone-0.9.92/tailbone/templates/batch/importer/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2381 2024-04-15 00:15:19.000000 tailbone-0.9.92/tailbone/templates/batch/importer/view_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     4716 2023-02-03 05:51:09.000000 tailbone-0.9.92/tailbone/templates/batch/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.520639 tailbone-0.9.92/tailbone/templates/batch/inventory/
+-rw-r--r--   0 lance     (1000) lance     (1000)    10321 2024-04-15 00:11:34.000000 tailbone-0.9.92/tailbone/templates/batch/inventory/desktop_form.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.520639 tailbone-0.9.92/tailbone/templates/batch/newproduct/
+-rw-r--r--   0 lance     (1000) lance     (1000)      160 2022-08-30 15:56:25.000000 tailbone-0.9.92/tailbone/templates/batch/newproduct/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.520639 tailbone-0.9.92/tailbone/templates/batch/pos/
+-rw-r--r--   0 lance     (1000) lance     (1000)      285 2023-10-07 04:17:54.000000 tailbone-0.9.92/tailbone/templates/batch/pos/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.520639 tailbone-0.9.92/tailbone/templates/batch/pricing/
+-rw-r--r--   0 lance     (1000) lance     (1000)      536 2022-06-14 18:18:31.000000 tailbone-0.9.92/tailbone/templates/batch/pricing/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.520639 tailbone-0.9.92/tailbone/templates/batch/vendorcatalog/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1388 2022-01-08 19:35:47.000000 tailbone-0.9.92/tailbone/templates/batch/vendorcatalog/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1288 2023-02-03 05:42:10.000000 tailbone-0.9.92/tailbone/templates/batch/vendorcatalog/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      309 2022-01-06 18:52:39.000000 tailbone-0.9.92/tailbone/templates/batch/vendorcatalog/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      241 2024-04-15 00:15:22.000000 tailbone-0.9.92/tailbone/templates/batch/vendorcatalog/view_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    11890 2024-04-15 00:15:17.000000 tailbone-0.9.92/tailbone/templates/batch/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      509 2023-02-03 05:50:25.000000 tailbone-0.9.92/tailbone/templates/batch/worksheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      121 2020-03-24 00:26:09.000000 tailbone-0.9.92/tailbone/templates/change_password.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    13008 2023-01-17 03:55:16.000000 tailbone-0.9.92/tailbone/templates/configure-menus.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     9425 2023-01-16 17:56:04.000000 tailbone-0.9.92/tailbone/templates/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.520639 tailbone-0.9.92/tailbone/templates/customers/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3775 2023-06-11 18:38:46.000000 tailbone-0.9.92/tailbone/templates/customers/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.520639 tailbone-0.9.92/tailbone/templates/customers/pending/
+-rw-r--r--   0 lance     (1000) lance     (1000)     5021 2021-12-24 01:59:01.000000 tailbone-0.9.92/tailbone/templates/customers/pending/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1096 2024-04-15 01:26:15.000000 tailbone-0.9.92/tailbone/templates/customers/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.520639 tailbone-0.9.92/tailbone/templates/custorders/
+-rw-r--r--   0 lance     (1000) lance     (1000)     6522 2023-10-25 00:29:26.000000 tailbone-0.9.92/tailbone/templates/custorders/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    92495 2023-10-26 14:28:39.000000 tailbone-0.9.92/tailbone/templates/custorders/create.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.520639 tailbone-0.9.92/tailbone/templates/custorders/items/
+-rw-r--r--   0 lance     (1000) lance     (1000)    16040 2024-04-15 00:15:26.000000 tailbone-0.9.92/tailbone/templates/custorders/items/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       81 2023-09-10 19:59:06.000000 tailbone-0.9.92/tailbone/templates/custorders/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.520639 tailbone-0.9.92/tailbone/templates/datasync/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.520639 tailbone-0.9.92/tailbone/templates/datasync/changes/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2125 2023-02-03 05:54:34.000000 tailbone-0.9.92/tailbone/templates/datasync/changes/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    31019 2023-02-02 00:43:40.000000 tailbone-0.9.92/tailbone/templates/datasync/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     5964 2023-02-02 00:35:51.000000 tailbone-0.9.92/tailbone/templates/datasync/status.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/deform/
+-rw-r--r--   0 lance     (1000) lance     (1000)      918 2023-02-03 05:52:17.000000 tailbone-0.9.92/tailbone/templates/deform/autocomplete_jquery.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      943 2023-02-03 05:53:06.000000 tailbone-0.9.92/tailbone/templates/deform/cases_units.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      492 2023-02-03 05:54:15.000000 tailbone-0.9.92/tailbone/templates/deform/checkbox.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      545 2021-01-06 00:19:12.000000 tailbone-0.9.92/tailbone/templates/deform/checkbox_dynamic.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1213 2023-02-03 05:51:23.000000 tailbone-0.9.92/tailbone/templates/deform/checked_password.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      597 2023-02-03 05:53:42.000000 tailbone-0.9.92/tailbone/templates/deform/date_jquery.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      581 2019-02-23 02:44:18.000000 tailbone-0.9.92/tailbone/templates/deform/date_plain.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      543 2023-09-17 01:00:05.000000 tailbone-0.9.92/tailbone/templates/deform/datetime_falafel.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      758 2023-02-03 05:52:34.000000 tailbone-0.9.92/tailbone/templates/deform/file_upload.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      601 2019-11-04 23:21:16.000000 tailbone-0.9.92/tailbone/templates/deform/message_recipients.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      257 2023-01-29 16:59:23.000000 tailbone-0.9.92/tailbone/templates/deform/multi_file_upload.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      963 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/templates/deform/numberinput.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      509 2019-06-28 17:09:23.000000 tailbone-0.9.92/tailbone/templates/deform/numericinput.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      616 2023-02-07 22:10:56.000000 tailbone-0.9.92/tailbone/templates/deform/password.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      710 2023-02-03 05:52:00.000000 tailbone-0.9.92/tailbone/templates/deform/percentinput.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     2102 2023-02-03 05:54:03.000000 tailbone-0.9.92/tailbone/templates/deform/permissions.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      875 2022-11-19 23:40:01.000000 tailbone-0.9.92/tailbone/templates/deform/problem_report_days.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     2164 2023-02-03 05:51:49.000000 tailbone-0.9.92/tailbone/templates/deform/select.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1177 2023-08-08 19:10:04.000000 tailbone-0.9.92/tailbone/templates/deform/select_dynamic.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1979 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/templates/deform/select_jquery.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1718 2019-09-06 22:13:34.000000 tailbone-0.9.92/tailbone/templates/deform/select_plain.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      550 2023-03-23 15:17:29.000000 tailbone-0.9.92/tailbone/templates/deform/textarea.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      894 2023-02-04 01:42:19.000000 tailbone-0.9.92/tailbone/templates/deform/textinput.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      230 2023-09-26 00:21:51.000000 tailbone-0.9.92/tailbone/templates/deform/time_falafel.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      655 2023-02-03 05:53:32.000000 tailbone-0.9.92/tailbone/templates/deform/time_jquery.pt
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/departments/
+-rw-rw-r--   0 lance     (1000) lance     (1000)      294 2023-02-03 05:31:15.000000 tailbone-0.9.92/tailbone/templates/departments/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      551 2023-10-09 05:16:53.000000 tailbone-0.9.92/tailbone/templates/diff.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/email-bounces/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1659 2023-09-08 15:46:55.000000 tailbone-0.9.92/tailbone/templates/email-bounces/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/employees/
+-rw-r--r--   0 lance     (1000) lance     (1000)      626 2023-06-11 04:11:26.000000 tailbone-0.9.92/tailbone/templates/employees/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      259 2019-04-12 19:47:07.000000 tailbone-0.9.92/tailbone/templates/employees/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1170 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/templates/exception.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1506 2024-04-15 00:15:12.000000 tailbone-0.9.92/tailbone/templates/form.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2779 2023-06-17 19:13:31.000000 tailbone-0.9.92/tailbone/templates/formposter.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/forms/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7053 2024-04-15 00:03:36.000000 tailbone-0.9.92/tailbone/templates/forms/deform.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    12583 2023-02-02 00:37:54.000000 tailbone-0.9.92/tailbone/templates/generate_feature.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/generated-projects/
+-rw-r--r--   0 lance     (1000) lance     (1000)      582 2023-05-04 18:51:55.000000 tailbone-0.9.92/tailbone/templates/generated-projects/create.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/grids/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3024 2023-02-02 00:24:21.000000 tailbone-0.9.92/tailbone/templates/grids/b-table.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    28542 2024-04-15 01:40:53.000000 tailbone-0.9.92/tailbone/templates/grids/complete.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1898 2023-10-11 03:10:01.000000 tailbone-0.9.92/tailbone/templates/grids/filters.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      755 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/templates/grids/nav.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      672 2019-08-24 02:39:03.000000 tailbone-0.9.92/tailbone/templates/home.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/ifps-plu-codes/
+-rw-r--r--   0 lance     (1000) lance     (1000)      281 2020-12-07 01:28:53.000000 tailbone-0.9.92/tailbone/templates/ifps-plu-codes/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)     6187 2023-02-02 00:43:01.000000 tailbone-0.9.92/tailbone/templates/importing/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      294 2021-12-06 18:34:10.000000 tailbone-0.9.92/tailbone/templates/importing/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2643 2021-12-07 03:29:19.000000 tailbone-0.9.92/tailbone/templates/importing/runjob.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      671 2021-12-07 03:21:19.000000 tailbone-0.9.92/tailbone/templates/importing/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.512639 tailbone-0.9.92/tailbone/templates/labels/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/labels/profiles/
+-rw-rw-r--   0 lance     (1000) lance     (1000)      314 2016-12-17 08:48:19.000000 tailbone-0.9.92/tailbone/templates/labels/profiles/create.mako
+-rw-rw-r--   0 lance     (1000) lance     (1000)      620 2016-12-17 08:48:19.000000 tailbone-0.9.92/tailbone/templates/labels/profiles/edit.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      432 2019-05-23 22:57:42.000000 tailbone-0.9.92/tailbone/templates/labels/profiles/printer.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1232 2023-02-09 02:19:12.000000 tailbone-0.9.92/tailbone/templates/labels/profiles/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1649 2023-02-07 22:11:44.000000 tailbone-0.9.92/tailbone/templates/login.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/luigi/
+-rw-r--r--   0 lance     (1000) lance     (1000)    14033 2023-02-02 00:30:45.000000 tailbone-0.9.92/tailbone/templates/luigi/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    12842 2023-02-02 00:29:33.000000 tailbone-0.9.92/tailbone/templates/luigi/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/master/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1364 2024-04-15 00:15:10.000000 tailbone-0.9.92/tailbone/templates/master/clone.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      893 2021-12-14 03:26:58.000000 tailbone-0.9.92/tailbone/templates/master/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      174 2019-05-22 20:24:53.000000 tailbone-0.9.92/tailbone/templates/master/create.mako
+-rw-rw-r--   0 lance     (1000) lance     (1000)      248 2016-12-17 08:48:19.000000 tailbone-0.9.92/tailbone/templates/master/create_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1389 2024-04-15 00:15:05.000000 tailbone-0.9.92/tailbone/templates/master/delete.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      226 2023-10-10 02:06:31.000000 tailbone-0.9.92/tailbone/templates/master/edit.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      879 2021-12-13 19:43:47.000000 tailbone-0.9.92/tailbone/templates/master/edit_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      584 2023-02-03 18:10:14.000000 tailbone-0.9.92/tailbone/templates/master/form.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      170 2018-11-23 00:24:59.000000 tailbone-0.9.92/tailbone/templates/master/import_file.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    25086 2024-04-13 15:01:04.000000 tailbone-0.9.92/tailbone/templates/master/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     5560 2023-06-19 02:20:45.000000 tailbone-0.9.92/tailbone/templates/master/merge.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1036 2024-04-13 15:00:59.000000 tailbone-0.9.92/tailbone/templates/master/versions.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    11305 2024-04-13 15:00:53.000000 tailbone-0.9.92/tailbone/templates/master/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      709 2023-02-03 05:26:29.000000 tailbone-0.9.92/tailbone/templates/master/view_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1413 2023-10-10 15:07:41.000000 tailbone-0.9.92/tailbone/templates/master/view_version.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/members/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2342 2023-08-26 14:11:45.000000 tailbone-0.9.92/tailbone/templates/members/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      262 2023-06-14 19:01:14.000000 tailbone-0.9.92/tailbone/templates/members/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1686 2023-02-02 22:24:46.000000 tailbone-0.9.92/tailbone/templates/menu.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/messages/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/messages/archive/
+-rw-r--r--   0 lance     (1000) lance     (1000)      353 2023-02-03 05:34:09.000000 tailbone-0.9.92/tailbone/templates/messages/archive/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1777 2023-03-23 15:22:59.000000 tailbone-0.9.92/tailbone/templates/messages/create.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/messages/inbox/
+-rw-r--r--   0 lance     (1000) lance     (1000)      355 2023-02-03 05:35:57.000000 tailbone-0.9.92/tailbone/templates/messages/inbox/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1761 2023-02-03 05:35:48.000000 tailbone-0.9.92/tailbone/templates/messages/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1101 2019-11-05 01:03:51.000000 tailbone-0.9.92/tailbone/templates/messages/recipients.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/messages/sent/
+-rw-rw-r--   0 lance     (1000) lance     (1000)      354 2016-12-17 08:48:19.000000 tailbone-0.9.92/tailbone/templates/messages/sent/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3206 2023-02-03 05:35:31.000000 tailbone-0.9.92/tailbone/templates/messages/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1509 2023-01-29 17:00:34.000000 tailbone-0.9.92/tailbone/templates/multi_file_upload.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/ordering/
+-rw-r--r--   0 lance     (1000) lance     (1000)      112 2023-02-03 05:36:48.000000 tailbone-0.9.92/tailbone/templates/ordering/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    16377 2021-02-01 03:51:46.000000 tailbone-0.9.92/tailbone/templates/ordering/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    11560 2023-02-03 05:37:47.000000 tailbone-0.9.92/tailbone/templates/ordering/worksheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1813 2023-08-28 02:36:03.000000 tailbone-0.9.92/tailbone/templates/page.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     7512 2022-12-28 04:29:27.000000 tailbone-0.9.92/tailbone/templates/page_help.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/people/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1296 2023-06-17 19:36:29.000000 tailbone-0.9.92/tailbone/templates/people/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3654 2023-02-03 05:40:07.000000 tailbone-0.9.92/tailbone/templates/people/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/people/merge-requests/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1183 2023-02-03 05:39:54.000000 tailbone-0.9.92/tailbone/templates/people/merge-requests/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1100 2024-04-15 00:14:52.000000 tailbone-0.9.92/tailbone/templates/people/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    84948 2024-04-15 00:33:25.000000 tailbone-0.9.92/tailbone/templates/people/view_profile.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/poser/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/poser/reports/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2382 2022-03-04 00:35:18.000000 tailbone-0.9.92/tailbone/templates/poser/reports/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3917 2022-03-21 22:32:51.000000 tailbone-0.9.92/tailbone/templates/poser/setup.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/poser/views/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1120 2022-03-21 22:32:51.000000 tailbone-0.9.92/tailbone/templates/poser/views/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/principal/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7971 2024-04-14 23:38:53.000000 tailbone-0.9.92/tailbone/templates/principal/find_by_perm.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      319 2023-10-18 21:45:40.000000 tailbone-0.9.92/tailbone/templates/principal/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.524639 tailbone-0.9.92/tailbone/templates/products/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3763 2024-04-15 00:12:29.000000 tailbone-0.9.92/tailbone/templates/products/batch.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     4184 2023-08-25 13:40:55.000000 tailbone-0.9.92/tailbone/templates/products/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2929 2023-02-03 05:58:51.000000 tailbone-0.9.92/tailbone/templates/products/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    11948 2023-10-26 15:05:27.000000 tailbone-0.9.92/tailbone/templates/products/lookup.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/products/pending/
+-rw-r--r--   0 lance     (1000) lance     (1000)     4913 2023-10-27 01:41:10.000000 tailbone-0.9.92/tailbone/templates/products/pending/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    13263 2024-04-15 00:33:50.000000 tailbone-0.9.92/tailbone/templates/products/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     6614 2023-02-03 22:10:08.000000 tailbone-0.9.92/tailbone/templates/progress.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/purchases/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/purchases/batches/
+-rw-r--r--   0 lance     (1000) lance     (1000)      117 2023-02-03 22:16:48.000000 tailbone-0.9.92/tailbone/templates/purchases/batches/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      278 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/templates/purchases/batches/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/purchases/credits/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2469 2023-02-03 23:08:13.000000 tailbone-0.9.92/tailbone/templates/purchases/credits/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2630 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/templates/purchases/receiving_worksheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      555 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/templates/purchases/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/receiving/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7668 2023-09-17 23:19:14.000000 tailbone-0.9.92/tailbone/templates/receiving/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      117 2023-02-03 05:32:11.000000 tailbone-0.9.92/tailbone/templates/receiving/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1415 2024-04-15 00:18:30.000000 tailbone-0.9.92/tailbone/templates/receiving/declare_credit.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1320 2024-04-15 00:18:40.000000 tailbone-0.9.92/tailbone/templates/receiving/receive_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      305 2018-10-24 22:53:24.000000 tailbone-0.9.92/tailbone/templates/receiving/transform_unit_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    13336 2023-11-02 01:52:57.000000 tailbone-0.9.92/tailbone/templates/receiving/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    21718 2023-07-07 22:11:23.000000 tailbone-0.9.92/tailbone/templates/receiving/view_row.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/reports/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/reports/generated/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1811 2024-04-15 00:15:00.000000 tailbone-0.9.92/tailbone/templates/reports/generated/choose.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      635 2022-01-08 19:00:03.000000 tailbone-0.9.92/tailbone/templates/reports/generated/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      346 2021-12-15 01:04:51.000000 tailbone-0.9.92/tailbone/templates/reports/generated/delete.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      685 2024-04-15 00:14:55.000000 tailbone-0.9.92/tailbone/templates/reports/generated/generate.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1082 2022-11-28 23:53:29.000000 tailbone-0.9.92/tailbone/templates/reports/generated/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1365 2023-02-03 22:10:08.000000 tailbone-0.9.92/tailbone/templates/reports/inventory.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3202 2023-02-03 22:10:08.000000 tailbone-0.9.92/tailbone/templates/reports/ordering.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/reports/problems/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2397 2022-11-19 18:52:15.000000 tailbone-0.9.92/tailbone/templates/reports/problems/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/roles/
+-rw-r--r--   0 lance     (1000) lance     (1000)      536 2020-07-17 00:43:21.000000 tailbone-0.9.92/tailbone/templates/roles/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      541 2020-06-22 19:53:23.000000 tailbone-0.9.92/tailbone/templates/roles/edit.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      407 2023-03-25 18:02:44.000000 tailbone-0.9.92/tailbone/templates/roles/find_by_perm.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      330 2020-06-22 20:36:16.000000 tailbone-0.9.92/tailbone/templates/roles/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      754 2024-04-15 01:27:32.000000 tailbone-0.9.92/tailbone/templates/roles/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.512639 tailbone-0.9.92/tailbone/templates/settings/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/settings/email/
+-rw-r--r--   0 lance     (1000) lance     (1000)     4605 2023-08-31 04:30:54.000000 tailbone-0.9.92/tailbone/templates/settings/email/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1923 2022-08-06 23:37:28.000000 tailbone-0.9.92/tailbone/templates/settings/email/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2993 2024-04-15 00:15:31.000000 tailbone-0.9.92/tailbone/templates/settings/email/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/shifts/
+-rw-r--r--   0 lance     (1000) lance     (1000)     6116 2023-02-03 22:43:25.000000 tailbone-0.9.92/tailbone/templates/shifts/base.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1025 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/templates/shifts/schedule.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2538 2023-02-03 22:44:07.000000 tailbone-0.9.92/tailbone/templates/shifts/schedule_edit.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      900 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/templates/shifts/schedule_print.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      813 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/templates/shifts/schedule_print_employee.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      833 2023-02-03 22:45:27.000000 tailbone-0.9.92/tailbone/templates/shifts/timesheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1463 2023-02-03 22:42:48.000000 tailbone-0.9.92/tailbone/templates/shifts/timesheet_edit.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/tables/
+-rw-r--r--   0 lance     (1000) lance     (1000)    31927 2023-05-13 02:23:37.000000 tailbone-0.9.92/tailbone/templates/tables/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      307 2023-05-13 01:29:02.000000 tailbone-0.9.92/tailbone/templates/tables/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      245 2023-05-13 01:31:53.000000 tailbone-0.9.92/tailbone/templates/tables/migrations.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/tempmon/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/tempmon/appliances/
+-rw-r--r--   0 lance     (1000) lance     (1000)      736 2020-04-05 00:31:41.000000 tailbone-0.9.92/tailbone/templates/tempmon/appliances/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      510 2023-01-14 00:38:46.000000 tailbone-0.9.92/tailbone/templates/tempmon/appliances/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/tempmon/clients/
+-rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:17:35.000000 tailbone-0.9.92/tailbone/templates/tempmon/clients/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1044 2023-10-05 17:49:24.000000 tailbone-0.9.92/tailbone/templates/tempmon/clients/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3718 2023-02-03 05:40:48.000000 tailbone-0.9.92/tailbone/templates/tempmon/dashboard.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/tempmon/probes/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3664 2023-07-07 22:38:34.000000 tailbone-0.9.92/tailbone/templates/tempmon/probes/graph.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:18:44.000000 tailbone-0.9.92/tailbone/templates/tempmon/probes/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2738 2023-10-05 17:29:42.000000 tailbone-0.9.92/tailbone/templates/tempmon/probes/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/tempmon/readings/
+-rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:17:35.000000 tailbone-0.9.92/tailbone/templates/tempmon/readings/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.512639 tailbone-0.9.92/tailbone/templates/themes/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/themes/falafel/
+-rw-r--r--   0 lance     (1000) lance     (1000)       93 2023-02-03 22:10:08.000000 tailbone-0.9.92/tailbone/templates/themes/falafel/base.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       97 2023-02-03 22:10:08.000000 tailbone-0.9.92/tailbone/templates/themes/falafel/progress.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       96 2023-02-03 22:10:08.000000 tailbone-0.9.92/tailbone/templates/themes/falafel/upgrade.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.512639 tailbone-0.9.92/tailbone/templates/trainwreck/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/trainwreck/transactions/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1862 2023-01-02 18:38:43.000000 tailbone-0.9.92/tailbone/templates/trainwreck/transactions/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      295 2022-01-01 22:14:16.000000 tailbone-0.9.92/tailbone/templates/trainwreck/transactions/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1625 2023-02-02 00:39:56.000000 tailbone-0.9.92/tailbone/templates/trainwreck/transactions/rollover.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      389 2022-03-17 21:59:40.000000 tailbone-0.9.92/tailbone/templates/trainwreck/transactions/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      357 2022-02-19 22:34:34.000000 tailbone-0.9.92/tailbone/templates/trainwreck/transactions/view_row.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/units-of-measure/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1899 2021-01-27 14:56:25.000000 tailbone-0.9.92/tailbone/templates/units-of-measure/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1736 2023-02-03 22:10:08.000000 tailbone-0.9.92/tailbone/templates/upgrade.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/upgrades/
+-rw-r--r--   0 lance     (1000) lance     (1000)     5196 2023-02-02 00:32:20.000000 tailbone-0.9.92/tailbone/templates/upgrades/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     9408 2024-04-15 00:15:24.000000 tailbone-0.9.92/tailbone/templates/upgrades/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/users/
+-rw-r--r--   0 lance     (1000) lance     (1000)      481 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/templates/users/find_by_perm.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1320 2024-04-14 23:56:36.000000 tailbone-0.9.92/tailbone/templates/users/preferences.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     4517 2023-05-15 13:10:42.000000 tailbone-0.9.92/tailbone/templates/users/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      797 2023-02-03 05:38:48.000000 tailbone-0.9.92/tailbone/templates/util.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/vendors/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1850 2022-05-15 21:04:06.000000 tailbone-0.9.92/tailbone/templates/vendors/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.512639 tailbone-0.9.92/tailbone/templates/views/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/views/model/
+-rw-r--r--   0 lance     (1000) lance     (1000)     9427 2023-01-16 19:50:05.000000 tailbone-0.9.92/tailbone/templates/views/model/create.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.528639 tailbone-0.9.92/tailbone/templates/workorders/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7838 2022-08-10 02:05:11.000000 tailbone-0.9.92/tailbone/templates/workorders/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2637 2019-02-26 03:11:49.000000 tailbone-0.9.92/tailbone/tweens.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13431 2024-04-16 14:47:35.000000 tailbone-0.9.92/tailbone/util.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.532640 tailbone-0.9.92/tailbone/views/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2797 2022-12-10 15:46:54.000000 tailbone-0.9.92/tailbone/views/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.532640 tailbone-0.9.92/tailbone/views/asgi/
+-rw-r--r--   0 lance     (1000) lance     (1000)     4315 2023-06-09 19:22:50.000000 tailbone-0.9.92/tailbone/views/asgi/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2654 2022-08-20 22:38:06.000000 tailbone-0.9.92/tailbone/views/asgi/datasync.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7840 2022-08-21 03:39:57.000000 tailbone-0.9.92/tailbone/views/asgi/upgrades.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9533 2023-12-13 18:05:29.000000 tailbone-0.9.92/tailbone/views/auth.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.532640 tailbone-0.9.92/tailbone/views/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1075 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/views/batch/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    59664 2024-04-15 01:48:34.000000 tailbone-0.9.92/tailbone/views/batch/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3698 2021-10-31 02:25:39.000000 tailbone-0.9.92/tailbone/views/batch/delproduct.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6098 2024-04-14 23:51:02.000000 tailbone-0.9.92/tailbone/views/batch/handheld.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9880 2024-04-15 01:55:22.000000 tailbone-0.9.92/tailbone/views/batch/importer.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    19323 2023-10-06 20:52:44.000000 tailbone-0.9.92/tailbone/views/batch/inventory.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7101 2022-01-10 20:54:44.000000 tailbone-0.9.92/tailbone/views/batch/labels.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6695 2023-08-31 01:01:47.000000 tailbone-0.9.92/tailbone/views/batch/newproduct.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9505 2024-04-15 00:34:44.000000 tailbone-0.9.92/tailbone/views/batch/pos.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    12439 2024-03-26 17:53:16.000000 tailbone-0.9.92/tailbone/views/batch/pricing.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9258 2024-04-14 23:44:49.000000 tailbone-0.9.92/tailbone/views/batch/product.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    15017 2023-05-30 18:24:14.000000 tailbone-0.9.92/tailbone/views/batch/vendorcatalog.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6644 2022-08-14 04:58:46.000000 tailbone-0.9.92/tailbone/views/batch/vendorinvoice.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7059 2023-10-18 23:04:31.000000 tailbone-0.9.92/tailbone/views/bouncer.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3974 2022-07-19 19:48:52.000000 tailbone-0.9.92/tailbone/views/brands.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3712 2022-11-23 17:57:17.000000 tailbone-0.9.92/tailbone/views/categories.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13198 2023-06-17 21:09:24.000000 tailbone-0.9.92/tailbone/views/common.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6188 2023-06-17 20:49:58.000000 tailbone-0.9.92/tailbone/views/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2502 2022-11-23 18:19:27.000000 tailbone-0.9.92/tailbone/views/customergroups.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    31934 2024-04-15 01:54:49.000000 tailbone-0.9.92/tailbone/views/customers.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.532640 tailbone-0.9.92/tailbone/views/custorders/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1213 2020-08-02 04:53:28.000000 tailbone-0.9.92/tailbone/views/custorders/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7676 2023-02-12 15:33:23.000000 tailbone-0.9.92/tailbone/views/custorders/batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1948 2022-11-23 18:19:21.000000 tailbone-0.9.92/tailbone/views/custorders/creating.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    26148 2024-04-15 00:35:12.000000 tailbone-0.9.92/tailbone/views/custorders/items.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    45521 2023-10-25 19:05:36.000000 tailbone-0.9.92/tailbone/views/custorders/orders.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    16525 2023-06-01 16:37:13.000000 tailbone-0.9.92/tailbone/views/datasync.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7781 2024-04-15 00:32:55.000000 tailbone-0.9.92/tailbone/views/departments.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2065 2022-11-23 18:19:03.000000 tailbone-0.9.92/tailbone/views/depositlinks.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    19409 2023-10-30 03:22:01.000000 tailbone-0.9.92/tailbone/views/email.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    14156 2023-10-18 22:53:40.000000 tailbone-0.9.92/tailbone/views/employees.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2229 2023-05-05 15:39:16.000000 tailbone-0.9.92/tailbone/views/essentials.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6163 2022-12-25 18:44:17.000000 tailbone-0.9.92/tailbone/views/exports.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3231 2022-11-23 18:00:03.000000 tailbone-0.9.92/tailbone/views/families.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4000 2023-05-15 13:10:42.000000 tailbone-0.9.92/tailbone/views/features.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2483 2022-11-23 18:18:45.000000 tailbone-0.9.92/tailbone/views/filemon.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1384 2023-09-10 18:50:16.000000 tailbone-0.9.92/tailbone/views/handheld.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2778 2022-11-23 18:18:37.000000 tailbone-0.9.92/tailbone/views/ifps.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    21962 2023-05-10 01:24:53.000000 tailbone-0.9.92/tailbone/views/importing.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2566 2022-11-23 18:18:26.000000 tailbone-0.9.92/tailbone/views/inventory.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.532640 tailbone-0.9.92/tailbone/views/labels/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1155 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/views/labels/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1326 2023-09-10 18:50:26.000000 tailbone-0.9.92/tailbone/views/labels/batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6330 2023-02-09 02:19:03.000000 tailbone-0.9.92/tailbone/views/labels/profiles.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11286 2023-02-03 06:49:24.000000 tailbone-0.9.92/tailbone/views/luigi.py
+-rw-r--r--   0 lance     (1000) lance     (1000)   228233 2024-04-16 01:21:11.000000 tailbone-0.9.92/tailbone/views/master.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    18131 2023-12-01 00:19:11.000000 tailbone-0.9.92/tailbone/views/members.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6801 2023-02-03 06:44:00.000000 tailbone-0.9.92/tailbone/views/menus.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    20407 2024-04-15 18:31:35.000000 tailbone-0.9.92/tailbone/views/messages.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    75831 2024-04-15 01:45:58.000000 tailbone-0.9.92/tailbone/views/people.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1816 2022-11-23 18:18:05.000000 tailbone-0.9.92/tailbone/views/permissions.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.532640 tailbone-0.9.92/tailbone/views/poser/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1138 2022-03-05 00:03:03.000000 tailbone-0.9.92/tailbone/views/poser/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2470 2022-05-11 01:00:46.000000 tailbone-0.9.92/tailbone/views/poser/master.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    10063 2022-05-11 01:00:44.000000 tailbone-0.9.92/tailbone/views/poser/reports.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11220 2022-07-26 17:01:09.000000 tailbone-0.9.92/tailbone/views/poser/views.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6454 2024-04-14 23:38:57.000000 tailbone-0.9.92/tailbone/views/principal.py
+-rw-r--r--   0 lance     (1000) lance     (1000)   102892 2024-04-15 01:46:20.000000 tailbone-0.9.92/tailbone/views/products.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2491 2022-11-23 18:17:55.000000 tailbone-0.9.92/tailbone/views/progress.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    15358 2023-05-20 00:45:29.000000 tailbone-0.9.92/tailbone/views/projects.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.532640 tailbone-0.9.92/tailbone/views/purchases/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1159 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/views/purchases/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13572 2023-10-18 23:17:47.000000 tailbone-0.9.92/tailbone/views/purchases/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6915 2023-09-17 23:22:43.000000 tailbone-0.9.92/tailbone/views/purchases/credits.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.532640 tailbone-0.9.92/tailbone/views/purchasing/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1266 2021-09-29 15:13:18.000000 tailbone-0.9.92/tailbone/views/purchasing/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    34167 2024-04-15 00:36:07.000000 tailbone-0.9.92/tailbone/views/purchasing/batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    12698 2023-06-27 23:18:35.000000 tailbone-0.9.92/tailbone/views/purchasing/costing.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    19673 2024-04-14 23:29:26.000000 tailbone-0.9.92/tailbone/views/purchasing/ordering.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    89356 2024-04-15 00:37:38.000000 tailbone-0.9.92/tailbone/views/purchasing/receiving.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3197 2022-11-23 18:17:10.000000 tailbone-0.9.92/tailbone/views/reportcodes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    29907 2024-04-15 00:32:35.000000 tailbone-0.9.92/tailbone/views/reports.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    20099 2024-04-15 00:39:14.000000 tailbone-0.9.92/tailbone/views/roles.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    16580 2024-04-15 01:25:01.000000 tailbone-0.9.92/tailbone/views/settings.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.536640 tailbone-0.9.92/tailbone/views/shifts/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1207 2018-03-01 00:58:49.000000 tailbone-0.9.92/tailbone/views/shifts/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6797 2023-10-18 23:14:40.000000 tailbone-0.9.92/tailbone/views/shifts/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    22006 2024-04-14 23:49:25.000000 tailbone-0.9.92/tailbone/views/shifts/lib.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9975 2023-02-12 03:56:46.000000 tailbone-0.9.92/tailbone/views/shifts/schedule.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5387 2023-02-12 03:56:32.000000 tailbone-0.9.92/tailbone/views/shifts/timesheet.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3726 2022-11-23 18:16:15.000000 tailbone-0.9.92/tailbone/views/stores.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5677 2023-02-03 22:10:08.000000 tailbone-0.9.92/tailbone/views/subdepartments.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    15898 2024-04-14 23:09:45.000000 tailbone-0.9.92/tailbone/views/tables.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2103 2023-10-07 02:23:35.000000 tailbone-0.9.92/tailbone/views/taxes.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.536640 tailbone-0.9.92/tailbone/views/tempmon/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1344 2020-04-04 20:42:25.000000 tailbone-0.9.92/tailbone/views/tempmon/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6526 2023-01-14 02:16:48.000000 tailbone-0.9.92/tailbone/views/tempmon/appliances.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9593 2023-10-05 18:08:20.000000 tailbone-0.9.92/tailbone/views/tempmon/clients.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3480 2024-04-15 00:40:07.000000 tailbone-0.9.92/tailbone/views/tempmon/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6056 2023-02-12 15:31:40.000000 tailbone-0.9.92/tailbone/views/tempmon/dashboard.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11672 2023-10-18 23:08:32.000000 tailbone-0.9.92/tailbone/views/tempmon/probes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4062 2023-10-18 23:16:37.000000 tailbone-0.9.92/tailbone/views/tempmon/readings.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2076 2023-10-19 22:38:32.000000 tailbone-0.9.92/tailbone/views/tenders.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.536640 tailbone-0.9.92/tailbone/views/trainwreck/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1135 2023-01-19 01:57:13.000000 tailbone-0.9.92/tailbone/views/trainwreck/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    14860 2024-04-15 00:40:27.000000 tailbone-0.9.92/tailbone/views/trainwreck/base.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1582 2022-11-23 18:15:06.000000 tailbone-0.9.92/tailbone/views/trainwreck/defaults.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2409 2023-10-07 01:55:59.000000 tailbone-0.9.92/tailbone/views/typical.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4350 2022-11-23 18:14:52.000000 tailbone-0.9.92/tailbone/views/uoms.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    24918 2024-04-15 01:52:07.000000 tailbone-0.9.92/tailbone/views/upgrades.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    27763 2024-04-15 00:33:08.000000 tailbone-0.9.92/tailbone/views/users.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.536640 tailbone-0.9.92/tailbone/views/vendors/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1236 2023-02-23 01:01:50.000000 tailbone-0.9.92/tailbone/views/vendors/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1363 2023-09-10 18:50:49.000000 tailbone-0.9.92/tailbone/views/vendors/catalogs.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7783 2023-10-24 22:43:48.000000 tailbone-0.9.92/tailbone/views/vendors/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1363 2023-09-10 18:50:41.000000 tailbone-0.9.92/tailbone/views/vendors/invoices.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4738 2023-02-23 04:40:20.000000 tailbone-0.9.92/tailbone/views/vendors/samplefiles.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2951 2021-11-09 23:17:17.000000 tailbone-0.9.92/tailbone/views/versions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6966 2023-10-18 23:16:11.000000 tailbone-0.9.92/tailbone/views/views.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13863 2023-09-02 20:50:35.000000 tailbone-0.9.92/tailbone/views/workorders.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4107 2024-04-16 14:47:52.000000 tailbone-0.9.92/tailbone/webapi.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1445 2024-04-15 15:57:32.000000 tailbone-0.9.92/tasks.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-16 15:44:49.536640 tailbone-0.9.92/tests/
+-rw-rw-r--   0 lance     (1000) lance     (1000)     1057 2023-05-25 19:55:35.000000 tailbone-0.9.92/tests/test_app.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      191 2013-09-10 19:45:40.000000 tailbone-0.9.92/tests/test_helpers.py
```

### Comparing `tailbone-0.9.91/CHANGES.rst` & `tailbone-0.9.92/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 
 CHANGELOG
 =========
 
 Unreleased
 ----------
 
+0.9.92 (2024-04-16)
+-------------------
+
+* Escape underscore char for "contains" query filter.
+
+* Rename custom ``user_css`` context.
+
+* Add support for Pyramid 2.x; new security policy.
+
 
 0.9.91 (2024-04-15)
 -------------------
 
 * Avoid uncaught error when updating order batch row quantities.
 
 * Try to return JSON error when receiving API call fails.
```

### Comparing `tailbone-0.9.91/COPYING.txt` & `tailbone-0.9.92/COPYING.txt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/PKG-INFO` & `tailbone-0.9.92/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tailbone
-Version: 0.9.91
+Version: 0.9.92
 Summary: Backoffice Web Application for Rattail
 Home-page: http://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -23,28 +23,28 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: COPYING.txt
 Requires-Dist: webhelpers2_grid==0.1
 Requires-Dist: deform<2.0.15
-Requires-Dist: pyramid<2
 Requires-Dist: asgiref
 Requires-Dist: colander
 Requires-Dist: ColanderAlchemy
 Requires-Dist: cornice
 Requires-Dist: cornice-swagger
 Requires-Dist: humanize
 Requires-Dist: Mako
 Requires-Dist: markdown
 Requires-Dist: openpyxl
 Requires-Dist: paginate
 Requires-Dist: paginate_sqlalchemy
 Requires-Dist: passlib
 Requires-Dist: Pillow
+Requires-Dist: pyramid
 Requires-Dist: pyramid_beaker>=0.6
 Requires-Dist: pyramid_deform
 Requires-Dist: pyramid_exclog
 Requires-Dist: pyramid_mako
 Requires-Dist: pyramid_retry
 Requires-Dist: pyramid_tm
 Requires-Dist: rattail[bouncer,db]
```

### Comparing `tailbone-0.9.91/Tailbone.egg-info/PKG-INFO` & `tailbone-0.9.92/Tailbone.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tailbone
-Version: 0.9.91
+Version: 0.9.92
 Summary: Backoffice Web Application for Rattail
 Home-page: http://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -23,28 +23,28 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: COPYING.txt
 Requires-Dist: webhelpers2_grid==0.1
 Requires-Dist: deform<2.0.15
-Requires-Dist: pyramid<2
 Requires-Dist: asgiref
 Requires-Dist: colander
 Requires-Dist: ColanderAlchemy
 Requires-Dist: cornice
 Requires-Dist: cornice-swagger
 Requires-Dist: humanize
 Requires-Dist: Mako
 Requires-Dist: markdown
 Requires-Dist: openpyxl
 Requires-Dist: paginate
 Requires-Dist: paginate_sqlalchemy
 Requires-Dist: passlib
 Requires-Dist: Pillow
+Requires-Dist: pyramid
 Requires-Dist: pyramid_beaker>=0.6
 Requires-Dist: pyramid_deform
 Requires-Dist: pyramid_exclog
 Requires-Dist: pyramid_mako
 Requires-Dist: pyramid_retry
 Requires-Dist: pyramid_tm
 Requires-Dist: rattail[bouncer,db]
```

### Comparing `tailbone-0.9.91/Tailbone.egg-info/SOURCES.txt` & `tailbone-0.9.92/Tailbone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/setup.cfg` & `tailbone-0.9.92/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -37,29 +37,28 @@
 [options]
 install_requires = 
 	
 	webhelpers2_grid==0.1
 	
 	deform<2.0.15
 	
-	pyramid<2
-	
 	asgiref
 	colander
 	ColanderAlchemy
 	cornice
 	cornice-swagger
 	humanize
 	Mako
 	markdown
 	openpyxl
 	paginate
 	paginate_sqlalchemy
 	passlib
 	Pillow
+	pyramid
 	pyramid_beaker>=0.6
 	pyramid_deform
 	pyramid_exclog
 	pyramid_mako
 	pyramid_retry
 	pyramid_tm
 	rattail[db,bouncer]
```

### Comparing `tailbone-0.9.91/setup.py` & `tailbone-0.9.92/setup.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/__init__.py` & `tailbone-0.9.92/tailbone/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/__init__.py` & `tailbone-0.9.92/tailbone/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/auth.py` & `tailbone-0.9.92/tailbone/api/auth.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/batch/__init__.py` & `tailbone-0.9.92/tailbone/api/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/batch/core.py` & `tailbone-0.9.92/tailbone/api/batch/core.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/batch/inventory.py` & `tailbone-0.9.92/tailbone/api/batch/inventory.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/batch/labels.py` & `tailbone-0.9.92/tailbone/api/batch/labels.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/batch/ordering.py` & `tailbone-0.9.92/tailbone/api/batch/ordering.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/batch/receiving.py` & `tailbone-0.9.92/tailbone/api/batch/receiving.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/common.py` & `tailbone-0.9.92/tailbone/api/common.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/core.py` & `tailbone-0.9.92/tailbone/api/core.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/customers.py` & `tailbone-0.9.92/tailbone/api/customers.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/essentials.py` & `tailbone-0.9.92/tailbone/api/essentials.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/labels.py` & `tailbone-0.9.92/tailbone/api/labels.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/master.py` & `tailbone-0.9.92/tailbone/api/master.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/master2.py` & `tailbone-0.9.92/tailbone/api/master2.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/people.py` & `tailbone-0.9.92/tailbone/api/people.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/products.py` & `tailbone-0.9.92/tailbone/api/products.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/upgrades.py` & `tailbone-0.9.92/tailbone/api/upgrades.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/users.py` & `tailbone-0.9.92/tailbone/api/users.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/vendors.py` & `tailbone-0.9.92/tailbone/api/vendors.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/api/workorders.py` & `tailbone-0.9.92/tailbone/api/workorders.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/app.py` & `tailbone-0.9.92/tailbone/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -129,16 +129,22 @@
         settings.setdefault('pyramid_deform.template_search_path', 'tailbone:templates/deform')
         config = Configurator(settings=settings, root_factory=Root)
 
     # add rattail config directly to registry
     config.registry['rattail_config'] = rattail_config
 
     # configure user authorization / authentication
-    config.set_authorization_policy(TailboneAuthorizationPolicy())
-    config.set_authentication_policy(SessionAuthenticationPolicy())
+    # TODO: security policy should become the default, for pyramid 2.x
+    if rattail_config.getbool('tailbone', 'pyramid.use_security_policy',
+                              usedb=False, default=False):
+        from tailbone.auth import TailboneSecurityPolicy
+        config.set_security_policy(TailboneSecurityPolicy())
+    else:
+        config.set_authorization_policy(TailboneAuthorizationPolicy())
+        config.set_authentication_policy(SessionAuthenticationPolicy())
 
     # maybe require CSRF token protection
     if configure_csrf:
         config.set_default_csrf_options(require_csrf=True,
                                         token=csrf_token_name(rattail_config),
                                         header=csrf_header_name(rattail_config))
```

### Comparing `tailbone-0.9.91/tailbone/asgi.py` & `tailbone-0.9.92/tailbone/asgi.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/auth.py` & `tailbone-0.9.92/tailbone/auth.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -23,15 +23,14 @@
 """
 Authentication & Authorization
 """
 
 import logging
 import re
 
-from rattail import enum
 from rattail.util import prettify, NOTSET
 
 from zope.interface import implementer
 from pyramid.interfaces import IAuthorizationPolicy
 from pyramid.security import remember, forget, Everyone, Authenticated
 from pyramid.authentication import SessionAuthenticationPolicy
 
@@ -42,31 +41,33 @@
 
 
 def login_user(request, user, timeout=NOTSET):
     """
     Perform the steps necessary to login the given user.  Note that this
     returns a ``headers`` dict which you should pass to the redirect.
     """
-    user.record_event(enum.USER_EVENT_LOGIN)
+    app = request.rattail_config.get_app()
+    user.record_event(app.enum.USER_EVENT_LOGIN)
     headers = remember(request, user.uuid)
     if timeout is NOTSET:
         timeout = session_timeout_for_user(user)
     log.debug("setting session timeout for '{}' to {}".format(user.username, timeout))
     set_session_timeout(request, timeout)
     return headers
 
 
 def logout_user(request):
     """
     Perform the logout action for the given request.  Note that this returns a
     ``headers`` dict which you should pass to the redirect.
     """
+    app = request.rattail_config.get_app()
     user = request.user
     if user:
-        user.record_event(enum.USER_EVENT_LOGOUT)
+        user.record_event(app.enum.USER_EVENT_LOGOUT)
     request.session.delete()
     request.session.invalidate()
     headers = forget(request)
     return headers
 
 
 def session_timeout_for_user(user):
@@ -113,15 +114,15 @@
                 app = rattail_config.get_app()
                 auth = app.get_auth_handler()
                 user = auth.authenticate_user_token(Session(), token)
                 if user:
                     return user.uuid
 
         # otherwise do normal session-based logic
-        return super(TailboneAuthenticationPolicy, self).unauthenticated_userid(request)
+        return super().unauthenticated_userid(request)
 
 
 @implementer(IAuthorizationPolicy)
 class TailboneAuthorizationPolicy(object):
 
     def permits(self, context, principals, permission):
         config = context.request.rattail_config
@@ -146,14 +147,80 @@
             return auth.has_permission(Session(), None, permission)
         return False
 
     def principals_allowed_by_permission(self, context, permission):
         raise NotImplementedError
 
 
+class TailboneSecurityPolicy:
+
+    def __init__(self, api_mode=False):
+        from pyramid.authentication import SessionAuthenticationHelper
+        from pyramid.request import RequestLocalCache
+
+        self.api_mode = api_mode
+        self.session_helper = SessionAuthenticationHelper()
+        self.identity_cache = RequestLocalCache(self.load_identity)
+
+    def load_identity(self, request):
+        config = request.registry.settings.get('rattail_config')
+        app = config.get_app()
+        user = None
+
+        if self.api_mode:
+
+            # determine/load user from header token if present
+            credentials = request.headers.get('Authorization')
+            if credentials:
+                match = re.match(r'^Bearer (\S+)$', credentials)
+                if match:
+                    token = match.group(1)
+                    auth = app.get_auth_handler()
+                    user = auth.authenticate_user_token(Session(), token)
+
+        if not user:
+
+            # fetch user uuid from current session
+            uuid = self.session_helper.authenticated_userid(request)
+            if not uuid:
+                return
+
+            # fetch user object from db
+            model = app.model
+            user = Session.get(model.User, uuid)
+            if not user:
+                return
+
+        # this user is responsible for data changes in current request
+        Session().set_continuum_user(user)
+        return user
+
+    def identity(self, request):
+        return self.identity_cache.get_or_create(request)
+
+    def authenticated_userid(self, request):
+        user = self.identity(request)
+        if user is not None:
+            return user.uuid
+
+    def remember(self, request, userid, **kw):
+        return self.session_helper.remember(request, userid, **kw)
+
+    def forget(self, request, **kw):
+        return self.session_helper.forget(request, **kw)
+
+    def permits(self, request, context, permission):
+        config = request.registry.settings.get('rattail_config')
+        app = config.get_app()
+        auth = app.get_auth_handler()
+
+        user = self.identity(request)
+        return auth.has_permission(Session(), user, permission)
+
+
 def add_permission_group(config, key, label=None, overwrite=True):
     """
     Add a permission group to the app configuration.
     """
     def action():
         perms = config.get_settings().get('tailbone_permissions', {})
         if key not in perms or overwrite:
```

### Comparing `tailbone-0.9.91/tailbone/beaker.py` & `tailbone-0.9.92/tailbone/beaker.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/cleanup.py` & `tailbone-0.9.92/tailbone/cleanup.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/config.py` & `tailbone-0.9.92/tailbone/config.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/db.py` & `tailbone-0.9.92/tailbone/db.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/diffs.py` & `tailbone-0.9.92/tailbone/diffs.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/exceptions.py` & `tailbone-0.9.92/tailbone/exceptions.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/forms/__init__.py` & `tailbone-0.9.92/tailbone/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/forms/common.py` & `tailbone-0.9.92/tailbone/forms/common.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/forms/core.py` & `tailbone-0.9.92/tailbone/forms/core.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/forms/receiving.py` & `tailbone-0.9.92/tailbone/forms/receiving.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/forms/types.py` & `tailbone-0.9.92/tailbone/forms/types.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/forms/widgets.py` & `tailbone-0.9.92/tailbone/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/grids/__init__.py` & `tailbone-0.9.92/tailbone/grids/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/grids/core.py` & `tailbone-0.9.92/tailbone/grids/core.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/grids/filters.py` & `tailbone-0.9.92/tailbone/grids/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -480,33 +480,40 @@
 
     def filter_contains(self, query, value):
         """
         Filter data with a full 'ILIKE' query.
         """
         if value is None or value == '':
             return query
-        return query.filter(sa.and_(
-            *[self.column.ilike(self.encode_value('%{}%'.format(v)))
-              for v in value.split()]))
+
+        criteria = []
+        for val in value.split():
+            val = val.replace('_', r'\_')
+            val = self.encode_value(f'%{val}%')
+            criteria.append(self.column.ilike(val))
+        return query.filter(sa.and_(*criteria))
 
     def filter_does_not_contain(self, query, value):
         """
         Filter data with a full 'NOT ILIKE' query.
         """
         if value is None or value == '':
             return query
 
+        criteria = []
+        for val in value.split():
+            val = val.replace('_', r'\_')
+            val = self.encode_value(f'%{val}%')
+            criteria.append(~self.column.ilike(val))
+
         # When saying something is 'not like' something else, we must also
         # include things which are nothing at all, in our result set.
         return query.filter(sa.or_(
             self.column == None,
-            sa.and_(
-                *[~self.column.ilike(self.encode_value('%{}%'.format(v)))
-                  for v in value.split()]),
-        ))
+            sa.and_(*criteria)))
 
     def filter_contains_any_of(self, query, value):
         """
         This filter expects "multiple values" separated by newline character,
         and will add an "OR" condition with each value being checked via
         "ILIKE".  For instance if the user submits a "value" like this:
 
@@ -527,17 +534,20 @@
         values = value.split('\n')
         values = [value for value in values if value]
         if not values:
             return query
 
         conditions = []
         for value in values:
-            conditions.append(sa.and_(
-                *[self.column.ilike(self.encode_value('%{}%'.format(v)))
-                  for v in value.split()]))
+            criteria = []
+            for val in value.split():
+                val = val.replace('_', r'\_')
+                val = self.encode_value(f'%{val}%')
+                criteria.append(self.column.ilike(val))
+            conditions.append(sa.and_(*criteria))
 
         return query.filter(sa.or_(*conditions))
 
     def filter_is_empty(self, query, value):
         return query.filter(sa.func.ltrim(sa.func.rtrim(self.column)) == self.encode_value(''))
 
     def filter_is_not_empty(self, query, value):
@@ -584,31 +594,39 @@
 
     def filter_contains(self, query, value):
         """
         Filter data with a full 'ILIKE' query.
         """
         if value is None or value == '':
             return query
-        return query.filter(sa.and_(
-            *[self.column.ilike(b'%{}%'.format(v)) for v in value.split()]))
+
+        criteria = []
+        for val in value.split():
+            val = val.replace('_', r'\_')
+            val = b'%{}%'.format(val)
+            criteria.append(self.column.ilike(val))
+        return query.filters(sa.and_(*criteria))
 
     def filter_does_not_contain(self, query, value):
         """
         Filter data with a full 'NOT ILIKE' query.
         """
         if value is None or value == '':
             return query
 
+        for val in value.split():
+            val = val.replace('_', '\_')
+            val = b'%{}%'.format(val)
+            criteria.append(~self.column.ilike(val))
+
         # When saying something is 'not like' something else, we must also
         # include things which are nothing at all, in our result set.
         return query.filter(sa.or_(
             self.column == None,
-            sa.and_(
-                *[~self.column.ilike(b'%{}%'.format(v)) for v in value.split()]),
-        ))
+            sa.and_(*criteria)))
 
 
 class AlchemyNumericFilter(AlchemyGridFilter):
     """
     Numeric filter for SQLAlchemy.
     """
     value_renderer_factory = NumericValueRenderer
```

### Comparing `tailbone-0.9.91/tailbone/handler.py` & `tailbone-0.9.92/tailbone/handler.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/helpers.py` & `tailbone-0.9.92/tailbone/helpers.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/menus.py` & `tailbone-0.9.92/tailbone/menus.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/progress.py` & `tailbone-0.9.92/tailbone/progress.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/providers.py` & `tailbone-0.9.92/tailbone/providers.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/reports/inventory_worksheet.mako` & `tailbone-0.9.92/tailbone/reports/inventory_worksheet.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/reports/ordering_worksheet.mako` & `tailbone-0.9.92/tailbone/reports/ordering_worksheet.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/scaffolds.py` & `tailbone-0.9.92/tailbone/scaffolds.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/__init__.py` & `tailbone-0.9.92/tailbone/static/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/css/codehilite.css` & `tailbone-0.9.92/tailbone/static/css/codehilite.css`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/css/diffs.css` & `tailbone-0.9.92/tailbone/static/css/diffs.css`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/css/forms.css` & `tailbone-0.9.92/tailbone/static/css/forms.css`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/css/grids.css` & `tailbone-0.9.92/tailbone/static/css/grids.css`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/css/grids.rowstatus.css` & `tailbone-0.9.92/tailbone/static/css/grids.rowstatus.css`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/css/layout.css` & `tailbone-0.9.92/tailbone/static/css/layout.css`

 * *Files 11% similar despite different names*

```diff
@@ -132,14 +132,20 @@
     overflow: visible !important;
 }
 
 .modal-card-body {
     overflow: visible !important;
 }
 
+/* TODO: a simpler option we might try sometime instead?  */
+/* cf. https://github.com/buefy/buefy/issues/292#issuecomment-1073851313 */
+
+/* .dropdown-content{ */
+/*     position: fixed; */
+/* } */
 
 /******************************
  * feedback
  ******************************/
 
 .feedback-dialog .red {
     color: red;
```

### Comparing `tailbone-0.9.91/tailbone/static/css/normalize.css` & `tailbone-0.9.92/tailbone/static/css/normalize.css`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/css/perms.css` & `tailbone-0.9.92/tailbone/static/css/perms.css`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/css/progress.css` & `tailbone-0.9.92/tailbone/static/css/progress.css`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/css/timesheet.css` & `tailbone-0.9.92/tailbone/static/css/timesheet.css`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/files/newproduct_template.xlsx` & `tailbone-0.9.92/tailbone/static/files/newproduct_template.xlsx`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/files/vendor_catalog_template.xlsx` & `tailbone-0.9.92/tailbone/static/files/vendor_catalog_template.xlsx`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/img/Hymenocephalus_italicus.jpg` & `tailbone-0.9.92/tailbone/static/img/Hymenocephalus_italicus.jpg`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/img/delete.png` & `tailbone-0.9.92/tailbone/static/img/delete.png`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/img/edit.png` & `tailbone-0.9.92/tailbone/static/img/edit.png`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/img/home_logo.png` & `tailbone-0.9.92/tailbone/static/img/home_logo.png`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/img/loading.gif` & `tailbone-0.9.92/tailbone/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/img/product.png` & `tailbone-0.9.92/tailbone/static/img/product.png`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/img/rattail.ico` & `tailbone-0.9.92/tailbone/static/img/rattail.ico`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/img/save.png` & `tailbone-0.9.92/tailbone/static/img/save.png`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/img/testing.png` & `tailbone-0.9.92/tailbone/static/img/testing.png`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/img/view.png` & `tailbone-0.9.92/tailbone/static/img/view.png`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/js/debounce.js` & `tailbone-0.9.92/tailbone/static/js/debounce.js`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/js/numeric.js` & `tailbone-0.9.92/tailbone/static/js/numeric.js`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/js/tailbone.buefy.autocomplete.js` & `tailbone-0.9.92/tailbone/static/js/tailbone.buefy.autocomplete.js`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/js/tailbone.buefy.datepicker.js` & `tailbone-0.9.92/tailbone/static/js/tailbone.buefy.datepicker.js`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/js/tailbone.buefy.grid.js` & `tailbone-0.9.92/tailbone/static/js/tailbone.buefy.grid.js`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/js/tailbone.buefy.message_recipients.js` & `tailbone-0.9.92/tailbone/static/js/tailbone.buefy.message_recipients.js`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/js/tailbone.buefy.numericinput.js` & `tailbone-0.9.92/tailbone/static/js/tailbone.buefy.numericinput.js`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/js/tailbone.buefy.oncebutton.js` & `tailbone-0.9.92/tailbone/static/js/tailbone.buefy.oncebutton.js`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/js/tailbone.buefy.timepicker.js` & `tailbone-0.9.92/tailbone/static/js/tailbone.buefy.timepicker.js`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/static/js/tailbone.feedback.js` & `tailbone-0.9.92/tailbone/static/js/tailbone.feedback.js`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/subscribers.py` & `tailbone-0.9.92/tailbone/subscribers.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,17 +179,15 @@
                 'tailbone', 'background_color')
 
         # maybe set custom stylesheet
         css = None
         if request.user:
             css = request.rattail_config.get('tailbone.{}'.format(request.user.uuid),
                                              'buefy_css')
-        if not css:
-            css = request.rattail_config.get('tailbone', 'theme.falafel.buefy_css')
-        renderer_globals['buefy_css'] = css
+        renderer_globals['user_css'] = css
 
         # add global search data for quick access
         renderer_globals['global_search_data'] = get_global_search_options(request)
 
         # here we globally declare widths for grid filter pseudo-columns
         widths = request.rattail_config.get('tailbone', 'grids.filters.column_widths')
         if widths:
```

### Comparing `tailbone-0.9.91/tailbone/templates/appinfo/configure.mako` & `tailbone-0.9.92/tailbone/templates/appinfo/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/appinfo/index.mako` & `tailbone-0.9.92/tailbone/templates/appinfo/index.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/appsettings.mako` & `tailbone-0.9.92/tailbone/templates/appsettings.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/autocomplete.mako` & `tailbone-0.9.92/tailbone/templates/autocomplete.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/base.mako` & `tailbone-0.9.92/tailbone/templates/base.mako`

 * *Files 2% similar despite different names*

```diff
@@ -158,17 +158,16 @@
     .filters .filter-verb {
         min-width: ${filter_verb_width};
     }
   </style>
 </%def>
 
 <%def name="buefy_styles()">
-  % if buefy_css:
-      ## custom Buefy CSS
-      ${h.stylesheet_link(buefy_css)}
+  % if user_css:
+      ${h.stylesheet_link(user_css)}
   % else:
       ## upstream Buefy CSS
       ${h.stylesheet_link(h.get_liburl(request, 'buefy.css'))}
   % endif
 </%def>
 
 <%def name="extra_styles()"></%def>
```

#### html2text {}

```diff
@@ -54,17 +54,17 @@
 (tailbone.__version__))} ${h.stylesheet_link(request.static_url('tailbone:
 static/css/filters.css') + '?ver={}'.format(tailbone.__version__))} $
 {h.stylesheet_link(request.static_url('tailbone:static/css/forms.css') + '?ver=
 {}'.format(tailbone.__version__))} ${h.stylesheet_link(request.static_url
 ('tailbone:static/css/diffs.css') + '?ver={}'.format(tailbone.__version__))} $
 {h.stylesheet_link(request.static_url('tailbone:static/css/codehilite.css') +
 '?ver={}'.format(tailbone.__version__))}
-def> <%def name="buefy_styles()"> % if buefy_css: ## custom Buefy CSS $
-{h.stylesheet_link(buefy_css)} % else: ## upstream Buefy CSS $
-{h.stylesheet_link(h.get_liburl(request, 'buefy.css'))} % endif
+def> <%def name="buefy_styles()"> % if user_css: ${h.stylesheet_link(user_css)}
+% else: ## upstream Buefy CSS ${h.stylesheet_link(h.get_liburl(request,
+'buefy.css'))} % endif
 def> <%def name="extra_styles()">
 def> <%def name="head_tags()">
 def> <%def name="render_whole_page_template()">
 ${page_help.render_template()} % if request.has_perm('common.feedback'):
 % endif ${tailbone_autocomplete_template()} ${multi_file_upload.render_template
 ()}
 def> <%def name="render_this_page_component()">
```

### Comparing `tailbone-0.9.91/tailbone/templates/base_meta.mako` & `tailbone-0.9.92/tailbone/templates/base_meta.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/batch/importer/view_row.mako` & `tailbone-0.9.92/tailbone/templates/batch/importer/view_row.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/batch/index.mako` & `tailbone-0.9.92/tailbone/templates/batch/index.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/batch/inventory/desktop_form.mako` & `tailbone-0.9.92/tailbone/templates/batch/inventory/desktop_form.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/batch/pricing/configure.mako` & `tailbone-0.9.92/tailbone/templates/batch/pricing/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/batch/vendorcatalog/configure.mako` & `tailbone-0.9.92/tailbone/templates/batch/vendorcatalog/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/batch/vendorcatalog/create.mako` & `tailbone-0.9.92/tailbone/templates/batch/vendorcatalog/create.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/batch/view.mako` & `tailbone-0.9.92/tailbone/templates/batch/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/configure-menus.mako` & `tailbone-0.9.92/tailbone/templates/configure-menus.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/configure.mako` & `tailbone-0.9.92/tailbone/templates/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/customers/configure.mako` & `tailbone-0.9.92/tailbone/templates/customers/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/customers/pending/view.mako` & `tailbone-0.9.92/tailbone/templates/customers/pending/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/customers/view.mako` & `tailbone-0.9.92/tailbone/templates/customers/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/custorders/configure.mako` & `tailbone-0.9.92/tailbone/templates/custorders/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/custorders/create.mako` & `tailbone-0.9.92/tailbone/templates/custorders/create.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/custorders/items/view.mako` & `tailbone-0.9.92/tailbone/templates/custorders/items/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/datasync/changes/index.mako` & `tailbone-0.9.92/tailbone/templates/datasync/changes/index.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/datasync/configure.mako` & `tailbone-0.9.92/tailbone/templates/datasync/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/datasync/status.mako` & `tailbone-0.9.92/tailbone/templates/datasync/status.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/autocomplete_jquery.pt` & `tailbone-0.9.92/tailbone/templates/deform/autocomplete_jquery.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/cases_units.pt` & `tailbone-0.9.92/tailbone/templates/deform/cases_units.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/checkbox_dynamic.pt` & `tailbone-0.9.92/tailbone/templates/deform/checkbox_dynamic.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/checked_password.pt` & `tailbone-0.9.92/tailbone/templates/deform/checked_password.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/date_jquery.pt` & `tailbone-0.9.92/tailbone/templates/deform/date_jquery.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/date_plain.pt` & `tailbone-0.9.92/tailbone/templates/deform/date_plain.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/datetime_falafel.pt` & `tailbone-0.9.92/tailbone/templates/deform/datetime_falafel.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/file_upload.pt` & `tailbone-0.9.92/tailbone/templates/deform/file_upload.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/message_recipients.pt` & `tailbone-0.9.92/tailbone/templates/deform/message_recipients.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/numberinput.pt` & `tailbone-0.9.92/tailbone/templates/deform/numberinput.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/password.pt` & `tailbone-0.9.92/tailbone/templates/deform/password.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/percentinput.pt` & `tailbone-0.9.92/tailbone/templates/deform/percentinput.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/permissions.pt` & `tailbone-0.9.92/tailbone/templates/deform/permissions.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/problem_report_days.pt` & `tailbone-0.9.92/tailbone/templates/deform/problem_report_days.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/select.pt` & `tailbone-0.9.92/tailbone/templates/deform/select.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/select_dynamic.pt` & `tailbone-0.9.92/tailbone/templates/deform/select_dynamic.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/select_jquery.pt` & `tailbone-0.9.92/tailbone/templates/deform/select_jquery.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/select_plain.pt` & `tailbone-0.9.92/tailbone/templates/deform/select_plain.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/textarea.pt` & `tailbone-0.9.92/tailbone/templates/deform/textarea.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/textinput.pt` & `tailbone-0.9.92/tailbone/templates/deform/textinput.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/deform/time_jquery.pt` & `tailbone-0.9.92/tailbone/templates/deform/time_jquery.pt`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/diff.mako` & `tailbone-0.9.92/tailbone/templates/diff.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/email-bounces/view.mako` & `tailbone-0.9.92/tailbone/templates/email-bounces/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/employees/configure.mako` & `tailbone-0.9.92/tailbone/templates/employees/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/exception.mako` & `tailbone-0.9.92/tailbone/templates/exception.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/form.mako` & `tailbone-0.9.92/tailbone/templates/form.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/formposter.mako` & `tailbone-0.9.92/tailbone/templates/formposter.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/forms/deform.mako` & `tailbone-0.9.92/tailbone/templates/forms/deform.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/generate_feature.mako` & `tailbone-0.9.92/tailbone/templates/generate_feature.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/generated-projects/create.mako` & `tailbone-0.9.92/tailbone/templates/generated-projects/create.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/grids/b-table.mako` & `tailbone-0.9.92/tailbone/templates/grids/b-table.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/grids/complete.mako` & `tailbone-0.9.92/tailbone/templates/grids/complete.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/grids/filters.mako` & `tailbone-0.9.92/tailbone/templates/grids/filters.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/grids/nav.mako` & `tailbone-0.9.92/tailbone/templates/grids/nav.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/home.mako` & `tailbone-0.9.92/tailbone/templates/home.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/importing/configure.mako` & `tailbone-0.9.92/tailbone/templates/importing/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/importing/runjob.mako` & `tailbone-0.9.92/tailbone/templates/importing/runjob.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/importing/view.mako` & `tailbone-0.9.92/tailbone/templates/importing/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/labels/profiles/edit.mako` & `tailbone-0.9.92/tailbone/templates/labels/profiles/edit.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/labels/profiles/view.mako` & `tailbone-0.9.92/tailbone/templates/labels/profiles/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/login.mako` & `tailbone-0.9.92/tailbone/templates/login.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/luigi/configure.mako` & `tailbone-0.9.92/tailbone/templates/luigi/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/luigi/index.mako` & `tailbone-0.9.92/tailbone/templates/luigi/index.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/master/clone.mako` & `tailbone-0.9.92/tailbone/templates/master/clone.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/master/configure.mako` & `tailbone-0.9.92/tailbone/templates/master/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/master/delete.mako` & `tailbone-0.9.92/tailbone/templates/master/delete.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/master/edit_row.mako` & `tailbone-0.9.92/tailbone/templates/master/edit_row.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/master/form.mako` & `tailbone-0.9.92/tailbone/templates/master/form.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/master/index.mako` & `tailbone-0.9.92/tailbone/templates/master/index.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/master/merge.mako` & `tailbone-0.9.92/tailbone/templates/master/merge.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/master/versions.mako` & `tailbone-0.9.92/tailbone/templates/master/versions.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/master/view.mako` & `tailbone-0.9.92/tailbone/templates/master/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/master/view_row.mako` & `tailbone-0.9.92/tailbone/templates/master/view_row.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/master/view_version.mako` & `tailbone-0.9.92/tailbone/templates/master/view_version.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/members/configure.mako` & `tailbone-0.9.92/tailbone/templates/members/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/menu.mako` & `tailbone-0.9.92/tailbone/templates/menu.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/messages/create.mako` & `tailbone-0.9.92/tailbone/templates/messages/create.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/messages/index.mako` & `tailbone-0.9.92/tailbone/templates/messages/index.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/messages/recipients.mako` & `tailbone-0.9.92/tailbone/templates/messages/recipients.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/messages/view.mako` & `tailbone-0.9.92/tailbone/templates/messages/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/multi_file_upload.mako` & `tailbone-0.9.92/tailbone/templates/multi_file_upload.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/ordering/view.mako` & `tailbone-0.9.92/tailbone/templates/ordering/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/ordering/worksheet.mako` & `tailbone-0.9.92/tailbone/templates/ordering/worksheet.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/page.mako` & `tailbone-0.9.92/tailbone/templates/page.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/page_help.mako` & `tailbone-0.9.92/tailbone/templates/page_help.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/people/configure.mako` & `tailbone-0.9.92/tailbone/templates/people/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/people/index.mako` & `tailbone-0.9.92/tailbone/templates/people/index.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/people/merge-requests/view.mako` & `tailbone-0.9.92/tailbone/templates/people/merge-requests/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/people/view.mako` & `tailbone-0.9.92/tailbone/templates/people/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/people/view_profile.mako` & `tailbone-0.9.92/tailbone/templates/people/view_profile.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/poser/reports/view.mako` & `tailbone-0.9.92/tailbone/templates/poser/reports/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/poser/setup.mako` & `tailbone-0.9.92/tailbone/templates/poser/setup.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/poser/views/configure.mako` & `tailbone-0.9.92/tailbone/templates/poser/views/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/principal/find_by_perm.mako` & `tailbone-0.9.92/tailbone/templates/principal/find_by_perm.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/products/batch.mako` & `tailbone-0.9.92/tailbone/templates/products/batch.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/products/configure.mako` & `tailbone-0.9.92/tailbone/templates/products/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/products/index.mako` & `tailbone-0.9.92/tailbone/templates/products/index.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/products/lookup.mako` & `tailbone-0.9.92/tailbone/templates/products/lookup.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/products/pending/view.mako` & `tailbone-0.9.92/tailbone/templates/products/pending/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/products/view.mako` & `tailbone-0.9.92/tailbone/templates/products/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/progress.mako` & `tailbone-0.9.92/tailbone/templates/progress.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/purchases/credits/index.mako` & `tailbone-0.9.92/tailbone/templates/purchases/credits/index.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/purchases/receiving_worksheet.mako` & `tailbone-0.9.92/tailbone/templates/purchases/receiving_worksheet.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/purchases/view.mako` & `tailbone-0.9.92/tailbone/templates/purchases/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/receiving/configure.mako` & `tailbone-0.9.92/tailbone/templates/receiving/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/receiving/declare_credit.mako` & `tailbone-0.9.92/tailbone/templates/receiving/declare_credit.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/receiving/receive_row.mako` & `tailbone-0.9.92/tailbone/templates/receiving/receive_row.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/receiving/view.mako` & `tailbone-0.9.92/tailbone/templates/receiving/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/receiving/view_row.mako` & `tailbone-0.9.92/tailbone/templates/receiving/view_row.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/reports/generated/choose.mako` & `tailbone-0.9.92/tailbone/templates/reports/generated/choose.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/reports/generated/configure.mako` & `tailbone-0.9.92/tailbone/templates/reports/generated/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/reports/generated/generate.mako` & `tailbone-0.9.92/tailbone/templates/reports/generated/generate.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/reports/generated/view.mako` & `tailbone-0.9.92/tailbone/templates/reports/generated/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/reports/inventory.mako` & `tailbone-0.9.92/tailbone/templates/reports/inventory.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/reports/ordering.mako` & `tailbone-0.9.92/tailbone/templates/reports/ordering.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/reports/problems/view.mako` & `tailbone-0.9.92/tailbone/templates/reports/problems/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/roles/create.mako` & `tailbone-0.9.92/tailbone/templates/roles/create.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/roles/edit.mako` & `tailbone-0.9.92/tailbone/templates/roles/edit.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/roles/view.mako` & `tailbone-0.9.92/tailbone/templates/roles/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/settings/email/configure.mako` & `tailbone-0.9.92/tailbone/templates/settings/email/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/settings/email/index.mako` & `tailbone-0.9.92/tailbone/templates/settings/email/index.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/settings/email/view.mako` & `tailbone-0.9.92/tailbone/templates/settings/email/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/shifts/base.mako` & `tailbone-0.9.92/tailbone/templates/shifts/base.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/shifts/schedule.mako` & `tailbone-0.9.92/tailbone/templates/shifts/schedule.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/shifts/schedule_edit.mako` & `tailbone-0.9.92/tailbone/templates/shifts/schedule_edit.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/shifts/schedule_print.mako` & `tailbone-0.9.92/tailbone/templates/shifts/schedule_print.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/shifts/schedule_print_employee.mako` & `tailbone-0.9.92/tailbone/templates/shifts/schedule_print_employee.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/shifts/timesheet.mako` & `tailbone-0.9.92/tailbone/templates/shifts/timesheet.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/shifts/timesheet_edit.mako` & `tailbone-0.9.92/tailbone/templates/shifts/timesheet_edit.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/tables/create.mako` & `tailbone-0.9.92/tailbone/templates/tables/create.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/tempmon/appliances/index.mako` & `tailbone-0.9.92/tailbone/templates/tempmon/appliances/index.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/tempmon/clients/view.mako` & `tailbone-0.9.92/tailbone/templates/tempmon/clients/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/tempmon/dashboard.mako` & `tailbone-0.9.92/tailbone/templates/tempmon/dashboard.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/tempmon/probes/graph.mako` & `tailbone-0.9.92/tailbone/templates/tempmon/probes/graph.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/tempmon/probes/view.mako` & `tailbone-0.9.92/tailbone/templates/tempmon/probes/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/trainwreck/transactions/configure.mako` & `tailbone-0.9.92/tailbone/templates/trainwreck/transactions/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/trainwreck/transactions/rollover.mako` & `tailbone-0.9.92/tailbone/templates/trainwreck/transactions/rollover.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/units-of-measure/index.mako` & `tailbone-0.9.92/tailbone/templates/units-of-measure/index.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/upgrade.mako` & `tailbone-0.9.92/tailbone/templates/upgrade.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/upgrades/configure.mako` & `tailbone-0.9.92/tailbone/templates/upgrades/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/upgrades/view.mako` & `tailbone-0.9.92/tailbone/templates/upgrades/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/users/preferences.mako` & `tailbone-0.9.92/tailbone/templates/users/preferences.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/users/view.mako` & `tailbone-0.9.92/tailbone/templates/users/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/util.mako` & `tailbone-0.9.92/tailbone/templates/util.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/vendors/configure.mako` & `tailbone-0.9.92/tailbone/templates/vendors/configure.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/views/model/create.mako` & `tailbone-0.9.92/tailbone/templates/views/model/create.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/templates/workorders/view.mako` & `tailbone-0.9.92/tailbone/templates/workorders/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/tweens.py` & `tailbone-0.9.92/tailbone/tweens.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/util.py` & `tailbone-0.9.92/tailbone/util.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/__init__.py` & `tailbone-0.9.92/tailbone/views/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/asgi/__init__.py` & `tailbone-0.9.92/tailbone/views/asgi/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/asgi/datasync.py` & `tailbone-0.9.92/tailbone/views/asgi/datasync.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/asgi/upgrades.py` & `tailbone-0.9.92/tailbone/views/asgi/upgrades.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/auth.py` & `tailbone-0.9.92/tailbone/views/auth.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/batch/__init__.py` & `tailbone-0.9.92/tailbone/views/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/batch/core.py` & `tailbone-0.9.92/tailbone/views/batch/core.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/batch/delproduct.py` & `tailbone-0.9.92/tailbone/views/batch/delproduct.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/batch/handheld.py` & `tailbone-0.9.92/tailbone/views/batch/handheld.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/batch/importer.py` & `tailbone-0.9.92/tailbone/views/batch/importer.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/batch/inventory.py` & `tailbone-0.9.92/tailbone/views/batch/inventory.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/batch/labels.py` & `tailbone-0.9.92/tailbone/views/batch/labels.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/batch/newproduct.py` & `tailbone-0.9.92/tailbone/views/batch/newproduct.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/batch/pos.py` & `tailbone-0.9.92/tailbone/views/batch/pos.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/batch/pricing.py` & `tailbone-0.9.92/tailbone/views/batch/pricing.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/batch/product.py` & `tailbone-0.9.92/tailbone/views/batch/product.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/batch/vendorcatalog.py` & `tailbone-0.9.92/tailbone/views/batch/vendorcatalog.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/batch/vendorinvoice.py` & `tailbone-0.9.92/tailbone/views/batch/vendorinvoice.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/bouncer.py` & `tailbone-0.9.92/tailbone/views/bouncer.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/brands.py` & `tailbone-0.9.92/tailbone/views/brands.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/categories.py` & `tailbone-0.9.92/tailbone/views/categories.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/common.py` & `tailbone-0.9.92/tailbone/views/common.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/core.py` & `tailbone-0.9.92/tailbone/views/core.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/customergroups.py` & `tailbone-0.9.92/tailbone/views/customergroups.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/customers.py` & `tailbone-0.9.92/tailbone/views/customers.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/custorders/__init__.py` & `tailbone-0.9.92/tailbone/views/custorders/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/custorders/batch.py` & `tailbone-0.9.92/tailbone/views/custorders/batch.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/custorders/creating.py` & `tailbone-0.9.92/tailbone/views/custorders/creating.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/custorders/items.py` & `tailbone-0.9.92/tailbone/views/custorders/items.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/custorders/orders.py` & `tailbone-0.9.92/tailbone/views/custorders/orders.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/datasync.py` & `tailbone-0.9.92/tailbone/views/datasync.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/departments.py` & `tailbone-0.9.92/tailbone/views/departments.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/depositlinks.py` & `tailbone-0.9.92/tailbone/views/depositlinks.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/email.py` & `tailbone-0.9.92/tailbone/views/email.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/employees.py` & `tailbone-0.9.92/tailbone/views/employees.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/essentials.py` & `tailbone-0.9.92/tailbone/views/essentials.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/exports.py` & `tailbone-0.9.92/tailbone/views/exports.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/families.py` & `tailbone-0.9.92/tailbone/views/families.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/features.py` & `tailbone-0.9.92/tailbone/views/features.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/filemon.py` & `tailbone-0.9.92/tailbone/views/filemon.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/handheld.py` & `tailbone-0.9.92/tailbone/views/handheld.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/ifps.py` & `tailbone-0.9.92/tailbone/views/ifps.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/importing.py` & `tailbone-0.9.92/tailbone/views/importing.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/inventory.py` & `tailbone-0.9.92/tailbone/views/inventory.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/labels/__init__.py` & `tailbone-0.9.92/tailbone/views/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/labels/batch.py` & `tailbone-0.9.92/tailbone/views/labels/batch.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/labels/profiles.py` & `tailbone-0.9.92/tailbone/views/labels/profiles.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/luigi.py` & `tailbone-0.9.92/tailbone/views/luigi.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/master.py` & `tailbone-0.9.92/tailbone/views/master.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/members.py` & `tailbone-0.9.92/tailbone/views/members.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/menus.py` & `tailbone-0.9.92/tailbone/views/menus.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/messages.py` & `tailbone-0.9.92/tailbone/views/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
         if self.creating:
             f.remove('sender', 'sent')
 
             # recipients
             f.insert_after('recipients', 'set_recipients')
             f.remove('recipients')
             f.set_node('set_recipients', colander.SchemaNode(colander.Set()))
-            f.set_widget('set_recipients', RecipientsWidgetBuefy())
+            f.set_widget('set_recipients', RecipientsWidget())
             f.set_label('set_recipients', "To")
 
             if self.replying:
                 old_message = self.get_instance()
                 f.set_default('subject', "Re: {}".format(old_message.subject))
                 f.set_default('body', self.get_reply_body(old_message))
 
@@ -510,15 +510,15 @@
         g.joiners['recipients'] = lambda q: q.join(model.MessageRecipient)\
                                              .join(model.User, model.User.uuid == model.MessageRecipient.recipient_uuid)\
                                              .join(model.Person)
         g.filters['recipients'] = g.make_filter('recipients', model.Person.display_name,
                                                 default_active=True, default_verb='contains')
 
 
-class RecipientsWidgetBuefy(dfwidget.Widget):
+class RecipientsWidget(dfwidget.Widget):
     """
     Custom "message recipients" widget, for use with Vue.js themes.
     """
     template = 'message_recipients'
 
     def deserialize(self, field, pstruct):
         if pstruct is colander.null:
```

### Comparing `tailbone-0.9.91/tailbone/views/people.py` & `tailbone-0.9.92/tailbone/views/people.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/permissions.py` & `tailbone-0.9.92/tailbone/views/permissions.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/poser/__init__.py` & `tailbone-0.9.92/tailbone/views/poser/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/poser/master.py` & `tailbone-0.9.92/tailbone/views/poser/master.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/poser/reports.py` & `tailbone-0.9.92/tailbone/views/poser/reports.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/poser/views.py` & `tailbone-0.9.92/tailbone/views/poser/views.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/principal.py` & `tailbone-0.9.92/tailbone/views/principal.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/products.py` & `tailbone-0.9.92/tailbone/views/products.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/progress.py` & `tailbone-0.9.92/tailbone/views/progress.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/projects.py` & `tailbone-0.9.92/tailbone/views/projects.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/purchases/__init__.py` & `tailbone-0.9.92/tailbone/views/purchases/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/purchases/core.py` & `tailbone-0.9.92/tailbone/views/purchases/core.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/purchases/credits.py` & `tailbone-0.9.92/tailbone/views/purchases/credits.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/purchasing/__init__.py` & `tailbone-0.9.92/tailbone/views/purchasing/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/purchasing/batch.py` & `tailbone-0.9.92/tailbone/views/purchasing/batch.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/purchasing/costing.py` & `tailbone-0.9.92/tailbone/views/purchasing/costing.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/purchasing/ordering.py` & `tailbone-0.9.92/tailbone/views/purchasing/ordering.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/purchasing/receiving.py` & `tailbone-0.9.92/tailbone/views/purchasing/receiving.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/reportcodes.py` & `tailbone-0.9.92/tailbone/views/reportcodes.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/reports.py` & `tailbone-0.9.92/tailbone/views/reports.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/roles.py` & `tailbone-0.9.92/tailbone/views/roles.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/settings.py` & `tailbone-0.9.92/tailbone/views/settings.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/shifts/__init__.py` & `tailbone-0.9.92/tailbone/views/shifts/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/shifts/core.py` & `tailbone-0.9.92/tailbone/views/shifts/core.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/shifts/lib.py` & `tailbone-0.9.92/tailbone/views/shifts/lib.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/shifts/schedule.py` & `tailbone-0.9.92/tailbone/views/shifts/schedule.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/shifts/timesheet.py` & `tailbone-0.9.92/tailbone/views/shifts/timesheet.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/stores.py` & `tailbone-0.9.92/tailbone/views/stores.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/subdepartments.py` & `tailbone-0.9.92/tailbone/views/subdepartments.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/tables.py` & `tailbone-0.9.92/tailbone/views/tables.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/taxes.py` & `tailbone-0.9.92/tailbone/views/taxes.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/tempmon/__init__.py` & `tailbone-0.9.92/tailbone/views/tempmon/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/tempmon/appliances.py` & `tailbone-0.9.92/tailbone/views/tempmon/appliances.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/tempmon/clients.py` & `tailbone-0.9.92/tailbone/views/tempmon/clients.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/tempmon/core.py` & `tailbone-0.9.92/tailbone/views/tempmon/core.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/tempmon/dashboard.py` & `tailbone-0.9.92/tailbone/views/tempmon/dashboard.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/tempmon/probes.py` & `tailbone-0.9.92/tailbone/views/tempmon/probes.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/tempmon/readings.py` & `tailbone-0.9.92/tailbone/views/tempmon/readings.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/tenders.py` & `tailbone-0.9.92/tailbone/views/tenders.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/trainwreck/__init__.py` & `tailbone-0.9.92/tailbone/views/trainwreck/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/trainwreck/base.py` & `tailbone-0.9.92/tailbone/views/trainwreck/base.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/trainwreck/defaults.py` & `tailbone-0.9.92/tailbone/views/trainwreck/defaults.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/typical.py` & `tailbone-0.9.92/tailbone/views/typical.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/uoms.py` & `tailbone-0.9.92/tailbone/views/uoms.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/upgrades.py` & `tailbone-0.9.92/tailbone/views/upgrades.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/users.py` & `tailbone-0.9.92/tailbone/views/users.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/vendors/__init__.py` & `tailbone-0.9.92/tailbone/views/vendors/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/vendors/catalogs.py` & `tailbone-0.9.92/tailbone/views/vendors/catalogs.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/vendors/core.py` & `tailbone-0.9.92/tailbone/views/vendors/core.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/vendors/invoices.py` & `tailbone-0.9.92/tailbone/views/vendors/invoices.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/vendors/samplefiles.py` & `tailbone-0.9.92/tailbone/views/vendors/samplefiles.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/versions.py` & `tailbone-0.9.92/tailbone/views/versions.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/views.py` & `tailbone-0.9.92/tailbone/views/views.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/views/workorders.py` & `tailbone-0.9.92/tailbone/views/workorders.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tailbone/webapi.py` & `tailbone-0.9.92/tailbone/webapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2023 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -46,16 +46,22 @@
     """
     Make a Pyramid config object from the given settings.
     """
     rattail_config = settings['rattail_config']
     pyramid_config = Configurator(settings=settings, root_factory=app.Root)
 
     # configure user authorization / authentication
-    pyramid_config.set_authentication_policy(TailboneAuthenticationPolicy())
-    pyramid_config.set_authorization_policy(TailboneAuthorizationPolicy())
+    # TODO: security policy should become the default, for pyramid 2.x
+    if rattail_config.getbool('tailbone', 'pyramid.use_security_policy',
+                              usedb=False, default=False):
+        from tailbone.auth import TailboneSecurityPolicy
+        pyramid_config.set_security_policy(TailboneSecurityPolicy(api_mode=True))
+    else:
+        pyramid_config.set_authentication_policy(TailboneAuthenticationPolicy())
+        pyramid_config.set_authorization_policy(TailboneAuthorizationPolicy())
 
     # always require CSRF token protection
     pyramid_config.set_default_csrf_options(require_csrf=True,
                                             token='_csrf',
                                             header='X-XSRF-TOKEN')
 
     # bring in some Pyramid goodies
```

### Comparing `tailbone-0.9.91/tasks.py` & `tailbone-0.9.92/tasks.py`

 * *Files identical despite different names*

### Comparing `tailbone-0.9.91/tests/test_app.py` & `tailbone-0.9.92/tests/test_app.py`

 * *Files identical despite different names*
