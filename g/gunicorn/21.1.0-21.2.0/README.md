# Comparing `tmp/gunicorn-21.1.0.tar.gz` & `tmp/gunicorn-21.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gunicorn-21.1.0.tar", last modified: Tue Jul 18 12:53:23 2023, max compression
+gzip compressed data, was "gunicorn-21.2.0.tar", last modified: Wed Jul 19 11:46:16 2023, max compression
```

## Comparing `gunicorn-21.1.0.tar` & `gunicorn-21.2.0.tar`

### file list

```diff
@@ -1,485 +1,485 @@
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.775562 gunicorn-21.1.0/
--rwxr-xr-x   0 benoitc    (501) staff       (20)      267 2023-07-17 19:03:36.000000 gunicorn-21.1.0/.gitignore
--rw-r--r--   0 benoitc    (501) staff       (20)     1136 2023-07-17 19:03:36.000000 gunicorn-21.1.0/LICENSE
--rw-r--r--   0 benoitc    (501) staff       (20)      324 2023-07-17 19:03:36.000000 gunicorn-21.1.0/MANIFEST.in
--rw-r--r--   0 benoitc    (501) staff       (20)     3777 2023-07-17 19:03:36.000000 gunicorn-21.1.0/NOTICE
--rw-r--r--   0 benoitc    (501) staff       (20)     3830 2023-07-18 12:53:23.775633 gunicorn-21.1.0/PKG-INFO
--rw-r--r--   0 benoitc    (501) staff       (20)     1988 2023-07-17 19:03:36.000000 gunicorn-21.1.0/README.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     6969 2023-07-17 19:03:36.000000 gunicorn-21.1.0/THANKS
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.726738 gunicorn-21.1.0/docs/
--rw-r--r--   0 benoitc    (501) staff       (20)     5791 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/Makefile
--rw-r--r--   0 benoitc    (501) staff       (20)      288 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/README.rst
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.722346 gunicorn-21.1.0/docs/build/
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.730758 gunicorn-21.1.0/docs/build/doctrees/
--rw-r--r--   0 benoitc    (501) staff       (20)    43583 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/2010-news.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    15287 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/2011-news.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    27991 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/2012-news.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    19851 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/2013-news.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    48784 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/2014-news.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    51800 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/2015-news.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    25377 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/2016-news.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    17557 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/2017-news.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    29568 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/2018-news.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    33177 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/2019-news.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)     2984 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/2020-news.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    13095 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/2021-news.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)     5292 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/2023-news.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    11251 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/community.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    17815 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/configure.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    10993 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/custom.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    54089 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/deploy.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    25657 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/design.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)  1267881 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/environment.pickle
--rw-r--r--   0 benoitc    (501) staff       (20)    35498 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/faq.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)     8337 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/index.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    27785 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/install.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)     9613 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/instrumentation.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)     6075 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/news.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    31793 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/run.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)   261405 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/settings.doctree
--rw-r--r--   0 benoitc    (501) staff       (20)    24042 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/doctrees/signals.doctree
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.734157 gunicorn-21.1.0/docs/build/html/
--rw-r--r--   0 benoitc    (501) staff       (20)      230 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/.buildinfo
--rw-r--r--   0 benoitc    (501) staff       (20)    19422 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/html/2010-news.html
--rw-r--r--   0 benoitc    (501) staff       (20)    10972 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/html/2011-news.html
--rw-r--r--   0 benoitc    (501) staff       (20)    15120 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/html/2012-news.html
--rw-r--r--   0 benoitc    (501) staff       (20)    13036 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/html/2013-news.html
--rw-r--r--   0 benoitc    (501) staff       (20)    20800 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/html/2014-news.html
--rw-r--r--   0 benoitc    (501) staff       (20)    23465 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/html/2015-news.html
--rw-r--r--   0 benoitc    (501) staff       (20)    15406 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/html/2016-news.html
--rw-r--r--   0 benoitc    (501) staff       (20)    12213 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/html/2017-news.html
--rw-r--r--   0 benoitc    (501) staff       (20)    17042 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/html/2018-news.html
--rw-r--r--   0 benoitc    (501) staff       (20)    14935 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/html/2019-news.html
--rw-r--r--   0 benoitc    (501) staff       (20)     7097 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/html/2020-news.html
--rw-r--r--   0 benoitc    (501) staff       (20)     9650 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/html/2021-news.html
--rw-r--r--   0 benoitc    (501) staff       (20)     7724 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/html/2023-news.html
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.734276 gunicorn-21.1.0/docs/build/html/_images/
--rw-r--r--   0 benoitc    (501) staff       (20)    14398 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_images/gunicorn.png
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.736900 gunicorn-21.1.0/docs/build/html/_sources/
--rw-r--r--   0 benoitc    (501) staff       (20)     6643 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/2010-news.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     2092 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/2011-news.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     4184 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/2012-news.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     3267 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/2013-news.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     6834 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/2014-news.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     5702 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/2015-news.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     2911 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/2016-news.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     2100 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/2017-news.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     2956 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/2018-news.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     4785 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/2019-news.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      112 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/2020-news.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     1905 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/2021-news.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      530 2023-07-17 20:14:25.000000 gunicorn-21.1.0/docs/build/html/_sources/2023-news.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     1377 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/community.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     3873 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/configure.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     1927 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/custom.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)    12260 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/deploy.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     6483 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/design.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     8672 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/faq.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     1043 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     5551 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/install.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     1325 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/instrumentation.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      727 2023-07-17 20:14:25.000000 gunicorn-21.1.0/docs/build/html/_sources/news.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     6485 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/run.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)    36935 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/html/_sources/settings.rst.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     5420 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_sources/signals.rst.txt
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.738007 gunicorn-21.1.0/docs/build/html/_static/
--rw-r--r--   0 benoitc    (501) staff       (20)    14813 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/_static/basic.css
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.738206 gunicorn-21.1.0/docs/build/html/_static/css/
--rw-r--r--   0 benoitc    (501) staff       (20)     3229 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/badge_only.css
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.741517 gunicorn-21.1.0/docs/build/html/_static/css/fonts/
--rw-r--r--   0 benoitc    (501) staff       (20)    87624 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 benoitc    (501) staff       (20)    67312 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 benoitc    (501) staff       (20)    86288 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 benoitc    (501) staff       (20)    66444 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 benoitc    (501) staff       (20)   165742 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 benoitc    (501) staff       (20)   444379 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 benoitc    (501) staff       (20)   165548 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 benoitc    (501) staff       (20)    98024 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 benoitc    (501) staff       (20)    77160 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 benoitc    (501) staff       (20)   323344 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 benoitc    (501) staff       (20)   193308 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 benoitc    (501) staff       (20)   309728 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 benoitc    (501) staff       (20)   184912 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 benoitc    (501) staff       (20)   328412 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 benoitc    (501) staff       (20)   195704 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 benoitc    (501) staff       (20)   309192 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 benoitc    (501) staff       (20)   182708 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 benoitc    (501) staff       (20)   135314 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/css/theme.css
--rw-r--r--   0 benoitc    (501) staff       (20)     4472 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/doctools.js
--rw-r--r--   0 benoitc    (501) staff       (20)      421 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/_static/documentation_options.js
--rw-r--r--   0 benoitc    (501) staff       (20)      286 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/file.png
--rw-r--r--   0 benoitc    (501) staff       (20)    14398 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/build/html/_static/gunicorn.png
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.742023 gunicorn-21.1.0/docs/build/html/_static/js/
--rw-r--r--   0 benoitc    (501) staff       (20)      934 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/js/badge_only.js
--rw-r--r--   0 benoitc    (501) staff       (20)     4370 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 benoitc    (501) staff       (20)     2734 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 benoitc    (501) staff       (20)     5023 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/js/theme.js
--rw-r--r--   0 benoitc    (501) staff       (20)     4758 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/_static/language_data.js
--rw-r--r--   0 benoitc    (501) staff       (20)       90 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/minus.png
--rw-r--r--   0 benoitc    (501) staff       (20)       90 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/plus.png
--rw-r--r--   0 benoitc    (501) staff       (20)     4846 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/_static/pygments.css
--rw-r--r--   0 benoitc    (501) staff       (20)    18215 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/searchtools.js
--rw-r--r--   0 benoitc    (501) staff       (20)     4712 2023-07-17 19:08:28.000000 gunicorn-21.1.0/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0 benoitc    (501) staff       (20)     7909 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/build/html/community.html
--rw-r--r--   0 benoitc    (501) staff       (20)    12328 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/configure.html
--rw-r--r--   0 benoitc    (501) staff       (20)    14413 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/custom.html
--rw-r--r--   0 benoitc    (501) staff       (20)    40350 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/deploy.html
--rw-r--r--   0 benoitc    (501) staff       (20)    14905 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/design.html
--rw-r--r--   0 benoitc    (501) staff       (20)    26212 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/faq.html
--rw-r--r--   0 benoitc    (501) staff       (20)     4623 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/genindex.html
--rw-r--r--   0 benoitc    (501) staff       (20)    13234 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/index.html
--rw-r--r--   0 benoitc    (501) staff       (20)    18129 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/install.html
--rw-r--r--   0 benoitc    (501) staff       (20)     7694 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/instrumentation.html
--rw-r--r--   0 benoitc    (501) staff       (20)     8954 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/news.html
--rw-r--r--   0 benoitc    (501) staff       (20)     1679 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/objects.inv
--rw-r--r--   0 benoitc    (501) staff       (20)    20340 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/run.html
--rw-r--r--   0 benoitc    (501) staff       (20)     4713 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/search.html
--rw-r--r--   0 benoitc    (501) staff       (20)    61641 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/searchindex.js
--rw-r--r--   0 benoitc    (501) staff       (20)   116855 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/settings.html
--rw-r--r--   0 benoitc    (501) staff       (20)    25507 2023-07-17 21:13:37.000000 gunicorn-21.1.0/docs/build/html/signals.html
--rwxr-xr-x   0 benoitc    (501) staff       (20)     3029 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/gunicorn_ext.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.742237 gunicorn-21.1.0/docs/logo/
--rw-r--r--   0 benoitc    (501) staff       (20)    21550 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/logo/gunicorn.png
--rw-r--r--   0 benoitc    (501) staff       (20)    12798 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/logo/gunicorn.svg
--rw-r--r--   0 benoitc    (501) staff       (20)     5109 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/make.bat
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.744017 gunicorn-21.1.0/docs/site/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/.nojekyll
--rw-r--r--   0 benoitc    (501) staff       (20)       13 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/CNAME
--rw-r--r--   0 benoitc    (501) staff       (20)      340 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/community.html
--rw-r--r--   0 benoitc    (501) staff       (20)      304 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/configuration.html
--rw-r--r--   0 benoitc    (501) staff       (20)      300 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/configure.html
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.744137 gunicorn-21.1.0/docs/site/css/
--rw-r--r--   0 benoitc    (501) staff       (20)     6671 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/css/style.css
--rw-r--r--   0 benoitc    (501) staff       (20)      343 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/deploy.html
--rw-r--r--   0 benoitc    (501) staff       (20)      342 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/deployment.html
--rw-r--r--   0 benoitc    (501) staff       (20)      297 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/design.html
--rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/faq.html
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.746127 gunicorn-21.1.0/docs/site/images/
--rw-r--r--   0 benoitc    (501) staff       (20)    17551 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/about.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)      408 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/arrow.png
--rw-r--r--   0 benoitc    (501) staff       (20)      611 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/banner-bg.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)    15593 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/community.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)    17566 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/documents.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)    15962 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/downloads.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)     1771 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/favicon.png
--rw-r--r--   0 benoitc    (501) staff       (20)      255 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/footer-arrow.png
--rw-r--r--   0 benoitc    (501) staff       (20)     2499 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/footer-logo.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)      335 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/greenbutton.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)     1553 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/gunicorn.png
--rw-r--r--   0 benoitc    (501) staff       (20)    21956 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/large_gunicorn.png
--rw-r--r--   0 benoitc    (501) staff       (20)     3145 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/logo-bottom.png
--rw-r--r--   0 benoitc    (501) staff       (20)    10238 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/logo.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)     7343 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/logo.png
--rw-r--r--   0 benoitc    (501) staff       (20)      577 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/redbutton.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)      440 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/separator.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)     3450 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/title.png
--rw-r--r--   0 benoitc    (501) staff       (20)     2184 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/images/user1.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)     7856 2023-07-18 12:48:51.000000 gunicorn-21.1.0/docs/site/index.html
--rw-r--r--   0 benoitc    (501) staff       (20)      298 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/install.html
--rw-r--r--   0 benoitc    (501) staff       (20)      298 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/installation.html
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.746223 gunicorn-21.1.0/docs/site/js/
--rwxr-xr-x   0 benoitc    (501) staff       (20)     1479 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/js/main.js
--rw-r--r--   0 benoitc    (501) staff       (20)      295 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/news.html
--rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/run.html
--rw-r--r--   0 benoitc    (501) staff       (20)     1990 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/sitemap.xml
--rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/tuning.html
--rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/site/usage.html
--rw-r--r--   0 benoitc    (501) staff       (20)     2088 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/sitemap_gen.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.749240 gunicorn-21.1.0/docs/source/
--rw-r--r--   0 benoitc    (501) staff       (20)     6643 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/2010-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     2092 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/2011-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     4184 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/2012-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     3267 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/2013-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     6834 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/2014-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     5702 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/2015-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     2911 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/2016-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     2100 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/2017-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     2956 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/2018-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     4785 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/2019-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)      112 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/2020-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1905 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/2021-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)      695 2023-07-18 12:48:51.000000 gunicorn-21.1.0/docs/source/2023-news.rst
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.749370 gunicorn-21.1.0/docs/source/_static/
--rw-r--r--   0 benoitc    (501) staff       (20)    14398 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/_static/gunicorn.png
--rw-r--r--   0 benoitc    (501) staff       (20)     1377 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/community.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1755 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/conf.py
--rw-r--r--   0 benoitc    (501) staff       (20)     3873 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/configure.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1927 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/custom.rst
--rw-r--r--   0 benoitc    (501) staff       (20)    12260 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/deploy.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     6483 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/design.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     8672 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/faq.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1043 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/index.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     5551 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/install.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1325 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/instrumentation.rst
--rw-r--r--   0 benoitc    (501) staff       (20)      892 2023-07-18 12:48:51.000000 gunicorn-21.1.0/docs/source/news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     6485 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/run.rst
--rw-r--r--   0 benoitc    (501) staff       (20)    36935 2023-07-17 21:13:36.000000 gunicorn-21.1.0/docs/source/settings.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     5420 2023-07-17 19:03:36.000000 gunicorn-21.1.0/docs/source/signals.rst
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.752460 gunicorn-21.1.0/examples/
--rw-r--r--   0 benoitc    (501) staff       (20)      738 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/alt_spec.py
--rw-r--r--   0 benoitc    (501) staff       (20)      204 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/bad.py
--rw-r--r--   0 benoitc    (501) staff       (20)      108 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/boot_fail.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.752698 gunicorn-21.1.0/examples/deep/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/deep/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)      659 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/deep/test.py
--rw-r--r--   0 benoitc    (501) staff       (20)      676 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/echo.py
--rw-r--r--   0 benoitc    (501) staff       (20)     7621 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/example_config.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.754317 gunicorn-21.1.0/examples/frameworks/
--rw-r--r--   0 benoitc    (501) staff       (20)      198 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/cherryapp.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.754442 gunicorn-21.1.0/examples/frameworks/django/
--rw-r--r--   0 benoitc    (501) staff       (20)       60 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/django/README
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.754570 gunicorn-21.1.0/examples/frameworks/django/testing/
--rwxr-xr-x   0 benoitc    (501) staff       (20)      244 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/django/testing/manage.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.754999 gunicorn-21.1.0/examples/frameworks/django/testing/testing/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/django/testing/testing/__init__.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.755110 gunicorn-21.1.0/examples/frameworks/django/testing/testing/apps/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/django/testing/testing/apps/__init__.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.755674 gunicorn-21.1.0/examples/frameworks/django/testing/testing/apps/someapp/
--rwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/django/testing/testing/apps/someapp/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)      627 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/django/testing/testing/apps/someapp/middleware.py
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/django/testing/testing/apps/someapp/models.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.755889 gunicorn-21.1.0/examples/frameworks/django/testing/testing/apps/someapp/templates/
--rw-r--r--   0 benoitc    (501) staff       (20)      759 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html
--rw-r--r--   0 benoitc    (501) staff       (20)      471 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/django/testing/testing/apps/someapp/templates/home.html
--rwxr-xr-x   0 benoitc    (501) staff       (20)      509 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/django/testing/testing/apps/someapp/tests.py
--rw-r--r--   0 benoitc    (501) staff       (20)      133 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/django/testing/testing/apps/someapp/urls.py
--rwxr-xr-x   0 benoitc    (501) staff       (20)     1548 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/django/testing/testing/apps/someapp/views.py
--rw-r--r--   0 benoitc    (501) staff       (20)     5730 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/django/testing/testing/settings.py
--rw-r--r--   0 benoitc    (501) staff       (20)      577 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/django/testing/testing/urls.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1359 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/django/testing/testing/wsgi.py
--rw-r--r--   0 benoitc    (501) staff       (20)      291 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/flask_sendfile.py
--rw-r--r--   0 benoitc    (501) staff       (20)      147 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/flaskapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)      501 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/flaskapp_aiohttp_wsgi.py
--rw-r--r--   0 benoitc    (501) staff       (20)      338 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/pyramidapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)      150 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/requirements.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        9 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/requirements_cherryapp.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        6 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/requirements_flaskapp.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        8 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/requirements_pyramidapp.txt
--rw-r--r--   0 benoitc    (501) staff       (20)       10 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/requirements_tornadoapp.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        7 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/requirements_webpyapp.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      873 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/tornadoapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)      197 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/frameworks/webpyapp.py
--rwxr-xr-x   0 benoitc    (501) staff       (20)      215 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/gunicorn_rc
--rw-r--r--   0 benoitc    (501) staff       (20)       13 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/hello.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      448 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/log_app.ini
--rw-r--r--   0 benoitc    (501) staff       (20)      372 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/log_app.py
--rw-r--r--   0 benoitc    (501) staff       (20)      841 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/logging.conf
--rw-r--r--   0 benoitc    (501) staff       (20)      737 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/longpoll.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1470 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/multiapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)      993 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/multidomainapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1980 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/nginx.conf
--rw-r--r--   0 benoitc    (501) staff       (20)      403 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/read_django_settings.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1015 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/readline_app.py
--rw-r--r--   0 benoitc    (501) staff       (20)      584 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/sendfile.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1257 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/server.crt
--rw-r--r--   0 benoitc    (501) staff       (20)     1679 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/server.key
--rw-r--r--   0 benoitc    (501) staff       (20)      604 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/slowclient.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1339 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/standalone_app.py
--rw-r--r--   0 benoitc    (501) staff       (20)      182 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/supervisor.conf
--rw-r--r--   0 benoitc    (501) staff       (20)      659 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/test.py
--rw-r--r--   0 benoitc    (501) staff       (20)      620 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/timeout.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.756188 gunicorn-21.1.0/examples/websocket/
--rw-r--r--   0 benoitc    (501) staff       (20)    15684 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/websocket/gevent_websocket.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1320 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/websocket/websocket.html
--rw-r--r--   0 benoitc    (501) staff       (20)    15729 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/websocket/websocket.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1020 2023-07-17 19:03:36.000000 gunicorn-21.1.0/examples/when_ready.conf.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.757403 gunicorn-21.1.0/gunicorn/
--rw-r--r--   0 benoitc    (501) staff       (20)      279 2023-07-18 12:48:51.000000 gunicorn-21.1.0/gunicorn/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)      171 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/__main__.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.758477 gunicorn-21.1.0/gunicorn/app/
--rw-r--r--   0 benoitc    (501) staff       (20)      127 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/app/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)     7400 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/app/base.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2038 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/app/pasterapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1926 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/app/wsgiapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)    21509 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/arbiter.py
--rw-r--r--   0 benoitc    (501) staff       (20)    63419 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/config.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2293 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/debug.py
--rw-r--r--   0 benoitc    (501) staff       (20)      919 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/errors.py
--rw-r--r--   0 benoitc    (501) staff       (20)    15303 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/glogging.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.759167 gunicorn-21.1.0/gunicorn/http/
--rw-r--r--   0 benoitc    (501) staff       (20)      277 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/http/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)     7296 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/http/body.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2850 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/http/errors.py
--rw-r--r--   0 benoitc    (501) staff       (20)    11958 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/http/message.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1364 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/http/parser.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1943 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/http/unreader.py
--rw-r--r--   0 benoitc    (501) staff       (20)    12366 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/http/wsgi.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.759348 gunicorn-21.1.0/gunicorn/instrument/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/instrument/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)     4690 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/instrument/statsd.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2367 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/pidfile.py
--rw-r--r--   0 benoitc    (501) staff       (20)     3791 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/reloader.py
--rw-r--r--   0 benoitc    (501) staff       (20)     6887 2023-07-18 12:00:28.000000 gunicorn-21.1.0/gunicorn/sock.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2520 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/systemd.py
--rw-r--r--   0 benoitc    (501) staff       (20)    19127 2023-07-17 21:06:48.000000 gunicorn-21.1.0/gunicorn/util.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.760273 gunicorn-21.1.0/gunicorn/workers/
--rw-r--r--   0 benoitc    (501) staff       (20)      594 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/workers/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)     9197 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/workers/base.py
--rw-r--r--   0 benoitc    (501) staff       (20)     5681 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/workers/base_async.py
--rw-r--r--   0 benoitc    (501) staff       (20)     6091 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/workers/geventlet.py
--rw-r--r--   0 benoitc    (501) staff       (20)     5800 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/workers/ggevent.py
--rw-r--r--   0 benoitc    (501) staff       (20)    12718 2023-07-18 12:48:51.000000 gunicorn-21.1.0/gunicorn/workers/gthread.py
--rw-r--r--   0 benoitc    (501) staff       (20)     5854 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/workers/gtornado.py
--rw-r--r--   0 benoitc    (501) staff       (20)     7272 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/workers/sync.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1651 2023-07-17 19:03:36.000000 gunicorn-21.1.0/gunicorn/workers/workertmp.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.758094 gunicorn-21.1.0/gunicorn.egg-info/
--rw-r--r--   0 benoitc    (501) staff       (20)     3830 2023-07-18 12:53:23.000000 gunicorn-21.1.0/gunicorn.egg-info/PKG-INFO
--rw-r--r--   0 benoitc    (501) staff       (20)    13924 2023-07-18 12:53:23.000000 gunicorn-21.1.0/gunicorn.egg-info/SOURCES.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        1 2023-07-18 12:53:23.000000 gunicorn-21.1.0/gunicorn.egg-info/dependency_links.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      113 2023-07-18 12:53:23.000000 gunicorn-21.1.0/gunicorn.egg-info/entry_points.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        1 2023-07-17 20:27:30.000000 gunicorn-21.1.0/gunicorn.egg-info/not-zip-safe
--rw-r--r--   0 benoitc    (501) staff       (20)      173 2023-07-18 12:53:23.000000 gunicorn-21.1.0/gunicorn.egg-info/requires.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        9 2023-07-18 12:53:23.000000 gunicorn-21.1.0/gunicorn.egg-info/top_level.txt
--rw-r--r--   0 benoitc    (501) staff       (20)       50 2023-07-17 19:03:36.000000 gunicorn-21.1.0/requirements_dev.txt
--rw-r--r--   0 benoitc    (501) staff       (20)       56 2023-07-17 20:45:55.000000 gunicorn-21.1.0/requirements_test.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      208 2023-07-18 12:53:23.775832 gunicorn-21.1.0/setup.cfg
--rw-r--r--   0 benoitc    (501) staff       (20)     3555 2023-07-17 19:03:36.000000 gunicorn-21.1.0/setup.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.761906 gunicorn-21.1.0/tests/
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.762281 gunicorn-21.1.0/tests/config/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/config/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)       88 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/config/test_cfg.py
--rw-r--r--   0 benoitc    (501) staff       (20)       24 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/config/test_cfg_alt.py
--rw-r--r--   0 benoitc    (501) staff       (20)       23 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/config/test_cfg_with_wsgi_app.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.724757 gunicorn-21.1.0/tests/requests/
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.767441 gunicorn-21.1.0/tests/requests/invalid/
--rw-r--r--   0 benoitc    (501) staff       (20)       29 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/001.http
--rw-r--r--   0 benoitc    (501) staff       (20)       64 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/001.py
--rw-r--r--   0 benoitc    (501) staff       (20)       21 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/002.http
--rw-r--r--   0 benoitc    (501) staff       (20)       81 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/002.py
--rw-r--r--   0 benoitc    (501) staff       (20)       30 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/003.http
--rw-r--r--   0 benoitc    (501) staff       (20)       84 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/003.py
--rw-r--r--   0 benoitc    (501) staff       (20)       25 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/004.http
--rw-r--r--   0 benoitc    (501) staff       (20)       80 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/004.py
--rw-r--r--   0 benoitc    (501) staff       (20)       41 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/005.http
--rw-r--r--   0 benoitc    (501) staff       (20)       78 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/005.py
--rw-r--r--   0 benoitc    (501) staff       (20)     4122 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/006.http
--rw-r--r--   0 benoitc    (501) staff       (20)       77 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/006.py
--rw-r--r--   0 benoitc    (501) staff       (20)     8358 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/007.http
--rw-r--r--   0 benoitc    (501) staff       (20)       83 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/007.py
--rw-r--r--   0 benoitc    (501) staff       (20)    12418 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/008.http
--rw-r--r--   0 benoitc    (501) staff       (20)       83 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/008.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1829 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/009.http
--rw-r--r--   0 benoitc    (501) staff       (20)       83 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/009.py
--rw-r--r--   0 benoitc    (501) staff       (20)       44 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/010.http
--rw-r--r--   0 benoitc    (501) staff       (20)      174 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/010.py
--rw-r--r--   0 benoitc    (501) staff       (20)      169 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/011.http
--rw-r--r--   0 benoitc    (501) staff       (20)      169 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/011.py
--rw-r--r--   0 benoitc    (501) staff       (20)      169 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/012.http
--rw-r--r--   0 benoitc    (501) staff       (20)      174 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/012.py
--rw-r--r--   0 benoitc    (501) staff       (20)       49 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/013.http
--rw-r--r--   0 benoitc    (501) staff       (20)      174 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/013.py
--rw-r--r--   0 benoitc    (501) staff       (20)       78 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/014.http
--rw-r--r--   0 benoitc    (501) staff       (20)       72 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/014.py
--rw-r--r--   0 benoitc    (501) staff       (20)       88 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/015.http
--rw-r--r--   0 benoitc    (501) staff       (20)       72 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/015.py
--rw-r--r--   0 benoitc    (501) staff       (20)       33 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/016.http
--rw-r--r--   0 benoitc    (501) staff       (20)       82 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/016.py
--rw-r--r--   0 benoitc    (501) staff       (20)     8222 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/017.http
--rw-r--r--   0 benoitc    (501) staff       (20)      134 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/017.py
--rw-r--r--   0 benoitc    (501) staff       (20)       48 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/018.http
--rw-r--r--   0 benoitc    (501) staff       (20)       81 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/018.py
--rw-r--r--   0 benoitc    (501) staff       (20)       82 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/019.http
--rw-r--r--   0 benoitc    (501) staff       (20)      172 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/019.py
--rw-r--r--   0 benoitc    (501) staff       (20)       69 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/020.http
--rw-r--r--   0 benoitc    (501) staff       (20)      130 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/020.py
--rw-r--r--   0 benoitc    (501) staff       (20)       90 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/021.http
--rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/021.py
--rw-r--r--   0 benoitc    (501) staff       (20)       51 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/022.http
--rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/022.py
--rw-r--r--   0 benoitc    (501) staff       (20)       52 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/023.http
--rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/023.py
--rw-r--r--   0 benoitc    (501) staff       (20)       51 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/024.http
--rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/024.py
--rw-r--r--   0 benoitc    (501) staff       (20)       37 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/pp_01.http
--rw-r--r--   0 benoitc    (501) staff       (20)      161 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/pp_01.py
--rw-r--r--   0 benoitc    (501) staff       (20)       53 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/pp_02.http
--rw-r--r--   0 benoitc    (501) staff       (20)      161 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/invalid/pp_02.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.775047 gunicorn-21.1.0/tests/requests/valid/
--rw-r--r--   0 benoitc    (501) staff       (20)      149 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/001.http
--rw-r--r--   0 benoitc    (501) staff       (20)      275 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/001.py
--rw-r--r--   0 benoitc    (501) staff       (20)      168 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/002.http
--rw-r--r--   0 benoitc    (501) staff       (20)      296 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/002.py
--rw-r--r--   0 benoitc    (501) staff       (20)      394 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/003.http
--rw-r--r--   0 benoitc    (501) staff       (20)      577 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/003.py
--rw-r--r--   0 benoitc    (501) staff       (20)       57 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/004.http
--rw-r--r--   0 benoitc    (501) staff       (20)      164 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/004.py
--rw-r--r--   0 benoitc    (501) staff       (20)       62 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/005.http
--rw-r--r--   0 benoitc    (501) staff       (20)      153 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/005.py
--rw-r--r--   0 benoitc    (501) staff       (20)       51 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/006.http
--rw-r--r--   0 benoitc    (501) staff       (20)      142 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/006.py
--rw-r--r--   0 benoitc    (501) staff       (20)       61 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/007.http
--rw-r--r--   0 benoitc    (501) staff       (20)      167 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/007.py
--rw-r--r--   0 benoitc    (501) staff       (20)       73 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/008.http
--rw-r--r--   0 benoitc    (501) staff       (20)      178 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/008.py
--rw-r--r--   0 benoitc    (501) staff       (20)      137 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/009.http
--rw-r--r--   0 benoitc    (501) staff       (20)      264 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/009.py
--rw-r--r--   0 benoitc    (501) staff       (20)      134 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/010.http
--rw-r--r--   0 benoitc    (501) staff       (20)      218 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/010.py
--rw-r--r--   0 benoitc    (501) staff       (20)      125 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/011.http
--rw-r--r--   0 benoitc    (501) staff       (20)      196 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/011.py
--rw-r--r--   0 benoitc    (501) staff       (20)      166 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/012.http
--rw-r--r--   0 benoitc    (501) staff       (20)      285 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/012.py
--rw-r--r--   0 benoitc    (501) staff       (20)      159 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/013.http
--rw-r--r--   0 benoitc    (501) staff       (20)      192 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/013.py
--rw-r--r--   0 benoitc    (501) staff       (20)       46 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/014.http
--rw-r--r--   0 benoitc    (501) staff       (20)      137 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/014.py
--rw-r--r--   0 benoitc    (501) staff       (20)       98 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/015.http
--rw-r--r--   0 benoitc    (501) staff       (20)      226 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/015.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2234 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/016.http
--rw-r--r--   0 benoitc    (501) staff       (20)     2376 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/016.py
--rw-r--r--   0 benoitc    (501) staff       (20)       91 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/017.http
--rw-r--r--   0 benoitc    (501) staff       (20)      207 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/017.py
--rw-r--r--   0 benoitc    (501) staff       (20)       58 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/018.http
--rw-r--r--   0 benoitc    (501) staff       (20)      258 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/018.py
--rw-r--r--   0 benoitc    (501) staff       (20)       58 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/019.http
--rw-r--r--   0 benoitc    (501) staff       (20)      119 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/019.py
--rw-r--r--   0 benoitc    (501) staff       (20)       81 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/020.http
--rw-r--r--   0 benoitc    (501) staff       (20)      171 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/020.py
--rw-r--r--   0 benoitc    (501) staff       (20)       80 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/021.http
--rw-r--r--   0 benoitc    (501) staff       (20)      142 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/021.py
--rw-r--r--   0 benoitc    (501) staff       (20)       85 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/022.http
--rw-r--r--   0 benoitc    (501) staff       (20)      286 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/022.py
--rw-r--r--   0 benoitc    (501) staff       (20)      155 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/023.http
--rw-r--r--   0 benoitc    (501) staff       (20)      335 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/023.py
--rw-r--r--   0 benoitc    (501) staff       (20)    16408 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/024.http
--rw-r--r--   0 benoitc    (501) staff       (20)    16639 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/024.py
--rw-r--r--   0 benoitc    (501) staff       (20)      364 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/025.http
--rw-r--r--   0 benoitc    (501) staff       (20)      476 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/025.py
--rw-r--r--   0 benoitc    (501) staff       (20)     8233 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/026.http
--rw-r--r--   0 benoitc    (501) staff       (20)     8463 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/026.py
--rw-r--r--   0 benoitc    (501) staff       (20)       30 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/027.http
--rw-r--r--   0 benoitc    (501) staff       (20)      130 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/027.py
--rw-r--r--   0 benoitc    (501) staff       (20)       68 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/028.http
--rw-r--r--   0 benoitc    (501) staff       (20)      261 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/028.py
--rw-r--r--   0 benoitc    (501) staff       (20)      129 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/029.http
--rw-r--r--   0 benoitc    (501) staff       (20)      278 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/029.py
--rw-r--r--   0 benoitc    (501) staff       (20)      129 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/030.http
--rw-r--r--   0 benoitc    (501) staff       (20)      278 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/030.py
--rw-r--r--   0 benoitc    (501) staff       (20)     9909 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/099.http
--rw-r--r--   0 benoitc    (501) staff       (20)     9135 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/099.py
--rw-r--r--   0 benoitc    (501) staff       (20)       41 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/100.http
--rw-r--r--   0 benoitc    (501) staff       (20)      131 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/100.py
--rw-r--r--   0 benoitc    (501) staff       (20)      199 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/pp_01.http
--rw-r--r--   0 benoitc    (501) staff       (20)      359 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/pp_01.py
--rw-r--r--   0 benoitc    (501) staff       (20)      361 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/pp_02.http
--rw-r--r--   0 benoitc    (501) staff       (20)      639 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/requests/valid/pp_02.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1745 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/support.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1614 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/t.py
--rw-r--r--   0 benoitc    (501) staff       (20)     6110 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/test_arbiter.py
--rw-r--r--   0 benoitc    (501) staff       (20)    14360 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/test_config.py
--rw-r--r--   0 benoitc    (501) staff       (20)     6853 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/test_http.py
--rw-r--r--   0 benoitc    (501) staff       (20)      597 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/test_invalid_requests.py
--rw-r--r--   0 benoitc    (501) staff       (20)     3140 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/test_logger.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1522 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/test_pidfile.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1851 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/test_reload.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1875 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/test_sock.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2013 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/test_ssl.py
--rw-r--r--   0 benoitc    (501) staff       (20)     4818 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/test_statsd.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2049 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/test_systemd.py
--rw-r--r--   0 benoitc    (501) staff       (20)     4367 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/test_util.py
--rw-r--r--   0 benoitc    (501) staff       (20)      608 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/test_valid_requests.py
--rw-r--r--   0 benoitc    (501) staff       (20)     9434 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/treq.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-18 12:53:23.775432 gunicorn-21.1.0/tests/workers/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/workers/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)      192 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/workers/test_geventlet.py
--rw-r--r--   0 benoitc    (501) staff       (20)      190 2023-07-17 19:03:36.000000 gunicorn-21.1.0/tests/workers/test_ggevent.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.622596 gunicorn-21.2.0/
+-rwxr-xr-x   0 benoitc    (501) staff       (20)      267 2023-07-17 19:03:36.000000 gunicorn-21.2.0/.gitignore
+-rw-r--r--   0 benoitc    (501) staff       (20)     1136 2023-07-17 19:03:36.000000 gunicorn-21.2.0/LICENSE
+-rw-r--r--   0 benoitc    (501) staff       (20)      324 2023-07-17 19:03:36.000000 gunicorn-21.2.0/MANIFEST.in
+-rw-r--r--   0 benoitc    (501) staff       (20)     3777 2023-07-17 19:03:36.000000 gunicorn-21.2.0/NOTICE
+-rw-r--r--   0 benoitc    (501) staff       (20)     3830 2023-07-19 11:46:16.622661 gunicorn-21.2.0/PKG-INFO
+-rw-r--r--   0 benoitc    (501) staff       (20)     1988 2023-07-17 19:03:36.000000 gunicorn-21.2.0/README.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     6969 2023-07-17 19:03:36.000000 gunicorn-21.2.0/THANKS
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.540439 gunicorn-21.2.0/docs/
+-rw-r--r--   0 benoitc    (501) staff       (20)     5791 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/Makefile
+-rw-r--r--   0 benoitc    (501) staff       (20)      288 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/README.rst
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.535694 gunicorn-21.2.0/docs/build/
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.548090 gunicorn-21.2.0/docs/build/doctrees/
+-rw-r--r--   0 benoitc    (501) staff       (20)    43583 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/2010-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    15287 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/2011-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    27991 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/2012-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    19851 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/2013-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    48784 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/2014-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    51800 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/2015-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    25377 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/2016-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    17557 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/2017-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    29568 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/2018-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    33177 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/2019-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)     2984 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/2020-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    13095 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/2021-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)     5292 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/2023-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    11251 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/community.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    17815 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/configure.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    10993 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/custom.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    54089 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/deploy.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    25657 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/design.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)  1267881 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/environment.pickle
+-rw-r--r--   0 benoitc    (501) staff       (20)    35498 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/faq.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)     8337 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/index.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    27785 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/install.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)     9613 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/instrumentation.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)     6075 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    31793 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/run.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)   261405 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/settings.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    24042 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/doctrees/signals.doctree
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.556346 gunicorn-21.2.0/docs/build/html/
+-rw-r--r--   0 benoitc    (501) staff       (20)      230 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/.buildinfo
+-rw-r--r--   0 benoitc    (501) staff       (20)    19422 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/html/2010-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    10972 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/html/2011-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    15120 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/html/2012-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    13036 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/html/2013-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    20800 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/html/2014-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    23465 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/html/2015-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    15406 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/html/2016-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    12213 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/html/2017-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    17042 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/html/2018-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    14935 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/html/2019-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     7097 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/html/2020-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     9650 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/html/2021-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     7724 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/html/2023-news.html
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.556506 gunicorn-21.2.0/docs/build/html/_images/
+-rw-r--r--   0 benoitc    (501) staff       (20)    14398 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_images/gunicorn.png
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.561340 gunicorn-21.2.0/docs/build/html/_sources/
+-rw-r--r--   0 benoitc    (501) staff       (20)     6643 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/2010-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     2092 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/2011-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     4184 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/2012-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     3267 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/2013-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     6834 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/2014-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     5702 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/2015-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     2911 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/2016-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     2100 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/2017-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     2956 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/2018-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     4785 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/2019-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      112 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/2020-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     1905 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/2021-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      530 2023-07-17 20:14:25.000000 gunicorn-21.2.0/docs/build/html/_sources/2023-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     1377 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/community.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     3873 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/configure.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     1927 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/custom.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)    12260 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/deploy.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     6483 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/design.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     8672 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/faq.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     1043 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     5551 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/install.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     1325 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/instrumentation.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      727 2023-07-17 20:14:25.000000 gunicorn-21.2.0/docs/build/html/_sources/news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     6485 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/run.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)    36935 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/html/_sources/settings.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     5420 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_sources/signals.rst.txt
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.562961 gunicorn-21.2.0/docs/build/html/_static/
+-rw-r--r--   0 benoitc    (501) staff       (20)    14813 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/_static/basic.css
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.563227 gunicorn-21.2.0/docs/build/html/_static/css/
+-rw-r--r--   0 benoitc    (501) staff       (20)     3229 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/badge_only.css
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.576965 gunicorn-21.2.0/docs/build/html/_static/css/fonts/
+-rw-r--r--   0 benoitc    (501) staff       (20)    87624 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 benoitc    (501) staff       (20)    67312 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 benoitc    (501) staff       (20)    86288 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 benoitc    (501) staff       (20)    66444 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 benoitc    (501) staff       (20)   165742 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 benoitc    (501) staff       (20)   444379 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 benoitc    (501) staff       (20)   165548 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 benoitc    (501) staff       (20)    98024 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 benoitc    (501) staff       (20)    77160 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 benoitc    (501) staff       (20)   323344 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 benoitc    (501) staff       (20)   193308 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 benoitc    (501) staff       (20)   309728 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 benoitc    (501) staff       (20)   184912 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 benoitc    (501) staff       (20)   328412 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 benoitc    (501) staff       (20)   195704 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 benoitc    (501) staff       (20)   309192 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 benoitc    (501) staff       (20)   182708 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 benoitc    (501) staff       (20)   135314 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/css/theme.css
+-rw-r--r--   0 benoitc    (501) staff       (20)     4472 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/doctools.js
+-rw-r--r--   0 benoitc    (501) staff       (20)      421 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0 benoitc    (501) staff       (20)      286 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/file.png
+-rw-r--r--   0 benoitc    (501) staff       (20)    14398 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/build/html/_static/gunicorn.png
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.580394 gunicorn-21.2.0/docs/build/html/_static/js/
+-rw-r--r--   0 benoitc    (501) staff       (20)      934 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0 benoitc    (501) staff       (20)     4370 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 benoitc    (501) staff       (20)     2734 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 benoitc    (501) staff       (20)     5023 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/js/theme.js
+-rw-r--r--   0 benoitc    (501) staff       (20)     4758 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/_static/language_data.js
+-rw-r--r--   0 benoitc    (501) staff       (20)       90 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/minus.png
+-rw-r--r--   0 benoitc    (501) staff       (20)       90 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/plus.png
+-rw-r--r--   0 benoitc    (501) staff       (20)     4846 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/_static/pygments.css
+-rw-r--r--   0 benoitc    (501) staff       (20)    18215 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/searchtools.js
+-rw-r--r--   0 benoitc    (501) staff       (20)     4712 2023-07-17 19:08:28.000000 gunicorn-21.2.0/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 benoitc    (501) staff       (20)     7909 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/build/html/community.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    12328 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/configure.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    14413 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/custom.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    40350 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/deploy.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    14905 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/design.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    26212 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/faq.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     4623 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/genindex.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    13234 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/index.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    18129 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/install.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     7694 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/instrumentation.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     8954 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     1679 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/objects.inv
+-rw-r--r--   0 benoitc    (501) staff       (20)    20340 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/run.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     4713 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/search.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    61641 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/searchindex.js
+-rw-r--r--   0 benoitc    (501) staff       (20)   116855 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/settings.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    25507 2023-07-17 21:13:37.000000 gunicorn-21.2.0/docs/build/html/signals.html
+-rwxr-xr-x   0 benoitc    (501) staff       (20)     3029 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/gunicorn_ext.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.581092 gunicorn-21.2.0/docs/logo/
+-rw-r--r--   0 benoitc    (501) staff       (20)    21550 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/logo/gunicorn.png
+-rw-r--r--   0 benoitc    (501) staff       (20)    12798 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/logo/gunicorn.svg
+-rw-r--r--   0 benoitc    (501) staff       (20)     5109 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/make.bat
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.583750 gunicorn-21.2.0/docs/site/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/.nojekyll
+-rw-r--r--   0 benoitc    (501) staff       (20)       13 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/CNAME
+-rw-r--r--   0 benoitc    (501) staff       (20)      340 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/community.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      304 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/configuration.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      300 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/configure.html
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.583889 gunicorn-21.2.0/docs/site/css/
+-rw-r--r--   0 benoitc    (501) staff       (20)     6671 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/css/style.css
+-rw-r--r--   0 benoitc    (501) staff       (20)      343 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/deploy.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      342 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/deployment.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      297 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/design.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/faq.html
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.586412 gunicorn-21.2.0/docs/site/images/
+-rw-r--r--   0 benoitc    (501) staff       (20)    17551 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/about.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)      408 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/arrow.png
+-rw-r--r--   0 benoitc    (501) staff       (20)      611 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/banner-bg.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)    15593 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/community.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)    17566 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/documents.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)    15962 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/downloads.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)     1771 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/favicon.png
+-rw-r--r--   0 benoitc    (501) staff       (20)      255 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/footer-arrow.png
+-rw-r--r--   0 benoitc    (501) staff       (20)     2499 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/footer-logo.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)      335 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/greenbutton.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)     1553 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/gunicorn.png
+-rw-r--r--   0 benoitc    (501) staff       (20)    21956 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/large_gunicorn.png
+-rw-r--r--   0 benoitc    (501) staff       (20)     3145 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/logo-bottom.png
+-rw-r--r--   0 benoitc    (501) staff       (20)    10238 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/logo.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)     7343 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/logo.png
+-rw-r--r--   0 benoitc    (501) staff       (20)      577 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/redbutton.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)      440 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/separator.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)     3450 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/title.png
+-rw-r--r--   0 benoitc    (501) staff       (20)     2184 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/images/user1.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)     7856 2023-07-19 11:30:01.000000 gunicorn-21.2.0/docs/site/index.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      298 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/install.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      298 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/installation.html
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.586538 gunicorn-21.2.0/docs/site/js/
+-rwxr-xr-x   0 benoitc    (501) staff       (20)     1479 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/js/main.js
+-rw-r--r--   0 benoitc    (501) staff       (20)      295 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/run.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     1990 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/sitemap.xml
+-rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/tuning.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/site/usage.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     2088 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/sitemap_gen.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.591018 gunicorn-21.2.0/docs/source/
+-rw-r--r--   0 benoitc    (501) staff       (20)     6643 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/2010-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     2092 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/2011-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     4184 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/2012-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     3267 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/2013-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     6834 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/2014-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     5702 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/2015-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     2911 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/2016-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     2100 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/2017-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     2956 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/2018-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     4785 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/2019-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)      112 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/2020-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1905 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/2021-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)      771 2023-07-19 11:30:45.000000 gunicorn-21.2.0/docs/source/2023-news.rst
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.591161 gunicorn-21.2.0/docs/source/_static/
+-rw-r--r--   0 benoitc    (501) staff       (20)    14398 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/_static/gunicorn.png
+-rw-r--r--   0 benoitc    (501) staff       (20)     1377 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/community.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1755 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/conf.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     3873 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/configure.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1927 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/custom.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)    12260 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/deploy.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     6483 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/design.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     8672 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/faq.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1043 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/index.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     5551 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/install.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1325 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/instrumentation.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1065 2023-07-19 11:30:29.000000 gunicorn-21.2.0/docs/source/news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     6485 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/run.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)    36935 2023-07-17 21:13:36.000000 gunicorn-21.2.0/docs/source/settings.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     5420 2023-07-17 19:03:36.000000 gunicorn-21.2.0/docs/source/signals.rst
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.594756 gunicorn-21.2.0/examples/
+-rw-r--r--   0 benoitc    (501) staff       (20)      738 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/alt_spec.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      204 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/bad.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      108 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/boot_fail.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.594996 gunicorn-21.2.0/examples/deep/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/deep/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      659 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/deep/test.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      676 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/echo.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     7621 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/example_config.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.596825 gunicorn-21.2.0/examples/frameworks/
+-rw-r--r--   0 benoitc    (501) staff       (20)      198 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/cherryapp.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.596964 gunicorn-21.2.0/examples/frameworks/django/
+-rw-r--r--   0 benoitc    (501) staff       (20)       60 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/django/README
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.597104 gunicorn-21.2.0/examples/frameworks/django/testing/
+-rwxr-xr-x   0 benoitc    (501) staff       (20)      244 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/django/testing/manage.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.597602 gunicorn-21.2.0/examples/frameworks/django/testing/testing/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/django/testing/testing/__init__.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.597737 gunicorn-21.2.0/examples/frameworks/django/testing/testing/apps/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/django/testing/testing/apps/__init__.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.598444 gunicorn-21.2.0/examples/frameworks/django/testing/testing/apps/someapp/
+-rwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/django/testing/testing/apps/someapp/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      627 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/django/testing/testing/apps/someapp/middleware.py
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/django/testing/testing/apps/someapp/models.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.598687 gunicorn-21.2.0/examples/frameworks/django/testing/testing/apps/someapp/templates/
+-rw-r--r--   0 benoitc    (501) staff       (20)      759 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      471 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/django/testing/testing/apps/someapp/templates/home.html
+-rwxr-xr-x   0 benoitc    (501) staff       (20)      509 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/django/testing/testing/apps/someapp/tests.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      133 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/django/testing/testing/apps/someapp/urls.py
+-rwxr-xr-x   0 benoitc    (501) staff       (20)     1548 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/django/testing/testing/apps/someapp/views.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     5730 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/django/testing/testing/settings.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      577 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/django/testing/testing/urls.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1359 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/django/testing/testing/wsgi.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      291 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/flask_sendfile.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      147 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/flaskapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      501 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/flaskapp_aiohttp_wsgi.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      338 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/pyramidapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      150 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/requirements.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        9 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/requirements_cherryapp.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        6 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/requirements_flaskapp.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        8 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/requirements_pyramidapp.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)       10 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/requirements_tornadoapp.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        7 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/requirements_webpyapp.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      873 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/tornadoapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      197 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/frameworks/webpyapp.py
+-rwxr-xr-x   0 benoitc    (501) staff       (20)      215 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/gunicorn_rc
+-rw-r--r--   0 benoitc    (501) staff       (20)       13 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/hello.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      448 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/log_app.ini
+-rw-r--r--   0 benoitc    (501) staff       (20)      372 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/log_app.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      841 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/logging.conf
+-rw-r--r--   0 benoitc    (501) staff       (20)      737 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/longpoll.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1470 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/multiapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      993 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/multidomainapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1980 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/nginx.conf
+-rw-r--r--   0 benoitc    (501) staff       (20)      403 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/read_django_settings.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1015 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/readline_app.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      584 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/sendfile.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1257 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/server.crt
+-rw-r--r--   0 benoitc    (501) staff       (20)     1679 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/server.key
+-rw-r--r--   0 benoitc    (501) staff       (20)      604 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/slowclient.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1339 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/standalone_app.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      182 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/supervisor.conf
+-rw-r--r--   0 benoitc    (501) staff       (20)      659 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/test.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      620 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/timeout.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.599040 gunicorn-21.2.0/examples/websocket/
+-rw-r--r--   0 benoitc    (501) staff       (20)    15684 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/websocket/gevent_websocket.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1320 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/websocket/websocket.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    15729 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/websocket/websocket.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1020 2023-07-17 19:03:36.000000 gunicorn-21.2.0/examples/when_ready.conf.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.600933 gunicorn-21.2.0/gunicorn/
+-rw-r--r--   0 benoitc    (501) staff       (20)      279 2023-07-19 11:28:17.000000 gunicorn-21.2.0/gunicorn/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      171 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/__main__.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.602329 gunicorn-21.2.0/gunicorn/app/
+-rw-r--r--   0 benoitc    (501) staff       (20)      127 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/app/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     7400 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/app/base.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2038 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/app/pasterapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1926 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/app/wsgiapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    21509 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/arbiter.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    63419 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/config.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2293 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/debug.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      919 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/errors.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    15303 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/glogging.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.603114 gunicorn-21.2.0/gunicorn/http/
+-rw-r--r--   0 benoitc    (501) staff       (20)      277 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/http/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     7296 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/http/body.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2850 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/http/errors.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    11958 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/http/message.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1364 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/http/parser.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1943 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/http/unreader.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    12366 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/http/wsgi.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.603307 gunicorn-21.2.0/gunicorn/instrument/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/instrument/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     4690 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/instrument/statsd.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2367 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/pidfile.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     3791 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/reloader.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     6887 2023-07-18 12:00:28.000000 gunicorn-21.2.0/gunicorn/sock.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2520 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/systemd.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    19127 2023-07-17 21:06:48.000000 gunicorn-21.2.0/gunicorn/util.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.604345 gunicorn-21.2.0/gunicorn/workers/
+-rw-r--r--   0 benoitc    (501) staff       (20)      594 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/workers/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     9197 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/workers/base.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     5681 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/workers/base_async.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     6091 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/workers/geventlet.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     5800 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/workers/ggevent.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    12575 2023-07-19 11:27:51.000000 gunicorn-21.2.0/gunicorn/workers/gthread.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     5854 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/workers/gtornado.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     7272 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/workers/sync.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1651 2023-07-17 19:03:36.000000 gunicorn-21.2.0/gunicorn/workers/workertmp.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.601900 gunicorn-21.2.0/gunicorn.egg-info/
+-rw-r--r--   0 benoitc    (501) staff       (20)     3830 2023-07-19 11:46:16.000000 gunicorn-21.2.0/gunicorn.egg-info/PKG-INFO
+-rw-r--r--   0 benoitc    (501) staff       (20)    13924 2023-07-19 11:46:16.000000 gunicorn-21.2.0/gunicorn.egg-info/SOURCES.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        1 2023-07-19 11:46:16.000000 gunicorn-21.2.0/gunicorn.egg-info/dependency_links.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      113 2023-07-19 11:46:16.000000 gunicorn-21.2.0/gunicorn.egg-info/entry_points.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        1 2023-07-17 20:27:30.000000 gunicorn-21.2.0/gunicorn.egg-info/not-zip-safe
+-rw-r--r--   0 benoitc    (501) staff       (20)      173 2023-07-19 11:46:16.000000 gunicorn-21.2.0/gunicorn.egg-info/requires.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        9 2023-07-19 11:46:16.000000 gunicorn-21.2.0/gunicorn.egg-info/top_level.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)       50 2023-07-17 19:03:36.000000 gunicorn-21.2.0/requirements_dev.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)       56 2023-07-17 20:45:55.000000 gunicorn-21.2.0/requirements_test.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      208 2023-07-19 11:46:16.622853 gunicorn-21.2.0/setup.cfg
+-rw-r--r--   0 benoitc    (501) staff       (20)     3555 2023-07-17 19:03:36.000000 gunicorn-21.2.0/setup.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.606725 gunicorn-21.2.0/tests/
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.607164 gunicorn-21.2.0/tests/config/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/config/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       88 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/config/test_cfg.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       24 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/config/test_cfg_alt.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       23 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/config/test_cfg_with_wsgi_app.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.538027 gunicorn-21.2.0/tests/requests/
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.613252 gunicorn-21.2.0/tests/requests/invalid/
+-rw-r--r--   0 benoitc    (501) staff       (20)       29 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/001.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       64 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/001.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       21 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/002.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       81 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/002.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       30 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/003.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       84 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/003.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       25 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/004.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       80 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/004.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       41 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/005.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       78 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/005.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     4122 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/006.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       77 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/006.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     8358 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/007.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       83 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/007.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    12418 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/008.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       83 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/008.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1829 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/009.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       83 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/009.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       44 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/010.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      174 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/010.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      169 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/011.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      169 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/011.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      169 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/012.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      174 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/012.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       49 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/013.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      174 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/013.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       78 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/014.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       72 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/014.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       88 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/015.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       72 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/015.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       33 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/016.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       82 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/016.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     8222 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/017.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      134 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/017.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       48 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/018.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       81 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/018.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       82 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/019.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      172 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/019.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       69 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/020.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      130 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/020.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       90 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/021.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/021.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       51 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/022.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/022.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       52 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/023.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/023.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       51 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/024.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/024.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       37 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/pp_01.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      161 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/pp_01.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       53 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/pp_02.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      161 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/invalid/pp_02.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.622175 gunicorn-21.2.0/tests/requests/valid/
+-rw-r--r--   0 benoitc    (501) staff       (20)      149 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/001.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      275 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/001.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      168 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/002.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      296 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/002.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      394 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/003.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      577 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/003.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       57 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/004.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      164 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/004.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       62 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/005.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      153 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/005.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       51 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/006.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      142 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/006.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       61 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/007.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      167 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/007.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       73 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/008.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      178 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/008.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      137 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/009.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      264 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/009.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      134 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/010.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      218 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/010.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      125 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/011.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      196 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/011.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      166 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/012.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      285 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/012.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      159 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/013.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      192 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/013.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       46 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/014.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      137 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/014.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       98 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/015.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      226 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/015.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2234 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/016.http
+-rw-r--r--   0 benoitc    (501) staff       (20)     2376 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/016.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       91 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/017.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      207 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/017.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       58 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/018.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      258 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/018.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       58 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/019.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      119 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/019.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       81 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/020.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      171 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/020.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       80 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/021.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      142 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/021.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       85 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/022.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      286 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/022.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      155 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/023.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      335 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/023.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    16408 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/024.http
+-rw-r--r--   0 benoitc    (501) staff       (20)    16639 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/024.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      364 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/025.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      476 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/025.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     8233 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/026.http
+-rw-r--r--   0 benoitc    (501) staff       (20)     8463 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/026.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       30 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/027.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      130 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/027.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       68 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/028.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      261 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/028.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      129 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/029.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      278 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/029.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      129 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/030.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      278 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/030.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     9909 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/099.http
+-rw-r--r--   0 benoitc    (501) staff       (20)     9135 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/099.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       41 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/100.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      131 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/100.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      199 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/pp_01.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      359 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/pp_01.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      361 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/pp_02.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      639 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/requests/valid/pp_02.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1745 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/support.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1614 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/t.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     6110 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/test_arbiter.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    14360 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/test_config.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     6853 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/test_http.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      597 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/test_invalid_requests.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     3140 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/test_logger.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1522 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/test_pidfile.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1851 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/test_reload.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1875 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/test_sock.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2013 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/test_ssl.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     4818 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/test_statsd.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2049 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/test_systemd.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     4367 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/test_util.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      608 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/test_valid_requests.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     9434 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/treq.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-19 11:46:16.622481 gunicorn-21.2.0/tests/workers/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/workers/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      192 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/workers/test_geventlet.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      190 2023-07-17 19:03:36.000000 gunicorn-21.2.0/tests/workers/test_ggevent.py
```

### Comparing `gunicorn-21.1.0/LICENSE` & `gunicorn-21.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/NOTICE` & `gunicorn-21.2.0/NOTICE`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/PKG-INFO` & `gunicorn-21.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunicorn
-Version: 21.1.0
+Version: 21.2.0
 Summary: WSGI HTTP Server for UNIX
 Home-page: https://gunicorn.org
 Author: Benoit Chesneau
 Author-email: benoitc@gunicorn.org
 License: MIT
 Project-URL: Documentation, https://docs.gunicorn.org
 Project-URL: Homepage, https://gunicorn.org
```

### Comparing `gunicorn-21.1.0/README.rst` & `gunicorn-21.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/THANKS` & `gunicorn-21.2.0/THANKS`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/Makefile` & `gunicorn-21.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/2010-news.doctree` & `gunicorn-21.2.0/docs/build/doctrees/2010-news.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/2011-news.doctree` & `gunicorn-21.2.0/docs/build/doctrees/2011-news.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/2012-news.doctree` & `gunicorn-21.2.0/docs/build/doctrees/2012-news.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/2013-news.doctree` & `gunicorn-21.2.0/docs/build/doctrees/2013-news.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/2014-news.doctree` & `gunicorn-21.2.0/docs/build/doctrees/2014-news.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/2015-news.doctree` & `gunicorn-21.2.0/docs/build/doctrees/2015-news.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/2016-news.doctree` & `gunicorn-21.2.0/docs/build/doctrees/2016-news.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/2017-news.doctree` & `gunicorn-21.2.0/docs/build/doctrees/2017-news.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/2018-news.doctree` & `gunicorn-21.2.0/docs/build/doctrees/2018-news.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/2019-news.doctree` & `gunicorn-21.2.0/docs/build/doctrees/2019-news.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/2020-news.doctree` & `gunicorn-21.2.0/docs/build/doctrees/2020-news.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/2021-news.doctree` & `gunicorn-21.2.0/docs/build/doctrees/2021-news.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/2023-news.doctree` & `gunicorn-21.2.0/docs/build/doctrees/2023-news.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/community.doctree` & `gunicorn-21.2.0/docs/build/doctrees/community.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/configure.doctree` & `gunicorn-21.2.0/docs/build/doctrees/configure.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/custom.doctree` & `gunicorn-21.2.0/docs/build/doctrees/custom.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/deploy.doctree` & `gunicorn-21.2.0/docs/build/doctrees/deploy.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/design.doctree` & `gunicorn-21.2.0/docs/build/doctrees/design.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/environment.pickle` & `gunicorn-21.2.0/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/faq.doctree` & `gunicorn-21.2.0/docs/build/doctrees/faq.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/index.doctree` & `gunicorn-21.2.0/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/install.doctree` & `gunicorn-21.2.0/docs/build/doctrees/install.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/instrumentation.doctree` & `gunicorn-21.2.0/docs/build/doctrees/instrumentation.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/news.doctree` & `gunicorn-21.2.0/docs/build/doctrees/news.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/run.doctree` & `gunicorn-21.2.0/docs/build/doctrees/run.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/settings.doctree` & `gunicorn-21.2.0/docs/build/doctrees/settings.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/doctrees/signals.doctree` & `gunicorn-21.2.0/docs/build/doctrees/signals.doctree`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/2010-news.html` & `gunicorn-21.2.0/docs/build/html/2010-news.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/2011-news.html` & `gunicorn-21.2.0/docs/build/html/2011-news.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/2012-news.html` & `gunicorn-21.2.0/docs/build/html/2012-news.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/2013-news.html` & `gunicorn-21.2.0/docs/build/html/2013-news.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/2014-news.html` & `gunicorn-21.2.0/docs/build/html/2014-news.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/2015-news.html` & `gunicorn-21.2.0/docs/build/html/2015-news.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/2016-news.html` & `gunicorn-21.2.0/docs/build/html/2016-news.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/2017-news.html` & `gunicorn-21.2.0/docs/build/html/2017-news.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/2018-news.html` & `gunicorn-21.2.0/docs/build/html/2018-news.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/2019-news.html` & `gunicorn-21.2.0/docs/build/html/2019-news.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/2020-news.html` & `gunicorn-21.2.0/docs/build/html/2020-news.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/2021-news.html` & `gunicorn-21.2.0/docs/build/html/2021-news.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/2023-news.html` & `gunicorn-21.2.0/docs/build/html/2023-news.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_images/gunicorn.png` & `gunicorn-21.2.0/docs/build/html/_images/gunicorn.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/2010-news.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/2010-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/2011-news.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/2011-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/2012-news.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/2012-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/2013-news.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/2013-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/2014-news.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/2014-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/2015-news.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/2015-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/2016-news.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/2016-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/2017-news.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/2017-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/2018-news.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/2018-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/2019-news.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/2019-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/2021-news.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/2021-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/2023-news.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/2023-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/community.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/community.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/configure.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/configure.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/custom.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/custom.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/deploy.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/deploy.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/design.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/design.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/faq.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/faq.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/index.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/install.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/install.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/instrumentation.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/instrumentation.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/news.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/run.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/run.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/settings.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/settings.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_sources/signals.rst.txt` & `gunicorn-21.2.0/docs/build/html/_sources/signals.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/basic.css` & `gunicorn-21.2.0/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/badge_only.css` & `gunicorn-21.2.0/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-bold.woff` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-bold.woff2` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-normal.woff` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/fonts/lato-normal.woff2` & `gunicorn-21.2.0/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/css/theme.css` & `gunicorn-21.2.0/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/doctools.js` & `gunicorn-21.2.0/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/gunicorn.png` & `gunicorn-21.2.0/docs/build/html/_static/gunicorn.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/js/badge_only.js` & `gunicorn-21.2.0/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `gunicorn-21.2.0/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/js/html5shiv.min.js` & `gunicorn-21.2.0/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/js/theme.js` & `gunicorn-21.2.0/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/language_data.js` & `gunicorn-21.2.0/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/pygments.css` & `gunicorn-21.2.0/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/searchtools.js` & `gunicorn-21.2.0/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/_static/sphinx_highlight.js` & `gunicorn-21.2.0/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/community.html` & `gunicorn-21.2.0/docs/build/html/community.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/configure.html` & `gunicorn-21.2.0/docs/build/html/configure.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/custom.html` & `gunicorn-21.2.0/docs/build/html/custom.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/deploy.html` & `gunicorn-21.2.0/docs/build/html/deploy.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/design.html` & `gunicorn-21.2.0/docs/build/html/design.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/faq.html` & `gunicorn-21.2.0/docs/build/html/faq.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/genindex.html` & `gunicorn-21.2.0/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/index.html` & `gunicorn-21.2.0/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/install.html` & `gunicorn-21.2.0/docs/build/html/install.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/instrumentation.html` & `gunicorn-21.2.0/docs/build/html/instrumentation.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/news.html` & `gunicorn-21.2.0/docs/build/html/news.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/objects.inv` & `gunicorn-21.2.0/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/run.html` & `gunicorn-21.2.0/docs/build/html/run.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/search.html` & `gunicorn-21.2.0/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/searchindex.js` & `gunicorn-21.2.0/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/settings.html` & `gunicorn-21.2.0/docs/build/html/settings.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/build/html/signals.html` & `gunicorn-21.2.0/docs/build/html/signals.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/gunicorn_ext.py` & `gunicorn-21.2.0/docs/gunicorn_ext.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/logo/gunicorn.png` & `gunicorn-21.2.0/docs/logo/gunicorn.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/logo/gunicorn.svg` & `gunicorn-21.2.0/docs/logo/gunicorn.svg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/make.bat` & `gunicorn-21.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/css/style.css` & `gunicorn-21.2.0/docs/site/css/style.css`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/images/about.jpg` & `gunicorn-21.2.0/docs/site/images/about.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/images/banner-bg.jpg` & `gunicorn-21.2.0/docs/site/images/banner-bg.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/images/community.jpg` & `gunicorn-21.2.0/docs/site/images/community.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/images/documents.jpg` & `gunicorn-21.2.0/docs/site/images/documents.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/images/downloads.jpg` & `gunicorn-21.2.0/docs/site/images/downloads.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/images/favicon.png` & `gunicorn-21.2.0/docs/site/images/favicon.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/images/footer-logo.jpg` & `gunicorn-21.2.0/docs/site/images/footer-logo.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/images/gunicorn.png` & `gunicorn-21.2.0/docs/site/images/gunicorn.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/images/large_gunicorn.png` & `gunicorn-21.2.0/docs/site/images/large_gunicorn.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/images/logo-bottom.png` & `gunicorn-21.2.0/docs/site/images/logo-bottom.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/images/logo.jpg` & `gunicorn-21.2.0/docs/site/images/logo.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/images/logo.png` & `gunicorn-21.2.0/docs/site/images/logo.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/images/redbutton.jpg` & `gunicorn-21.2.0/docs/site/images/redbutton.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/images/title.png` & `gunicorn-21.2.0/docs/site/images/title.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/images/user1.jpg` & `gunicorn-21.2.0/docs/site/images/user1.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/index.html` & `gunicorn-21.2.0/docs/site/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 </head>
 <body>
   <div class="logo-wrapper">
     <div class="logo-div">
       <div class="latest">
         Latest version: <strong><a
-            href="https://docs.gunicorn.org/en/stable/">21.1.0</a></strong>
+            href="https://docs.gunicorn.org/en/stable/">21.2.0</a></strong>
       </div>
 
       <div class="logo"><img src="images/logo.jpg" ></div>
     </div>
   </div>
   <div class="banner-wrapper">
     <div class="banner">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Latest version: _22_11_.._11_.._00
+Latest version: _22_11_.._22_.._00
 [images/logo.jpg]
 [images/title.png]
 ************ GGuunniiccoorrnn ''GGrreeeenn UUnniiccoorrnn'' iiss aa PPyytthhoonn WWSSGGII HHTTTTPP SSeerrvveerr ffoorr UUNNIIXX.. IItt''ss aa
 pprree--ffoorrkk wwoorrkkeerr mmooddeell.. TThhee GGuunniiccoorrnn sseerrvveerr iiss bbrrooaaddllyy ccoommppaattiibbllee wwiitthh vvaarriioouuss
 wweebb ffrraammeewwoorrkkss,, ssiimmppllyy iimmpplleemmeenntteedd,, lliigghhtt oonn sseerrvveerr rreessoouurrcceess,, aanndd ffaaiirrllyy
 ssppeeeeddyy.. ************
 _V_i_e_w_ _s_o_u_r_c_e _D_o_w_n_l_o_a_d
```

### Comparing `gunicorn-21.1.0/docs/site/js/main.js` & `gunicorn-21.2.0/docs/site/js/main.js`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/site/sitemap.xml` & `gunicorn-21.2.0/docs/site/sitemap.xml`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/sitemap_gen.py` & `gunicorn-21.2.0/docs/sitemap_gen.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/2010-news.rst` & `gunicorn-21.2.0/docs/source/2010-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/2011-news.rst` & `gunicorn-21.2.0/docs/source/2011-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/2012-news.rst` & `gunicorn-21.2.0/docs/source/2012-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/2013-news.rst` & `gunicorn-21.2.0/docs/source/2013-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/2014-news.rst` & `gunicorn-21.2.0/docs/source/2014-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/2015-news.rst` & `gunicorn-21.2.0/docs/source/2015-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/2016-news.rst` & `gunicorn-21.2.0/docs/source/2016-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/2017-news.rst` & `gunicorn-21.2.0/docs/source/2017-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/2018-news.rst` & `gunicorn-21.2.0/docs/source/2018-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/2019-news.rst` & `gunicorn-21.2.0/docs/source/2019-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/2021-news.rst` & `gunicorn-21.2.0/docs/source/2021-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/2023-news.rst` & `gunicorn-21.2.0/docs/source/2023-news.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 ================
 Changelog - 2023
 ================
 
-21.1.0 - 2023-07-18
+21.2.0 - 2023-07-19
 ===================
 
-- fix thread worker: fix socket removal from the queue
+- fix thread worker: revert change considering connection as idle . 
+
+*** NOTE ***
+
+This is fixing the bad file description error.
 
 21.0.1 - 2023-07-17
 ===================
 
 - fix documentation build
 
 21.0.0 - 2023-07-17
```

### Comparing `gunicorn-21.1.0/docs/source/_static/gunicorn.png` & `gunicorn-21.2.0/docs/source/_static/gunicorn.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/community.rst` & `gunicorn-21.2.0/docs/source/community.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/conf.py` & `gunicorn-21.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/configure.rst` & `gunicorn-21.2.0/docs/source/configure.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/custom.rst` & `gunicorn-21.2.0/docs/source/custom.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/deploy.rst` & `gunicorn-21.2.0/docs/source/deploy.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/design.rst` & `gunicorn-21.2.0/docs/source/design.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/faq.rst` & `gunicorn-21.2.0/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/index.rst` & `gunicorn-21.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/install.rst` & `gunicorn-21.2.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/instrumentation.rst` & `gunicorn-21.2.0/docs/source/instrumentation.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/news.rst` & `gunicorn-21.2.0/docs/source/news.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 =========
 Changelog
 =========
 
+21.2.0 - 2023-07-19
+===================
+
+- fix thread worker: revert change considering connection as idle . 
+
+*** NOTE ***
+
+This is fixing the bad file description error.
+
 21.1.0 - 2023-07-18
 ===================
 
 - fix thread worker: fix socket removal from the queue
 
 21.0.1 - 2023-07-17
 ===================
```

### Comparing `gunicorn-21.1.0/docs/source/run.rst` & `gunicorn-21.2.0/docs/source/run.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/settings.rst` & `gunicorn-21.2.0/docs/source/settings.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/docs/source/signals.rst` & `gunicorn-21.2.0/docs/source/signals.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/alt_spec.py` & `gunicorn-21.2.0/examples/alt_spec.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/deep/test.py` & `gunicorn-21.2.0/examples/deep/test.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/echo.py` & `gunicorn-21.2.0/examples/echo.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/example_config.py` & `gunicorn-21.2.0/examples/example_config.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/frameworks/django/testing/testing/apps/someapp/middleware.py` & `gunicorn-21.2.0/examples/frameworks/django/testing/testing/apps/someapp/middleware.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html` & `gunicorn-21.2.0/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/frameworks/django/testing/testing/apps/someapp/views.py` & `gunicorn-21.2.0/examples/frameworks/django/testing/testing/apps/someapp/views.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/frameworks/django/testing/testing/settings.py` & `gunicorn-21.2.0/examples/frameworks/django/testing/testing/settings.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/frameworks/django/testing/testing/urls.py` & `gunicorn-21.2.0/examples/frameworks/django/testing/testing/urls.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/frameworks/django/testing/testing/wsgi.py` & `gunicorn-21.2.0/examples/frameworks/django/testing/testing/wsgi.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/frameworks/tornadoapp.py` & `gunicorn-21.2.0/examples/frameworks/tornadoapp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/logging.conf` & `gunicorn-21.2.0/examples/logging.conf`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/longpoll.py` & `gunicorn-21.2.0/examples/longpoll.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/multiapp.py` & `gunicorn-21.2.0/examples/multiapp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/multidomainapp.py` & `gunicorn-21.2.0/examples/multidomainapp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/nginx.conf` & `gunicorn-21.2.0/examples/nginx.conf`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/readline_app.py` & `gunicorn-21.2.0/examples/readline_app.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/sendfile.py` & `gunicorn-21.2.0/examples/sendfile.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/server.crt` & `gunicorn-21.2.0/examples/server.crt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/server.key` & `gunicorn-21.2.0/examples/server.key`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/slowclient.py` & `gunicorn-21.2.0/examples/slowclient.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/standalone_app.py` & `gunicorn-21.2.0/examples/standalone_app.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/test.py` & `gunicorn-21.2.0/examples/test.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/timeout.py` & `gunicorn-21.2.0/examples/timeout.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/websocket/gevent_websocket.py` & `gunicorn-21.2.0/examples/websocket/gevent_websocket.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/websocket/websocket.html` & `gunicorn-21.2.0/examples/websocket/websocket.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/websocket/websocket.py` & `gunicorn-21.2.0/examples/websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/examples/when_ready.conf.py` & `gunicorn-21.2.0/examples/when_ready.conf.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/app/base.py` & `gunicorn-21.2.0/gunicorn/app/base.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/app/pasterapp.py` & `gunicorn-21.2.0/gunicorn/app/pasterapp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/app/wsgiapp.py` & `gunicorn-21.2.0/gunicorn/app/wsgiapp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/arbiter.py` & `gunicorn-21.2.0/gunicorn/arbiter.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/config.py` & `gunicorn-21.2.0/gunicorn/config.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/debug.py` & `gunicorn-21.2.0/gunicorn/debug.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/errors.py` & `gunicorn-21.2.0/gunicorn/errors.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/glogging.py` & `gunicorn-21.2.0/gunicorn/glogging.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/http/body.py` & `gunicorn-21.2.0/gunicorn/http/body.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/http/errors.py` & `gunicorn-21.2.0/gunicorn/http/errors.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/http/message.py` & `gunicorn-21.2.0/gunicorn/http/message.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/http/parser.py` & `gunicorn-21.2.0/gunicorn/http/parser.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/http/unreader.py` & `gunicorn-21.2.0/gunicorn/http/unreader.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/http/wsgi.py` & `gunicorn-21.2.0/gunicorn/http/wsgi.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/instrument/statsd.py` & `gunicorn-21.2.0/gunicorn/instrument/statsd.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/pidfile.py` & `gunicorn-21.2.0/gunicorn/pidfile.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/reloader.py` & `gunicorn-21.2.0/gunicorn/reloader.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/sock.py` & `gunicorn-21.2.0/gunicorn/sock.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/systemd.py` & `gunicorn-21.2.0/gunicorn/systemd.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/util.py` & `gunicorn-21.2.0/gunicorn/util.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/workers/__init__.py` & `gunicorn-21.2.0/gunicorn/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/workers/base.py` & `gunicorn-21.2.0/gunicorn/workers/base.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/workers/base_async.py` & `gunicorn-21.2.0/gunicorn/workers/base_async.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/workers/geventlet.py` & `gunicorn-21.2.0/gunicorn/workers/geventlet.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/workers/ggevent.py` & `gunicorn-21.2.0/gunicorn/workers/ggevent.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/workers/gthread.py` & `gunicorn-21.2.0/gunicorn/workers/gthread.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,21 +118,18 @@
         self._wrap_future(fs, conn)
 
     def accept(self, server, listener):
         try:
             sock, client = listener.accept()
             # initialize the connection object
             conn = TConn(self.cfg, sock, client, server)
-            # set timeout to ensure it will not be in the loop too long
-            conn.set_timeout()
 
             self.nr_conns += 1
             # wait until socket is readable
             with self._lock:
-                self._keep.append(conn)
                 self.poller.register(conn.sock, selectors.EVENT_READ,
                                      partial(self.on_client_socket_readable, conn))
         except EnvironmentError as e:
             if e.errno not in (errno.EAGAIN, errno.ECONNABORTED,
                                errno.EWOULDBLOCK):
                 raise
```

### Comparing `gunicorn-21.1.0/gunicorn/workers/gtornado.py` & `gunicorn-21.2.0/gunicorn/workers/gtornado.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/workers/sync.py` & `gunicorn-21.2.0/gunicorn/workers/sync.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn/workers/workertmp.py` & `gunicorn-21.2.0/gunicorn/workers/workertmp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/gunicorn.egg-info/PKG-INFO` & `gunicorn-21.2.0/gunicorn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunicorn
-Version: 21.1.0
+Version: 21.2.0
 Summary: WSGI HTTP Server for UNIX
 Home-page: https://gunicorn.org
 Author: Benoit Chesneau
 Author-email: benoitc@gunicorn.org
 License: MIT
 Project-URL: Documentation, https://docs.gunicorn.org
 Project-URL: Homepage, https://gunicorn.org
```

### Comparing `gunicorn-21.1.0/gunicorn.egg-info/SOURCES.txt` & `gunicorn-21.2.0/gunicorn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/setup.py` & `gunicorn-21.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/requests/invalid/006.http` & `gunicorn-21.2.0/tests/requests/invalid/006.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/requests/invalid/007.http` & `gunicorn-21.2.0/tests/requests/invalid/007.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/requests/invalid/008.http` & `gunicorn-21.2.0/tests/requests/invalid/008.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/requests/invalid/009.http` & `gunicorn-21.2.0/tests/requests/invalid/009.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/requests/invalid/017.http` & `gunicorn-21.2.0/tests/requests/invalid/017.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/requests/valid/003.py` & `gunicorn-21.2.0/tests/requests/valid/003.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/requests/valid/016.http` & `gunicorn-21.2.0/tests/requests/valid/016.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/requests/valid/016.py` & `gunicorn-21.2.0/tests/requests/valid/016.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/requests/valid/024.http` & `gunicorn-21.2.0/tests/requests/valid/024.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/requests/valid/024.py` & `gunicorn-21.2.0/tests/requests/valid/024.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/requests/valid/026.http` & `gunicorn-21.2.0/tests/requests/valid/026.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/requests/valid/026.py` & `gunicorn-21.2.0/tests/requests/valid/026.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/requests/valid/099.http` & `gunicorn-21.2.0/tests/requests/valid/099.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/requests/valid/099.py` & `gunicorn-21.2.0/tests/requests/valid/099.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/requests/valid/pp_02.py` & `gunicorn-21.2.0/tests/requests/valid/pp_02.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/support.py` & `gunicorn-21.2.0/tests/support.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/t.py` & `gunicorn-21.2.0/tests/t.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/test_arbiter.py` & `gunicorn-21.2.0/tests/test_arbiter.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/test_config.py` & `gunicorn-21.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/test_http.py` & `gunicorn-21.2.0/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/test_invalid_requests.py` & `gunicorn-21.2.0/tests/test_invalid_requests.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/test_logger.py` & `gunicorn-21.2.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/test_pidfile.py` & `gunicorn-21.2.0/tests/test_pidfile.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/test_reload.py` & `gunicorn-21.2.0/tests/test_reload.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/test_sock.py` & `gunicorn-21.2.0/tests/test_sock.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/test_ssl.py` & `gunicorn-21.2.0/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/test_statsd.py` & `gunicorn-21.2.0/tests/test_statsd.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/test_systemd.py` & `gunicorn-21.2.0/tests/test_systemd.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/test_util.py` & `gunicorn-21.2.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/test_valid_requests.py` & `gunicorn-21.2.0/tests/test_valid_requests.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.1.0/tests/treq.py` & `gunicorn-21.2.0/tests/treq.py`

 * *Files identical despite different names*

