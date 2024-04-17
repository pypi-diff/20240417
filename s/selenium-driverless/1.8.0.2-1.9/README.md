# Comparing `tmp/selenium_driverless-1.8.0.2.tar.gz` & `tmp/selenium_driverless-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_driverless-1.8.0.2.tar", last modified: Sun Mar 10 11:03:06 2024, max compression
+gzip compressed data, was "selenium_driverless-1.9.tar", last modified: Wed Apr 17 11:26:49 2024, max compression
```

## Comparing `selenium_driverless-1.8.0.2.tar` & `selenium_driverless-1.9.tar`

### file list

```diff
@@ -1,170 +1,155 @@
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.747114 selenium_driverless-1.8.0.2/
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.490099 selenium_driverless-1.8.0.2/.github/
--rw-rw-rw-   0        0        0      512 2023-10-29 12:51:12.000000 selenium_driverless-1.8.0.2/.github/dependabot.yml
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.492099 selenium_driverless-1.8.0.2/.github/workflows/
--rw-rw-rw-   0        0        0      905 2023-10-29 12:51:12.000000 selenium_driverless-1.8.0.2/.github/workflows/dependency-review.yml
--rw-rw-rw-   0        0        0      738 2023-09-19 13:08:57.000000 selenium_driverless-1.8.0.2/LICENSE.md
--rw-rw-rw-   0        0        0      185 2023-11-30 15:16:31.000000 selenium_driverless-1.8.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    16280 2024-03-10 11:03:06.747114 selenium_driverless-1.8.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    14663 2024-03-10 11:01:45.000000 selenium_driverless-1.8.0.2/README.md
--rw-rw-rw-   0        0        0      696 2024-01-29 19:33:57.000000 selenium_driverless-1.8.0.2/build_upload.md
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.496099 selenium_driverless-1.8.0.2/dev/
--rw-rw-rw-   0        0        0     1067 2023-10-29 12:51:12.000000 selenium_driverless-1.8.0.2/dev/README.md
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.513433 selenium_driverless-1.8.0.2/dev/assets/
--rw-rw-rw-   0        0        0   429242 2023-08-27 15:04:01.000000 selenium_driverless-1.8.0.2/dev/assets/bypass_turnstile.mp4
--rw-rw-rw-   0        0        0    12478 2023-08-19 09:44:36.000000 selenium_driverless-1.8.0.2/dev/assets/events_mouse.png
--rw-rw-rw-   0        0        0     6691 2023-08-19 09:42:33.000000 selenium_driverless-1.8.0.2/dev/assets/events_mousepad.png
--rw-rw-rw-   0        0        0    55585 2023-08-17 15:09:30.000000 selenium_driverless-1.8.0.2/dev/assets/heatmap.png
--rw-rw-rw-   0        0        0    98170 2023-08-26 16:55:56.000000 selenium_driverless-1.8.0.2/dev/assets/mouse_path_gen.png
--rw-rw-rw-   0        0        0    40709 2023-08-26 16:54:15.000000 selenium_driverless-1.8.0.2/dev/assets/mousemove_events_gen.png
--rw-rw-rw-   0        0        0    38402 2023-08-26 17:36:05.000000 selenium_driverless-1.8.0.2/dev/assets/mousemove_events_test_sample_based.png
--rw-rw-rw-   0        0        0    88273 2023-08-26 19:31:36.000000 selenium_driverless-1.8.0.2/dev/assets/mousemove_events_test_samples_based.png
--rw-rw-rw-   0        0        0    10468 2023-08-19 09:33:39.000000 selenium_driverless-1.8.0.2/dev/assets/real_mouse_path.png
--rw-rw-rw-   0        0        0     2109 2024-01-24 23:45:42.000000 selenium_driverless-1.8.0.2/dev/human_like_path.py
--rw-rw-rw-   0        0        0     5672 2024-01-24 23:45:42.000000 selenium_driverless-1.8.0.2/dev/new_elem_calc.py
--rw-rw-rw-   0        0        0      876 2023-12-16 22:17:44.000000 selenium_driverless-1.8.0.2/dev/random_point_heatmap.py
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.517433 selenium_driverless-1.8.0.2/docs/
--rw-rw-rw-   0        0        0      234 2024-03-10 11:02:07.000000 selenium_driverless-1.8.0.2/docs/.buildinfo
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.527433 selenium_driverless-1.8.0.2/docs/.doctrees/
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.532433 selenium_driverless-1.8.0.2/docs/.doctrees/classes/
--rw-rw-rw-   0        0        0   395283 2024-03-10 11:02:04.000000 selenium_driverless-1.8.0.2/docs/.doctrees/classes/Chrome.doctree
--rw-rw-rw-   0        0        0    63629 2024-03-10 11:02:04.000000 selenium_driverless-1.8.0.2/docs/.doctrees/classes/ChromeOptions.doctree
--rw-rw-rw-   0        0        0  1714098 2024-03-10 11:02:05.000000 selenium_driverless-1.8.0.2/docs/.doctrees/environment.pickle
--rw-rw-rw-   0        0        0     4624 2024-03-10 11:02:05.000000 selenium_driverless-1.8.0.2/docs/.doctrees/index.doctree
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.533433 selenium_driverless-1.8.0.2/docs/_modules/
--rw-rw-rw-   0        0        0     4732 2024-03-10 11:02:07.000000 selenium_driverless-1.8.0.2/docs/_modules/index.html
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.467355 selenium_driverless-1.8.0.2/docs/_modules/selenium_driverless/
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.467355 selenium_driverless-1.8.0.2/docs/_modules/selenium_driverless/types/
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.534433 selenium_driverless-1.8.0.2/docs/_modules/selenium_driverless/types/options/
--rw-rw-rw-   0        0        0    50274 2024-03-10 11:02:06.000000 selenium_driverless-1.8.0.2/docs/_modules/selenium_driverless/types/options/index.html
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.536433 selenium_driverless-1.8.0.2/docs/_modules/selenium_driverless/webdriver/
--rw-rw-rw-   0        0        0   238700 2024-03-10 11:02:07.000000 selenium_driverless-1.8.0.2/docs/_modules/selenium_driverless/webdriver/index.html
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.538435 selenium_driverless-1.8.0.2/docs/_sources/
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.541433 selenium_driverless-1.8.0.2/docs/_sources/classes/
--rw-rw-rw-   0        0        0      217 2024-02-03 17:19:10.000000 selenium_driverless-1.8.0.2/docs/_sources/classes/Chrome.rst.txt
--rw-rw-rw-   0        0        0      139 2024-02-02 12:51:25.000000 selenium_driverless-1.8.0.2/docs/_sources/classes/ChromeOptions.rst.txt
--rw-rw-rw-   0        0        0      393 2024-02-03 17:25:34.000000 selenium_driverless-1.8.0.2/docs/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.558446 selenium_driverless-1.8.0.2/docs/_static/
--rw-rw-rw-   0        0        0     4289 2024-03-10 11:02:02.000000 selenium_driverless-1.8.0.2/docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-rw-   0        0        0    16018 2024-03-10 11:02:05.000000 selenium_driverless-1.8.0.2/docs/_static/basic.css
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.561447 selenium_driverless-1.8.0.2/docs/_static/css/
--rw-rw-rw-   0        0        0     3229 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/badge_only.css
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.607595 selenium_driverless-1.8.0.2/docs/_static/css/fonts/
--rw-rw-rw-   0        0        0    87624 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-rw-rw-   0        0        0    67312 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-rw-rw-   0        0        0    86288 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-rw-rw-   0        0        0    66444 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-rw-rw-   0        0        0   165742 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   444379 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/fontawesome-webfont.woff2
--rw-rw-rw-   0        0        0   323344 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-bold-italic.woff
--rw-rw-rw-   0        0        0   193308 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-bold-italic.woff2
--rw-rw-rw-   0        0        0   309728 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-bold.woff
--rw-rw-rw-   0        0        0   184912 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-bold.woff2
--rw-rw-rw-   0        0        0   328412 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-normal-italic.woff
--rw-rw-rw-   0        0        0   195704 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-normal-italic.woff2
--rw-rw-rw-   0        0        0   309192 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-normal.woff
--rw-rw-rw-   0        0        0   182708 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-normal.woff2
--rw-rw-rw-   0        0        0   135314 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/css/theme.css
--rw-rw-rw-   0        0        0     4472 2024-01-23 09:09:05.000000 selenium_driverless-1.8.0.2/docs/_static/doctools.js
--rw-rw-rw-   0        0        0      345 2024-03-10 11:02:05.000000 selenium_driverless-1.8.0.2/docs/_static/documentation_options.js
--rw-rw-rw-   0        0        0      286 2024-01-23 09:09:05.000000 selenium_driverless-1.8.0.2/docs/_static/file.png
--rw-rw-rw-   0        0        0    89501 2024-03-10 11:02:02.000000 selenium_driverless-1.8.0.2/docs/_static/jquery.js
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.618582 selenium_driverless-1.8.0.2/docs/_static/js/
--rw-rw-rw-   0        0        0      934 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/js/badge_only.js
--rw-rw-rw-   0        0        0     4370 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/js/html5shiv-printshiv.min.js
--rw-rw-rw-   0        0        0     2734 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/js/html5shiv.min.js
--rw-rw-rw-   0        0        0     5023 2024-01-23 15:14:55.000000 selenium_driverless-1.8.0.2/docs/_static/js/theme.js
--rw-rw-rw-   0        0        0     4957 2024-03-10 11:02:05.000000 selenium_driverless-1.8.0.2/docs/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2024-01-23 09:09:05.000000 selenium_driverless-1.8.0.2/docs/_static/minus.png
--rw-rw-rw-   0        0        0       90 2024-01-23 09:09:05.000000 selenium_driverless-1.8.0.2/docs/_static/plus.png
--rw-rw-rw-   0        0        0     4976 2024-03-10 11:02:05.000000 selenium_driverless-1.8.0.2/docs/_static/pygments.css
--rw-rw-rw-   0        0        0    18732 2024-01-23 09:09:05.000000 selenium_driverless-1.8.0.2/docs/_static/searchtools.js
--rw-rw-rw-   0        0        0     5123 2024-01-23 09:09:05.000000 selenium_driverless-1.8.0.2/docs/_static/sphinx_highlight.js
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.469355 selenium_driverless-1.8.0.2/docs/classes/
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.621580 selenium_driverless-1.8.0.2/docs/classes/Chrome/
--rw-rw-rw-   0        0        0   178583 2024-03-10 11:02:06.000000 selenium_driverless-1.8.0.2/docs/classes/Chrome/index.html
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.625613 selenium_driverless-1.8.0.2/docs/classes/ChromeOptions/
--rw-rw-rw-   0        0        0    32547 2024-03-10 11:02:06.000000 selenium_driverless-1.8.0.2/docs/classes/ChromeOptions/index.html
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.627577 selenium_driverless-1.8.0.2/docs/genindex/
--rw-rw-rw-   0        0        0    52984 2024-03-10 11:02:06.000000 selenium_driverless-1.8.0.2/docs/genindex/index.html
--rw-rw-rw-   0        0        0     7772 2024-03-10 11:02:06.000000 selenium_driverless-1.8.0.2/docs/index.html
--rw-rw-rw-   0        0        0     2081 2024-03-10 11:02:07.000000 selenium_driverless-1.8.0.2/docs/objects.inv
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.630579 selenium_driverless-1.8.0.2/docs/search/
--rw-rw-rw-   0        0        0     4481 2024-03-10 11:02:07.000000 selenium_driverless-1.8.0.2/docs/search/index.html
--rw-rw-rw-   0        0        0    59470 2024-03-10 11:02:07.000000 selenium_driverless-1.8.0.2/docs/searchindex.js
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.636316 selenium_driverless-1.8.0.2/docs_source/
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.643235 selenium_driverless-1.8.0.2/docs_source/classes/
--rw-rw-rw-   0        0        0      217 2024-02-03 17:19:10.000000 selenium_driverless-1.8.0.2/docs_source/classes/Chrome.rst
--rw-rw-rw-   0        0        0      139 2024-02-02 12:51:25.000000 selenium_driverless-1.8.0.2/docs_source/classes/ChromeOptions.rst
--rw-rw-rw-   0        0        0     1358 2024-02-02 12:18:19.000000 selenium_driverless-1.8.0.2/docs_source/conf.py
--rw-rw-rw-   0        0        0      393 2024-02-03 17:25:34.000000 selenium_driverless-1.8.0.2/docs_source/index.rst
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.646229 selenium_driverless-1.8.0.2/examples/
--rw-rw-rw-   0        0        0      661 2024-01-13 02:29:22.000000 selenium_driverless-1.8.0.2/examples/proxy_with_auth.py
--rw-rw-rw-   0        0        0      330 2023-09-19 13:08:57.000000 selenium_driverless-1.8.0.2/main.py
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.8.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      251 2024-02-08 09:45:22.000000 selenium_driverless-1.8.0.2/requirements.txt
--rw-rw-rw-   0        0        0      133 2024-03-10 11:03:06.748098 selenium_driverless-1.8.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2016 2024-01-29 19:20:30.000000 selenium_driverless-1.8.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.472322 selenium_driverless-1.8.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.654329 selenium_driverless-1.8.0.2/src/selenium_driverless/
--rw-rw-rw-   0        0        0       94 2024-03-10 10:59:27.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.674208 selenium_driverless-1.8.0.2/src/selenium_driverless/files/
--rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/files/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.675105 selenium_driverless-1.8.0.2/src/selenium_driverless/files/js/
--rw-rw-rw-   0        0        0     7941 2023-09-27 20:37:25.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/files/js/show_mousemove.js
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.681117 selenium_driverless-1.8.0.2/src/selenium_driverless/files/mv3_extension/
--rw-rw-rw-   0        0        0      866 2023-07-06 16:49:03.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/files/mv3_extension/driverless_background_mv3_243ffdd55e32a012b4f253b2879af978.js
--rw-rw-rw-   0        0        0     1895 2024-01-25 12:59:36.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/files/mv3_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.686141 selenium_driverless-1.8.0.2/src/selenium_driverless/input/
--rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/input/__init__.py
--rw-rw-rw-   0        0        0     8365 2024-02-15 19:38:18.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/input/pointer.py
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.695098 selenium_driverless-1.8.0.2/src/selenium_driverless/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/scripts/__init__.py
--rw-rw-rw-   0        0        0     4079 2024-02-03 16:33:48.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/scripts/driver_utils.py
--rw-rw-rw-   0        0        0     7061 2023-12-16 21:52:11.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/scripts/geometry.py
--rw-rw-rw-   0        0        0     1005 2023-12-16 21:52:11.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/scripts/prefs.py
--rw-rw-rw-   0        0        0     6751 2024-02-03 17:21:37.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/scripts/switch_to.py
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.712097 selenium_driverless-1.8.0.2/src/selenium_driverless/sync/
--rw-rw-rw-   0        0        0        0 2023-07-26 11:51:40.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/sync/__init__.py
--rw-rw-rw-   0        0        0     1102 2023-09-19 13:27:55.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/sync/alert.py
--rw-rw-rw-   0        0        0     1300 2023-12-16 21:52:11.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/sync/base_target.py
--rw-rw-rw-   0        0        0     1377 2023-12-16 21:52:11.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/sync/context.py
--rw-rw-rw-   0        0        0     1244 2023-09-19 13:06:07.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/sync/executor.py
--rw-rw-rw-   0        0        0     1124 2023-09-19 13:27:55.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/sync/pointer.py
--rw-rw-rw-   0        0        0     1111 2023-09-19 13:27:55.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/sync/switch_to.py
--rw-rw-rw-   0        0        0     1446 2024-02-03 16:33:48.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/sync/target.py
--rw-rw-rw-   0        0        0     1420 2023-12-16 21:52:11.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/sync/webdriver.py
--rw-rw-rw-   0        0        0     1615 2023-12-16 21:52:11.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/sync/webelement.py
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.729097 selenium_driverless-1.8.0.2/src/selenium_driverless/types/
--rw-rw-rw-   0        0        0      631 2023-09-25 19:30:05.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/types/__init__.py
--rw-rw-rw-   0        0        0     4151 2024-01-24 23:45:42.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/types/alert.py
--rw-rw-rw-   0        0        0     5258 2024-02-03 16:03:53.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/types/base_target.py
--rw-rw-rw-   0        0        0     1209 2024-03-10 10:42:18.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/types/by.py
--rw-rw-rw-   0        0        0    38458 2024-02-06 11:51:27.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/types/context.py
--rw-rw-rw-   0        0        0    29930 2024-02-03 11:02:55.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/types/deserialize.py
--rw-rw-rw-   0        0        0    13951 2024-03-10 10:13:26.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/types/options.py
--rw-rw-rw-   0        0        0    42992 2024-03-02 09:58:18.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/types/target.py
--rw-rw-rw-   0        0        0    34498 2024-02-06 11:51:27.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/types/webelement.py
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.732097 selenium_driverless-1.8.0.2/src/selenium_driverless/utils/
--rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/utils/__init__.py
--rw-rw-rw-   0        0        0     5332 2024-03-10 10:52:08.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/utils/utils.py
--rw-rw-rw-   0        0        0    66265 2024-03-10 10:09:02.000000 selenium_driverless-1.8.0.2/src/selenium_driverless/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.745096 selenium_driverless-1.8.0.2/src/selenium_driverless.egg-info/
--rw-rw-rw-   0        0        0    16280 2024-03-10 11:03:06.000000 selenium_driverless-1.8.0.2/src/selenium_driverless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4566 2024-03-10 11:03:06.000000 selenium_driverless-1.8.0.2/src/selenium_driverless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-10 11:03:06.000000 selenium_driverless-1.8.0.2/src/selenium_driverless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2024-03-10 11:03:06.000000 selenium_driverless-1.8.0.2/src/selenium_driverless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-03-10 11:03:06.000000 selenium_driverless-1.8.0.2/src/selenium_driverless.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      223 2023-09-19 13:08:57.000000 selenium_driverless-1.8.0.2/sync_main.py
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.740096 selenium_driverless-1.8.0.2/tests/
--rw-rw-rw-   0        0        0     2204 2024-02-02 18:30:39.000000 selenium_driverless-1.8.0.2/tests/bypass_turnstile.py
-drwxrwxrwx   0        0        0        0 2024-03-10 11:03:06.743096 selenium_driverless-1.8.0.2/tests/selenium_detector/
--rw-rw-rw-   0        0        0     1046 2024-02-03 11:40:25.000000 selenium_driverless-1.8.0.2/tests/selenium_detector/selenium_detector.py
--rw-rw-rw-   0        0        0     1028 2024-02-03 11:40:25.000000 selenium_driverless-1.8.0.2/tests/selenium_detector/sync_selenium_detector.py
--rw-rw-rw-   0        0        0     1028 2023-12-16 22:00:41.000000 selenium_driverless-1.8.0.2/tests/show_mousemove.py
--rw-rw-rw-   0        0        0     1525 2024-01-29 18:56:18.000000 selenium_driverless-1.8.0.2/tests/target_interception.py
--rw-rw-rw-   0        0        0     4464 2024-02-03 16:44:08.000000 selenium_driverless-1.8.0.2/tests/test_driverless.py
--rw-rw-rw-   0        0        0    30286 2024-03-10 10:56:04.000000 selenium_driverless-1.8.0.2/tests/turnstile_captcha.png
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.804611 selenium_driverless-1.9/
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.734253 selenium_driverless-1.9/.github/
+-rw-rw-rw-   0        0        0      512 2023-10-29 12:51:12.000000 selenium_driverless-1.9/.github/dependabot.yml
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.738253 selenium_driverless-1.9/.github/workflows/
+-rw-rw-rw-   0        0        0      905 2023-10-29 12:51:12.000000 selenium_driverless-1.9/.github/workflows/dependency-review.yml
+-rw-rw-rw-   0        0        0      738 2023-09-19 13:08:57.000000 selenium_driverless-1.9/LICENSE.md
+-rw-rw-rw-   0        0        0      185 2023-11-30 15:16:31.000000 selenium_driverless-1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    13633 2024-04-17 11:26:49.802610 selenium_driverless-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    12052 2024-04-17 11:26:14.000000 selenium_driverless-1.9/README.md
+-rw-rw-rw-   0        0        0      696 2024-01-29 19:33:57.000000 selenium_driverless-1.9/build_upload.md
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.745241 selenium_driverless-1.9/dev/
+-rw-rw-rw-   0        0        0     1112 2024-03-28 13:55:11.000000 selenium_driverless-1.9/dev/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.863731 selenium_driverless-1.9/dev/assets/
+-rw-rw-rw-   0        0        0   429242 2023-08-27 15:04:01.000000 selenium_driverless-1.9/dev/assets/bypass_turnstile.mp4
+-rw-rw-rw-   0        0        0    12478 2023-08-19 09:44:36.000000 selenium_driverless-1.9/dev/assets/events_mouse.png
+-rw-rw-rw-   0        0        0     6691 2023-08-19 09:42:33.000000 selenium_driverless-1.9/dev/assets/events_mousepad.png
+-rw-rw-rw-   0        0        0   166789 2024-03-28 13:50:09.000000 selenium_driverless-1.9/dev/assets/heatmap.png
+-rw-rw-rw-   0        0        0    98170 2023-08-26 16:55:56.000000 selenium_driverless-1.9/dev/assets/mouse_path_gen.png
+-rw-rw-rw-   0        0        0    40709 2023-08-26 16:54:15.000000 selenium_driverless-1.9/dev/assets/mousemove_events_gen.png
+-rw-rw-rw-   0        0        0    38402 2023-08-26 17:36:05.000000 selenium_driverless-1.9/dev/assets/mousemove_events_test_sample_based.png
+-rw-rw-rw-   0        0        0    88273 2023-08-26 19:31:36.000000 selenium_driverless-1.9/dev/assets/mousemove_events_test_samples_based.png
+-rw-rw-rw-   0        0        0    10468 2023-08-19 09:33:39.000000 selenium_driverless-1.9/dev/assets/real_mouse_path.png
+-rw-rw-rw-   0        0        0     2109 2024-01-24 23:45:42.000000 selenium_driverless-1.9/dev/human_like_path.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.881453 selenium_driverless-1.9/docs/
+-rw-rw-rw-   0        0        0      234 2024-04-17 11:22:40.000000 selenium_driverless-1.9/docs/.buildinfo
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.077910 selenium_driverless-1.9/docs/.doctrees/
+-rw-rw-rw-   0        0        0  2696582 2024-04-17 11:22:38.000000 selenium_driverless-1.9/docs/.doctrees/environment.pickle
+-rw-rw-rw-   0        0        0     7192 2024-04-17 10:22:19.000000 selenium_driverless-1.9/docs/.doctrees/index.doctree
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.082918 selenium_driverless-1.9/docs/_modules/
+-rw-rw-rw-   0        0        0     5232 2024-04-17 11:22:40.000000 selenium_driverless-1.9/docs/_modules/index.html
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.672089 selenium_driverless-1.9/docs/_modules/selenium_driverless/
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.671089 selenium_driverless-1.9/docs/_modules/selenium_driverless/types/
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.087907 selenium_driverless-1.9/docs/_modules/selenium_driverless/types/options/
+-rw-rw-rw-   0        0        0    50445 2024-04-17 11:22:39.000000 selenium_driverless-1.9/docs/_modules/selenium_driverless/types/options/index.html
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.096926 selenium_driverless-1.9/docs/_modules/selenium_driverless/webdriver/
+-rw-rw-rw-   0        0        0   241680 2024-04-17 11:22:40.000000 selenium_driverless-1.9/docs/_modules/selenium_driverless/webdriver/index.html
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.119706 selenium_driverless-1.9/docs/_sources/
+-rw-rw-rw-   0        0        0     1425 2024-04-16 23:06:25.000000 selenium_driverless-1.9/docs/_sources/index.rst.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.186585 selenium_driverless-1.9/docs/_static/
+-rw-rw-rw-   0        0        0     4289 2024-04-17 11:22:37.000000 selenium_driverless-1.9/docs/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-rw-   0        0        0    16018 2024-04-17 11:22:38.000000 selenium_driverless-1.9/docs/_static/basic.css
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.193718 selenium_driverless-1.9/docs/_static/css/
+-rw-rw-rw-   0        0        0     3229 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/badge_only.css
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.524370 selenium_driverless-1.9/docs/_static/css/fonts/
+-rw-rw-rw-   0        0        0    87624 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-rw-rw-   0        0        0    67312 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-rw-rw-   0        0        0    86288 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-rw-rw-   0        0        0    66444 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-rw-rw-   0        0        0   165742 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   444379 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0   323344 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-bold-italic.woff
+-rw-rw-rw-   0        0        0   193308 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-bold-italic.woff2
+-rw-rw-rw-   0        0        0   309728 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-bold.woff
+-rw-rw-rw-   0        0        0   184912 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-bold.woff2
+-rw-rw-rw-   0        0        0   328412 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-normal-italic.woff
+-rw-rw-rw-   0        0        0   195704 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-normal-italic.woff2
+-rw-rw-rw-   0        0        0   309192 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-normal.woff
+-rw-rw-rw-   0        0        0   182708 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-normal.woff2
+-rw-rw-rw-   0        0        0   135314 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/theme.css
+-rw-rw-rw-   0        0        0     4472 2024-01-23 09:09:05.000000 selenium_driverless-1.9/docs/_static/doctools.js
+-rw-rw-rw-   0        0        0      345 2024-04-17 11:22:38.000000 selenium_driverless-1.9/docs/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      286 2024-01-23 09:09:05.000000 selenium_driverless-1.9/docs/_static/file.png
+-rw-rw-rw-   0        0        0    89501 2024-04-17 11:22:37.000000 selenium_driverless-1.9/docs/_static/jquery.js
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.561036 selenium_driverless-1.9/docs/_static/js/
+-rw-rw-rw-   0        0        0      934 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/js/badge_only.js
+-rw-rw-rw-   0        0        0     4370 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/js/html5shiv-printshiv.min.js
+-rw-rw-rw-   0        0        0     2734 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/js/html5shiv.min.js
+-rw-rw-rw-   0        0        0     5023 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/js/theme.js
+-rw-rw-rw-   0        0        0     4957 2024-04-17 11:22:38.000000 selenium_driverless-1.9/docs/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2024-01-23 09:09:05.000000 selenium_driverless-1.9/docs/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2024-01-23 09:09:05.000000 selenium_driverless-1.9/docs/_static/plus.png
+-rw-rw-rw-   0        0        0     4976 2024-04-17 11:22:38.000000 selenium_driverless-1.9/docs/_static/pygments.css
+-rw-rw-rw-   0        0        0    18732 2024-01-23 09:09:05.000000 selenium_driverless-1.9/docs/_static/searchtools.js
+-rw-rw-rw-   0        0        0     5123 2024-01-23 09:09:05.000000 selenium_driverless-1.9/docs/_static/sphinx_highlight.js
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.564684 selenium_driverless-1.9/docs/genindex/
+-rw-rw-rw-   0        0        0    83639 2024-04-17 11:22:39.000000 selenium_driverless-1.9/docs/genindex/index.html
+-rw-rw-rw-   0        0        0    14429 2024-04-17 11:22:39.000000 selenium_driverless-1.9/docs/index.html
+-rw-rw-rw-   0        0        0     3220 2024-04-17 11:22:40.000000 selenium_driverless-1.9/docs/objects.inv
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.576692 selenium_driverless-1.9/docs/search/
+-rw-rw-rw-   0        0        0     4666 2024-04-17 11:22:40.000000 selenium_driverless-1.9/docs/search/index.html
+-rw-rw-rw-   0        0        0    44475 2024-04-17 11:22:40.000000 selenium_driverless-1.9/docs/searchindex.js
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.585683 selenium_driverless-1.9/docs_source/
+-rw-rw-rw-   0        0        0     1394 2024-03-28 15:03:07.000000 selenium_driverless-1.9/docs_source/conf.py
+-rw-rw-rw-   0        0        0     1425 2024-04-16 23:06:25.000000 selenium_driverless-1.9/docs_source/index.rst
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.591689 selenium_driverless-1.9/examples/
+-rw-rw-rw-   0        0        0      661 2024-01-13 02:29:22.000000 selenium_driverless-1.9/examples/proxy_with_auth.py
+-rw-rw-rw-   0        0        0      330 2023-09-19 13:08:57.000000 selenium_driverless-1.9/main.py
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      288 2024-04-16 12:32:39.000000 selenium_driverless-1.9/requirements.txt
+-rw-rw-rw-   0        0        0      133 2024-04-17 11:26:49.809702 selenium_driverless-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1997 2024-03-28 14:43:45.000000 selenium_driverless-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.684090 selenium_driverless-1.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.602702 selenium_driverless-1.9/src/selenium_driverless/
+-rw-rw-rw-   0        0        0       90 2024-04-17 11:24:02.000000 selenium_driverless-1.9/src/selenium_driverless/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.628866 selenium_driverless-1.9/src/selenium_driverless/files/
+-rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.9/src/selenium_driverless/files/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.629863 selenium_driverless-1.9/src/selenium_driverless/files/js/
+-rw-rw-rw-   0        0        0     7941 2023-09-27 20:37:25.000000 selenium_driverless-1.9/src/selenium_driverless/files/js/show_mousemove.js
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.635890 selenium_driverless-1.9/src/selenium_driverless/files/mv3_extension/
+-rw-rw-rw-   0        0        0      866 2023-07-06 16:49:03.000000 selenium_driverless-1.9/src/selenium_driverless/files/mv3_extension/driverless_background_mv3_243ffdd55e32a012b4f253b2879af978.js
+-rw-rw-rw-   0        0        0     1895 2024-01-25 12:59:36.000000 selenium_driverless-1.9/src/selenium_driverless/files/mv3_extension/manifest.json
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.639862 selenium_driverless-1.9/src/selenium_driverless/input/
+-rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.9/src/selenium_driverless/input/__init__.py
+-rw-rw-rw-   0        0        0    11698 2024-04-17 10:38:30.000000 selenium_driverless-1.9/src/selenium_driverless/input/pointer.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.661876 selenium_driverless-1.9/src/selenium_driverless/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.9/src/selenium_driverless/scripts/__init__.py
+-rw-rw-rw-   0        0        0     4079 2024-02-03 16:33:48.000000 selenium_driverless-1.9/src/selenium_driverless/scripts/driver_utils.py
+-rw-rw-rw-   0        0        0     5933 2024-04-17 10:04:35.000000 selenium_driverless-1.9/src/selenium_driverless/scripts/geometry.py
+-rw-rw-rw-   0        0        0    30549 2024-04-17 10:35:33.000000 selenium_driverless-1.9/src/selenium_driverless/scripts/network_interceptor.py
+-rw-rw-rw-   0        0        0     1005 2023-12-16 21:52:11.000000 selenium_driverless-1.9/src/selenium_driverless/scripts/prefs.py
+-rw-rw-rw-   0        0        0     6830 2024-03-28 15:00:20.000000 selenium_driverless-1.9/src/selenium_driverless/scripts/switch_to.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.701167 selenium_driverless-1.9/src/selenium_driverless/sync/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:51:40.000000 selenium_driverless-1.9/src/selenium_driverless/sync/__init__.py
+-rw-rw-rw-   0        0        0     1102 2023-09-19 13:27:55.000000 selenium_driverless-1.9/src/selenium_driverless/sync/alert.py
+-rw-rw-rw-   0        0        0     1300 2023-12-16 21:52:11.000000 selenium_driverless-1.9/src/selenium_driverless/sync/base_target.py
+-rw-rw-rw-   0        0        0     1377 2023-12-16 21:52:11.000000 selenium_driverless-1.9/src/selenium_driverless/sync/context.py
+-rw-rw-rw-   0        0        0     1244 2023-09-19 13:06:07.000000 selenium_driverless-1.9/src/selenium_driverless/sync/executor.py
+-rw-rw-rw-   0        0        0     1124 2023-09-19 13:27:55.000000 selenium_driverless-1.9/src/selenium_driverless/sync/pointer.py
+-rw-rw-rw-   0        0        0     1111 2023-09-19 13:27:55.000000 selenium_driverless-1.9/src/selenium_driverless/sync/switch_to.py
+-rw-rw-rw-   0        0        0     1446 2024-02-03 16:33:48.000000 selenium_driverless-1.9/src/selenium_driverless/sync/target.py
+-rw-rw-rw-   0        0        0     1420 2023-12-16 21:52:11.000000 selenium_driverless-1.9/src/selenium_driverless/sync/webdriver.py
+-rw-rw-rw-   0        0        0     1615 2023-12-16 21:52:11.000000 selenium_driverless-1.9/src/selenium_driverless/sync/webelement.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.743602 selenium_driverless-1.9/src/selenium_driverless/types/
+-rw-rw-rw-   0        0        0      631 2023-09-25 19:30:05.000000 selenium_driverless-1.9/src/selenium_driverless/types/__init__.py
+-rw-rw-rw-   0        0        0     4151 2024-01-24 23:45:42.000000 selenium_driverless-1.9/src/selenium_driverless/types/alert.py
+-rw-rw-rw-   0        0        0     5749 2024-04-16 21:43:55.000000 selenium_driverless-1.9/src/selenium_driverless/types/base_target.py
+-rw-rw-rw-   0        0        0     1184 2024-03-28 15:03:07.000000 selenium_driverless-1.9/src/selenium_driverless/types/by.py
+-rw-rw-rw-   0        0        0    41099 2024-04-17 11:07:13.000000 selenium_driverless-1.9/src/selenium_driverless/types/context.py
+-rw-rw-rw-   0        0        0    29930 2024-02-03 11:02:55.000000 selenium_driverless-1.9/src/selenium_driverless/types/deserialize.py
+-rw-rw-rw-   0        0        0    13951 2024-03-10 10:13:26.000000 selenium_driverless-1.9/src/selenium_driverless/types/options.py
+-rw-rw-rw-   0        0        0    57931 2024-04-17 11:08:17.000000 selenium_driverless-1.9/src/selenium_driverless/types/target.py
+-rw-rw-rw-   0        0        0    38016 2024-04-17 11:22:35.000000 selenium_driverless-1.9/src/selenium_driverless/types/webelement.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.753615 selenium_driverless-1.9/src/selenium_driverless/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.9/src/selenium_driverless/utils/__init__.py
+-rw-rw-rw-   0        0        0     5340 2024-03-28 18:41:47.000000 selenium_driverless-1.9/src/selenium_driverless/utils/utils.py
+-rw-rw-rw-   0        0        0    66796 2024-04-17 11:07:13.000000 selenium_driverless-1.9/src/selenium_driverless/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.797663 selenium_driverless-1.9/src/selenium_driverless.egg-info/
+-rw-rw-rw-   0        0        0    13633 2024-04-17 11:26:48.000000 selenium_driverless-1.9/src/selenium_driverless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4270 2024-04-17 11:26:48.000000 selenium_driverless-1.9/src/selenium_driverless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 11:26:48.000000 selenium_driverless-1.9/src/selenium_driverless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2024-04-17 11:26:48.000000 selenium_driverless-1.9/src/selenium_driverless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-17 11:26:48.000000 selenium_driverless-1.9/src/selenium_driverless.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      223 2023-09-19 13:08:57.000000 selenium_driverless-1.9/sync_main.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.780683 selenium_driverless-1.9/tests/
+-rw-rw-rw-   0        0        0     1884 2024-04-17 10:45:25.000000 selenium_driverless-1.9/tests/bypass_turnstile.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.792611 selenium_driverless-1.9/tests/selenium_detector/
+-rw-rw-rw-   0        0        0     1054 2024-04-17 11:18:06.000000 selenium_driverless-1.9/tests/selenium_detector/selenium_detector.py
+-rw-rw-rw-   0        0        0     1036 2024-04-17 11:19:31.000000 selenium_driverless-1.9/tests/selenium_detector/sync_selenium_detector.py
+-rw-rw-rw-   0        0        0     1102 2024-04-17 10:22:08.000000 selenium_driverless-1.9/tests/show_mousemove.py
+-rw-rw-rw-   0        0        0     1637 2024-03-28 18:46:42.000000 selenium_driverless-1.9/tests/target_interception.py
+-rw-rw-rw-   0        0        0     4539 2024-04-17 11:19:31.000000 selenium_driverless-1.9/tests/test_driverless.py
+-rw-rw-rw-   0        0        0    23694 2024-04-17 10:45:41.000000 selenium_driverless-1.9/tests/turnstile_captcha.png
```

### Comparing `selenium_driverless-1.8.0.2/.github/dependabot.yml` & `selenium_driverless-1.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/.github/workflows/dependency-review.yml` & `selenium_driverless-1.9/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/LICENSE.md` & `selenium_driverless-1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/PKG-INFO` & `selenium_driverless-1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_driverless
-Version: 1.8.0.2
+Version: 1.9
 Summary: Undetected selenium without chromedriver usage (Non-commercial use only!)
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 License: CC BY-NC-SA 4.0
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
@@ -26,52 +26,61 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: selenium~=4.6
 Requires-Dist: cdp-socket>=1.2.5
 Requires-Dist: numpy
-Requires-Dist: matplotlib~=3.5
 Requires-Dist: scipy~=1.7
 Requires-Dist: aiofiles
 Requires-Dist: platformdirs
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 
-# Selenium-Driverless (Non-commercial use only!)
+# Driverless (Non-commercial use only!)
 
 [![Downloads](https://static.pepy.tech/badge/selenium-driverless)](https://pepy.tech/project/selenium-driverless) [![](https://img.shields.io/pypi/v/selenium-driverless.svg?color=3399EE)](https://pypi.org/project/selenium-driverless/)
 [Documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/#)
 
 
 - Use Selenium __without chromedriver__
 - Currently passes __Cloudflare__, __Bet365__, [Turnstile](https://github.com/kaliiiiiiiiii/Selenium-Driverless/tree/master/dev#bypass-turnstile), and others
 - Multiple tabs simultaneously
-- Multiple Incognito-contexts with individual proxy & cookies
-- Async (`asyncio`) and sync (experimental) support
-- Proxy-auth support (experimental, [example code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/dev/examples/proxy_with_auth.py))
-- Network-interception
-- headless supported
+- Multiple Incognito-contexts with isolated cookies & local storage
+- Proxy-auth support ([example code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/dev/examples/proxy_with_auth.py))
+- Network-interception ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Chrome/RequestInterception/))
+- Single requests ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Target/#selenium_driverless.types.target.Target.fetch))
 
 ### Questions? 
 Feel free to join the [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on **Discord**:)
 
 Also, see [dev-branch](https://github.com/kaliiiiiiiiii/Selenium-Driverless/tree/dev) for the latest implementations.
 <details>
 <summary>dev-installation (click to expand)</summary>
 
 ```shell
 pip uninstall -y selenium-driverless
 pip install https://github.com/kaliiiiiiiiii/Selenium-Driverless/archive/refs/heads/dev.zip
 ```
 </details>
 
-### Still getting detected?
-Feel free to give me a feedback! \
-You're a company and looking for another solution? Maybe **[undetect.io](https://undetect.io/partner/steve)** is smth for you
+<!---
+
+## Sponsors
+
+### [Capsolver](https://capsolver.com/?utm_source=github&utm_medium=banner_github&utm_campaign=selenium-driverless)
+
+[![img.png](assets/capsolver.png)](https://capsolver.com/?utm_source=github&utm_medium=banner_github&utm_campaign=selenium-driverless)
+
+an AI-powered service that provides **automatic captcha solving** capabilities. It supports a range of captcha types,
+including `reCAPTCHA`, `hCaptcha`, and `FunCaptcha`, `AWS Captcha`, `Geetest` and image captcha among others.
+Capsolver offers browser-extensions for ease of use, API integration for developers, and various pricing packages to suit
+different needs.
+
+-->
 
 #### Also, feel free to
 <a href="https://www.buymeacoffee.com/kaliiii">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="https://www.buymeacoffee.com/assets/img/custom_images/black_img.png" />
     <source media="(prefers-color-scheme: light)" srcset="https://www.buymeacoffee.com/assets/img/custom_images/white_img.png" />
     <img alt="Star History Chart" src="https://www.buymeacoffee.com/assets/img/custom_images/black_img.png" />
@@ -97,15 +106,15 @@
 from selenium_driverless.types.by import By
 import asyncio
 
 
 async def main():
     options = webdriver.ChromeOptions()
     async with webdriver.Chrome(options=options) as driver:
-        await driver.get('http://nowsecure.nl#relax')
+        await driver.get('http://nowsecure.nl#relax', wait_load=True)
         await driver.sleep(0.5)
         await driver.wait_for_cdp("Page.domContentEventFired", timeout=15)
         
         # wait 10s for elem to exist
         elem = await driver.find_element(By.XPATH, '/html/body/div[2]/div/main/p[2]/a', timeout=10)
         await elem.click(move_to=True)
 
@@ -148,91 +157,14 @@
 # specify if you don't want to run remote
 # options.add_argument("--remote-debugging-port=2005")
 
 async with webdriver.Chrome(options=options) as driver:
   await driver.get('http://nowsecure.nl#relax', wait_load=True)
 ```
 
-### Network-Interception
-- use CDP events (see [chrome-developer-protocoll](https://chromedevtools.github.io/devtools-protocol/) for possible events) 
-
-**Notes**: synchronous might not work properly
-
-<details>
-<summary>Example Code (Click to expand)</summary>
-
-warning: network interception with `Fetch.enable` might have issues with cross-domain iframes, maximum websocket message size or Font requests.\
-You might try using [`Network.setRequestInterception](https://chromedevtools.github.io/devtools-protocol/tot/Network/#method-setRequestInterception) (officially deprecated) or narrowing the pattern
-
-```python
-import asyncio
-import base64
-import sys
-import time
-import traceback
-
-from cdp_socket.exceptions import CDPError
-from selenium_driverless import webdriver
-
-
-async def on_request(params, global_conn):
-    url = params["request"]["url"]
-    _params = {"requestId": params['requestId']}
-    if params.get('responseStatusCode') in [301, 302, 303, 307, 308]:
-        # redirected request
-        return await global_conn.execute_cdp_cmd("Fetch.continueResponse", _params)
-    else:
-        try:
-            body = await global_conn.execute_cdp_cmd("Fetch.getResponseBody", _params, timeout=1)
-        except CDPError as e:
-            if e.code == -32000 and e.message == 'Can only get response body on requests captured after headers received.':
-                print(params, "\n", file=sys.stderr)
-                traceback.print_exc()
-                await global_conn.execute_cdp_cmd("Fetch.continueResponse", _params)
-            else:
-                raise e
-        else:
-            start = time.perf_counter()
-            body_decoded = base64.b64decode(body['body'])
-
-            # modify body here
-
-            body_modified = base64.b64encode(body_decoded).decode("ascii")
-            fulfill_params = {"responseCode": 200, "body": body_modified, "responseHeaders": params["responseHeaders"]}
-            fulfill_params.update(_params)
-            if params["responseStatusText"] != "":
-                # empty string throws "Invalid http status code or phrase"
-                fulfill_params["responsePhrase"] = params["responseStatusText"]
-
-            _time = time.perf_counter() - start
-            if _time > 0.01:
-                print(f"decoding took long: {_time} s")
-            await global_conn.execute_cdp_cmd("Fetch.fulfillRequest", fulfill_params)
-            print("Mocked response", url)
-
-
-async def main():
-    async with webdriver.Chrome(max_ws_size=2 ** 30) as driver:
-        driver.base_target.socket.on_closed.append(lambda code, reason: print(f"chrome exited"))
-
-        global_conn = driver.base_target
-        await global_conn.execute_cdp_cmd("Fetch.enable",
-                                          cmd_args={"patterns": [{"requestStage": "Response", "urlPattern": "*"}]})
-        await global_conn.add_cdp_listener("Fetch.requestPaused", lambda data: on_request(data, global_conn))
-
-        await driver.get("https://nowsecure.nl/#relax", timeout=60, wait_load=False)
-        while True:
-            # time.sleep(10) # no. cloudflare would hang
-            await asyncio.sleep(10)
-
-
-asyncio.run(main())
-```
-</details>
-
 ## Multiple tabs simultaneously
 Note: asyncio is recommended, threading only works on independent webdriver.Chrome instances.
 
 <details>
 <summary>Example Code (Click to expand)</summary>
 
 ```python
@@ -311,15 +243,15 @@
 
 </details>
 
 ### Pointer Interaction
 see [@master/dev/show_mousemove.py](https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/master/dev/show_mousemove.py) for visualization
 
 ```python
-pointer = await driver.current_pointer
+pointer = driver.current_pointer
 move_kwargs = {"total_time": 0.7, "accel": 2, "smooth_soft": 20}
 
 await pointer.move_to(100, 500)
 await pointer.click(500, 50, move_kwargs=move_kwargs, move_to=True)
 ```
 ### Iframes
 - switch and interact with iframes
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: selenium_driverless Version: 1.8.0.2 Summary:
+Metadata-Version: 2.1 Name: selenium_driverless Version: 1.9 Summary:
 Undetected selenium without chromedriver usage (Non-commercial use only!) Home-
 page: https://github.com/kaliiiiiiiiii/Selenium-Driverless Author: Aurin
 Aegerter Author-email: aurinliun@gmx.ch License: CC BY-NC-SA 4.0 Project-URL:
 Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless Project-
 URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Keywords: Selenium,webautomation Classifier: Development Status :: 2 - Pre-
@@ -12,98 +12,62 @@
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: Free
 for non-commercial use Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Topic :: Internet :: Proxy
 Servers Classifier: Topic :: Internet Classifier: Topic :: Internet :: WWW/HTTP
 :: Browsers Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE.md Requires-Dist: selenium~=4.6 Requires-Dist: cdp-
-socket>=1.2.5 Requires-Dist: numpy Requires-Dist: matplotlib~=3.5 Requires-
-Dist: scipy~=1.7 Requires-Dist: aiofiles Requires-Dist: platformdirs Provides-
-Extra: dev Requires-Dist: check-manifest; extra == "dev" # Selenium-Driverless
-(Non-commercial use only!) [![Downloads](https://static.pepy.tech/badge/
-selenium-driverless)](https://pepy.tech/project/selenium-driverless) [![]
-(https://img.shields.io/pypi/v/selenium-driverless.svg?color=3399EE)](https://
-pypi.org/project/selenium-driverless/) [Documentation](https://
-kaliiiiiiiiii.github.io/Selenium-Driverless/#) - Use Selenium __without
-chromedriver__ - Currently passes __Cloudflare__, __Bet365__, [Turnstile]
-(https://github.com/kaliiiiiiiiii/Selenium-Driverless/tree/master/dev#bypass-
-turnstile), and others - Multiple tabs simultaneously - Multiple Incognito-
-contexts with individual proxy & cookies - Async (`asyncio`) and sync
-(experimental) support - Proxy-auth support (experimental, [example code]
-(https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/dev/examples/
-proxy_with_auth.py)) - Network-interception - headless supported ### Questions?
-Feel free to join the [Driverless-Community](https://discord.com/invite/
-MzZZjr2ZM3) on **Discord**:) Also, see [dev-branch](https://github.com/
-kaliiiiiiiiii/Selenium-Driverless/tree/dev) for the latest implementations.
-dev-installation (click to expand) ```shell pip uninstall -y selenium-
-driverless pip install https://github.com/kaliiiiiiiiii/Selenium-Driverless/
-archive/refs/heads/dev.zip ``` ### Still getting detected? Feel free to give me
-a feedback! \ You're a company and looking for another solution? Maybe **
-[undetect.io](https://undetect.io/partner/steve)** is smth for you #### Also,
-feel free to _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]### Dependencies * [Python >= 3.7](https://
-www.python.org/downloads/) * [Google-Chrome](https://www.google.de/chrome/
-) installed (Chromium not tested) ### Installing * Install [Google-Chrome]
-(https://www.google.de/chrome/) * ```pip install selenium-driverless``` ###
-Usage ### with asyncio ```python from selenium_driverless import webdriver from
-selenium_driverless.types.by import By import asyncio async def main(): options
-= webdriver.ChromeOptions() async with webdriver.Chrome(options=options) as
-driver: await driver.get('http://nowsecure.nl#relax') await driver.sleep(0.5)
-await driver.wait_for_cdp("Page.domContentEventFired", timeout=15) # wait 10s
-for elem to exist elem = await driver.find_element(By.XPATH, '/html/body/div
-[2]/div/main/p[2]/a', timeout=10) await elem.click(move_to=True) alert = await
-driver.switch_to.alert print(alert.text) await alert.accept() print(await
-driver.title) asyncio.run(main()) ``` ### synchronous asyncified, might be
-buggy ```python from selenium_driverless.sync import webdriver options =
-webdriver.ChromeOptions() with webdriver.Chrome(options=options) as driver:
-driver.get('http://nowsecure.nl#relax') driver.sleep(0.5) driver.wait_for_cdp
+socket>=1.2.5 Requires-Dist: numpy Requires-Dist: scipy~=1.7 Requires-Dist:
+aiofiles Requires-Dist: platformdirs Provides-Extra: dev Requires-Dist: check-
+manifest; extra == "dev" # Driverless (Non-commercial use only!) [![Downloads]
+(https://static.pepy.tech/badge/selenium-driverless)](https://pepy.tech/
+project/selenium-driverless) [![](https://img.shields.io/pypi/v/selenium-
+driverless.svg?color=3399EE)](https://pypi.org/project/selenium-driverless/)
+[Documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/#) - Use
+Selenium __without chromedriver__ - Currently passes __Cloudflare__,
+__Bet365__, [Turnstile](https://github.com/kaliiiiiiiiii/Selenium-Driverless/
+tree/master/dev#bypass-turnstile), and others - Multiple tabs simultaneously -
+Multiple Incognito-contexts with isolated cookies & local storage - Proxy-auth
+support ([example code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/
+blob/dev/examples/proxy_with_auth.py)) - Network-interception ([documentation]
+(https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Chrome/
+RequestInterception/)) - Single requests ([documentation](https://
+kaliiiiiiiiii.github.io/Selenium-Driverless/api/Target/
+#selenium_driverless.types.target.Target.fetch)) ### Questions? Feel free to
+join the [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on
+**Discord**:) Also, see [dev-branch](https://github.com/kaliiiiiiiiii/Selenium-
+Driverless/tree/dev) for the latest implementations. dev-installation (click to
+expand) ```shell pip uninstall -y selenium-driverless pip install https://
+github.com/kaliiiiiiiiii/Selenium-Driverless/archive/refs/heads/dev.zip ```
+#### Also, feel free to _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]### Dependencies * [Python >= 3.7]
+(https://www.python.org/downloads/) * [Google-Chrome](https://www.google.de/
+chrome/) installed (Chromium not tested) ### Installing * Install [Google-
+Chrome](https://www.google.de/chrome/) * ```pip install selenium-driverless```
+### Usage ### with asyncio ```python from selenium_driverless import webdriver
+from selenium_driverless.types.by import By import asyncio async def main():
+options = webdriver.ChromeOptions() async with webdriver.Chrome
+(options=options) as driver: await driver.get('http://nowsecure.nl#relax',
+wait_load=True) await driver.sleep(0.5) await driver.wait_for_cdp
+("Page.domContentEventFired", timeout=15) # wait 10s for elem to exist elem =
+await driver.find_element(By.XPATH, '/html/body/div[2]/div/main/p[2]/a',
+timeout=10) await elem.click(move_to=True) alert = await driver.switch_to.alert
+print(alert.text) await alert.accept() print(await driver.title) asyncio.run
+(main()) ``` ### synchronous asyncified, might be buggy ```python from
+selenium_driverless.sync import webdriver options = webdriver.ChromeOptions()
+with webdriver.Chrome(options=options) as driver: driver.get('http://
+nowsecure.nl#relax') driver.sleep(0.5) driver.wait_for_cdp
 ("Page.domContentEventFired", timeout=15) title = driver.title url =
 driver.current_url source = driver.page_source print(title) ``` ### custom
 debugger address ```python from selenium_driverless import webdriver options =
 webdriver.ChromeOptions() options.debugger_address = "127.0.0.1:2005" # specify
 if you don't want to run remote # options.add_argument("--remote-debugging-
 port=2005") async with webdriver.Chrome(options=options) as driver: await
-driver.get('http://nowsecure.nl#relax', wait_load=True) ``` ### Network-
-Interception - use CDP events (see [chrome-developer-protocoll](https://
-chromedevtools.github.io/devtools-protocol/) for possible events) **Notes**:
-synchronous might not work properly Example Code (Click to expand) warning:
-network interception with `Fetch.enable` might have issues with cross-domain
-iframes, maximum websocket message size or Font requests.\ You might try using
-[`Network.setRequestInterception](https://chromedevtools.github.io/devtools-
-protocol/tot/Network/#method-setRequestInterception) (officially deprecated) or
-narrowing the pattern ```python import asyncio import base64 import sys import
-time import traceback from cdp_socket.exceptions import CDPError from
-selenium_driverless import webdriver async def on_request(params, global_conn):
-url = params["request"]["url"] _params = {"requestId": params['requestId']} if
-params.get('responseStatusCode') in [301, 302, 303, 307, 308]: # redirected
-request return await global_conn.execute_cdp_cmd("Fetch.continueResponse",
-_params) else: try: body = await global_conn.execute_cdp_cmd
-("Fetch.getResponseBody", _params, timeout=1) except CDPError as e: if e.code
-== -32000 and e.message == 'Can only get response body on requests captured
-after headers received.': print(params, "\n", file=sys.stderr)
-traceback.print_exc() await global_conn.execute_cdp_cmd
-("Fetch.continueResponse", _params) else: raise e else: start =
-time.perf_counter() body_decoded = base64.b64decode(body['body']) # modify body
-here body_modified = base64.b64encode(body_decoded).decode("ascii")
-fulfill_params = {"responseCode": 200, "body": body_modified,
-"responseHeaders": params["responseHeaders"]} fulfill_params.update(_params) if
-params["responseStatusText"] != "": # empty string throws "Invalid http status
-code or phrase" fulfill_params["responsePhrase"] = params["responseStatusText"]
-_time = time.perf_counter() - start if _time > 0.01: print(f"decoding took
-long: {_time} s") await global_conn.execute_cdp_cmd("Fetch.fulfillRequest",
-fulfill_params) print("Mocked response", url) async def main(): async with
-webdriver.Chrome(max_ws_size=2 ** 30) as driver:
-driver.base_target.socket.on_closed.append(lambda code, reason: print(f"chrome
-exited")) global_conn = driver.base_target await global_conn.execute_cdp_cmd
-("Fetch.enable", cmd_args={"patterns": [{"requestStage": "Response",
-"urlPattern": "*"}]}) await global_conn.add_cdp_listener("Fetch.requestPaused",
-lambda data: on_request(data, global_conn)) await driver.get("https://
-nowsecure.nl/#relax", timeout=60, wait_load=False) while True: # time.sleep(10)
-# no. cloudflare would hang await asyncio.sleep(10) asyncio.run(main()) ``` ##
-Multiple tabs simultaneously Note: asyncio is recommended, threading only works
-on independent webdriver.Chrome instances. Example Code (Click to expand)
+driver.get('http://nowsecure.nl#relax', wait_load=True) ``` ## Multiple tabs
+simultaneously Note: asyncio is recommended, threading only works on
+independent webdriver.Chrome instances. Example Code (Click to expand)
 ```python from selenium_driverless.sync import webdriver from
 selenium_driverless.utils.utils import read from selenium_driverless import
 webdriver import asyncio async def target_1_handler(target): await target.get
 ('https://abrahamjuliot.github.io/creepjs/') print(await target.title) async
 def target_2_handler(target): await target.get("about:blank") await
 target.execute_script(script=read("/files/js/show_mousemove.js")) await
 target.pointer.move_to(500, 500, total_time=2) async def main(): options =
@@ -123,15 +87,15 @@
 Object.defineProperty(document, "documentElement", { value: proxy }) """ await
 driver.execute_script(script) src = await driver.execute_script("return
 document.documentElement.outerHTML", unique_context=True) mocked = await
 driver.execute_script("return document.documentElement.outerHTML",
 unique_context=False) print(src, mocked) asyncio.run(main()) ``` ### Pointer
 Interaction see [@master/dev/show_mousemove.py](https://github.com/
 kaliiiiiiiiii/Selenium-Driverless/blob/master/dev/show_mousemove.py) for
-visualization ```python pointer = await driver.current_pointer move_kwargs =
+visualization ```python pointer = driver.current_pointer move_kwargs =
 {"total_time": 0.7, "accel": 2, "smooth_soft": 20} await pointer.move_to(100,
 500) await pointer.click(500, 50, move_kwargs=move_kwargs, move_to=True) ```
 ### Iframes - switch and interact with iframes ```python iframes = await
 driver.find_elements(By.TAG_NAME, "iframe") await asyncio.sleep(0.5)
 iframe_document = await iframes[0].content_document #
 iframe_document.find_elements(...) ``` ### use preferences ```python from
 selenium_driverless import webdriver options = webdriver.ChromeOptions() #
```

### Comparing `selenium_driverless-1.8.0.2/README.md` & `selenium_driverless-1.9/src/selenium_driverless.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,86 @@
-# Selenium-Driverless (Non-commercial use only!)
+Metadata-Version: 2.1
+Name: selenium_driverless
+Version: 1.9
+Summary: Undetected selenium without chromedriver usage (Non-commercial use only!)
+Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
+Author: Aurin Aegerter
+Author-email: aurinliun@gmx.ch
+License: CC BY-NC-SA 4.0
+Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
+Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
+Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
+Keywords: Selenium,webautomation
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: Free for non-commercial use
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Internet :: Proxy Servers
+Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: selenium~=4.6
+Requires-Dist: cdp-socket>=1.2.5
+Requires-Dist: numpy
+Requires-Dist: scipy~=1.7
+Requires-Dist: aiofiles
+Requires-Dist: platformdirs
+Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
+
+# Driverless (Non-commercial use only!)
 
 [![Downloads](https://static.pepy.tech/badge/selenium-driverless)](https://pepy.tech/project/selenium-driverless) [![](https://img.shields.io/pypi/v/selenium-driverless.svg?color=3399EE)](https://pypi.org/project/selenium-driverless/)
 [Documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/#)
 
 
 - Use Selenium __without chromedriver__
 - Currently passes __Cloudflare__, __Bet365__, [Turnstile](https://github.com/kaliiiiiiiiii/Selenium-Driverless/tree/master/dev#bypass-turnstile), and others
 - Multiple tabs simultaneously
-- Multiple Incognito-contexts with individual proxy & cookies
-- Async (`asyncio`) and sync (experimental) support
-- Proxy-auth support (experimental, [example code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/dev/examples/proxy_with_auth.py))
-- Network-interception
-- headless supported
+- Multiple Incognito-contexts with isolated cookies & local storage
+- Proxy-auth support ([example code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/dev/examples/proxy_with_auth.py))
+- Network-interception ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Chrome/RequestInterception/))
+- Single requests ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Target/#selenium_driverless.types.target.Target.fetch))
 
 ### Questions? 
 Feel free to join the [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on **Discord**:)
 
 Also, see [dev-branch](https://github.com/kaliiiiiiiiii/Selenium-Driverless/tree/dev) for the latest implementations.
 <details>
 <summary>dev-installation (click to expand)</summary>
 
 ```shell
 pip uninstall -y selenium-driverless
 pip install https://github.com/kaliiiiiiiiii/Selenium-Driverless/archive/refs/heads/dev.zip
 ```
 </details>
 
-### Still getting detected?
-Feel free to give me a feedback! \
-You're a company and looking for another solution? Maybe **[undetect.io](https://undetect.io/partner/steve)** is smth for you
+<!---
+
+## Sponsors
+
+### [Capsolver](https://capsolver.com/?utm_source=github&utm_medium=banner_github&utm_campaign=selenium-driverless)
+
+[![img.png](assets/capsolver.png)](https://capsolver.com/?utm_source=github&utm_medium=banner_github&utm_campaign=selenium-driverless)
+
+an AI-powered service that provides **automatic captcha solving** capabilities. It supports a range of captcha types,
+including `reCAPTCHA`, `hCaptcha`, and `FunCaptcha`, `AWS Captcha`, `Geetest` and image captcha among others.
+Capsolver offers browser-extensions for ease of use, API integration for developers, and various pricing packages to suit
+different needs.
+
+-->
 
 #### Also, feel free to
 <a href="https://www.buymeacoffee.com/kaliiii">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="https://www.buymeacoffee.com/assets/img/custom_images/black_img.png" />
     <source media="(prefers-color-scheme: light)" srcset="https://www.buymeacoffee.com/assets/img/custom_images/white_img.png" />
     <img alt="Star History Chart" src="https://www.buymeacoffee.com/assets/img/custom_images/black_img.png" />
@@ -58,15 +106,15 @@
 from selenium_driverless.types.by import By
 import asyncio
 
 
 async def main():
     options = webdriver.ChromeOptions()
     async with webdriver.Chrome(options=options) as driver:
-        await driver.get('http://nowsecure.nl#relax')
+        await driver.get('http://nowsecure.nl#relax', wait_load=True)
         await driver.sleep(0.5)
         await driver.wait_for_cdp("Page.domContentEventFired", timeout=15)
         
         # wait 10s for elem to exist
         elem = await driver.find_element(By.XPATH, '/html/body/div[2]/div/main/p[2]/a', timeout=10)
         await elem.click(move_to=True)
 
@@ -109,91 +157,14 @@
 # specify if you don't want to run remote
 # options.add_argument("--remote-debugging-port=2005")
 
 async with webdriver.Chrome(options=options) as driver:
   await driver.get('http://nowsecure.nl#relax', wait_load=True)
 ```
 
-### Network-Interception
-- use CDP events (see [chrome-developer-protocoll](https://chromedevtools.github.io/devtools-protocol/) for possible events) 
-
-**Notes**: synchronous might not work properly
-
-<details>
-<summary>Example Code (Click to expand)</summary>
-
-warning: network interception with `Fetch.enable` might have issues with cross-domain iframes, maximum websocket message size or Font requests.\
-You might try using [`Network.setRequestInterception](https://chromedevtools.github.io/devtools-protocol/tot/Network/#method-setRequestInterception) (officially deprecated) or narrowing the pattern
-
-```python
-import asyncio
-import base64
-import sys
-import time
-import traceback
-
-from cdp_socket.exceptions import CDPError
-from selenium_driverless import webdriver
-
-
-async def on_request(params, global_conn):
-    url = params["request"]["url"]
-    _params = {"requestId": params['requestId']}
-    if params.get('responseStatusCode') in [301, 302, 303, 307, 308]:
-        # redirected request
-        return await global_conn.execute_cdp_cmd("Fetch.continueResponse", _params)
-    else:
-        try:
-            body = await global_conn.execute_cdp_cmd("Fetch.getResponseBody", _params, timeout=1)
-        except CDPError as e:
-            if e.code == -32000 and e.message == 'Can only get response body on requests captured after headers received.':
-                print(params, "\n", file=sys.stderr)
-                traceback.print_exc()
-                await global_conn.execute_cdp_cmd("Fetch.continueResponse", _params)
-            else:
-                raise e
-        else:
-            start = time.perf_counter()
-            body_decoded = base64.b64decode(body['body'])
-
-            # modify body here
-
-            body_modified = base64.b64encode(body_decoded).decode("ascii")
-            fulfill_params = {"responseCode": 200, "body": body_modified, "responseHeaders": params["responseHeaders"]}
-            fulfill_params.update(_params)
-            if params["responseStatusText"] != "":
-                # empty string throws "Invalid http status code or phrase"
-                fulfill_params["responsePhrase"] = params["responseStatusText"]
-
-            _time = time.perf_counter() - start
-            if _time > 0.01:
-                print(f"decoding took long: {_time} s")
-            await global_conn.execute_cdp_cmd("Fetch.fulfillRequest", fulfill_params)
-            print("Mocked response", url)
-
-
-async def main():
-    async with webdriver.Chrome(max_ws_size=2 ** 30) as driver:
-        driver.base_target.socket.on_closed.append(lambda code, reason: print(f"chrome exited"))
-
-        global_conn = driver.base_target
-        await global_conn.execute_cdp_cmd("Fetch.enable",
-                                          cmd_args={"patterns": [{"requestStage": "Response", "urlPattern": "*"}]})
-        await global_conn.add_cdp_listener("Fetch.requestPaused", lambda data: on_request(data, global_conn))
-
-        await driver.get("https://nowsecure.nl/#relax", timeout=60, wait_load=False)
-        while True:
-            # time.sleep(10) # no. cloudflare would hang
-            await asyncio.sleep(10)
-
-
-asyncio.run(main())
-```
-</details>
-
 ## Multiple tabs simultaneously
 Note: asyncio is recommended, threading only works on independent webdriver.Chrome instances.
 
 <details>
 <summary>Example Code (Click to expand)</summary>
 
 ```python
@@ -272,15 +243,15 @@
 
 </details>
 
 ### Pointer Interaction
 see [@master/dev/show_mousemove.py](https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/master/dev/show_mousemove.py) for visualization
 
 ```python
-pointer = await driver.current_pointer
+pointer = driver.current_pointer
 move_kwargs = {"total_time": 0.7, "accel": 2, "smooth_soft": 20}
 
 await pointer.move_to(100, 500)
 await pointer.click(500, 50, move_kwargs=move_kwargs, move_to=True)
 ```
 ### Iframes
 - switch and interact with iframes
```

#### html2text {}

```diff
@@ -1,88 +1,73 @@
-# Selenium-Driverless (Non-commercial use only!) [![Downloads](https://
-static.pepy.tech/badge/selenium-driverless)](https://pepy.tech/project/
-selenium-driverless) [![](https://img.shields.io/pypi/v/selenium-
+Metadata-Version: 2.1 Name: selenium_driverless Version: 1.9 Summary:
+Undetected selenium without chromedriver usage (Non-commercial use only!) Home-
+page: https://github.com/kaliiiiiiiiii/Selenium-Driverless Author: Aurin
+Aegerter Author-email: aurinliun@gmx.ch License: CC BY-NC-SA 4.0 Project-URL:
+Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless Project-
+URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
+Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
+Keywords: Selenium,webautomation Classifier: Development Status :: 2 - Pre-
+Alpha Classifier: Intended Audience :: Developers Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: Free
+for non-commercial use Classifier: Natural Language :: English Classifier:
+Operating System :: OS Independent Classifier: Topic :: Internet :: Proxy
+Servers Classifier: Topic :: Internet Classifier: Topic :: Internet :: WWW/HTTP
+:: Browsers Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE.md Requires-Dist: selenium~=4.6 Requires-Dist: cdp-
+socket>=1.2.5 Requires-Dist: numpy Requires-Dist: scipy~=1.7 Requires-Dist:
+aiofiles Requires-Dist: platformdirs Provides-Extra: dev Requires-Dist: check-
+manifest; extra == "dev" # Driverless (Non-commercial use only!) [![Downloads]
+(https://static.pepy.tech/badge/selenium-driverless)](https://pepy.tech/
+project/selenium-driverless) [![](https://img.shields.io/pypi/v/selenium-
 driverless.svg?color=3399EE)](https://pypi.org/project/selenium-driverless/)
 [Documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/#) - Use
 Selenium __without chromedriver__ - Currently passes __Cloudflare__,
 __Bet365__, [Turnstile](https://github.com/kaliiiiiiiiii/Selenium-Driverless/
 tree/master/dev#bypass-turnstile), and others - Multiple tabs simultaneously -
-Multiple Incognito-contexts with individual proxy & cookies - Async (`asyncio`)
-and sync (experimental) support - Proxy-auth support (experimental, [example
-code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/dev/examples/
-proxy_with_auth.py)) - Network-interception - headless supported ### Questions?
-Feel free to join the [Driverless-Community](https://discord.com/invite/
-MzZZjr2ZM3) on **Discord**:) Also, see [dev-branch](https://github.com/
-kaliiiiiiiiii/Selenium-Driverless/tree/dev) for the latest implementations.
-dev-installation (click to expand) ```shell pip uninstall -y selenium-
-driverless pip install https://github.com/kaliiiiiiiiii/Selenium-Driverless/
-archive/refs/heads/dev.zip ``` ### Still getting detected? Feel free to give me
-a feedback! \ You're a company and looking for another solution? Maybe **
-[undetect.io](https://undetect.io/partner/steve)** is smth for you #### Also,
-feel free to _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]### Dependencies * [Python >= 3.7](https://
-www.python.org/downloads/) * [Google-Chrome](https://www.google.de/chrome/
-) installed (Chromium not tested) ### Installing * Install [Google-Chrome]
-(https://www.google.de/chrome/) * ```pip install selenium-driverless``` ###
-Usage ### with asyncio ```python from selenium_driverless import webdriver from
-selenium_driverless.types.by import By import asyncio async def main(): options
-= webdriver.ChromeOptions() async with webdriver.Chrome(options=options) as
-driver: await driver.get('http://nowsecure.nl#relax') await driver.sleep(0.5)
-await driver.wait_for_cdp("Page.domContentEventFired", timeout=15) # wait 10s
-for elem to exist elem = await driver.find_element(By.XPATH, '/html/body/div
-[2]/div/main/p[2]/a', timeout=10) await elem.click(move_to=True) alert = await
-driver.switch_to.alert print(alert.text) await alert.accept() print(await
-driver.title) asyncio.run(main()) ``` ### synchronous asyncified, might be
-buggy ```python from selenium_driverless.sync import webdriver options =
-webdriver.ChromeOptions() with webdriver.Chrome(options=options) as driver:
-driver.get('http://nowsecure.nl#relax') driver.sleep(0.5) driver.wait_for_cdp
+Multiple Incognito-contexts with isolated cookies & local storage - Proxy-auth
+support ([example code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/
+blob/dev/examples/proxy_with_auth.py)) - Network-interception ([documentation]
+(https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Chrome/
+RequestInterception/)) - Single requests ([documentation](https://
+kaliiiiiiiiii.github.io/Selenium-Driverless/api/Target/
+#selenium_driverless.types.target.Target.fetch)) ### Questions? Feel free to
+join the [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on
+**Discord**:) Also, see [dev-branch](https://github.com/kaliiiiiiiiii/Selenium-
+Driverless/tree/dev) for the latest implementations. dev-installation (click to
+expand) ```shell pip uninstall -y selenium-driverless pip install https://
+github.com/kaliiiiiiiiii/Selenium-Driverless/archive/refs/heads/dev.zip ```
+#### Also, feel free to _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]### Dependencies * [Python >= 3.7]
+(https://www.python.org/downloads/) * [Google-Chrome](https://www.google.de/
+chrome/) installed (Chromium not tested) ### Installing * Install [Google-
+Chrome](https://www.google.de/chrome/) * ```pip install selenium-driverless```
+### Usage ### with asyncio ```python from selenium_driverless import webdriver
+from selenium_driverless.types.by import By import asyncio async def main():
+options = webdriver.ChromeOptions() async with webdriver.Chrome
+(options=options) as driver: await driver.get('http://nowsecure.nl#relax',
+wait_load=True) await driver.sleep(0.5) await driver.wait_for_cdp
+("Page.domContentEventFired", timeout=15) # wait 10s for elem to exist elem =
+await driver.find_element(By.XPATH, '/html/body/div[2]/div/main/p[2]/a',
+timeout=10) await elem.click(move_to=True) alert = await driver.switch_to.alert
+print(alert.text) await alert.accept() print(await driver.title) asyncio.run
+(main()) ``` ### synchronous asyncified, might be buggy ```python from
+selenium_driverless.sync import webdriver options = webdriver.ChromeOptions()
+with webdriver.Chrome(options=options) as driver: driver.get('http://
+nowsecure.nl#relax') driver.sleep(0.5) driver.wait_for_cdp
 ("Page.domContentEventFired", timeout=15) title = driver.title url =
 driver.current_url source = driver.page_source print(title) ``` ### custom
 debugger address ```python from selenium_driverless import webdriver options =
 webdriver.ChromeOptions() options.debugger_address = "127.0.0.1:2005" # specify
 if you don't want to run remote # options.add_argument("--remote-debugging-
 port=2005") async with webdriver.Chrome(options=options) as driver: await
-driver.get('http://nowsecure.nl#relax', wait_load=True) ``` ### Network-
-Interception - use CDP events (see [chrome-developer-protocoll](https://
-chromedevtools.github.io/devtools-protocol/) for possible events) **Notes**:
-synchronous might not work properly Example Code (Click to expand) warning:
-network interception with `Fetch.enable` might have issues with cross-domain
-iframes, maximum websocket message size or Font requests.\ You might try using
-[`Network.setRequestInterception](https://chromedevtools.github.io/devtools-
-protocol/tot/Network/#method-setRequestInterception) (officially deprecated) or
-narrowing the pattern ```python import asyncio import base64 import sys import
-time import traceback from cdp_socket.exceptions import CDPError from
-selenium_driverless import webdriver async def on_request(params, global_conn):
-url = params["request"]["url"] _params = {"requestId": params['requestId']} if
-params.get('responseStatusCode') in [301, 302, 303, 307, 308]: # redirected
-request return await global_conn.execute_cdp_cmd("Fetch.continueResponse",
-_params) else: try: body = await global_conn.execute_cdp_cmd
-("Fetch.getResponseBody", _params, timeout=1) except CDPError as e: if e.code
-== -32000 and e.message == 'Can only get response body on requests captured
-after headers received.': print(params, "\n", file=sys.stderr)
-traceback.print_exc() await global_conn.execute_cdp_cmd
-("Fetch.continueResponse", _params) else: raise e else: start =
-time.perf_counter() body_decoded = base64.b64decode(body['body']) # modify body
-here body_modified = base64.b64encode(body_decoded).decode("ascii")
-fulfill_params = {"responseCode": 200, "body": body_modified,
-"responseHeaders": params["responseHeaders"]} fulfill_params.update(_params) if
-params["responseStatusText"] != "": # empty string throws "Invalid http status
-code or phrase" fulfill_params["responsePhrase"] = params["responseStatusText"]
-_time = time.perf_counter() - start if _time > 0.01: print(f"decoding took
-long: {_time} s") await global_conn.execute_cdp_cmd("Fetch.fulfillRequest",
-fulfill_params) print("Mocked response", url) async def main(): async with
-webdriver.Chrome(max_ws_size=2 ** 30) as driver:
-driver.base_target.socket.on_closed.append(lambda code, reason: print(f"chrome
-exited")) global_conn = driver.base_target await global_conn.execute_cdp_cmd
-("Fetch.enable", cmd_args={"patterns": [{"requestStage": "Response",
-"urlPattern": "*"}]}) await global_conn.add_cdp_listener("Fetch.requestPaused",
-lambda data: on_request(data, global_conn)) await driver.get("https://
-nowsecure.nl/#relax", timeout=60, wait_load=False) while True: # time.sleep(10)
-# no. cloudflare would hang await asyncio.sleep(10) asyncio.run(main()) ``` ##
-Multiple tabs simultaneously Note: asyncio is recommended, threading only works
-on independent webdriver.Chrome instances. Example Code (Click to expand)
+driver.get('http://nowsecure.nl#relax', wait_load=True) ``` ## Multiple tabs
+simultaneously Note: asyncio is recommended, threading only works on
+independent webdriver.Chrome instances. Example Code (Click to expand)
 ```python from selenium_driverless.sync import webdriver from
 selenium_driverless.utils.utils import read from selenium_driverless import
 webdriver import asyncio async def target_1_handler(target): await target.get
 ('https://abrahamjuliot.github.io/creepjs/') print(await target.title) async
 def target_2_handler(target): await target.get("about:blank") await
 target.execute_script(script=read("/files/js/show_mousemove.js")) await
 target.pointer.move_to(500, 500, total_time=2) async def main(): options =
@@ -102,15 +87,15 @@
 Object.defineProperty(document, "documentElement", { value: proxy }) """ await
 driver.execute_script(script) src = await driver.execute_script("return
 document.documentElement.outerHTML", unique_context=True) mocked = await
 driver.execute_script("return document.documentElement.outerHTML",
 unique_context=False) print(src, mocked) asyncio.run(main()) ``` ### Pointer
 Interaction see [@master/dev/show_mousemove.py](https://github.com/
 kaliiiiiiiiii/Selenium-Driverless/blob/master/dev/show_mousemove.py) for
-visualization ```python pointer = await driver.current_pointer move_kwargs =
+visualization ```python pointer = driver.current_pointer move_kwargs =
 {"total_time": 0.7, "accel": 2, "smooth_soft": 20} await pointer.move_to(100,
 500) await pointer.click(500, 50, move_kwargs=move_kwargs, move_to=True) ```
 ### Iframes - switch and interact with iframes ```python iframes = await
 driver.find_elements(By.TAG_NAME, "iframe") await asyncio.sleep(0.5)
 iframe_document = await iframes[0].content_document #
 iframe_document.find_elements(...) ``` ### use preferences ```python from
 selenium_driverless import webdriver options = webdriver.ChromeOptions() #
```

### Comparing `selenium_driverless-1.8.0.2/build_upload.md` & `selenium_driverless-1.9/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/dev/README.md` & `selenium_driverless-1.9/dev/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 ## Page Interactions
 
 
 ### element click
-- generated
 
+default
+![img.png](assets/heatmap.png)
 
-![heatmap.png](assets%2Fheatmap.png)
+`bias_a = 0.7`
+![img.png](assets/heatmap_biased.png)
 
 
 ### mouse path
 
 #### generated example
 ![img.png](assets/mousemove_events_gen.png)
 ![img.png](assets/mouse_path_gen.png)
```

### Comparing `selenium_driverless-1.8.0.2/dev/assets/bypass_turnstile.mp4` & `selenium_driverless-1.9/dev/assets/bypass_turnstile.mp4`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/dev/assets/events_mouse.png` & `selenium_driverless-1.9/dev/assets/events_mouse.png`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/dev/assets/events_mousepad.png` & `selenium_driverless-1.9/dev/assets/events_mousepad.png`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/dev/assets/mouse_path_gen.png` & `selenium_driverless-1.9/dev/assets/mouse_path_gen.png`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/dev/assets/mousemove_events_gen.png` & `selenium_driverless-1.9/dev/assets/mousemove_events_gen.png`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/dev/assets/mousemove_events_test_sample_based.png` & `selenium_driverless-1.9/dev/assets/mousemove_events_test_sample_based.png`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/dev/assets/mousemove_events_test_samples_based.png` & `selenium_driverless-1.9/dev/assets/mousemove_events_test_samples_based.png`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/dev/assets/real_mouse_path.png` & `selenium_driverless-1.9/dev/assets/real_mouse_path.png`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/dev/human_like_path.py` & `selenium_driverless-1.9/dev/human_like_path.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_modules/index.html` & `selenium_driverless-1.9/docs/_modules/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -38,20 +38,22 @@
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
-<li class="toctree-l1"><a class="reference internal" href="../classes/By/">By Element Locator</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../classes/Chrome/">webdriver.Chrome</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../classes/ChromeOptions/">ChromeOptions</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../classes/Context/">Context</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../classes/Target/">Target</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../classes/WebELement/">WebElement</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/By/">By Element Locator</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/Chrome/">webdriver.Chrome</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/ChromeOptions/">ChromeOptions</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/Context/">Context</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/Input/">Input</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/RequestInterception/">Request-Interception</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/Target/">Target</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/WebELement/">WebElement</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
     <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
@@ -70,15 +72,18 @@
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <h1>All modules for which code is available</h1>
-<ul><li><a href="selenium_driverless/scripts/switch_to/">selenium_driverless.scripts.switch_to</a></li>
+<ul><li><a href="selenium_driverless/input/pointer/">selenium_driverless.input.pointer</a></li>
+<li><a href="selenium_driverless/scripts/network_interceptor/">selenium_driverless.scripts.network_interceptor</a></li>
+<li><a href="selenium_driverless/scripts/switch_to/">selenium_driverless.scripts.switch_to</a></li>
+<li><a href="selenium_driverless/types/base_target/">selenium_driverless.types.base_target</a></li>
 <li><a href="selenium_driverless/types/by/">selenium_driverless.types.by</a></li>
 <li><a href="selenium_driverless/types/context/">selenium_driverless.types.context</a></li>
 <li><a href="selenium_driverless/types/options/">selenium_driverless.types.options</a></li>
 <li><a href="selenium_driverless/types/target/">selenium_driverless.types.target</a></li>
 <li><a href="selenium_driverless/types/webelement/">selenium_driverless.types.webelement</a></li>
 <li><a href="selenium_driverless/webdriver/">selenium_driverless.webdriver</a></li>
 </ul>
```

#### html2text {}

```diff
@@ -1,20 +1,25 @@
 _S_e_l_e_n_i_u_m_-_D_r_i_v_e_r_l_e_s_s
 [q                   ]
     * _B_y_ _E_l_e_m_e_n_t_ _L_o_c_a_t_o_r
     * _w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
     * _C_h_r_o_m_e_O_p_t_i_o_n_s
     * _C_o_n_t_e_x_t
+    * _I_n_p_u_t
+    * _R_e_q_u_e_s_t_-_I_n_t_e_r_c_e_p_t_i_o_n
     * _T_a_r_g_e_t
     * _W_e_b_E_l_e_m_e_n_t
 _S_e_l_e_n_i_u_m_-_D_r_i_v_e_r_l_e_s_s
     * Overview: module code
 ===============================================================================
 ************ AAllll mmoodduulleess ffoorr wwhhiicchh ccooddee iiss aavvaaiillaabbllee ************
+    * _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r
+    * _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r
     * _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._s_w_i_t_c_h___t_o
+    * _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_a_s_e___t_a_r_g_e_t
     * _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_y
     * _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t
     * _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s
     * _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t
     * _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t
     * _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r
 ===============================================================================
```

### Comparing `selenium_driverless-1.8.0.2/docs/_modules/selenium_driverless/types/options/index.html` & `selenium_driverless-1.9/docs/_modules/selenium_driverless/types/options/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -38,20 +38,22 @@
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
-<li class="toctree-l1"><a class="reference internal" href="../../../../classes/By/">By Element Locator</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../../../classes/Chrome/">webdriver.Chrome</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../../../classes/ChromeOptions/">ChromeOptions</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../../../classes/Context/">Context</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../../../classes/Target/">Target</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../../../classes/WebELement/">WebElement</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../../api/By/">By Element Locator</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../../api/Chrome/">webdriver.Chrome</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../../api/ChromeOptions/">ChromeOptions</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../../api/Context/">Context</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../../api/Input/">Input</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../../api/RequestInterception/">Request-Interception</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../../api/Target/">Target</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../../api/WebELement/">WebElement</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
     <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
@@ -103,15 +105,15 @@
 
 <span class="kn">from</span> <span class="nn">selenium_driverless.utils.utils</span> <span class="kn">import</span> <span class="n">sel_driverless_path</span>
 <span class="kn">from</span> <span class="nn">selenium_driverless.scripts.prefs</span> <span class="kn">import</span> <span class="n">prefs_to_json</span>
 
 
 <span class="c1"># noinspection PyUnreachableCode,PyUnusedLocal</span>
 <div class="viewcode-block" id="Options">
-<a class="viewcode-back" href="../../../../classes/ChromeOptions/#selenium_driverless.types.options.Options">[docs]</a>
+<a class="viewcode-back" href="../../../../api/ChromeOptions/#selenium_driverless.types.options.Options">[docs]</a>
 <span class="k">class</span> <span class="nc">Options</span><span class="p">(</span><span class="n">metaclass</span><span class="o">=</span><span class="n">ABCMeta</span><span class="p">):</span>
 
     <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_single_proxy</span> <span class="o">=</span> <span class="kc">None</span>
         <span class="kn">from</span> <span class="nn">selenium_driverless.utils.utils</span> <span class="kn">import</span> <span class="n">find_chrome_executable</span><span class="p">,</span> <span class="n">IS_POSIX</span>
         <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="fm">__init__</span><span class="p">()</span>
@@ -188,15 +190,15 @@
     <span class="k">def</span> <span class="nf">arguments</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">typing</span><span class="o">.</span><span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        used arguments for the chrome executable</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_arguments</span>
 
 <div class="viewcode-block" id="Options.add_argument">
-<a class="viewcode-back" href="../../../../classes/ChromeOptions/#selenium_driverless.types.options.Options.add_argument">[docs]</a>
+<a class="viewcode-back" href="../../../../api/ChromeOptions/#selenium_driverless.types.options.Options.add_argument">[docs]</a>
     <span class="k">def</span> <span class="nf">add_argument</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">argument</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Adds an argument for launching chrome</span>
 
 <span class="sd">        :param argument: argument to add</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="kn">import</span> <span class="nn">os</span>
         <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">argument</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
@@ -222,15 +224,15 @@
                         <span class="ne">DeprecationWarning</span><span class="p">)</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_arguments</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">argument</span><span class="p">)</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;argument has to be str&quot;</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Options.add_arguments">
-<a class="viewcode-back" href="../../../../classes/ChromeOptions/#selenium_driverless.types.options.Options.add_arguments">[docs]</a>
+<a class="viewcode-back" href="../../../../api/ChromeOptions/#selenium_driverless.types.options.Options.add_arguments">[docs]</a>
     <span class="k">def</span> <span class="nf">add_arguments</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">arguments</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;add multiple arguments</span>
 
 <span class="sd">        :param arguments: arguments to add</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">for</span> <span class="n">arg</span> <span class="ow">in</span> <span class="n">arguments</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span></div>
@@ -238,15 +240,15 @@
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">prefs</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;the preferences as json&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_prefs</span>
 
 <div class="viewcode-block" id="Options.update_pref">
-<a class="viewcode-back" href="../../../../classes/ChromeOptions/#selenium_driverless.types.options.Options.update_pref">[docs]</a>
+<a class="viewcode-back" href="../../../../api/ChromeOptions/#selenium_driverless.types.options.Options.update_pref">[docs]</a>
     <span class="k">def</span> <span class="nf">update_pref</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">pref</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">value</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;update a preference</span>
 
 <span class="sd">        :param pref: name of the preference (&quot;.&quot; dot path)</span>
 <span class="sd">        :param value: the value to set the preference to</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_prefs</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">prefs_to_json</span><span class="p">({</span><span class="n">pref</span><span class="p">:</span> <span class="n">value</span><span class="p">}))</span></div>
@@ -366,15 +368,15 @@
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_env</span>
 
     <span class="nd">@env</span><span class="o">.</span><span class="n">setter</span>
     <span class="k">def</span> <span class="nf">env</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">env</span><span class="p">):</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_env</span> <span class="o">=</span> <span class="n">env</span>
 
 <div class="viewcode-block" id="Options.add_extension">
-<a class="viewcode-back" href="../../../../classes/ChromeOptions/#selenium_driverless.types.options.Options.add_extension">[docs]</a>
+<a class="viewcode-back" href="../../../../api/ChromeOptions/#selenium_driverless.types.options.Options.add_extension">[docs]</a>
     <span class="k">def</span> <span class="nf">add_extension</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Adds an extension to Chrome</span>
 <span class="sd">        The extension can either be a compressed file (zip, crx, etc.) or extracted in a directory</span>
 
 <span class="sd">        :param path: path to the extension</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">extension_to_add</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">abspath</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">expanduser</span><span class="p">(</span><span class="n">path</span><span class="p">))</span>
@@ -408,15 +410,15 @@
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_auto_clean_dirs</span>
 
     <span class="nd">@auto_clean_dirs</span><span class="o">.</span><span class="n">setter</span>
     <span class="k">def</span> <span class="nf">auto_clean_dirs</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">enabled</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_auto_clean_dirs</span> <span class="o">=</span> <span class="n">enabled</span>
 
 <div class="viewcode-block" id="Options.enable_mobile">
-<a class="viewcode-back" href="../../../../classes/ChromeOptions/#selenium_driverless.types.options.Options.enable_mobile">[docs]</a>
+<a class="viewcode-back" href="../../../../api/ChromeOptions/#selenium_driverless.types.options.Options.enable_mobile">[docs]</a>
     <span class="k">def</span> <span class="nf">enable_mobile</span><span class="p">(</span>
             <span class="bp">self</span><span class="p">,</span>
             <span class="n">android_package</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;com.android.chrome&quot;</span><span class="p">,</span>
             <span class="n">android_activity</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
             <span class="n">device_serial</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
     <span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Enables mobile browser use for browsers that support it.</span>
@@ -447,28 +449,28 @@
 <span class="sd">        .. warning::</span>
 <span class="sd">            NotImplemented yet</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">raise</span> <span class="ne">NotImplementedError</span><span class="p">()</span>
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_caps</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;acceptInsecureCerts&quot;</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
 
 <div class="viewcode-block" id="Options.ignore_local_proxy_environment_variables">
-<a class="viewcode-back" href="../../../../classes/ChromeOptions/#selenium_driverless.types.options.Options.ignore_local_proxy_environment_variables">[docs]</a>
+<a class="viewcode-back" href="../../../../api/ChromeOptions/#selenium_driverless.types.options.Options.ignore_local_proxy_environment_variables">[docs]</a>
     <span class="k">def</span> <span class="nf">ignore_local_proxy_environment_variables</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;By calling this you will ignore HTTP_PROXY and HTTPS_PROXY from</span>
 <span class="sd">        being picked up and used.</span>
 
 <span class="sd">        .. warning::</span>
 <span class="sd">            NotImplemented yet</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">raise</span> <span class="ne">NotImplementedError</span><span class="p">()</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_ignore_local_proxy</span> <span class="o">=</span> <span class="kc">True</span></div>
 
 
 <div class="viewcode-block" id="Options.add_experimental_option">
-<a class="viewcode-back" href="../../../../classes/ChromeOptions/#selenium_driverless.types.options.Options.add_experimental_option">[docs]</a>
+<a class="viewcode-back" href="../../../../api/ChromeOptions/#selenium_driverless.types.options.Options.add_experimental_option">[docs]</a>
     <span class="k">def</span> <span class="nf">add_experimental_option</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Adds an experimental option which is passed to chromium.</span>
 
 <span class="sd">        .. warning::</span>
 <span class="sd">            only ``name=&quot;prefs&quot;`` supported.</span>
 <span class="sd">            This method is deprecated and will be removed. Use :obj:`ChromeOptions.update_pref` instead.</span>
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 _S_e_l_e_n_i_u_m_-_D_r_i_v_e_r_l_e_s_s
 [q                   ]
     * _B_y_ _E_l_e_m_e_n_t_ _L_o_c_a_t_o_r
     * _w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
     * _C_h_r_o_m_e_O_p_t_i_o_n_s
     * _C_o_n_t_e_x_t
+    * _I_n_p_u_t
+    * _R_e_q_u_e_s_t_-_I_n_t_e_r_c_e_p_t_i_o_n
     * _T_a_r_g_e_t
     * _W_e_b_E_l_e_m_e_n_t
 _S_e_l_e_n_i_u_m_-_D_r_i_v_e_r_l_e_s_s
     * _M_o_d_u_l_e_ _c_o_d_e
     * selenium_driverless.types.options
 ===============================================================================
 ************ SSoouurrccee ccooddee ffoorr sseelleenniiuumm__ddrriivveerrlleessss..ttyyppeess..ooppttiioonnss ************
```

### Comparing `selenium_driverless-1.8.0.2/docs/_modules/selenium_driverless/webdriver/index.html` & `selenium_driverless-1.9/docs/_modules/selenium_driverless/webdriver/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,22 @@
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
-<li class="toctree-l1"><a class="reference internal" href="../../../classes/By/">By Element Locator</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../../classes/Chrome/">webdriver.Chrome</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../../classes/ChromeOptions/">ChromeOptions</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../../classes/Context/">Context</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../../classes/Target/">Target</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../../classes/WebELement/">WebElement</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../api/By/">By Element Locator</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../api/Chrome/">webdriver.Chrome</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../api/ChromeOptions/">ChromeOptions</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../api/Context/">Context</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../api/Input/">Input</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../api/RequestInterception/">Request-Interception</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../api/Target/">Target</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../../api/WebELement/">WebElement</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
     <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
@@ -132,15 +134,15 @@
 <span class="kn">from</span> <span class="nn">cdp_socket.utils.conn</span> <span class="kn">import</span> <span class="n">get_json</span>
 <span class="kn">from</span> <span class="nn">selenium_driverless.types.options</span> <span class="kn">import</span> <span class="n">Options</span> <span class="k">as</span> <span class="n">ChromeOptions</span>
 <span class="kn">from</span> <span class="nn">selenium_driverless.types</span> <span class="kn">import</span> <span class="n">JSEvalException</span>
 <span class="kn">from</span> <span class="nn">selenium_driverless</span> <span class="kn">import</span> <span class="n">EXC_HANDLER</span>
 
 
 <div class="viewcode-block" id="Chrome">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome">[docs]</a>
 <span class="k">class</span> <span class="nc">Chrome</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Control the chromium based browsers without any driver.&quot;&quot;&quot;</span>
 
     <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
             <span class="bp">self</span><span class="p">,</span>
             <span class="n">options</span><span class="p">:</span> <span class="n">ChromeOptions</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
             <span class="n">timeout</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">30</span><span class="p">,</span>
@@ -366,16 +368,14 @@
                     <span class="k">def</span> <span class="nf">remove_context</span><span class="p">():</span>
                         <span class="k">if</span> <span class="n">_id</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_contexts</span><span class="p">:</span>
                             <span class="k">del</span> <span class="bp">self</span><span class="o">.</span><span class="n">_contexts</span><span class="p">[</span><span class="n">_id</span><span class="p">]</span>
                         <span class="bp">self</span><span class="o">.</span><span class="n">_base_context</span> <span class="o">=</span> <span class="kc">None</span>
 
                     <span class="c1"># noinspection PyProtectedMember</span>
                     <span class="n">context</span><span class="o">.</span><span class="n">_closed_callbacks</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">remove_context</span><span class="p">)</span>
-                    <span class="bp">self</span><span class="o">.</span><span class="n">base_target</span><span class="o">.</span><span class="n">socket</span><span class="o">.</span><span class="n">on_closed</span><span class="o">.</span><span class="n">append</span><span class="p">(</span>
-                        <span class="k">lambda</span> <span class="n">code</span><span class="p">,</span> <span class="n">reason</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">quit</span><span class="p">(</span><span class="n">clean_dirs</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_options</span><span class="o">.</span><span class="n">auto_clean_dirs</span><span class="p">))</span>
                     <span class="bp">self</span><span class="o">.</span><span class="n">_current_context</span> <span class="o">=</span> <span class="n">context</span>
                     <span class="bp">self</span><span class="o">.</span><span class="n">_base_context</span> <span class="o">=</span> <span class="n">context</span>
                     <span class="bp">self</span><span class="o">.</span><span class="n">_contexts</span><span class="p">[</span><span class="n">_id</span><span class="p">]</span> <span class="o">=</span> <span class="n">context</span>
                     <span class="k">break</span>
             <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_cdp_cmd</span><span class="p">(</span><span class="s2">&quot;Emulation.setFocusEmulationEnabled&quot;</span><span class="p">,</span> <span class="p">{</span><span class="s2">&quot;enabled&quot;</span><span class="p">:</span> <span class="kc">True</span><span class="p">})</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_options</span><span class="o">.</span><span class="n">single_proxy</span><span class="p">:</span>
                 <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">set_single_proxy</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_options</span><span class="o">.</span><span class="n">single_proxy</span><span class="p">)</span>
@@ -424,15 +424,15 @@
                         <span class="n">context</span> <span class="o">=</span> <span class="k">await</span> <span class="n">Context</span><span class="p">(</span><span class="n">base_target</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_current_target</span><span class="p">,</span> <span class="n">context_id</span><span class="o">=</span><span class="n">_id</span><span class="p">,</span>
                                                 <span class="n">loop</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_loop</span><span class="p">,</span> <span class="n">max_ws_size</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_max_ws_size</span><span class="p">,</span> <span class="n">driver</span><span class="o">=</span><span class="bp">self</span><span class="p">)</span>
                 <span class="n">contexts</span><span class="p">[</span><span class="n">_id</span><span class="p">]</span> <span class="o">=</span> <span class="n">context</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_contexts</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">contexts</span><span class="p">)</span>
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_contexts</span>
 
 <div class="viewcode-block" id="Chrome.new_context">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.new_context">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.new_context">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">new_context</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">proxy_bypass_list</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">proxy_server</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
                           <span class="n">universal_access_origins</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;about:blank&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Context</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        creates a new (incognito) context</span>
 
 <span class="sd">        :param url: the url the first tab will start at. &quot;about:blank&quot; by default</span>
 <span class="sd">        :param universal_access_origins: An optional list of origins to grant unlimited cross-origin access to. Parts of the URL other than those constituting origin are ignored</span>
@@ -514,15 +514,15 @@
                     <span class="bp">self</span><span class="o">.</span><span class="n">_auth_interception_enabled</span> <span class="o">=</span> <span class="kc">True</span>
                     <span class="bp">self</span><span class="o">.</span><span class="n">_mv3_extension</span> <span class="o">=</span> <span class="n">mv3_target</span>
                     <span class="k">return</span> <span class="n">context</span>
         <span class="k">return</span> <span class="n">context</span></div>
 
 
 <div class="viewcode-block" id="Chrome.get_targets">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get_targets">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_targets">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_targets</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span>
                           <span class="n">_type</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Literal</span><span class="p">[</span><span class="s2">&quot;page&quot;</span><span class="p">,</span> <span class="s2">&quot;background_page&quot;</span><span class="p">,</span> <span class="s2">&quot;service_worker&quot;</span><span class="p">,</span> <span class="s2">&quot;browser&quot;</span><span class="p">,</span> <span class="s2">&quot;other&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
                           <span class="n">context_id</span><span class="p">:</span> <span class="nb">str</span> <span class="ow">or</span> <span class="kc">None</span> <span class="o">=</span> <span class="s2">&quot;self&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">typing</span><span class="o">.</span><span class="n">Dict</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="n">TargetInfo</span><span class="p">]:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        get all targets within the current context</span>
 <span class="sd">        :param _type: filter by target type</span>
 <span class="sd">        :param context_id: if ``None``, this function returns all targets for all contexts.</span>
@@ -572,15 +572,15 @@
                                 <span class="sa">r</span><span class="s2">&quot;chrome-extension://(.*)/&quot;</span>
                                 <span class="sa">r</span><span class="s2">&quot;driverless_background_mv3_243ffdd55e32a012b4f253b2879af978\.js&quot;</span><span class="p">,</span>
                                 <span class="n">target</span><span class="o">.</span><span class="n">url</span><span class="p">):</span>
                             <span class="n">extension_target</span> <span class="o">=</span> <span class="n">target</span><span class="o">.</span><span class="n">Target</span>
                             <span class="k">break</span>
                 <span class="k">if</span> <span class="ow">not</span> <span class="n">extension_target</span><span class="p">:</span>
                     <span class="k">if</span> <span class="p">(</span><span class="n">time</span><span class="o">.</span><span class="n">perf_counter</span><span class="p">()</span> <span class="o">-</span> <span class="n">start</span><span class="p">)</span> <span class="o">&gt;</span> <span class="n">timeout</span><span class="p">:</span>
-                        <span class="k">raise</span> <span class="ne">TimeoutError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Couldn&#39;t find mv3 extension within </span><span class="si">{</span><span class="n">timeout</span><span class="si">}</span><span class="s2"> seconds&quot;</span><span class="p">)</span>
+                        <span class="k">raise</span> <span class="n">asyncio</span><span class="o">.</span><span class="n">TimeoutError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Couldn&#39;t find mv3 extension within </span><span class="si">{</span><span class="n">timeout</span><span class="si">}</span><span class="s2"> seconds&quot;</span><span class="p">)</span>
             <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
                 <span class="k">try</span><span class="p">:</span>
                     <span class="c1"># fix WebRTC leak</span>
                     <span class="k">await</span> <span class="n">extension_target</span><span class="o">.</span><span class="n">execute_script</span><span class="p">(</span>
                         <span class="s2">&quot;chrome.privacy.network.webRTCIPHandlingPolicy.set(arguments[0])&quot;</span><span class="p">,</span>
                         <span class="p">{</span><span class="s2">&quot;value&quot;</span><span class="p">:</span> <span class="s2">&quot;disable_non_proxied_udp&quot;</span><span class="p">},</span> <span class="n">timeout</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span>
                 <span class="k">except</span> <span class="p">(</span><span class="n">asyncio</span><span class="o">.</span><span class="n">TimeoutError</span><span class="p">,</span> <span class="ne">TimeoutError</span><span class="p">):</span>
@@ -593,15 +593,15 @@
                         <span class="k">await</span> <span class="n">asyncio</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.2</span><span class="p">)</span>
                 <span class="k">else</span><span class="p">:</span>
                     <span class="k">break</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_mv3_extension</span> <span class="o">=</span> <span class="n">extension_target</span>
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_mv3_extension</span>
 
 <div class="viewcode-block" id="Chrome.ensure_extensions_incognito_allowed">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.ensure_extensions_incognito_allowed">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.ensure_extensions_incognito_allowed">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">ensure_extensions_incognito_allowed</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        ensure that all installed Chrome-extensions are allowed in incognito context.</span>
 
 <span class="sd">        .. warning::</span>
 <span class="sd">            Generally, the extension decides whether to use the ``split``, ``spanning`` or ``not_allowed`` configuration.</span>
 <span class="sd">            For changing this behaviour, you&#39;ll have to modify the ``manifest.json`` file within the compressed extension or directory.</span>
@@ -647,15 +647,15 @@
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">downloads_dir</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;the current downloads directory for the current context&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">base_target</span><span class="o">.</span><span class="n">downloads_dir_for_context</span><span class="p">(</span><span class="n">context_id</span><span class="o">=</span><span class="s2">&quot;DEFAULT&quot;</span><span class="p">)</span>
 
 <div class="viewcode-block" id="Chrome.set_download_behaviour">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.set_download_behaviour">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.set_download_behaviour">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">set_download_behaviour</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span><span class="n">behaviour</span><span class="p">:</span><span class="n">typing</span><span class="o">.</span><span class="n">Literal</span><span class="p">[</span><span class="s2">&quot;deny&quot;</span><span class="p">,</span> <span class="s2">&quot;allow&quot;</span><span class="p">,</span> <span class="s2">&quot;allowAndName&quot;</span><span class="p">,</span> <span class="s2">&quot;default&quot;</span><span class="p">],</span>
                                      <span class="n">path</span><span class="p">:</span><span class="nb">str</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;set the download behaviour</span>
 
 <span class="sd">        :param behaviour: the behaviour to set the downloading to</span>
 <span class="sd">        :param path: the path to the default download directory</span>
 
@@ -678,55 +678,55 @@
 
     <span class="nd">@property</span>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">_isolated_context_id</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="c1"># noinspection PyProtectedMember</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_context</span><span class="o">.</span><span class="n">_isolated_context_id</span>
 
 <div class="viewcode-block" id="Chrome.get_target">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get_target">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_target">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_target</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">timeout</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">2</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Target</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        get a Target by TargetId for advanced usage of the CDP protocol</span>
 <span class="sd">        :param target_id:</span>
 <span class="sd">        :param timeout: timeout in seconds for connecting to the target if it&#39;s not tracked already</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="n">target_id</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_context</span><span class="o">.</span><span class="n">get_target</span><span class="p">(</span><span class="n">target_id</span><span class="o">=</span><span class="n">target_id</span><span class="p">,</span> <span class="n">timeout</span><span class="o">=</span><span class="n">timeout</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.get_target_for_iframe">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get_target_for_iframe">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_target_for_iframe">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_target_for_iframe</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">iframe</span><span class="p">:</span> <span class="n">WebElement</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Target</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        get the Target for a specific iframe</span>
 
 <span class="sd">        .. warning::</span>
 <span class="sd">            only cross-iframes have a Target due to `OOPIF &lt;https://www.chromium.org/developers/design-documents/oop-iframes/&gt;`__. See `site-isolation &lt;https://www.chromium.org/Home/chromium-security/site-isolation/&gt;`__</span>
 <span class="sd">            For a general solution, have a look at ``WebElement.content_document`` instead</span>
 
 <span class="sd">        :param iframe: the iframe to get the Target for</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">get_target_for_iframe</span><span class="p">(</span><span class="n">iframe</span><span class="o">=</span><span class="n">iframe</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.get_targets_for_iframes">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get_targets_for_iframes">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_targets_for_iframes">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_targets_for_iframes</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">iframes</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">List</span><span class="p">[</span><span class="n">WebElement</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">typing</span><span class="o">.</span><span class="n">List</span><span class="p">[</span><span class="n">Target</span><span class="p">]:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        returns a list of targets for iframes</span>
 <span class="sd">        see ``webdriver.Chrome.get_target_for_iframe`` for more information</span>
 
 <span class="sd">        :param iframes: the iframe to get the targets for</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">get_targets_for_iframes</span><span class="p">(</span><span class="n">iframes</span><span class="o">=</span><span class="n">iframes</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.wait_download">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.wait_download">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.wait_download">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">wait_download</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">timeout</span><span class="p">:</span><span class="nb">float</span> <span class="ow">or</span> <span class="kc">None</span><span class="o">=</span><span class="mi">30</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        wait for a download on the current tab</span>
 
 <span class="sd">        returns something like</span>
 
 <span class="sd">        .. code-block:: python</span>
@@ -747,15 +747,15 @@
 <span class="sd">            downloads from iframes not supported yet</span>
 
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">wait_download</span><span class="p">(</span><span class="n">timeout</span><span class="o">=</span><span class="n">timeout</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.get">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">referrer</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wait_load</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">timeout</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">30</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">typing</span><span class="o">.</span><span class="n">Union</span><span class="p">[</span><span class="kc">None</span><span class="p">,</span> <span class="nb">dict</span><span class="p">]:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Loads a web page in the current Target</span>
 
 <span class="sd">        :param url: the url to load.</span>
 <span class="sd">        :param referrer: the referrer to load the page with</span>
 <span class="sd">        :param wait_load: whether to wait for the webpage to load</span>
 <span class="sd">        :param timeout: the maximum time in seconds for waiting on load</span>
@@ -768,23 +768,32 @@
     <span class="nd">@property</span>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">title</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;**async** the title of the current target&quot;&quot;&quot;</span>
         <span class="n">target</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target_info</span>
         <span class="k">return</span> <span class="n">target</span><span class="o">.</span><span class="n">title</span>
 
     <span class="nd">@property</span>
-    <span class="k">async</span> <span class="k">def</span> <span class="nf">current_pointer</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Pointer</span><span class="p">:</span>
-<span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
-<span class="sd">        **async** the Pointer of the current Target</span>
-<span class="sd">        &quot;&quot;&quot;</span>
+    <span class="k">def</span> <span class="nf">current_pointer</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Pointer</span><span class="p">:</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;the :class:`Pointer &lt;selenium_driverless.input.pointer.Pointer&gt;` for this target&quot;&quot;&quot;</span>
         <span class="n">target</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span>
         <span class="k">return</span> <span class="n">target</span><span class="o">.</span><span class="n">pointer</span>
 
+<div class="viewcode-block" id="Chrome.send_keys">
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.send_keys">[docs]</a>
+    <span class="k">async</span> <span class="k">def</span> <span class="nf">send_keys</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">text</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
+<span class="sd">        send text &amp; keys to the current target</span>
+
+<span class="sd">        :param text: the text to send</span>
+<span class="sd">        &quot;&quot;&quot;</span>
+        <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">send_keys</span><span class="p">(</span><span class="n">text</span><span class="p">)</span></div>
+
+
 <div class="viewcode-block" id="Chrome.execute_raw_script">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.execute_raw_script">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.execute_raw_script">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">execute_raw_script</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">script</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="n">await_res</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
                                  <span class="n">serialization</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Literal</span><span class="p">[</span><span class="s2">&quot;deep&quot;</span><span class="p">,</span> <span class="s2">&quot;json&quot;</span><span class="p">,</span> <span class="s2">&quot;idOnly&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;deep&quot;</span><span class="p">,</span>
                                  <span class="n">max_depth</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">timeout</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">2</span><span class="p">,</span> <span class="n">execution_context_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
                                  <span class="n">unique_context</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;executes a JavaScript on ``GlobalThis`` such as</span>
 
 <span class="sd">        .. code-block:: js</span>
@@ -807,15 +816,15 @@
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">execute_raw_script</span><span class="p">(</span><span class="n">script</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="n">await_res</span><span class="o">=</span><span class="n">await_res</span><span class="p">,</span>
                                                             <span class="n">serialization</span><span class="o">=</span><span class="n">serialization</span><span class="p">,</span> <span class="n">max_depth</span><span class="o">=</span><span class="n">max_depth</span><span class="p">,</span>
                                                             <span class="n">timeout</span><span class="o">=</span><span class="n">timeout</span><span class="p">,</span> <span class="n">execution_context_id</span><span class="o">=</span><span class="n">execution_context_id</span><span class="p">,</span>
                                                             <span class="n">unique_context</span><span class="o">=</span><span class="n">unique_context</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.execute_script">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.execute_script">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.execute_script">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">execute_script</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">script</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="n">max_depth</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">2</span><span class="p">,</span> <span class="n">serialization</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
                              <span class="n">timeout</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
                              <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">execution_context_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
                              <span class="n">unique_context</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;executes JavaScript synchronously on ``GlobalThis`` such as</span>
 
 <span class="sd">        .. code-block:: js</span>
@@ -829,15 +838,15 @@
         <span class="n">target</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_target</span><span class="p">(</span><span class="n">target_id</span><span class="p">)</span>
         <span class="k">return</span> <span class="k">await</span> <span class="n">target</span><span class="o">.</span><span class="n">execute_script</span><span class="p">(</span><span class="n">script</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="n">max_depth</span><span class="o">=</span><span class="n">max_depth</span><span class="p">,</span> <span class="n">serialization</span><span class="o">=</span><span class="n">serialization</span><span class="p">,</span>
                                            <span class="n">timeout</span><span class="o">=</span><span class="n">timeout</span><span class="p">,</span> <span class="n">execution_context_id</span><span class="o">=</span><span class="n">execution_context_id</span><span class="p">,</span>
                                            <span class="n">unique_context</span><span class="o">=</span><span class="n">unique_context</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.execute_async_script">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.execute_async_script">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.execute_async_script">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">execute_async_script</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">script</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="n">max_depth</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">2</span><span class="p">,</span>
                                    <span class="n">serialization</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">timeout</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">2</span><span class="p">,</span>
                                    <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">execution_context_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
                                    <span class="n">unique_context</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;executes JavaScript asynchronously on ``GlobalThis`` such as</span>
 
 <span class="sd">        .. warning::</span>
@@ -856,15 +865,15 @@
         <span class="k">return</span> <span class="k">await</span> <span class="n">target</span><span class="o">.</span><span class="n">execute_async_script</span><span class="p">(</span><span class="n">script</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="n">max_depth</span><span class="o">=</span><span class="n">max_depth</span><span class="p">,</span> <span class="n">serialization</span><span class="o">=</span><span class="n">serialization</span><span class="p">,</span>
                                                  <span class="n">timeout</span><span class="o">=</span><span class="n">timeout</span><span class="p">,</span>
                                                  <span class="n">execution_context_id</span><span class="o">=</span><span class="n">execution_context_id</span><span class="p">,</span>
                                                  <span class="n">unique_context</span><span class="o">=</span><span class="n">unique_context</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.eval_async">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.eval_async">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.eval_async">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">eval_async</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">script</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="n">max_depth</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">2</span><span class="p">,</span>
                          <span class="n">serialization</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">timeout</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">2</span><span class="p">,</span>
                          <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">execution_context_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
                          <span class="n">unique_context</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;executes JavaScript asynchronously on ``GlobalThis`` such as</span>
 
 <span class="sd">        .. code-block:: js</span>
@@ -896,32 +905,32 @@
     <span class="k">async</span> <span class="k">def</span> <span class="nf">page_source</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;**async** html of the current page.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">target</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span>
         <span class="k">return</span> <span class="k">await</span> <span class="n">target</span><span class="o">.</span><span class="n">page_source</span>
 
 <div class="viewcode-block" id="Chrome.close">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.close">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.close">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">close</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">timeout</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">2</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Closes the current target (only works for tabs).</span>
 <span class="sd">        :param timeout: timeout in seconds for the tab to close</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">close</span><span class="p">(</span><span class="n">timeout</span><span class="o">=</span><span class="n">timeout</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.focus">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.focus">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.focus">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">focus</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;focuses the current target (only works for tabs)</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">focus</span><span class="p">()</span></div>
 
 
 <div class="viewcode-block" id="Chrome.quit">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.quit">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.quit">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">quit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">timeout</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">30</span><span class="p">,</span> <span class="n">clean_dirs</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Closes Chrome</span>
 <span class="sd">        :param timeout: the maximum time waiting for chrome to quit correctly</span>
 <span class="sd">        :param clean_dirs: whether to clean out the user-data-dir directory</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="kn">from</span> <span class="nn">selenium_driverless</span> <span class="kn">import</span> <span class="n">EXC_HANDLER</span>
 
@@ -1054,15 +1063,15 @@
         <span class="n">targets</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">targets</span>
         <span class="k">for</span> <span class="n">info</span> <span class="ow">in</span> <span class="nb">list</span><span class="p">(</span><span class="n">targets</span><span class="o">.</span><span class="n">values</span><span class="p">()):</span>
             <span class="k">if</span> <span class="n">info</span><span class="o">.</span><span class="n">type</span> <span class="o">==</span> <span class="s2">&quot;page&quot;</span><span class="p">:</span>
                 <span class="n">tabs</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">info</span><span class="p">)</span>
         <span class="k">return</span> <span class="n">tabs</span>
 
 <div class="viewcode-block" id="Chrome.new_window">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.new_window">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.new_window">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">new_window</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">type_hint</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Literal</span><span class="p">[</span><span class="s2">&quot;tab&quot;</span><span class="p">,</span> <span class="s2">&quot;window&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;tab&quot;</span><span class="p">,</span> <span class="n">url</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">,</span>
                          <span class="n">activate</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Target</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Creates a new window or tab in the current context</span>
 
 <span class="sd">        :param type_hint: whether to create a tab or window</span>
 <span class="sd">        :param url: the url which the new window should start on. Defaults to about:blank</span>
 <span class="sd">        :param activate: whether to explicitly activate/focus the window</span>
@@ -1071,61 +1080,61 @@
 
 <span class="sd">            new_target = driver.new_window(&#39;tab&#39;)</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_context</span><span class="o">.</span><span class="n">new_window</span><span class="p">(</span><span class="n">type_hint</span><span class="o">=</span><span class="n">type_hint</span><span class="p">,</span> <span class="n">url</span><span class="o">=</span><span class="n">url</span><span class="p">,</span> <span class="n">activate</span><span class="o">=</span><span class="n">activate</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.set_window_state">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.set_window_state">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.set_window_state">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">set_window_state</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">state</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Literal</span><span class="p">[</span><span class="s2">&quot;normal&quot;</span><span class="p">,</span> <span class="s2">&quot;minimized&quot;</span><span class="p">,</span> <span class="s2">&quot;maximized&quot;</span><span class="p">,</span> <span class="s2">&quot;fullscreen&quot;</span><span class="p">]):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;sets the window state on the window the current Target belongs to</span>
 <span class="sd">        :param state: the state to set</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">window_id</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_window_id</span>
         <span class="n">bounds</span> <span class="o">=</span> <span class="p">{</span><span class="s2">&quot;windowState&quot;</span><span class="p">:</span> <span class="n">state</span><span class="p">}</span>
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_cdp_cmd</span><span class="p">(</span><span class="s2">&quot;Browser.setWindowBounds&quot;</span><span class="p">,</span> <span class="p">{</span><span class="s2">&quot;bounds&quot;</span><span class="p">:</span> <span class="n">bounds</span><span class="p">,</span> <span class="s2">&quot;windowId&quot;</span><span class="p">:</span> <span class="n">window_id</span><span class="p">})</span></div>
 
 
 <div class="viewcode-block" id="Chrome.normalize_window">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.normalize_window">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.normalize_window">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">normalize_window</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Normalizes the window position and size on the window the current Target belongs to</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">set_window_state</span><span class="p">(</span><span class="s2">&quot;normal&quot;</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.maximize_window">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.maximize_window">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.maximize_window">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">maximize_window</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Maximizes the window the current Target belongs to&quot;&quot;&quot;</span>
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">set_window_state</span><span class="p">(</span><span class="s2">&quot;maximized&quot;</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.fullscreen_window">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.fullscreen_window">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.fullscreen_window">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">fullscreen_window</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;enters fullscreen on the window the current Target belongs to&quot;&quot;&quot;</span>
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">set_window_state</span><span class="p">(</span><span class="s2">&quot;fullscreen&quot;</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.minimize_window">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.minimize_window">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.minimize_window">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">minimize_window</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;minimizes the window the current Target belongs to.</span>
 
 <span class="sd">        .. warning::</span>
 
 <span class="sd">            Minimizing isn&#39;t recommended as it can throttle some functionalities in chrome.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">set_window_state</span><span class="p">(</span><span class="s2">&quot;maximized&quot;</span><span class="p">)</span></div>
 
 
     <span class="c1"># noinspection PyUnusedLocal</span>
 <div class="viewcode-block" id="Chrome.print_page">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.print_page">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.print_page">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">print_page</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Prints the page (current target =&gt; tab) to PDF</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">target</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span>
         <span class="k">return</span> <span class="k">await</span> <span class="n">target</span><span class="o">.</span><span class="n">print_page</span><span class="p">()</span></div>
 
 
@@ -1133,192 +1142,192 @@
     <span class="k">def</span> <span class="nf">switch_to</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">SwitchTo</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;SwitchTo handle</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_context</span><span class="o">.</span><span class="n">switch_to</span>
 
     <span class="c1"># Navigation</span>
 <div class="viewcode-block" id="Chrome.back">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.back">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.back">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">back</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Goes one step backward in the browser history on the current target (has to be a tab).</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">back</span><span class="p">()</span></div>
 
 
 <div class="viewcode-block" id="Chrome.forward">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.forward">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.forward">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">forward</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Goes one step forward in the browser history on the current target (has to be a tab).</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">forward</span><span class="p">()</span></div>
 
 
 <div class="viewcode-block" id="Chrome.refresh">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.refresh">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.refresh">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">refresh</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Refreshes the current tab (target).</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">refresh</span><span class="p">()</span></div>
 
 
     <span class="c1"># Options</span>
 <div class="viewcode-block" id="Chrome.get_cookies">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get_cookies">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_cookies">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_cookies</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">List</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;list of cookies for the current tab</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">get_cookies</span><span class="p">()</span></div>
 
 
 <div class="viewcode-block" id="Chrome.get_cookie">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get_cookie">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_cookie">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_cookie</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">typing</span><span class="o">.</span><span class="n">Optional</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Dict</span><span class="p">]:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Get a single cookie by name. Returns the cookie if found, None if</span>
 <span class="sd">        not.</span>
 
 <span class="sd">        :param name: name of the cookie</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">get_cookie</span><span class="p">(</span><span class="n">name</span><span class="o">=</span><span class="n">name</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.delete_cookie">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.delete_cookie">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.delete_cookie">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">delete_cookie</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">domain</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
                             <span class="n">path</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Deletes a single cookie with the given name in the current tab.</span>
 
 <span class="sd">        :param name: name of the cookie to delete</span>
 <span class="sd">        :param url: url of the cookie</span>
 <span class="sd">        :param domain: domain of the cookie</span>
 <span class="sd">        :param path: path of the cookie</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">delete_cookie</span><span class="p">(</span><span class="n">name</span><span class="o">=</span><span class="n">name</span><span class="p">,</span> <span class="n">url</span><span class="o">=</span><span class="n">url</span><span class="p">,</span> <span class="n">domain</span><span class="o">=</span><span class="n">domain</span><span class="p">,</span> <span class="n">path</span><span class="o">=</span><span class="n">path</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.delete_all_cookies">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.delete_all_cookies">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.delete_all_cookies">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">delete_all_cookies</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Delete all cookies in the current (incognito-) context.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">delete_all_cookies</span><span class="p">()</span></div>
 
 
     <span class="c1"># noinspection GrazieInspection</span>
 <div class="viewcode-block" id="Chrome.add_cookie">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.add_cookie">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.add_cookie">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">add_cookie</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">cookie_dict</span><span class="p">:</span> <span class="nb">dict</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Adds a cookie in the current (incognito-) context</span>
 
 <span class="sd">        :param cookie_dict: see `Network.CookieParam &lt;https://chromedevtools.github.io/devtools-protocol/tot/Network/#type-CookieParam&gt;`__</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">add_cookie</span><span class="p">(</span><span class="n">cookie_dict</span><span class="o">=</span><span class="n">cookie_dict</span><span class="p">)</span></div>
 
 
     <span class="c1"># Timeouts</span>
 <div class="viewcode-block" id="Chrome.sleep">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.sleep">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.sleep">[docs]</a>
     <span class="nd">@staticmethod</span>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">sleep</span><span class="p">(</span><span class="n">time_to_wait</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
         <span class="c1"># noinspection GrazieInspection</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;sleep</span>
 <span class="sd">                .. note::</span>
 <span class="sd">                    use this one instead of time.sleep in the sync version.</span>
 
 <span class="sd">                :param time_to_wait: time in seconds to sleep</span>
 <span class="sd">                &quot;&quot;&quot;</span>
         <span class="k">await</span> <span class="n">asyncio</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="n">time_to_wait</span><span class="p">)</span></div>
 
 
     <span class="c1"># noinspection PyUnusedLocal</span>
 <div class="viewcode-block" id="Chrome.find_element">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.find_element">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.find_element">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">find_element</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">by</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">timeout</span><span class="p">:</span> <span class="nb">int</span> <span class="ow">or</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">WebElement</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;find an element in the current target</span>
 
 <span class="sd">        :param by: one of the locators at :func:`By &lt;selenium_driverless.types.by.By&gt;`</span>
 <span class="sd">        :param value: the actual query to find the element by</span>
 <span class="sd">        :param timeout: how long to wait for the element to exist</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">find_element</span><span class="p">(</span><span class="n">by</span><span class="o">=</span><span class="n">by</span><span class="p">,</span> <span class="n">value</span><span class="o">=</span><span class="n">value</span><span class="p">,</span> <span class="n">timeout</span><span class="o">=</span><span class="n">timeout</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.find_elements">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.find_elements">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.find_elements">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">find_elements</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">by</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">typing</span><span class="o">.</span><span class="n">List</span><span class="p">[</span><span class="n">WebElement</span><span class="p">]:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;find multiple elements in the current target</span>
 
 <span class="sd">        :param by: one of the locators at :func:`By &lt;selenium_driverless.types.by.By&gt;`</span>
 <span class="sd">        :param value: the actual query to find the elements by</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">find_elements</span><span class="p">(</span><span class="n">by</span><span class="o">=</span><span class="n">by</span><span class="p">,</span> <span class="n">value</span><span class="o">=</span><span class="n">value</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.search_elements">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.search_elements">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.search_elements">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">search_elements</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">typing</span><span class="o">.</span><span class="n">List</span><span class="p">[</span><span class="n">WebElement</span><span class="p">]:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        find elements similarly to how &quot;CTRL+F&quot; in the DevTools Console works</span>
 
 <span class="sd">        :param query: Plain text to find elements with</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">search_elements</span><span class="p">(</span><span class="n">query</span><span class="o">=</span><span class="n">query</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.get_screenshot_as_file">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get_screenshot_as_file">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_screenshot_as_file">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_screenshot_as_file</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">filename</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Saves a screenshot of the current tab to a PNG image file.</span>
 <span class="sd">        :param filename: The path you wish to save your screenshot to. should end with a `.png` extension.</span>
 
 <span class="sd">        .. code-block:: python</span>
 
 <span class="sd">            driver.get_screenshot_as_file(&#39;screenshots/test.png&#39;)</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">get_screenshot_as_file</span><span class="p">(</span><span class="n">filename</span><span class="o">=</span><span class="n">filename</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.save_screenshot">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.save_screenshot">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.save_screenshot">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">save_screenshot</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">filename</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;alias to :func: `driver.get_screenshot_as_file &lt;selenium_driverless.webdriver.Chrome.get_screenshot_as_file&gt;`&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_screenshot_as_file</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.get_screenshot_as_png">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get_screenshot_as_png">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_screenshot_as_png">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_screenshot_as_png</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bytes</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Gets the screenshot of the current tab as a binary data.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">get_screenshot_as_png</span><span class="p">()</span></div>
 
 
 <div class="viewcode-block" id="Chrome.get_screenshot_as_base64">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get_screenshot_as_base64">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_screenshot_as_base64">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_screenshot_as_base64</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Gets the screenshot of the current tab as a base64 encoded string</span>
 <span class="sd">        which is useful in embedded images in HTML.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">get_screenshot_as_base64</span><span class="p">()</span></div>
 
 
     <span class="c1"># noinspection PyPep8Naming</span>
 <div class="viewcode-block" id="Chrome.set_window_size">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.set_window_size">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.set_window_size">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">set_window_size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">width</span><span class="p">:</span> <span class="nb">int</span><span class="p">,</span> <span class="n">height</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Sets the width and height of the window, the current tab is within (unless ``windowHandle`` specified)</span>
 
 <span class="sd">        :param width: the width in pixels to set the window to</span>
 <span class="sd">        :param height: the height in pixels to set the window to</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">set_window_rect</span><span class="p">(</span><span class="n">width</span><span class="o">=</span><span class="nb">int</span><span class="p">(</span><span class="n">width</span><span class="p">),</span> <span class="n">height</span><span class="o">=</span><span class="nb">int</span><span class="p">(</span><span class="n">height</span><span class="p">))</span></div>
 
 
     <span class="c1"># noinspection PyPep8Naming</span>
 <div class="viewcode-block" id="Chrome.get_window_size">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get_window_size">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_window_size">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_window_size</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Gets the width and height of the current window.</span>
 
 <span class="sd">        returns something like:</span>
 <span class="sd">        .. code-block: json</span>
 
 <span class="sd">            {&quot;width&quot;:1280, &quot;height&quot;:720}</span>
@@ -1329,42 +1338,42 @@
             <span class="n">size</span> <span class="o">=</span> <span class="n">size</span><span class="p">[</span><span class="s2">&quot;value&quot;</span><span class="p">]</span>
 
         <span class="k">return</span> <span class="p">{</span><span class="n">k</span><span class="p">:</span> <span class="n">size</span><span class="p">[</span><span class="n">k</span><span class="p">]</span> <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="p">(</span><span class="s2">&quot;width&quot;</span><span class="p">,</span> <span class="s2">&quot;height&quot;</span><span class="p">)}</span></div>
 
 
     <span class="c1"># noinspection PyPep8Naming</span>
 <div class="viewcode-block" id="Chrome.set_window_position">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.set_window_position">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.set_window_position">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">set_window_position</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">x</span><span class="p">:</span> <span class="nb">int</span><span class="p">,</span> <span class="n">y</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Sets the x,y position of the window, the current tab is in.</span>
 
 <span class="sd">        :param x: the x-coordinate in pixels to set the window position</span>
 <span class="sd">        :param y: the y-coordinate in pixels to set the window position</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">set_window_rect</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="nb">int</span><span class="p">(</span><span class="n">x</span><span class="p">),</span> <span class="n">y</span><span class="o">=</span><span class="nb">int</span><span class="p">(</span><span class="n">y</span><span class="p">))</span></div>
 
 
     <span class="c1"># noinspection PyPep8Naming</span>
 <div class="viewcode-block" id="Chrome.get_window_position">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get_window_position">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_window_position">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_window_position</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Gets the x,y position of the window, the current tab is in.</span>
 
 <span class="sd">        returns something like:</span>
 <span class="sd">        .. code-block: json</span>
 
 <span class="sd">            {&quot;x&quot;:0, &quot;y&quot;:0}</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">position</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_window_rect</span><span class="p">()</span>
 
         <span class="k">return</span> <span class="p">{</span><span class="n">k</span><span class="p">:</span> <span class="n">position</span><span class="p">[</span><span class="n">k</span><span class="p">]</span> <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="p">(</span><span class="s2">&quot;x&quot;</span><span class="p">,</span> <span class="s2">&quot;y&quot;</span><span class="p">)}</span></div>
 
 
 <div class="viewcode-block" id="Chrome.get_window_rect">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get_window_rect">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_window_rect">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_window_rect</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Gets the x, y, with and height coordinates of the window, the current tab is in.</span>
 
 <span class="sd">        returns something like:</span>
 <span class="sd">        .. code-block: json</span>
 
 <span class="sd">            {&quot;x&quot;:0, &quot;y&quot;:0,</span>
@@ -1382,15 +1391,15 @@
         <span class="k">del</span> <span class="n">json</span><span class="p">[</span><span class="s2">&quot;left&quot;</span><span class="p">]</span>
         <span class="n">json</span><span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">json</span><span class="p">[</span><span class="s2">&quot;top&quot;</span><span class="p">]</span>
         <span class="k">del</span> <span class="n">json</span><span class="p">[</span><span class="s2">&quot;top&quot;</span><span class="p">]</span>
         <span class="k">return</span> <span class="n">json</span></div>
 
 
 <div class="viewcode-block" id="Chrome.set_window_rect">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.set_window_rect">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.set_window_rect">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">set_window_rect</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">x</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">width</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">height</span><span class="o">=</span><span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Sets the x, y, width and height coordinates of the window the current target is in.</span>
 
 <span class="sd">        :param x: the x-coordinate in pixels to set the window position</span>
 <span class="sd">        :param y: the y-coordinate in pixels to set the window position</span>
 <span class="sd">        :param width: the width in pixels to set the window to</span>
 <span class="sd">        :param height: the height in pixels to set the window to</span>
@@ -1411,15 +1420,15 @@
         <span class="n">bounds</span><span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">bounds</span><span class="p">[</span><span class="s2">&quot;top&quot;</span><span class="p">]</span>
         <span class="k">del</span> <span class="n">bounds</span><span class="p">[</span><span class="s2">&quot;top&quot;</span><span class="p">]</span>
 
         <span class="k">return</span> <span class="n">bounds</span></div>
 
 
 <div class="viewcode-block" id="Chrome.get_network_conditions">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get_network_conditions">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_network_conditions">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_network_conditions</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Gets Chromium network emulation settings.</span>
 
 <span class="sd">        returns a dict like:</span>
 
 <span class="sd">        .. code-block:: python</span>
 
@@ -1427,15 +1436,15 @@
 <span class="sd">            &quot;offline&quot;: False}</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">get_network_conditions</span><span class="p">()</span></div>
 
 
     <span class="c1"># noinspection SpellCheckingInspection</span>
 <div class="viewcode-block" id="Chrome.set_network_conditions">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.set_network_conditions">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.set_network_conditions">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">set_network_conditions</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">offline</span><span class="p">:</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">latency</span><span class="p">:</span> <span class="nb">int</span><span class="p">,</span> <span class="n">download_throughput</span><span class="p">:</span> <span class="nb">int</span><span class="p">,</span>
                                      <span class="n">upload_throughput</span><span class="p">:</span> <span class="nb">int</span><span class="p">,</span>
                                      <span class="n">connection_type</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Literal</span><span class="p">[</span>
                                          <span class="s2">&quot;none&quot;</span><span class="p">,</span> <span class="s2">&quot;cellular2g&quot;</span><span class="p">,</span> <span class="s2">&quot;cellular3g&quot;</span><span class="p">,</span> <span class="s2">&quot;cellular4g&quot;</span><span class="p">,</span> <span class="s2">&quot;bluetooth&quot;</span><span class="p">,</span> <span class="s2">&quot;ethernet&quot;</span><span class="p">,</span> <span class="s2">&quot;wifi&quot;</span><span class="p">,</span> <span class="s2">&quot;wimax&quot;</span><span class="p">,</span> <span class="s2">&quot;other&quot;</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
         <span class="c1"># noinspection GrazieInspection</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Sets Chromium network emulation settings.</span>
 
@@ -1452,22 +1461,22 @@
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">set_network_conditions</span><span class="p">(</span><span class="n">offline</span><span class="o">=</span><span class="n">offline</span><span class="p">,</span> <span class="n">latency</span><span class="o">=</span><span class="n">latency</span><span class="p">,</span>
                                                                 <span class="n">download_throughput</span><span class="o">=</span><span class="n">download_throughput</span><span class="p">,</span>
                                                                 <span class="n">upload_throughput</span><span class="o">=</span><span class="n">upload_throughput</span><span class="p">,</span>
                                                                 <span class="n">connection_type</span><span class="o">=</span><span class="n">connection_type</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.delete_network_conditions">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.delete_network_conditions">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.delete_network_conditions">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">delete_network_conditions</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Resets Chromium network emulation settings.&quot;&quot;&quot;</span>
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">delete_network_conditions</span><span class="p">()</span></div>
 
 
 <div class="viewcode-block" id="Chrome.set_permissions">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.set_permissions">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.set_permissions">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">set_permissions</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Literal</span><span class="p">[</span><span class="s2">&quot;granted&quot;</span><span class="p">,</span> <span class="s2">&quot;denied&quot;</span><span class="p">,</span> <span class="s2">&quot;prompt&quot;</span><span class="p">],</span>
                               <span class="n">origin</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Sets Applicable Permission</span>
 
 <span class="sd">        :param name: The item to set the permission on.</span>
 <span class="sd">        :param value: The value to set on the item</span>
 <span class="sd">        :param origin: the origin the permission for. Applies to any origin if not set</span>
@@ -1482,15 +1491,15 @@
         <span class="n">args</span> <span class="o">=</span> <span class="p">{</span><span class="s2">&quot;permission&quot;</span><span class="p">:</span> <span class="p">{</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">},</span> <span class="s2">&quot;setting&quot;</span><span class="p">:</span> <span class="n">value</span><span class="p">}</span>
         <span class="k">if</span> <span class="n">origin</span><span class="p">:</span>
             <span class="n">args</span><span class="p">[</span><span class="s2">&quot;origin&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">origin</span>
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_cdp_cmd</span><span class="p">(</span><span class="s2">&quot;Browser.setPermission&quot;</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.set_proxy">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.set_proxy">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.set_proxy">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">set_proxy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">proxy_config</span><span class="p">):</span>
         <span class="c1"># noinspection GrazieInspection</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot; set a proxy dynamically</span>
 
 <span class="sd">        Example parameters:</span>
 
 <span class="sd">        .. code-block:: python</span>
@@ -1528,15 +1537,15 @@
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">extension</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">mv3_extension</span>
         <span class="k">await</span> <span class="n">extension</span><span class="o">.</span><span class="n">eval_async</span><span class="p">(</span><span class="s2">&quot;await chrome.proxy.settings.set(arguments[0])&quot;</span><span class="p">,</span>
                                    <span class="p">{</span><span class="s2">&quot;value&quot;</span><span class="p">:</span> <span class="n">proxy_config</span><span class="p">,</span> <span class="s2">&quot;scope&quot;</span><span class="p">:</span> <span class="s1">&#39;regular&#39;</span><span class="p">})</span></div>
 
 
 <div class="viewcode-block" id="Chrome.set_single_proxy">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.set_single_proxy">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.set_single_proxy">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">set_single_proxy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">proxy</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">bypass_list</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Set a single proxy dynamically to be applied in all contexts.</span>
 
 <span class="sd">        .. code-block:: python</span>
 
 <span class="sd">            &quot;http://user1:passwrd1@example.proxy.com:5001/&quot;</span>
@@ -1593,15 +1602,15 @@
         <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">set_proxy</span><span class="p">(</span><span class="n">proxy_config</span><span class="p">)</span>
         <span class="k">if</span> <span class="n">creds</span><span class="p">:</span>
             <span class="n">user</span><span class="p">,</span> <span class="n">passw</span> <span class="o">=</span> <span class="n">creds</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;:&quot;</span><span class="p">)</span>
             <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">set_auth</span><span class="p">(</span><span class="n">user</span><span class="p">,</span> <span class="n">passw</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">host</span><span class="si">}</span><span class="s2">:</span><span class="si">{</span><span class="n">port</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.clear_proxy">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.clear_proxy">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.clear_proxy">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">clear_proxy</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Clear the applied proxy (=&gt; use no proxy at all) in all contexts.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">extension</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">mv3_extension</span>
         <span class="k">await</span> <span class="n">extension</span><span class="o">.</span><span class="n">eval_async</span><span class="p">(</span><span class="s2">&quot;&quot;&quot;</span>
 <span class="s2">            await chrome.proxy.settings.set(</span>
@@ -1626,15 +1635,15 @@
 <span class="s2">                        &quot;&quot;&quot;</span>
             <span class="n">mv3_target</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">mv3_extension</span>
             <span class="k">await</span> <span class="n">mv3_target</span><span class="o">.</span><span class="n">execute_script</span><span class="p">(</span><span class="n">script</span><span class="p">,</span> <span class="n">timeout</span><span class="o">=</span><span class="n">timeout</span><span class="p">)</span>
             <span class="k">if</span> <span class="n">set_flag</span><span class="p">:</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_auth_interception_enabled</span> <span class="o">=</span> <span class="kc">True</span>
 
 <div class="viewcode-block" id="Chrome.set_auth">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.set_auth">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.set_auth">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">set_auth</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">username</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">password</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">host_with_port</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        Set authentication dynamically to be applied in all contexts.</span>
 
 <span class="sd">        .. code-block:: python</span>
 
 <span class="sd">            driver.set_auth(&quot;user1&quot;,&quot;passwrd1&quot;, &quot;example.com:5001&quot;)</span>
@@ -1660,152 +1669,161 @@
             <span class="p">}</span>
         <span class="p">}</span>
         <span class="k">await</span> <span class="n">mv3_target</span><span class="o">.</span><span class="n">execute_script</span><span class="p">(</span><span class="s2">&quot;globalThis.authCreds[arguments[1]] = arguments[0]&quot;</span><span class="p">,</span> <span class="n">arg</span><span class="p">,</span> <span class="n">host_with_port</span><span class="p">)</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_auth</span><span class="p">[</span><span class="n">host_with_port</span><span class="p">]</span> <span class="o">=</span> <span class="n">arg</span></div>
 
 
 <div class="viewcode-block" id="Chrome.clear_auth">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.clear_auth">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.clear_auth">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">clear_auth</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        clear the applied auth from :func:`webdriver.Chrome.set_auth &lt;selenium_driverless.webdriver.Chrome.set_auth&gt;`</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="c1"># provide auth</span>
         <span class="n">mv3_target</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">mv3_extension</span>
         <span class="n">script</span> <span class="o">=</span> <span class="s2">&quot;chrome.webRequest.onAuthRequired.removeListener(globalThis.onAuth);&quot;</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_auth</span> <span class="o">=</span> <span class="p">{}</span>
         <span class="k">await</span> <span class="n">mv3_target</span><span class="o">.</span><span class="n">execute_script</span><span class="p">(</span><span class="n">script</span><span class="p">)</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_auth_interception_enabled</span> <span class="o">=</span> <span class="kc">False</span></div>
 
 
 <div class="viewcode-block" id="Chrome.wait_for_cdp">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.wait_for_cdp">[docs]</a>
-    <span class="k">async</span> <span class="k">def</span> <span class="nf">wait_for_cdp</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">event</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">timeout</span><span class="p">:</span> <span class="nb">float</span> <span class="ow">or</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.wait_for_cdp">[docs]</a>
+    <span class="k">async</span> <span class="k">def</span> <span class="nf">wait_for_cdp</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">event</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">timeout</span><span class="p">:</span> <span class="nb">float</span> <span class="ow">or</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
-<span class="sd">        wait for a CDP-event (current target)</span>
-
-<span class="sd">        :param event: an even such as ``Page.windowOpen``</span>
-<span class="sd">        :param timeout: timeout to wait for the event</span>
+<span class="sd">        wait for an event on the current target</span>
+<span class="sd">        see :func:`Target.wait_for_cdp &lt;selenium_driverless.types.target.Target.wait_for_cdp&gt;` for reference</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">wait_for_cdp</span><span class="p">(</span><span class="n">event</span><span class="o">=</span><span class="n">event</span><span class="p">,</span> <span class="n">timeout</span><span class="o">=</span><span class="n">timeout</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.add_cdp_listener">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.add_cdp_listener">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.add_cdp_listener">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">add_cdp_listener</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">event</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">callback</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Callable</span><span class="p">[[</span><span class="nb">dict</span><span class="p">],</span> <span class="nb">any</span><span class="p">]):</span>
-<span class="w">        </span><span class="sd">&quot;&quot;&quot;add a listener on a CDP event (current target)</span>
-
-<span class="sd">        :param event: the name of the event</span>
-<span class="sd">        :param callback: the callback on the event</span>
-<span class="sd">            has to accept one parameter (event data as json)</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
+<span class="sd">        add a listener for a CDP event on the current target</span>
+<span class="sd">        see :func:`Target.add_cdp_listener &lt;selenium_driverless.types.target.Target.add_cdp_listener&gt;` for reference</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">add_cdp_listener</span><span class="p">(</span><span class="n">event</span><span class="o">=</span><span class="n">event</span><span class="p">,</span> <span class="n">callback</span><span class="o">=</span><span class="n">callback</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.remove_cdp_listener">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.remove_cdp_listener">[docs]</a>
-    <span class="k">async</span> <span class="k">def</span> <span class="nf">remove_cdp_listener</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">event</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">callback</span><span class="p">:</span> <span class="nb">callable</span><span class="p">):</span>
-<span class="w">        </span><span class="sd">&quot;&quot;&quot;remove a listener for CDP-event (current target)</span>
-
-<span class="sd">        :param event: the name of the event</span>
-<span class="sd">        :param callback: the callback function to remove</span>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.remove_cdp_listener">[docs]</a>
+    <span class="k">async</span> <span class="k">def</span> <span class="nf">remove_cdp_listener</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">event</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">callback</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Callable</span><span class="p">[[</span><span class="nb">dict</span><span class="p">],</span> <span class="nb">any</span><span class="p">]):</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
+<span class="sd">        remove a listener for a CDP event on the current target</span>
+<span class="sd">        see :func:`Target.remove_cdp_listener &lt;selenium_driverless.types.target.Target.remove_cdp_listener&gt;` for reference</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="c1"># todo: documentation from here on</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">remove_cdp_listener</span><span class="p">(</span><span class="n">event</span><span class="o">=</span><span class="n">event</span><span class="p">,</span> <span class="n">callback</span><span class="o">=</span><span class="n">callback</span><span class="p">)</span></div>
 
 
-    <span class="k">async</span> <span class="k">def</span> <span class="nf">get_cdp_event_iter</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">event</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+<div class="viewcode-block" id="Chrome.get_cdp_event_iter">
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_cdp_event_iter">[docs]</a>
+    <span class="k">async</span> <span class="k">def</span> <span class="nf">get_cdp_event_iter</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">event</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">typing</span><span class="o">.</span><span class="n">AsyncIterable</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
+<span class="sd">        iterate over CDP events on the current target</span>
+<span class="sd">        see :func:`Target.get_cdp_event_iter &lt;selenium_driverless.types.target.Target.get_cdp_event_iter&gt;` for reference</span>
+<span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">target</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_target</span><span class="p">(</span><span class="n">target_id</span><span class="o">=</span><span class="n">target_id</span><span class="p">)</span>
-        <span class="k">return</span> <span class="k">await</span> <span class="n">target</span><span class="o">.</span><span class="n">get_cdp_event_iter</span><span class="p">(</span><span class="n">event</span><span class="o">=</span><span class="n">event</span><span class="p">)</span>
+        <span class="k">return</span> <span class="k">await</span> <span class="n">target</span><span class="o">.</span><span class="n">get_cdp_event_iter</span><span class="p">(</span><span class="n">event</span><span class="o">=</span><span class="n">event</span><span class="p">)</span></div>
+
 
 <div class="viewcode-block" id="Chrome.execute_cdp_cmd">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.execute_cdp_cmd">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.execute_cdp_cmd">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">execute_cdp_cmd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">cmd</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">cmd_args</span><span class="p">:</span> <span class="nb">dict</span> <span class="ow">or</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
                               <span class="n">timeout</span><span class="p">:</span> <span class="nb">float</span> <span class="ow">or</span> <span class="kc">None</span> <span class="o">=</span> <span class="mi">10</span><span class="p">,</span> <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
-<span class="w">        </span><span class="sd">&quot;&quot;&quot;Execute Chrome Devtools Protocol command and get returned result The</span>
-<span class="sd">        command and command args should follow chrome devtools protocol</span>
-<span class="sd">        domains/commands, refer to link</span>
-<span class="sd">        https://chromedevtools.github.io/devtools-protocol/</span>
-
-<span class="sd">        :Args:</span>
-<span class="sd">         - cmd: A str, command name</span>
-<span class="sd">         - cmd_args: A dict, command args. empty dict {} if there is no command args</span>
-<span class="sd">        :Usage:</span>
-<span class="sd">            ::</span>
-
-<span class="sd">                target.execute_cdp_cmd(&#39;Network.getResponseBody&#39;, {&#39;requestId&#39;: requestId})</span>
-<span class="sd">        :Returns:</span>
-<span class="sd">            A dict, empty dict {} if there is no result to return.</span>
-<span class="sd">            For example to getResponseBody:</span>
-<span class="sd">            {&#39;base64Encoded&#39;: False, &#39;body&#39;: &#39;response body string&#39;}</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;Execute Chrome Devtools Protocol command on the current target</span>
+<span class="sd">        executes it on :class:`Target.execute_cdp_cmd &lt;selenium_driverless.types.base_target.BaseTarget&gt;`</span>
+<span class="sd">        if ``message:&#39;Not allowed&#39;`` received</span>
+<span class="sd">        see :func:`Target.execute_cdp_cmd &lt;selenium_driverless.types.target.Target.execute_cdp_cmd&gt;` for reference</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_context</span><span class="o">.</span><span class="n">execute_cdp_cmd</span><span class="p">(</span><span class="n">cmd</span><span class="o">=</span><span class="n">cmd</span><span class="p">,</span> <span class="n">cmd_args</span><span class="o">=</span><span class="n">cmd_args</span><span class="p">,</span> <span class="n">timeout</span><span class="o">=</span><span class="n">timeout</span><span class="p">,</span>
                                                           <span class="n">target_id</span><span class="o">=</span><span class="n">target_id</span><span class="p">)</span></div>
 
 
+<div class="viewcode-block" id="Chrome.fetch">
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.fetch">[docs]</a>
+    <span class="k">async</span> <span class="k">def</span> <span class="nf">fetch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
+<span class="sd">        executes a JS ``fetch`` request within the current target</span>
+<span class="sd">        see :func:`Target.fetch &lt;selenium_driverless.types.target.Target.fetch&gt;` for reference</span>
+<span class="sd">        &quot;&quot;&quot;</span>
+        <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">fetch</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span></div>
+
+
+<div class="viewcode-block" id="Chrome.xhr">
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.xhr">[docs]</a>
+    <span class="k">async</span> <span class="k">def</span> <span class="nf">xhr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
+<span class="sd">        executes a JS ``XMLHttpRequest`` request within the current target</span>
+<span class="sd">        see :func:`Target.fetch &lt;selenium_driverless.types.target.Target.fetch&gt;` for reference</span>
+<span class="sd">        &quot;&quot;&quot;</span>
+        <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">xhr</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span></div>
+
+
     <span class="c1"># noinspection PyTypeChecker</span>
 <div class="viewcode-block" id="Chrome.get_sinks">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get_sinks">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_sinks">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_sinks</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        :Returns: A list of sinks available for Cast.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">target</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_target</span><span class="p">(</span><span class="n">target_id</span><span class="o">=</span><span class="n">target_id</span><span class="p">)</span>
         <span class="k">return</span> <span class="k">await</span> <span class="n">target</span><span class="o">.</span><span class="n">get_sinks</span><span class="p">()</span></div>
 
 
 <div class="viewcode-block" id="Chrome.get_issue_message">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.get_issue_message">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_issue_message">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_issue_message</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">        :Returns: An error message when there is any issue in a Cast session.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">target</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_target</span><span class="p">(</span><span class="n">target_id</span><span class="o">=</span><span class="n">target_id</span><span class="p">)</span>
         <span class="k">return</span> <span class="k">await</span> <span class="n">target</span><span class="o">.</span><span class="n">get_issue_message</span><span class="p">()</span></div>
 
 
 <div class="viewcode-block" id="Chrome.set_sink_to_use">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.set_sink_to_use">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.set_sink_to_use">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">set_sink_to_use</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sink_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Sets a specific sink, using its name, as a Cast session receiver</span>
 <span class="sd">        target.</span>
 
 <span class="sd">        :Args:</span>
 <span class="sd">         - sink_name: Name of the sink to use as the target.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">target</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_target</span><span class="p">(</span><span class="n">target_id</span><span class="o">=</span><span class="n">target_id</span><span class="p">)</span>
         <span class="k">return</span> <span class="k">await</span> <span class="n">target</span><span class="o">.</span><span class="n">set_sink_to_use</span><span class="p">(</span><span class="n">sink_name</span><span class="o">=</span><span class="n">sink_name</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.start_desktop_mirroring">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.start_desktop_mirroring">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.start_desktop_mirroring">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">start_desktop_mirroring</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sink_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Starts a desktop mirroring session on a specific receiver target.</span>
 
 <span class="sd">        :Args:</span>
 <span class="sd">         - sink_name: Name of the sink to use as the target.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">target</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_target</span><span class="p">(</span><span class="n">target_id</span><span class="o">=</span><span class="n">target_id</span><span class="p">)</span>
         <span class="k">return</span> <span class="k">await</span> <span class="n">target</span><span class="o">.</span><span class="n">start_desktop_mirroring</span><span class="p">(</span><span class="n">sink_name</span><span class="o">=</span><span class="n">sink_name</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.start_tab_mirroring">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.start_tab_mirroring">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.start_tab_mirroring">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">start_tab_mirroring</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sink_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Starts a tab mirroring session on a specific receiver target.</span>
 
 <span class="sd">        :Args:</span>
 <span class="sd">         - sink_name: Name of the sink to use as the target.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">target</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_target</span><span class="p">(</span><span class="n">target_id</span><span class="o">=</span><span class="n">target_id</span><span class="p">)</span>
         <span class="k">return</span> <span class="k">await</span> <span class="n">target</span><span class="o">.</span><span class="n">start_tab_mirroring</span><span class="p">(</span><span class="n">sink_name</span><span class="o">=</span><span class="n">sink_name</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.stop_casting">
-<a class="viewcode-back" href="../../../classes/Chrome/#selenium_driverless.webdriver.Chrome.stop_casting">[docs]</a>
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.stop_casting">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">stop_casting</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sink_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Stops the existing Cast session on a specific receiver target.</span>
 
 <span class="sd">        :Args:</span>
 <span class="sd">         - sink_name: Name of the sink to stop the Cast session.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">target</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_target</span><span class="p">(</span><span class="n">target_id</span><span class="o">=</span><span class="n">target_id</span><span class="p">)</span>
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 _S_e_l_e_n_i_u_m_-_D_r_i_v_e_r_l_e_s_s
 [q                   ]
     * _B_y_ _E_l_e_m_e_n_t_ _L_o_c_a_t_o_r
     * _w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
     * _C_h_r_o_m_e_O_p_t_i_o_n_s
     * _C_o_n_t_e_x_t
+    * _I_n_p_u_t
+    * _R_e_q_u_e_s_t_-_I_n_t_e_r_c_e_p_t_i_o_n
     * _T_a_r_g_e_t
     * _W_e_b_E_l_e_m_e_n_t
 _S_e_l_e_n_i_u_m_-_D_r_i_v_e_r_l_e_s_s
     * _M_o_d_u_l_e_ _c_o_d_e
     * selenium_driverless.webdriver
 ===============================================================================
 ************ SSoouurrccee ccooddee ffoorr sseelleenniiuumm__ddrriivveerrlleessss..wweebbddrriivveerr ************
@@ -327,17 +329,14 @@
                     def remove_context():
                         if _id in self._contexts:
                             del self._contexts[_id]
                         self._base_context = None
 
                     # noinspection PyProtectedMember
                     context._closed_callbacks.append(remove_context)
-                    self.base_target.socket.on_closed.append(
-                        lambda code, reason: self.quit
-(clean_dirs=self._options.auto_clean_dirs))
                     self._current_context = context
                     self._base_context = context
                     self._contexts[_id] = context
                     break
             await self.execute_cdp_cmd("Emulation.setFocusEmulationEnabled",
 {"enabled": True})
             if self._options.single_proxy:
@@ -565,16 +564,16 @@
 
 r"driverless_background_mv3_243ffdd55e32a012b4f253b2879af978\.js",
                                 target.url):
                             extension_target = target.Target
                             break
                 if not extension_target:
                     if (time.perf_counter() - start) > timeout:
-                        raise TimeoutError(f"Couldn't find mv3 extension within
-{timeout} seconds")
+                        raise asyncio.TimeoutError(f"Couldn't find mv3
+extension within {timeout} seconds")
             while True:
                 try:
                     # fix WebRTC leak
                     await extension_target.execute_script(
                         "chrome.privacy.network.webRTCIPHandlingPolicy.set
 (arguments[0])",
                         {"value": "disable_non_proxied_udp"}, timeout=2)
@@ -796,23 +795,34 @@
     @property
     async def title(self) -> str:
         """**async** the title of the current target"""
         target = await self.current_target_info
         return target.title
 
     @property
-    async def current_pointer(self) -> Pointer:
-        """
-        **async** the Pointer of the current Target
-        """
+    def current_pointer(self) -> Pointer:
+        """the :class:`Pointer <selenium_driverless.input.pointer.Pointer>` for
+this target"""
         target = self.current_target
         return target.pointer
 
 
 _[_d_o_c_s_]
+    async def send_keys(self, text: str):
+        """
+        send text & keys to the current target
+
+        :param text: the text to send
+        """
+        await self.current_target.send_keys(text)
+
+
+
+
+_[_d_o_c_s_]
     async def execute_raw_script(self, script: str, *args, await_res: bool =
 False,
                                  serialization: typing.Literal["deep", "json",
 "idOnly"] = "deep",
                                  max_depth: int = None, timeout: int = 2,
 execution_context_id: str = None,
                                  unique_context: bool = False):
@@ -1850,89 +1860,110 @@
         await mv3_target.execute_script(script)
         self._auth_interception_enabled = False
 
 
 
 
 _[_d_o_c_s_]
-    async def wait_for_cdp(self, event: str, timeout: float or None = None):
+    async def wait_for_cdp(self, event: str, timeout: float or None = None) -
+> dict:
         """
-        wait for a CDP-event (current target)
-
-        :param event: an even such as ``Page.windowOpen``
-        :param timeout: timeout to wait for the event
+        wait for an event on the current target
+        see :func:`Target.wait_for_cdp
+<selenium_driverless.types.target.Target.wait_for_cdp>` for reference
         """
         return await self.current_target.wait_for_cdp(event=event,
 timeout=timeout)
 
 
 
 
 _[_d_o_c_s_]
     async def add_cdp_listener(self, event: str, callback: typing.Callable[
 [dict], any]):
-        """add a listener on a CDP event (current target)
-
-        :param event: the name of the event
-        :param callback: the callback on the event
-            has to accept one parameter (event data as json)
+        """
+        add a listener for a CDP event on the current target
+        see :func:`Target.add_cdp_listener
+<selenium_driverless.types.target.Target.add_cdp_listener>` for reference
         """
         return await self.current_target.add_cdp_listener(event=event,
 callback=callback)
 
 
 
 
 _[_d_o_c_s_]
-    async def remove_cdp_listener(self, event: str, callback: callable):
-        """remove a listener for CDP-event (current target)
-
-        :param event: the name of the event
-        :param callback: the callback function to remove
+    async def remove_cdp_listener(self, event: str, callback: typing.Callable[
+[dict], any]):
+        """
+        remove a listener for a CDP event on the current target
+        see :func:`Target.remove_cdp_listener
+<selenium_driverless.types.target.Target.remove_cdp_listener>` for reference
         """
-        # todo: documentation from here on
         return await self.current_target.remove_cdp_listener(event=event,
 callback=callback)
 
 
 
-    async def get_cdp_event_iter(self, event: str, target_id: str = None):
+
+_[_d_o_c_s_]
+    async def get_cdp_event_iter(self, event: str, target_id: str = None) -
+> typing.AsyncIterable[dict]:
+        """
+        iterate over CDP events on the current target
+        see :func:`Target.get_cdp_event_iter
+<selenium_driverless.types.target.Target.get_cdp_event_iter>` for reference
+        """
         target = await self.get_target(target_id=target_id)
         return await target.get_cdp_event_iter(event=event)
 
 
+
+
 _[_d_o_c_s_]
     async def execute_cdp_cmd(self, cmd: str, cmd_args: dict or None = None,
                               timeout: float or None = 10, target_id: str =
 None) -> dict:
-        """Execute Chrome Devtools Protocol command and get returned result The
-        command and command args should follow chrome devtools protocol
-        domains/commands, refer to link
-        https://chromedevtools.github.io/devtools-protocol/
-
-        :Args:
-         - cmd: A str, command name
-         - cmd_args: A dict, command args. empty dict {} if there is no command
-args
-        :Usage:
-            ::
-
-                target.execute_cdp_cmd('Network.getResponseBody', {'requestId':
-requestId})
-        :Returns:
-            A dict, empty dict {} if there is no result to return.
-            For example to getResponseBody:
-            {'base64Encoded': False, 'body': 'response body string'}
+        """Execute Chrome Devtools Protocol command on the current target
+        executes it on :class:`Target.execute_cdp_cmd
+<selenium_driverless.types.base_target.BaseTarget>`
+        if ``message:'Not allowed'`` received
+        see :func:`Target.execute_cdp_cmd
+<selenium_driverless.types.target.Target.execute_cdp_cmd>` for reference
         """
         return await self.current_context.execute_cdp_cmd(cmd=cmd,
 cmd_args=cmd_args, timeout=timeout,
                                                           target_id=target_id)
 
 
 
+
+_[_d_o_c_s_]
+    async def fetch(self, *args, **kwargs) -> dict:
+        """
+        executes a JS ``fetch`` request within the current target
+        see :func:`Target.fetch
+<selenium_driverless.types.target.Target.fetch>` for reference
+        """
+        return await self.current_target.fetch(*args, **kwargs)
+
+
+
+
+_[_d_o_c_s_]
+    async def xhr(self, *args, **kwargs) -> dict:
+        """
+        executes a JS ``XMLHttpRequest`` request within the current target
+        see :func:`Target.fetch
+<selenium_driverless.types.target.Target.fetch>` for reference
+        """
+        return await self.current_target.xhr(*args, **kwargs)
+
+
+
     # noinspection PyTypeChecker
 
 _[_d_o_c_s_]
     async def get_sinks(self, target_id: str = None) -> list:
         """
         :Returns: A list of sinks available for Cast.
         """
```

### Comparing `selenium_driverless-1.8.0.2/docs/_static/_sphinx_javascript_frameworks_compat.js` & `selenium_driverless-1.9/docs/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/basic.css` & `selenium_driverless-1.9/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/badge_only.css` & `selenium_driverless-1.9/docs/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff` & `selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff2` & `selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff` & `selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff2` & `selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/fontawesome-webfont.eot` & `selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/fontawesome-webfont.svg` & `selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/fontawesome-webfont.ttf` & `selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/fontawesome-webfont.woff` & `selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/fontawesome-webfont.woff2` & `selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-bold-italic.woff` & `selenium_driverless-1.9/docs/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-bold-italic.woff2` & `selenium_driverless-1.9/docs/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-bold.woff` & `selenium_driverless-1.9/docs/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-bold.woff2` & `selenium_driverless-1.9/docs/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-normal-italic.woff` & `selenium_driverless-1.9/docs/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-normal-italic.woff2` & `selenium_driverless-1.9/docs/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-normal.woff` & `selenium_driverless-1.9/docs/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/fonts/lato-normal.woff2` & `selenium_driverless-1.9/docs/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/css/theme.css` & `selenium_driverless-1.9/docs/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/doctools.js` & `selenium_driverless-1.9/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/jquery.js` & `selenium_driverless-1.9/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/js/badge_only.js` & `selenium_driverless-1.9/docs/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/js/html5shiv-printshiv.min.js` & `selenium_driverless-1.9/docs/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/js/html5shiv.min.js` & `selenium_driverless-1.9/docs/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/js/theme.js` & `selenium_driverless-1.9/docs/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/language_data.js` & `selenium_driverless-1.9/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/pygments.css` & `selenium_driverless-1.9/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/searchtools.js` & `selenium_driverless-1.9/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/_static/sphinx_highlight.js` & `selenium_driverless-1.9/docs/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/docs/search/index.html` & `selenium_driverless-1.9/docs/search/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -41,20 +41,22 @@
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
-<li class="toctree-l1"><a class="reference internal" href="../classes/By/">By Element Locator</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../classes/Chrome/">webdriver.Chrome</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../classes/ChromeOptions/">ChromeOptions</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../classes/Context/">Context</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../classes/Target/">Target</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../classes/WebELement/">WebElement</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/By/">By Element Locator</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/Chrome/">webdriver.Chrome</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/ChromeOptions/">ChromeOptions</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/Context/">Context</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/Input/">Input</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/RequestInterception/">Request-Interception</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/Target/">Target</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../api/WebELement/">WebElement</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
     <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 _S_e_l_e_n_i_u_m_-_D_r_i_v_e_r_l_e_s_s
 [q                   ]
     * _B_y_ _E_l_e_m_e_n_t_ _L_o_c_a_t_o_r
     * _w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
     * _C_h_r_o_m_e_O_p_t_i_o_n_s
     * _C_o_n_t_e_x_t
+    * _I_n_p_u_t
+    * _R_e_q_u_e_s_t_-_I_n_t_e_r_c_e_p_t_i_o_n
     * _T_a_r_g_e_t
     * _W_e_b_E_l_e_m_e_n_t
 _S_e_l_e_n_i_u_m_-_D_r_i_v_e_r_l_e_s_s
     * Search
 ===============================================================================
 Please activate JavaScript to enable the search functionality.
 ===============================================================================
```

### Comparing `selenium_driverless-1.8.0.2/docs_source/conf.py` & `selenium_driverless-1.9/docs_source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 import sys
 
 sys.path.insert(0, r"/")
 from selenium_driverless import __version__
 
 project = 'Selenium-Driverless'
+# noinspection PyShadowingBuiltins
 copyright = '2024, Aurin Aegerter (aka Steve, kaliiiiiiiiii)'
 author = 'Aurin Aegerter (aka Steve, kaliiiiiiiiii)'
 release = __version__
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
```

### Comparing `selenium_driverless-1.8.0.2/examples/proxy_with_auth.py` & `selenium_driverless-1.9/examples/proxy_with_auth.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/setup.py` & `selenium_driverless-1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-requirements = ['selenium~=4.6', "cdp-socket>=1.2.5", "numpy", "matplotlib~=3.5", "scipy~=1.7", "aiofiles",
+requirements = ['selenium~=4.6', "cdp-socket>=1.2.5", "numpy", "scipy~=1.7", "aiofiles",
                 'platformdirs']
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='selenium_driverless',
```

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/files/js/show_mousemove.js` & `selenium_driverless-1.9/src/selenium_driverless/files/js/show_mousemove.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/files/mv3_extension/driverless_background_mv3_243ffdd55e32a012b4f253b2879af978.js` & `selenium_driverless-1.9/src/selenium_driverless/files/mv3_extension/driverless_background_mv3_243ffdd55e32a012b4f253b2879af978.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/files/mv3_extension/manifest.json` & `selenium_driverless-1.9/src/selenium_driverless/files/mv3_extension/manifest.json`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/scripts/driver_utils.py` & `selenium_driverless-1.9/src/selenium_driverless/scripts/driver_utils.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/scripts/geometry.py` & `selenium_driverless-1.9/src/selenium_driverless/scripts/geometry.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,113 +1,78 @@
 import numpy as np
 import random
+import typing
 
-from matplotlib.patches import Polygon
 from scipy.interpolate import splprep, splev
 
 
-# Element middle
-def gen_heatmap(polygon_vertices: np.array, num_points: int = 70):
-    polygon = Polygon(polygon_vertices, closed=True, edgecolor='black', facecolor='none')
-
-    x_min, y_min, x_max, y_max = get_bounds(polygon_vertices)
-
-    x_vals = np.linspace(x_min, x_max, num_points)
-    y_vals = np.linspace(y_min, y_max, num_points)
-    x, y = np.meshgrid(x_vals, y_vals)
-    points = np.column_stack((x.flatten(), y.flatten()))
-
-    distances = np.empty(num_points ** 2)
-    for i, point in enumerate(points):
-        min_distance = np.inf
-        for j in range(len(polygon_vertices)):
-            edge_start = polygon_vertices[j]
-            edge_end = polygon_vertices[(j + 1) % len(polygon_vertices)]
-
-            v1 = edge_end - edge_start
-            # noinspection PyUnresolvedReferences
-            v2 = point - edge_start
-            distance = np.linalg.norm(np.cross(v1, v2)) / np.linalg.norm(v1)
-
-            min_distance = min(min_distance, distance)
-        distances[i] = min_distance
-
-    distances_normalized = distances / np.max(distances)
-    distances_grid = distances_normalized.reshape((num_points, num_points))
-
-    path = polygon.get_path()
-    mask = ~path.contains_points(points).reshape((num_points, num_points))
-    distances_grid[mask] = 0.0
-
-    return distances_grid
-
-
-def gen_rand_point(polygon_vertices: np.array, heatmap_grid: np.array, bias_value: float = 7):
-    num_points = len(heatmap_grid)
-
-    heatmap_probs = heatmap_grid.flatten() ** bias_value
-    heatmap_probs /= np.sum(heatmap_probs)
-
-    try:
-        sampled_index = np.random.choice(num_points ** 2, p=heatmap_probs)
-    except ValueError as e:
-        if e.args[0] == 'probabilities contain NaN':
-            raise ValueError("Can't generate point from heatmap with 0-values only")
-        else:
-            raise e
-
-    row = sampled_index // num_points
-    col = sampled_index % num_points
-
-    x_min, y_min, x_max, y_max = get_bounds(polygon_vertices)
-
-    x_range = polygon_vertices.max(axis=0) - polygon_vertices.min(axis=0)
-    x_sample = x_min + col * (x_range[0] / (num_points - 1))
-    y_sample = y_min + row * (x_range[1] / (num_points - 1))
-
-    return x_sample, y_sample
+def gaussian_bias_rand(spread, border=0.05, bias=0.5) -> float:
+    """Generate random Gaussian distributed values with bias."""
+    if spread == 0:
+        return bias
+    res = np.random.normal(scale=spread / 6, loc=bias)
+    while not (border <= res <= 1 - border):
+        res = np.random.normal(scale=spread / 6, loc=bias)
+    return res
+
+
+ElemType = typing.Union[np.ndarray[(int, int)], typing.List[typing.Union[typing.List, typing.Tuple]]]
+
+
+def point_in_rectangle(points: np.ndarray[(int, int)], a, b) -> typing.List[float]:
+    """
+    Args:
+    - points: List of four coordinates [[x1, y1], [x2, y2], [x3, y3], [x4, y4]]
+    - a: float, a point ranging from 0 to 1 on line |AB|
+    - b: float, a point ranging from 0 to 1 on line |BC|
+
+    Returns:
+    - List: Coordinates of a point within the rectangle.
+    """
+    # Validate input points
+    if len(points) != 4:
+        raise ValueError("Input should contain four points defining a rectangle.")
+
+    # Calculate coordinates of the point within the rectangle
+    x = (1 - b) * (points[0][0] + a * (points[1][0] - points[0][0])) + b * (
+            points[3][0] + a * (points[2][0] - points[3][0]))
+    y = (1 - b) * (points[0][1] + a * (points[1][1] - points[0][1])) + b * (
+            points[3][1] + a * (points[2][1] - points[3][1]))
+
+    return [x, y]
+
+
+# noinspection PyUnusedLocal
+def rand_mid_loc(elem: ElemType, spread_a: float = 1, spread_b: float = 1, bias_a: float = 0.5, bias_b: float = 0.5, border:float=0.05) -> typing.List[float]:
+    if len(elem) != 4:
+        raise ValueError("Input should contain four points defining a rectangle.")
+    assert 0 <= bias_a <= 1
+    assert 0 <= bias_b <= 1
+    elem = np.array(elem)
+
+    # ensure element has an area
+    a_b = elem[1] - elem[0]
+    b_c = elem[2] - elem[1]
+    # noinspection PyUnreachableCode
+    area = np.abs(np.cross(a_b, b_c))
+    if area == 0:
+        raise ValueError("The area of the element is 0")
+
+    point_a = gaussian_bias_rand(spread_a, bias=bias_a, border=border)
+    point_b = gaussian_bias_rand(spread_b, bias=bias_b, border=border)
+    return point_in_rectangle(elem, point_a, point_b)
 
 
 def get_bounds(vertices: np.array):
     x_min, y_min = vertices.min(axis=0)
     x_max, y_max = vertices.max(axis=0)
     return x_min, y_min, x_max, y_max
 
 
-def centroid(vertices):
-    polygon2 = np.roll(vertices, -1, axis=0)
-
-    # Compute signed area of each triangle
-    signed_areas = 0.5 * np.cross(vertices, polygon2)
-
-    # Compute centroid of each triangle
-    centroids = (vertices + polygon2) / 3.0
-
-    # Get average of those centroids, weighted by the signed areas.
-    return np.average(centroids, axis=0, weights=signed_areas)
-
-
-def visualize(rand_points: np.array, heatmap_grid: np.array, polygon_vertices: np.array):
-    import matplotlib.pyplot as plt
-    x_min, y_min, x_max, y_max = get_bounds(polygon_vertices)
-
-    fig, ax = plt.subplots(figsize=(8, 6))
-
-    ax.imshow(heatmap_grid, cmap='hot', extent=[x_min, x_max, y_min, y_max], origin='lower')
-    ax.add_patch(
-        Polygon(polygon_vertices, closed=True, edgecolor='yellow', facecolor='none'))  # Changed edgecolor to yellow
-
-    ax.scatter(rand_points[:, 0], rand_points[:, 1], color='blue')
-    ax.set_title('Random points inside element (Polygon) based on heatmap')
-
-    plt.tight_layout()
-    plt.show(block=True)
-
-
-def bias_0_dot_5(strength: float, max_offset: float):
+def bias_0_dot_5(strength: float, max_offset: float) -> float:
     # Calculate alpha and beta parameters for the beta distribution
     alpha = 2 * strength
     beta = 2 * (1 - strength)
 
     # Calculate the valid range for the random value based on max_offset
     lower_bound = max(0.5 - max_offset, 0)
     upper_bound = min(0.5 + max_offset, 1)
@@ -118,15 +83,15 @@
     # Adjust the random value to the valid range
     biased_value = lower_bound + (rand_value * (upper_bound - lower_bound))
 
     return biased_value
 
 
 # Mouse Path
-def pos_at_time(path, total_time, time, accel, mid_time=0.5):
+def pos_at_time(path, total_time, time, accel, mid_time=0.5) -> typing.Tuple[int]:
     if time > total_time or time < 0:
         raise ValueError("Time needs to be between 0 and total_time")
 
     def cubic_ease_in(t):
         return t ** accel
 
     def cubic_ease_out(t):
```

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/scripts/prefs.py` & `selenium_driverless-1.9/src/selenium_driverless/scripts/prefs.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/scripts/switch_to.py` & `selenium_driverless-1.9/src/selenium_driverless/scripts/switch_to.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # specific language governing permissions and limitations
 # under the License.
 
 # modified by kaliiiiiiiiii | Aurin Aegerter
 
 import asyncio
 import typing
-from typing import Optional
 from typing import Union
 import warnings
 
 
 from selenium_driverless.types.by import By
 from selenium_driverless.types.alert import Alert
 from selenium_driverless.types.target import TargetInfo, Target
@@ -122,15 +121,15 @@
                 except NoSuchElementException:
                     raise NoSuchIframe(frame_reference, f"couldn't get element by: {frame_reference}")
         target = await self._context.current_target.get_target_for_iframe(frame_reference)
         if activate:
             await target.focus()
         return target
 
-    async def target(self, target_id: typing.Union[str, TargetInfo, WebElement], activate: bool = True) -> Target:
+    async def target(self, target_id: typing.Union[str, TargetInfo, Target], activate: bool = True) -> Target:
         """
         switches to a target
 
         :param target_id: the target to switch to
         :param activate: whether to activate the target
         """
         if isinstance(target_id, TargetInfo):
@@ -147,14 +146,16 @@
             await self._context.current_target.focus()
         return self._context.current_target
 
     async def new_window(self, type_hint: typing.Literal["tab", "window"] = "tab", url="", activate: bool = True) -> Target:
         """Switches to a new window
 
         :param type_hint: what kind of window to switch to
+        :param url: url to load in the new target
+        :param activate: whether to activate the new target
         """
         target = await self._context.new_window(type_hint=type_hint, url=url, activate=activate)
         return await self.target(target, activate=activate)
 
     async def parent_frame(self, activate: bool = False) -> None:
         """Switches focus to the parent context. If the current context is the
         top level browsing context, the context remains unchanged.
```

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/sync/alert.py` & `selenium_driverless-1.9/src/selenium_driverless/sync/alert.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/sync/base_target.py` & `selenium_driverless-1.9/src/selenium_driverless/sync/base_target.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/sync/context.py` & `selenium_driverless-1.9/src/selenium_driverless/sync/context.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/sync/executor.py` & `selenium_driverless-1.9/src/selenium_driverless/sync/executor.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/sync/pointer.py` & `selenium_driverless-1.9/src/selenium_driverless/sync/pointer.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/sync/switch_to.py` & `selenium_driverless-1.9/src/selenium_driverless/sync/switch_to.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/sync/target.py` & `selenium_driverless-1.9/src/selenium_driverless/sync/target.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/sync/webdriver.py` & `selenium_driverless-1.9/src/selenium_driverless/sync/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/sync/webelement.py` & `selenium_driverless-1.9/src/selenium_driverless/sync/webelement.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/types/__init__.py` & `selenium_driverless-1.9/src/selenium_driverless/types/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/types/alert.py` & `selenium_driverless-1.9/src/selenium_driverless/types/alert.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/types/base_target.py` & `selenium_driverless-1.9/src/selenium_driverless/types/base_target.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import asyncio
+import time
+import typing
 
 import aiohttp
 import websockets
 from cdp_socket.exceptions import CDPError
 from cdp_socket.socket import SingleCDPSocket
 
 
 class BaseTarget:
-    """Allows you to drive the browser without chromedriver."""
+    """the baseTarget for the ChromeInstance
+    represents a connection to the whole browser.
+
+    .. note::
+        commands executed on BaseTarget usually are on a global scope over the whole Chrome instance.
+        unfortunately, not all are supported
+
+    """
 
     # noinspection PyMissingConstructor
     def __init__(self, host: str, is_remote: bool = False,
                  loop: asyncio.AbstractEventLoop or None = None, timeout: float = 30,
                  max_ws_size: int = 2 ** 20) -> None:
-        """Creates a new instance of the chrome target. Starts the service and
-        then creates new instance of chrome target.
-
-        :Args:
-         - options - this takes an instance of ChromeOptions.rst
-        """
         self._socket = None
 
         self._is_remote = is_remote
         self._host = host
         self._id = "BaseTarget"
 
         self._loop = loop
@@ -40,14 +43,15 @@
 
     @property
     async def type(self):
         return "BaseTarget"
 
     @property
     def socket(self) -> SingleCDPSocket:
+        """the cdp-socket for the connection"""
         return self._socket
 
     async def __aenter__(self):
         await self._init()
         return self
 
     def __enter__(self):
@@ -60,92 +64,90 @@
         pass
 
     def __await__(self):
         return self._init().__await__()
 
     async def _init(self):
         if not self._started:
-            res = None
-            while not res:
+            start = time.perf_counter()
+            url = f"http://{self._host}/json/version"
+            while True:
                 try:
                     async with aiohttp.ClientSession() as session:
-                        res = await session.get(f"http://{self._host}/json/version", timeout=self._timeout)
+                        res = await session.get(url, timeout=10)
                         _json = await res.json()
-                except aiohttp.ClientError:
-                    pass
+                        break
+                except (aiohttp.ClientError, asyncio.TimeoutError, OSError) as e:
+                    if (time.perf_counter() - start) > self._timeout:
+                        raise asyncio.TimeoutError(
+                            f"Couldn't connect to chrome within {self._timeout} seconds")
             self._socket = await SingleCDPSocket(websock_url=_json["webSocketDebuggerUrl"], timeout=self._timeout,
                                                  loop=self._loop, max_size=self._max_ws_size)
             self._started = True
         return self
 
     async def close(self) -> None:
-        """Closes the current window.
-
-        :Usage:
-            ::
-
-                target.close()
-        """
         try:
             await self._socket.close()
         except websockets.ConnectionClosedError:
             pass
         except CDPError as e:
             if e.code == -32000 and e.message == 'Command can only be executed on top-level targets':
                 pass
             else:
                 raise e
 
     async def wait_for_cdp(self, event: str, timeout: float or None = None):
+        """wait for an event
+        see :func:`Target.wait_for_cdp <selenium_driverless.types.target.Target.wait_for_cdp>` for reference
+        """
         if not self.socket:
             await self._init()
         return await self.socket.wait_for(event, timeout=timeout)
 
-    async def add_cdp_listener(self, event: str, callback: callable):
+    async def add_cdp_listener(self, event: str, callback: typing.Callable[[dict], any]):
+        """
+        add a listener for a CDP event
+        see :func:`Target.add_cdp_listener <selenium_driverless.types.target.Target.add_cdp_listener>` for reference
+        """
         if not self.socket:
             await self._init()
         self.socket.add_listener(method=event, callback=callback)
 
-    async def remove_cdp_listener(self, event: str, callback: callable):
+    async def remove_cdp_listener(self, event: str, callback: typing.Callable[[dict], any]):
+        """
+        remove a listener for a CDP event
+        see :func:`Target.remove_cdp_listener <selenium_driverless.types.target.Target.remove_cdp_listener>` for reference
+        """
         if not self.socket:
             await self._init()
         self.socket.remove_listener(method=event, callback=callback)
 
-    async def get_cdp_event_iter(self, event: str):
+    async def get_cdp_event_iter(self, event: str) -> typing.AsyncIterable[dict]:
+        """
+        iterate over CDP events on the current target
+        see :func:`Target.get_cdp_event_iter <selenium_driverless.types.target.Target.get_cdp_event_iter>` for reference
+        """
         if not self.socket:
             await self._init()
         return self.socket.method_iterator(method=event)
 
     async def execute_cdp_cmd(self, cmd: str, cmd_args: dict or None = None,
                               timeout: float or None = 10) -> dict:
-        """Execute Chrome Devtools Protocol command and get returned result The
-        command and command args should follow chrome devtools protocol
-        domains/commands, refer to link
-        https://chromedevtools.github.io/devtools-protocol/
-
-        :Args:
-         - cmd: A str, command name
-         - cmd_args: A dict, command args. empty dict {} if there is no command args
-        :Usage:
-            ::
-
-                target.execute_cdp_cmd('Network.getResponseBody', {'requestId': requestId})
-        :Returns:
-            A dict, empty dict {} if there is no result to return.
-            For example to getResponseBody:
-            {'base64Encoded': False, 'body': 'response body string'}
+        """Execute Chrome Devtools Protocol command and get returned result
+        see :func:`Target.execute_cdp_cmd <selenium_driverless.types.target.Target.execute_cdp_cmd>` for reference
         """
         if not self.socket:
             await self._init()
         if cmd == "Browser.setDownloadBehavior":
             path = cmd_args.get("downloadPath")
             if path:
                 self._downloads_paths[cmd_args.get("browserContextId", "DEFAULT")] = path
         result = await self.socket.exec(method=cmd, params=cmd_args, timeout=timeout)
         return result
 
-    def downloads_dir_for_context(self, context_id:str="DEFAULT") -> str:
+    def downloads_dir_for_context(self, context_id: str = "DEFAULT") -> str:
         """get the default download directory for a specific context
 
         :param context_id: the id of the context to get the directory for
         """
         return self._downloads_paths.get(context_id)
```

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/types/by.py` & `selenium_driverless-1.9/src/selenium_driverless/types/by.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 # edited by github/kaliiiiiiiiii
 
-from enum import Enum
-
 
 class By:
     """Set of supported locator strategies."""
     ID = "id"
     """"""
     NAME = "name"
     """"""
```

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/types/context.py` & `selenium_driverless-1.9/src/selenium_driverless/types/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,26 +171,26 @@
             # noinspection PyProtectedMember
             target._on_closed.append(remove_target)
         return target
 
     async def get_target_for_iframe(self, iframe: WebElement):
         return await self.current_target.get_target_for_iframe(iframe=iframe)
 
-    async def set_download_behaviour(self,behavior:typing.Literal["deny", "allow", "allowAndName", "default"],
-                                     path:str=None):
+    async def set_download_behaviour(self, behavior: typing.Literal["deny", "allow", "allowAndName", "default"],
+                                     path: str = None):
         """set the download behaviour
 
         :param behavior: the behaviour to set the downloading to
         :param path: the path to the default download directory
 
         .. warning::
             setting ``behaviour=allow`` instead of ``allowAndName`` can cause some bugs
 
         """
-        params = {"behavior":behavior, "eventsEnabled":True}
+        params = {"behavior": behavior, "eventsEnabled": True}
         if path:
             _dir = str(pathlib.Path(path))
             if os.path.isfile(_dir):
                 raise OSError("path can't point to a file")
             params["downloadPath"] = _dir
         if self._is_incognito:
             params["browserContextId"] = self.context_id
@@ -200,15 +200,14 @@
     def downloads_dir(self):
         """the current downloads directory"""
         if self._is_incognito:
             return self.base_target.downloads_dir_for_context(context_id=self.context_id)
         else:
             return self.base_target.downloads_dir_for_context(context_id="DEFAULT")
 
-
     async def wait_download(self, timeout: float or None = 30) -> dict:
         """
         wait for a download on the current tab
 
         returns something like
 
         .. code-block:: python
@@ -249,17 +248,25 @@
     @property
     async def title(self) -> str:
         """Returns the title of the current target"""
         target = await self.current_target_info
         return target.title
 
     @property
-    async def current_pointer(self) -> Pointer:
+    def current_pointer(self) -> Pointer:
+        """the :class:`Pointer <selenium_driverless.input.pointer.Pointer>` for the current target"""
         target = self.current_target
         return target.pointer
+    async def send_keys(self, text: str):
+        """
+        send text & keys to the current target
+
+        :param text: the text to send
+        """
+        await self.current_target.send_keys(text)
 
     async def execute_raw_script(self, script: str, *args, await_res: bool = False, serialization: str = None,
                                  max_depth: int = None, timeout: int = 2, target_id: str = None,
                                  execution_context_id: str = None, unique_context: bool = False):
         """
         example:
         script= "function(...arguments){obj.click()}"
@@ -271,26 +278,47 @@
                                                serialization=serialization, max_depth=max_depth,
                                                timeout=timeout, execution_context_id=execution_context_id,
                                                unique_context=unique_context)
 
     async def execute_script(self, script: str, *args, max_depth: int = 2, serialization: str = None,
                              timeout: int = None, target_id: str = None, execution_context_id: str = None,
                              unique_context: bool = False):
-        """
-        example: script = "return obj.click()"
+        """executes JavaScript synchronously on ``GlobalThis`` such as
+
+        .. code-block:: js
+
+            return document
+
+        ``this`` and ``obj`` refers to ``globalThis`` (=> window) here
+
+        see :func:`Target.execute_raw_script <selenium_driverless.types.target.Target.execute_raw_script>` for argument descriptions
         """
         target = await self.get_target(target_id)
         return await target.execute_script(script, *args, max_depth=max_depth, serialization=serialization,
                                            timeout=timeout, execution_context_id=execution_context_id,
                                            unique_context=unique_context)
 
     async def execute_async_script(self, script: str, *args, max_depth: int = 2,
                                    serialization: str = None, timeout: int = 2,
                                    target_id: str = None, execution_context_id: str = None,
                                    unique_context: bool = False):
+        """executes JavaScript asynchronously on ``GlobalThis`` such as
+
+        .. warning::
+            using execute_async_script is not recommended as it doesn't handle exceptions correctly.
+            Use :func:`Chrome.eval_async <selenium_driverless.webdriver.Chrome.eval_async>`
+
+        .. code-block:: js
+
+            resolve = arguments[arguments.length-1]
+
+        ``this`` refers to ``globalThis`` (=> window)
+
+        see :func:`Target.execute_raw_script <selenium_driverless.types.target.Target.execute_raw_script>` for argument descriptions
+        """
         target = await self.get_target(target_id)
         return await target.execute_async_script(script, *args, max_depth=max_depth, serialization=serialization,
                                                  timeout=timeout,
                                                  execution_context_id=execution_context_id,
                                                  unique_context=unique_context)
 
     async def eval_async(self, script: str, *args, max_depth: int = 2,
@@ -614,22 +642,32 @@
 
     # Timeouts
     @staticmethod
     async def sleep(time_to_wait: float) -> None:
         await asyncio.sleep(time_to_wait)
 
     # noinspection PyUnusedLocal
-    async def find_element(self, by: str, value: str, parent=None, target_id: str = None,
-                           timeout: int or None = None) -> WebElement:
-        target = await self.get_target(target_id=target_id)
-        return await target.find_element(by=by, value=value, parent=parent, timeout=timeout)
+    async def find_element(self, by: str, value: str, timeout: int or None = None) -> WebElement:
+        """find an element in the current target
 
-    async def find_elements(self, by: str, value: str, parent=None, target_id: str = None) -> typing.List[WebElement]:
-        target = await self.get_target(target_id=target_id)
-        return await target.find_elements(by=by, value=value, parent=parent)
+        :param by: one of the locators at :func:`By <selenium_driverless.types.by.By>`
+        :param value: the actual query to find the element by
+        :param timeout: how long to wait for the element to exist
+        """
+        target = await self.get_target()
+        return await target.find_element(by=by, value=value, timeout=timeout)
+
+    async def find_elements(self, by: str, value: str) -> typing.List[WebElement]:
+        """find multiple elements in the current target
+
+        :param by: one of the locators at :func:`By <selenium_driverless.types.by.By>`
+        :param value: the actual query to find the elements by
+        """
+        target = await self.get_target()
+        return await target.find_elements(by=by, value=value)
 
     async def search_elements(self, query: str, target_id: str = None) -> typing.List[WebElement]:
         """
         query:str | Plain text or query selector or XPath search query.
         """
         target = await self.get_target(target_id=target_id)
         return await target.search_elements(query=query)
@@ -867,57 +905,74 @@
         args = {"permission": {"name": name}, "setting": value}
         if self.context_id:
             args["browserContextId"] = self.context_id
         if origin:
             args["origin"] = origin
         await self.execute_cdp_cmd("Browser.setPermission", args)
 
-    async def wait_for_cdp(self, event: str, timeout: float or None = None, target_id: str = None):
+    async def wait_for_cdp(self, event: str, timeout: float or None = None, target_id: str = None) -> dict:
+        """
+        wait for an event on the current target
+        see :func:`Target.wait_for_cdp <selenium_driverless.types.target.Target.wait_for_cdp>` for reference
+        """
         target = await self.get_target(target_id=target_id)
         return await target.wait_for_cdp(event=event, timeout=timeout)
 
-    async def add_cdp_listener(self, event: str, callback: callable, target_id: str = None):
+    async def add_cdp_listener(self, event: str, callback: typing.Callable[[dict], any], target_id: str = None):
+        """
+        add a listener for a CDP event on the current target
+        see :func:`Target.add_cdp_listener <selenium_driverless.types.target.Target.add_cdp_listener>` for reference
+        """
         target = await self.get_target(target_id=target_id)
         return await target.add_cdp_listener(event=event, callback=callback)
 
-    async def remove_cdp_listener(self, event: str, callback: callable, target_id: str = None):
+    async def remove_cdp_listener(self, event: str, callback: typing.Callable[[dict], any], target_id: str = None):
+        """
+        remove a listener for a CDP event on the current target
+        see :func:`Target.remove_cdp_listener <selenium_driverless.types.target.Target.remove_cdp_listener>` for reference
+        """
         target = await self.get_target(target_id=target_id)
         return await target.remove_cdp_listener(event=event, callback=callback)
 
-    async def get_cdp_event_iter(self, event: str, target_id: str = None):
+    async def get_cdp_event_iter(self, event: str, target_id: str = None) -> typing.AsyncIterable[dict]:
+        """
+        iterate over CDP events on the current target
+        see :func:`Target.get_cdp_event_iter <selenium_driverless.types.target.Target.get_cdp_event_iter>` for reference
+        """
         target = await self.get_target(target_id=target_id)
         return await target.get_cdp_event_iter(event=event)
 
     async def execute_cdp_cmd(self, cmd: str, cmd_args: dict or None = None,
                               timeout: float or None = 10, target_id: str = None) -> dict:
-        """Execute Chrome Devtools Protocol command and get returned result The
-        command and command args should follow chrome devtools protocol
-        domains/commands, refer to link
-        https://chromedevtools.github.io/devtools-protocol/
-
-        :Args:
-         - cmd: A str, command name
-         - cmd_args: A dict, command args. empty dict {} if there is no command args
-        :Usage:
-            ::
-
-                target.execute_cdp_cmd('Network.getResponseBody', {'requestId': requestId})
-        :Returns:
-            A dict, empty dict {} if there is no result to return.
-            For example to getResponseBody:
-            {'base64Encoded': False, 'body': 'response body string'}
+        """Execute Chrome Devtools Protocol command on the current target
+        executes it on :class:`Target.execute_cdp_cmd <selenium_driverless.types.base_target.BaseTarget>`
+        if ``message:'Not allowed'`` received
+        see :func:`Target.execute_cdp_cmd <selenium_driverless.types.target.Target.execute_cdp_cmd>` for reference
         """
-
         target = await self.get_target(target_id=target_id)
         try:
             return await target.execute_cdp_cmd(cmd=cmd, cmd_args=cmd_args, timeout=timeout)
         except CDPError as e:
             if e.code == -32000 and e.message == 'Not allowed':
                 return await self.base_target.execute_cdp_cmd(cmd=cmd, cmd_args=cmd_args, timeout=timeout)
 
+    async def fetch(self, *args, **kwargs) -> dict:
+        """
+        executes a JS ``fetch`` request within the current target
+        see :func:`Target.fetch <selenium_driverless.types.target.Target.fetch>` for reference
+        """
+        return await self.current_target.fetch(*args, **kwargs)
+
+    async def xhr(self, *args, **kwargs) -> dict:
+        """
+        executes a JS ``XMLHttpRequest`` request within the current target
+        see :func:`Target.fetch <selenium_driverless.types.target.Target.fetch>` for reference
+        """
+        return await self.current_target.xhr(*args, **kwargs)
+
     # noinspection PyTypeChecker
     async def get_sinks(self, target_id: str = None) -> list:
         """
         :Returns: A list of sinks available for Cast.
         """
         target = await self.get_target(target_id=target_id)
         return await target.get_sinks()
```

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/types/deserialize.py` & `selenium_driverless-1.9/src/selenium_driverless/types/deserialize.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/types/options.py` & `selenium_driverless-1.9/src/selenium_driverless/types/options.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/types/target.py` & `selenium_driverless-1.9/src/selenium_driverless/types/webelement.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1083 +1,937 @@
-# io
+# Licensed to the Software Freedom Conservancy (SFC) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The SFC licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+# edited by kaliiiiiiiiiii
+from __future__ import annotations
+
 import asyncio
-import os.path
 import time
-import typing
-from typing_extensions import TypedDict
 import warnings
-from base64 import b64decode
+import numpy as np
+import typing
 import aiofiles
-from typing import List
-import pathlib
 
-import websockets
+from base64 import b64decode
+from collections import defaultdict
 from cdp_socket.exceptions import CDPError
-from cdp_socket.socket import SingleCDPSocket
 
-# pointer
-from selenium_driverless.sync.pointer import Pointer as SyncPointer
-from selenium_driverless.input.pointer import Pointer
-# other
-from selenium_driverless.scripts.driver_utils import get_targets, get_target, get_cookies, get_cookie, delete_cookie, \
-    delete_all_cookies, add_cookie
-from selenium_driverless.utils.utils import safe_wrap_fut
-from selenium_driverless.types.deserialize import StaleJSRemoteObjReference
-from selenium_driverless.types.webelement import StaleElementReferenceException, NoSuchElementException
-from selenium_driverless.sync.alert import Alert as SyncAlert
-# Alert
-from selenium_driverless.types.alert import Alert
-from selenium_driverless.types.webelement import WebElement
-from selenium_driverless.sync.webelement import WebElement as SyncWebElement
-
-
-class NoSuchIframe(Exception):
-    def __init__(self, elem: WebElement, message: str):
-        self._elem = elem
-        super().__init__(message)
-
-    @property
-    def elem(self):
-        return self._elem
-
-
-class Target:
-    """Allows you to drive the browser without chromedriver."""
-
-    # noinspection PyShadowingBuiltins
-    def __init__(self, host: str, target_id: str, driver, context, is_remote: bool = False,
-                 loop: asyncio.AbstractEventLoop or None = None, timeout: float = 30,
-                 type: str = None, start_socket: bool = False, max_ws_size: int = 2 ** 20) -> None:
-        """Creates a new instance of the chrome target. Starts the service and
-        then creates new instance of chrome target.
+# driverless
+from selenium_driverless.types.by import By
+from selenium_driverless.types.deserialize import JSRemoteObj, StaleJSRemoteObjReference
+from selenium_driverless.scripts.geometry import rand_mid_loc
 
-        :Args:
-         - options - this takes an instance of ChromeOptions.rst
-        """
-        from selenium_driverless.types.context import Context
-        self._parent_target = None
-        self._context: Context = context
-        self._window_id = None
-        self._pointer = None
-        self._page_enabled = None
-        self._dom_enabled = None
-        self._max_ws_size = max_ws_size
-
-        self._global_this_ = {}
-        self._document_elem_ = None
-        self._alert = None
-
-        self._targets: list = []
-        self._socket = None
-        self._isolated_context_id_ = None
-        self._exec_context_id_ = ""
-        self._targets: typing.Dict[str, Target] = {}
-
-        self._is_remote = is_remote
-        self._host = host
-        self._id = target_id
-        self._context_id = None
-        self._type = type
-        self._timeout = timeout
 
-        self._loop = loop
-        self._start_socket = start_socket
-        self._on_closed_ = []
+class NoSuchElementException(Exception):
+    pass
 
-        self._driver = driver
 
-    def __repr__(self):
-        return f'<{type(self).__module__}.{type(self).__name__} (target_id="{self.id}", host="{self._host}")>'
+class StaleElementReferenceException(StaleJSRemoteObjReference):
+    def __init__(self, elem):
+        elem._stale = True
+        message = f"Page or Frame has been reloaded, or the element removed, {elem}"
+        super().__init__(_object=elem, message=message)
 
-    @property
-    def id(self):
-        return self._id
 
-    @property
-    async def browser_context_id(self):
-        if not self._context_id:
-            info = await self.info
-            return info.browser_context_id
-        return self._context_id
+class ElementNotVisible(Exception):
+    pass
 
-    @property
-    def base_target(self):
-        return self._driver.base_target
 
-    @property
-    def socket(self) -> SingleCDPSocket:
-        return self._socket
+class ElementNotInteractable(Exception):
+    def __init__(self, x: float, y: float, _type: str = "interactable"):
+        super().__init__(f"element not {_type} at x:{x}, y:{y}, it might be hidden under another one")
 
-    def __eq__(self, other):
-        if isinstance(other, Target):
-            return other.socket == self.socket
-        return False
 
-    def __enter__(self):
-        return self
+class ElementNotClickable(ElementNotInteractable):
+    def __init__(self, x: float, y: float):
+        super().__init__(x, y, _type="clickable")
 
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        await self.close()
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        pass
+# noinspection PyProtectedMember
+class WebElement(JSRemoteObj):
+    """Represents a DOM element.
 
-    async def __aenter__(self):
-        # doesn't do anything (start_socket=False)
-        return self
+    Generally, all interesting operations that interact with a document will be
+    performed through this interface.
 
-    def __await__(self):
-        if self._start_socket:
-            return self._init().__await__()
-        else:
-            # doesn't do anything (start_socket=False)
-            return self.__aenter__().__await__()
+    All method calls will do a freshness check to ensure that the element
+    reference is still valid.  This essentially determines whether the
+    element is still attached to the DOM.  If this test fails, then a
+    ``StaleElementReferenceException`` is thrown, and all future calls to this
+    instance will fail.
+    """
 
-    async def _init(self):
-        if not self._socket:
-            self._socket = await SingleCDPSocket(websock_url=f'ws://{self._host}/devtools/page/{self._id}',
-                                                 timeout=self._timeout, loop=self._loop, max_size=self._max_ws_size)
-            if self._loop:
-                self._pointer = SyncPointer(target=self, loop=self._loop)
-            else:
-                self._pointer = Pointer(target=self)
+    def __init__(self, target, frame_id: int or None, isolated_exec_id: int or None, obj_id=None,
+                 node_id=None, backend_node_id: str = None, loop=None, class_name: str = None,
+                 context_id: int = None, is_iframe: bool = False) -> None:
+        self._loop = loop
+        if not (obj_id or node_id or backend_node_id):
+            raise ValueError("either js, obj_id or node_id need to be specified")
+        self._node_id = node_id
+        self._backend_node_id = backend_node_id
+        self._class_name = class_name
+        self._started = False
+        self.___context_id__ = context_id
+        self._obj_ids = {context_id: obj_id}
+        self.___frame_id__ = None
+        self._is_iframe = is_iframe
+        self._stale = False
+        if obj_id and context_id:
+            self._obj_ids[context_id] = obj_id
+        self.___obj_id__ = None
+        super().__init__(target=target, frame_id=frame_id, obj_id=obj_id, isolated_exec_id=isolated_exec_id)
+
+    def __await__(self):
+        return self.__aenter__().__await__()
 
-            def set_alert(alert):
-                self._alert = alert
+    async def __aenter__(self):
+        if not self._started:
+            if not self.__target__._page_enabled:
+                await self.__target__.execute_cdp_cmd("Page.enable")
+            self._started = True
 
-            # noinspection PyUnusedLocal
-            def remove_alert(alert):
-                self._alert = None
-
-            await self.add_cdp_listener("Page.javascriptDialogOpening", set_alert)
-            await self.add_cdp_listener("Page.javascriptDialogClosed", remove_alert)
-            await self.add_cdp_listener("Page.loadEventFired", self._on_loaded)
-            await self.add_cdp_listener("Page.windowOpen", self._on_loaded)
-            self.socket.on_closed.extend(self._on_closed)
         return self
 
     @property
-    def _on_closed(self):
-        if self.socket:
-            return self.socket.on_closed
-        else:
-            return self._on_closed_
+    async def obj_id(self) -> str:
+        """**async** returns the `Runtime.RemoteObjectId <https://vanilla.aslushnikov.com/?Runtime.RemoteObjectId>`_ for the element
+        """
+        return await self.__obj_id_for_context__()
 
-    # noinspection PyUnusedLocals,PyUnusedLocal
-    async def _on_loaded(self, *args, **kwargs):
-        self._global_this_ = {}
-        self._document_elem_ = None
-        self._isolated_context_id_ = None
-        self._exec_context_id_ = None
-
-    async def get_alert(self, timeout: float = 5):
-        if not self._page_enabled:
-            await self.execute_cdp_cmd("Page.enable", timeout=timeout)
-        if self._loop:
-            alert = SyncAlert(self, loop=self._loop, timeout=timeout)
+    @property
+    async def context_id(self):
+        self._check_stale()
+        if not self.___context_id__:
+            await self.obj_id
+        return self.__context_id__
+
+    def _check_stale(self):
+        if self._stale:
+            raise StaleElementReferenceException(elem=self)
+
+    @property
+    def _args_builder(self) -> dict:
+        self._check_stale()
+        if self._node_id:
+            return {"nodeId": self._node_id}
+        elif self.__obj_id__:
+            return {"objectId": self.__obj_id__}
+        elif self._backend_node_id:
+            return {"backendNodeId": self._backend_node_id}
         else:
-            alert = await Alert(self, timeout=timeout)
-        return alert
-
-    async def get_targets_for_iframes(self, iframes: typing.List[WebElement]):
-        if not iframes:
-            raise ValueError(f"Expected WebElements, but got{iframes}")
-
-        async def target_getter(target_id: str, timeout: float = 2, max_ws_size: int = 2 ** 20):
-            return await get_target(target_id=target_id, host=self._host, loop=self._loop, is_remote=self._is_remote,
-                                    timeout=timeout, max_ws_size=max_ws_size, driver=self._driver,
-                                    context=self._context)
-
-        _targets = await get_targets(cdp_exec=self.execute_cdp_cmd, target_getter=target_getter,
-                                     _type="iframe", context_id=self._context_id, max_ws_size=self._max_ws_size)
-        targets = {}
-
-        for targetinfo in list(_targets.values()):
-            # iterate over iframes
-            target = targetinfo.Target
-            base_frame = await target.base_frame
-
-            #  check if iframe element is within iframes to search
-            for iframe in iframes:
-                tag_name = await iframe.tag_name
-                if tag_name.upper() != "IFRAME":
-                    raise NoSuchIframe(iframe, "element isn't a iframe")
-                await iframe.obj_id
-                iframe_frame_id = await iframe.__frame_id__
-                if base_frame["id"] == iframe_frame_id:
-                    if await self.type == "iframe":
-                        target._parent_target = self
-                    else:
-                        target._base_target = self
-                    targets[target.id] = target
-        return list(targets.values())
-
-    async def get_target_for_iframe(self, iframe: WebElement):
-        targets = await self.get_targets_for_iframes([iframe])
-        if not targets:
-            raise NoSuchIframe(iframe, "no target for iframe found")
-        return targets[0]
-
-    async def wait_download(self, timeout: float or None = 30) -> dict:
-        """
-        wait for a download on the current tab
-
-        returns something like
-
-        .. code-block:: python
-
-            {
-                "frameId": "2D543B5E8B14945B280C537A4882A695",
-                "guid": "c91df4d5-9b45-4962-84df-3749bd3f926d",
-                "url": "https://www.w3.org/WAI/ER/tests/xhtml/testfiles/resources/pdf/dummy.pdf",
-                "suggestedFilename": "dummy.pdf",
-
-                # only if options.downloads_dir specified
-                "guid_file": "D:\\System\\AppData\\PyCharm\\scratches\\downloads\\c91df4d5-9b45-4962-84df-3749bd3f926d"
-            }
-
-        :param timeout: time in seconds to wait for a download
+            raise ValueError(f"missing remote element id's for {self}")
 
-        .. warning::
-            downloads from iframes not supported yet
-
-        """
-
-        # todo: support downloads from iframes
-        async def _wait_download():
-            base_frame = await self.base_frame
-            _id = base_frame.get("id")
-            _dir = [self._context.downloads_dir][0]
-            async for data in await self.base_target.get_cdp_event_iter("Browser.downloadWillBegin"):
-                base_frame = await self.base_frame
-                curr_id = base_frame.get("id")
-                if data["frameId"] in [_id, curr_id]:
-                    if _dir:
-                        guid_file = str(pathlib.Path(_dir + "/" + data["guid"]))
-                        named_file = str(pathlib.Path(_dir + "/" + "suggestedFilename"))
-                        data["guid_file"] = guid_file
-                        data["named_file"] = named_file
-                        while not (os.path.exists(guid_file) or os.path.exists(named_file)):
-                            # wait for file to exist
-                            await asyncio.sleep(0.01)
-                    return data
-
-        return await asyncio.wait_for(_wait_download(), timeout=timeout)
-
-    # noinspection PyUnboundLocalVariable,PyProtectedMember
-    async def get(self, url: str, referrer: str = None, wait_load: bool = True, timeout: float = 30) -> dict:
-        """Loads a web page
-
-        :param url: the url to load.
-        :param referrer: the referrer to load the page with
-        :param wait_load: whether to wait for the webpage to load
-        :param timeout: the maximum time in seconds for waiting on load
-
-        returns the same as :func:`Target.wait_download <selenium_driverless.types.target.Target.wait_download>` if the url initiates a download
-        """
-        if url == "about:blank":
-            wait_load = False
-        result = {}
-
-        if "#" in url:
-            # thanks to https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/139#issuecomment-1877197974
-            current_url_base = (await self.current_url).split("#")[0]
-            if url[0] == "#":
-                # allow to navigate only by fragment ID of the current url
-                url = current_url_base + url
-                wait_load = False
-            elif url.split("#")[0] == current_url_base:
-                wait_load = False
-
-        if wait_load:
-            if not self._page_enabled:
-                await self.execute_cdp_cmd("Page.enable")
-
-            # wait for download or loadEventFired
-            wait = asyncio.ensure_future(asyncio.wait([
-                safe_wrap_fut(self.wait_for_cdp("Page.loadEventFired", timeout=None)),
-                safe_wrap_fut(self.wait_download(timeout=None))
-            ], timeout=timeout, return_when=asyncio.FIRST_COMPLETED))
-
-            await asyncio.sleep(0.01)  # ensure listening for events has already started
-
-        # send navigate cmd
-        args = {"url": url, "transitionType": "link"}
-        if referrer:
-            args["referrer"] = referrer
-        get = asyncio.ensure_future(self.execute_cdp_cmd("Page.navigate", args, timeout=timeout))
-
-        if wait_load:
-            done, pending = await wait
-            pending.pop().cancel()
-            if not done:
-                pending.pop().cancel()
-                try:
-                    await get  # ensure get is awaited in every case
-                except Exception as e:
-                    raise e
-                raise asyncio.TimeoutError(f'page: "{url}" didn\'t load within timeout of {timeout}')
-            result = done.pop().result()  # data of the event waited for
-        try:
-            await get  # wait for navigate cmd response
-        except Exception as e:
-            raise e
-        await self._on_loaded()
-        return result
+    async def __obj_id_for_context__(self, context_id: int = None):
+        self._check_stale()
+        if not self._obj_ids.get(context_id):
+            args = {}
+            if self._backend_node_id:
+                args["backendNodeId"] = self._backend_node_id
+            elif self._node_id:
+                args["nodeId"] = self._node_id
+            else:
+                raise ValueError(f"missing remote element id's for {self}")
 
-    async def _global_this(self, context_id: str = None):
-        if not context_id:
-            context_id = self._exec_context_id_
-        if (not self._global_this_.get(context_id)) or self._loop:
-            from selenium_driverless.types.deserialize import JSRemoteObj
-            from selenium_driverless.types import JSEvalException
-            args = {"expression": "globalThis",
-                    "serializationOptions": {
-                        "serialization": "idOnly"}}
             if context_id:
-                args["contextId"] = context_id
+                args["executionContextId"] = context_id
             try:
-                res = await self.execute_cdp_cmd("Runtime.evaluate", args)
+                res = await self.__target__.execute_cdp_cmd("DOM.resolveNode", args)
             except CDPError as e:
-                if e.code == -32000 and e.message == 'Cannot find context with specified id':
-                    raise StaleJSRemoteObjReference("GlobalThis")
+                if e.code == -32000 and 'No node with given id found' in e.message:
+                    raise StaleElementReferenceException(self)
                 else:
                     raise e
+            obj_id = res["object"].get("objectId")
+            if obj_id:
+                if self.__context_id__ == context_id:
+                    self.___obj_id__ = obj_id
+                self._obj_ids[context_id] = obj_id
+            class_name = res["object"].get("className")
+            if class_name:
+                self._class_name = class_name
+        return self._obj_ids.get(context_id)
 
-            if "exceptionDetails" in res.keys():
-                raise JSEvalException(res["exceptionDetails"])
-            obj_id = res["result"]['objectId']
-
-            base_frame = await self.base_frame
-            # target can have no frames at all
-            frame_id = None
-            if base_frame:
-                frame_id = base_frame.get("id")
-
-            # noinspection PyUnresolvedReferences
-            obj = JSRemoteObj(obj_id=obj_id, target=self, isolated_exec_id=None,
-                              frame_id=frame_id)
-            if not context_id:
-                context_id = obj.__context_id__
-                self._exec_context_id_ = context_id
-            self._global_this_[context_id] = obj
-        return self._global_this_[context_id]
-
-    @property
-    async def _isolated_context_id(self) -> int:
-        doc = await self._document_elem
-        return await doc.__isolated_exec_id__
+    @property
+    def __context_id__(self):
+        if self.__obj_id__:
+            return int(self.__obj_id__.split(".")[1])
+        else:
+            return self.___context_id__
 
     @property
-    def pointer(self) -> Pointer:
-        return self._pointer
+    async def node_id(self):
+        self._check_stale()
+        if not self._node_id:
+            node = await self.__target__.execute_cdp_cmd("DOM.requestNode", {"objectId": await self.obj_id})
+            self._node_id = node["nodeId"]
+        return self._node_id
+
+    @property
+    async def __frame_id__(self) -> int:
+        if not self.___frame_id__:
+            await self._describe()
+        return self.___frame_id__
+
+    @property
+    async def content_document(self):
+        """
+        gets the document of the iframe
+        """
+        _desc = await self._describe()
+        if _desc.get("localName") == "iframe":
+            node = _desc.get("contentDocument")
+            if node:
+                frame_id = _desc.get("frameId")
+                if node['documentURL'] == 'about:blank':
+                    # wait for frame to load
+                    if not self.__target__._page_enabled:
+                        await self.__target__.execute_cdp_cmd("Page.enable")
+                    async for data in await self.__target__.get_cdp_event_iter("Page.frameNavigated"):
+                        frame = data["frame"]
+                        if frame["id"] == frame_id:
+                            break
+                    self._stale = False
+                    _desc = await self._describe()
+                    node = _desc.get("contentDocument")
+                if self._loop:
+                    from selenium_driverless.sync.webelement import WebElement as SyncWebElement
+                    return await SyncWebElement(backend_node_id=node.get('backendNodeId'),
+                                                target=self.__target__, loop=self._loop,
+                                                class_name='HTMLIFrameElement',
+                                                isolated_exec_id=None, frame_id=frame_id)
+                else:
+                    return await WebElement(backend_node_id=node.get('backendNodeId'),
+                                            target=self.__target__, loop=self._loop,
+                                            class_name='HTMLIFrameElement',
+                                            isolated_exec_id=None, frame_id=frame_id)
 
-    async def execute_raw_script(self, script: str, *args, await_res: bool = False, serialization: str = None,
-                                 max_depth: int = None, timeout: float = 2, execution_context_id: str = None,
-                                 unique_context: bool = False):
-        """executes a JavaScript on ``GlobalThis`` such as
+            # different target for cross-site
+            targets = await self.__target__.get_targets_for_iframes([self])
+            if targets:
+                return await targets[0]._document_elem
 
-        .. code-block:: js
+    @property
+    async def document_url(self):
+        """gets the url if the element is an iframe, else returns ``None``"""
+        res = await self._describe()
+        return res.get('documentURL')
 
-            function(...arguments){return document}
+    @property
+    async def backend_node_id(self):
+        if not self._backend_node_id:
+            await self._describe()
+        return self._backend_node_id
 
-        ``this`` and ``obj`` refers to ``globalThis`` (=> window) here
+    @property
+    def class_name(self):
+        return self._class_name
 
-        :param script: the script as a string
-        :param args: the argument which are passed to the function. Those can be either json-serializable or a RemoteObject such as WebELement
-        :param await_res: whether to await the function or the return value of it
-        :param serialization: can be one of ``deep``, ``json``, ``idOnly``
-        :param max_depth: The maximum depth objects get serialized.
-        :param timeout: the maximum time to wait for the execution to complete
-        :param execution_context_id: the execution context id to run the JavaScript in. Exclusive with unique_context
-        :param unique_context: whether to use a isolated context to run the Script in.
+    async def find_element(self, by: str, value: str, idx: int = 0, timeout: int or None = None):
+        """find an element in the current target
 
-        see `Runtime.callFunctionOn <https://chromedevtools.github.io/devtools-protocol/tot/Runtime/#method-callFunctionOn>`_
+        :param by: one of the locators at :func:`By <selenium_driverless.types.by.By>`
+        :param value: the actual query to find the element by
+        :param timeout: how long to wait for the element to exist
+        :param idx: might be removed
         """
-
-        if execution_context_id and unique_context:
-            warnings.warn("got execution_context_id and unique_context=True, defaulting to execution_context_id")
-        if unique_context:
-            execution_context_id = await self._isolated_context_id
-
-        if timeout is None:
-            timeout = 2
-
+        elems = []
         start = time.perf_counter()
-        exc = None
-        while (time.perf_counter() - start) > timeout:
-            try:
-                global_this = await self._global_this(execution_context_id)
-                res = await global_this.__exec_raw__(script, *args, await_res=await_res, serialization=serialization,
-                                                    max_depth=max_depth, timeout=timeout,
-                                                    execution_context_id=execution_context_id)
-            except StaleJSRemoteObjReference as e:
-                exc = e
+        while not elems:
+            elems = await self.find_elements(by=by, value=value)
+            if (not timeout) or (time.perf_counter() - start) > timeout:
+                break
+        if elems:
+            if isinstance(elems, list):
+                return elems[idx]
             else:
-                return res
-        if exc:
-            raise exc
-        else:
-            raise asyncio.TimeoutError(f"Couldn't execute script due to stale reference within {timeout} s, "
-                                       f"possibly due to a reload loop")
-
-    async def execute_script(self, script: str, *args, max_depth: int = 2, serialization: str = None,
-                             timeout: float = None, execution_context_id: str = None,
-                             unique_context: bool = None):
-        """executes JavaScript synchronously on ``GlobalThis`` such as
-
-        .. code-block:: js
-
-            return document
-
-        ``this`` and ``obj`` refers to ``globalThis`` (=> window) here
-
-        see :func:`Target.execute_raw_script <selenium_driverless.types.target.Target.execute_raw_script>` for argument descriptions
-        """
-        if execution_context_id and unique_context:
-            warnings.warn("got execution_context_id and unique_context=True, defaulting to execution_context_id")
-        if unique_context:
-            execution_context_id = await self._isolated_context_id
-        if timeout is None:
-            timeout = 2
-
-        start = time.perf_counter()
-        while (time.perf_counter() - start) < timeout:
-            global_this = await self._global_this(execution_context_id)
-            try:
-                res = await global_this.__exec__(script, *args, serialization=serialization,
-                                                 max_depth=max_depth, timeout=timeout,
-                                                 execution_context_id=execution_context_id)
-                return res
-            except StaleJSRemoteObjReference:
-                pass
-        raise asyncio.TimeoutError("Couldn't execute script, possibly due to a reload loop")
-
-    async def execute_async_script(self, script: str, *args, max_depth: int = 2, serialization: str = None,
-                                   timeout: float = None, execution_context_id: str = None,
-                                   unique_context: bool = None):
-        """executes JavaScript asynchronously on ``GlobalThis``
-
-        .. code-block:: js
+                raise Exception("find_elements returned not a list. This possibly is related to https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/84\n", elems)
+        raise NoSuchElementException()
 
-            resolve = arguments[arguments.length-1]
-
-        ``this`` and ``obj`` refers to ``globalThis`` (=> window) here
+    async def find_elements(self, by: str = By.ID, value: str or None = None):
+        """find multiple elements in the current target
 
-        see :func:`Target.execute_raw_script <selenium_driverless.types.target.Target.execute_raw_script>` for argument descriptions
+        :param by: one of the locators at :func:`By <selenium_driverless.types.by.By>`
+        :param value: the actual query to find the elements by
         """
-        if execution_context_id and unique_context:
-            warnings.warn("got execution_context_id and unique_context=True, defaulting to execution_context_id")
-        if unique_context:
-            execution_context_id = await self._isolated_context_id
-        if timeout is None:
-            timeout = 2
-
-        start = time.perf_counter()
-        while (time.perf_counter() - start) < timeout:
-            global_this = await self._global_this(execution_context_id)
-            try:
-                res = await global_this.__exec_async__(script, *args, serialization=serialization,
-                                                       max_depth=max_depth, timeout=timeout,
-                                                       execution_context_id=execution_context_id)
-                return res
-            except StaleJSRemoteObjReference:
-                await asyncio.sleep(0)
-        raise asyncio.TimeoutError("Couldn't execute script, possibly due to a reload loop")
-
-    async def eval_async(self, script: str, *args, max_depth: int = 2, serialization: str = None,
-                         timeout: float = None, execution_context_id: str = None,
-                         unique_context: bool = None):
-        """executes JavaScript asynchronously on ``GlobalThis`` such as
-
-        .. code-block:: js
-
-            res = await fetch("https://httpbin.org/get");
-            // mind CORS!
-            json = await res.json()
-            return json
+        from selenium_driverless.types.by import By
+
+        if by == By.ID:
+            by = By.XPATH
+            value = f'//*[@id="{value}"]'
+        elif by == By.CLASS_NAME:
+            by = By.XPATH
+            value = f'//*[@class="{value}"]'
+        elif by == By.NAME:
+            by = By.XPATH
+            value = f'//*[@name="{value}"]'
+
+        if by == By.TAG_NAME:
+            return await self.execute_script("return obj.getElementsByTagName(arguments[0])",
+                                             value, serialization="deep", unique_context=True, timeout=10)
+        elif by == By.CSS_SELECTOR:
+            return await self.execute_script("return obj.querySelectorAll(arguments[0])", value, timeout=10,
+                                             unique_context=True)
+        elif by == By.XPATH:
+            script = """return document.evaluate(
+                          arguments[0],
+                          obj,
+                          null,
+                          XPathResult.ORDERED_NODE_SNAPSHOT_TYPE,
+                          null,
+                        );"""
+            return await self.execute_script(script, value, serialization="deep", timeout=10, unique_context=True)
+        else:
+            raise ValueError("unexpected by")
 
-        ``this`` refers to ``globalThis`` (=> window)
+    async def _describe(self):
+        args = {"pierce": True}
+        args.update(self._args_builder)
+        res = await self.__target__.execute_cdp_cmd("DOM.describeNode", args)
+        res = res["node"]
+        self._backend_node_id = res["backendNodeId"]
+        self._node_id = res["nodeId"]
+        self.___frame_id__ = res.get("frameId")
+        return res
 
-        see :func:`Target.execute_raw_script <selenium_driverless.types.target.Target.execute_raw_script>` for argument descriptions
+    async def get_listeners(self, depth: int = 3):
         """
-        if execution_context_id and unique_context:
-            warnings.warn("got execution_context_id and unique_context=True, defaulting to execution_context_id")
-        if unique_context:
-            execution_context_id = await self._isolated_context_id
-        if timeout is None:
-            timeout = 2
-
-        start = time.perf_counter()
-        while (time.perf_counter() - start) < timeout:
-            global_this = await self._global_this(execution_context_id)
-            try:
-                res = await global_this.__eval_async__(script, *args, serialization=serialization,
-                                                       max_depth=max_depth, timeout=timeout,
-                                                       execution_context_id=execution_context_id)
-                return res
-            except StaleJSRemoteObjReference:
-                await asyncio.sleep(0)
-        raise asyncio.TimeoutError("Couldn't execute script, possibly due to a reload loop")
+        gets all listeners on the element. see `DOMDebugger.getEventListeners <https://vanilla.aslushnikov.com/?DOMDebugger.getEventListeners>`_
 
-    @property
-    async def current_url(self) -> str:
-        """Gets the URL of the current page.
-
-        :Usage:
-            ::
-
-                target.current_url
+        :param depth: maximum depth (nested elements) to find listeners for
         """
-        target = await self.info
-        return target.url
+        res = await self.__target__.execute_cdp_cmd(
+            "DOMDebugger.getEventListeners", {"objectId": await self.obj_id, "depth": depth, "pierce": True})
+        return res['listeners']
 
     @property
-    async def page_source(self) -> str:
-        """Gets the docs_source of the current page.
-
-        :Usage:
-            ::
-
-                target.page_source
+    async def source(self):
         """
-        elem = await self._document_elem
-        return await elem.source
-
-    async def close(self, timeout: float = 2) -> None:
-        """Closes the current window.
-
-        :Usage:
-            ::
-
-                target.close()
+        **async** the OuterHtml of the element
         """
+        args = self._args_builder
         try:
-            await self.execute_cdp_cmd("Page.close", timeout=timeout)
-            await self._socket.close()
-        except websockets.ConnectionClosedError:
-            pass
+            res = await self.__target__.execute_cdp_cmd("DOM.getOuterHTML", args)
         except CDPError as e:
-            if e.code == -32000 and e.message == 'Command can only be executed on top-level targets':
-                pass
+            if e.code == -32000 and e.message == 'Could not find node with given id':
+                raise StaleElementReferenceException(self)
             else:
                 raise e
-        except (asyncio.TimeoutError, TimeoutError):
-            pass
+        return res["outerHTML"]
 
-    async def focus(self):
-        await self.execute_cdp_cmd("Target.activateTarget",
-                                   {"targetId": self.id})
+    async def set_source(self, value: str):
+        """
+        sets the OuterHTML of the element
+        """
         try:
-            await self.execute_cdp_cmd("Emulation.setFocusEmulationEnabled", {"enabled": True})
+            await self.__target__.execute_cdp_cmd("DOM.setOuterHTML",
+                                                  {"nodeId": await self.node_id, "outerHTML": value})
         except CDPError as e:
-            if not (e.code == -32601 and e.message == "'Emulation.setFocusEmulationEnabled' wasn't found"):
+            if e.code == -32000 and 'Could not find node with given id' in e.message:
+                raise StaleElementReferenceException(self)
+            else:
                 raise e
 
-    @property
-    async def info(self):
-        res = await self.execute_cdp_cmd("Target.getTargetInfo", {"targetId": self.id})
-        return await TargetInfo(res["targetInfo"], self)
+    async def get_property(self, name: str) -> str or None:
+        """Gets the given property of the element.
 
-    @property
-    async def frame_tree(self):
-        try:
-            res = await self.execute_cdp_cmd("Page.getFrameTree")
-            return res["frameTree"]
-        except CDPError as e:
-            if not (e.code == -32601 and e.message == "'Page.getFrameTree' wasn't found"):
-                raise e
+        :param name: the name of the property to get
 
-    @property
-    async def base_frame(self):
-        res = await self.frame_tree
-        if res:
-            return res["frame"]
+        .. warning::
+            this gets the JavaScript property (``elem[name]``), and not HTML property
+        """
+        return await self.execute_script(f"return obj[arguments[0]]", name)
 
     @property
-    async def type(self):
-        if not self._type:
-            info = await self.info
-            self._type = info.type
-        return self._type
+    async def tag_name(self) -> str:
+        """This element's ``tagName`` property."""
+        node = await self._describe()
+        return node["localName"]
 
     @property
-    async def title(self) -> str:
-        # noinspection GrazieInspection
-        """Returns the title of the target"""
-        target = await self.info
-        return target.title
+    async def text(self) -> str:
+        """**async** The text of the element. (``elem.textContent``)"""
+        return await self.get_property("textContent")
 
     @property
-    async def url(self) -> str:
-        info = await self.info
-        return info.url
+    async def value(self) -> str:
+        """**async** The value of the element. (``elem.value``)"""
+        return await self.get_property("value")
 
-    @property
-    async def window_id(self):
-        if not self._window_id:
-            result = await self.execute_cdp_cmd("Browser.getWindowForTarget", {"targetId": self.id})
-            self._window_id = result["windowId"]
-        return self._window_id
+    async def clear(self) -> None:
+        """Clears the text if it's a text entry element. (``elem.value = ""``)
+        """
+        await self.execute_script("obj.value = ''", unique_context=True)
 
-    async def print_page(self) -> str:
-        """Takes PDF of the current page.
+    async def remove(self):
+        """
+        remove the element from the page//dom//html
+        """
+        await self.__target__.execute_cdp_cmd("DOM.removeNode", {"nodeId": await self.node_id})
+
+    async def highlight(self, highlight=True):
+        """
+        highlight the element
+
+        :param highlight: whether to disable or enable highlight
+
+        .. note::
+            highlight automatically fades on any user-interaction, you might use a for-loop
+        """
+        if not self.__target__._dom_enabled:
+            await self.__target__.execute_cdp_cmd("DOM.enable")
+        if highlight:
+            args = self._args_builder
+            args["highlightConfig"] = {
+                "showInfo": True,
+                "borderColor": {
+                    "r": 76, "g": 175, "b": 80, "a": 1
+                },
+                "contentColor": {
+                    "r": 76, "g": 175, "b": 80,
+                    "a": 0.24
+                },
+                "shapeColor": {
+                    "r": 76, "g": 175, "b": 80,
+                    "a": 0.24
+                }
+            }
+            await self.__target__.execute_cdp_cmd("Overlay.enable")
+            await self.__target__.execute_cdp_cmd("Overlay.highlightNode", args)
+        else:
+            await self.__target__.execute_cdp_cmd("Overlay.disable")
 
-        The target makes the best effort to return a PDF based on the
-        provided parameters.
+    async def focus(self):
+        """
+        focuses the element (``Dom.focus``)
+        """
+        args = self._args_builder
+        return await self.__target__.execute_cdp_cmd("DOM.focus", args)
 
-        returns Base64-encoded pdf data as a string
+    async def is_clickable(self, listener_depth=3):
         """
-        page = await self.execute_cdp_cmd("Page.printToPDF")
-        return page["data"]
+        returns ``True`` if the element type is one of "a", "button", "command", "details", "input", "select", "textarea", "video", "map"
+        else wise checks for "click", "mousedown" or "mouseup" event listeners on the element
+
+        :param listener_depth: the depth (nested elements) to get event-listeners for
+        """
+        _type = await self.tag_name
+        if _type in ["a", "button", "command", "details", "input", "select", "textarea", "video", "map"]:
+            return True
+        is_clickable: bool = listener_depth is None
+        if not is_clickable:
+            listeners = await self.get_listeners(depth=listener_depth)
+            for listener in listeners:
+                _type = listener["type"]
+                if _type in ["click", "mousedown", "mouseup"]:
+                    is_clickable = True
+                    break
+        return is_clickable
+
+    async def click(self, timeout: float = None, visible_timeout: float = 30,spread_a: float = 1, spread_b: float = 1, bias_a: float = 0.5, bias_b: float = 0.5, border:float=0.05, scroll_to=True, move_to: bool = True,
+                    ensure_clickable: typing.Union[bool, int] = False) -> None:
+        """Clicks the element.
+
+        :param timeout: the time in seconds to take for clicking on the element
+        :param visible_timeout: the time in seconds to wait for being able to compute the elements box model
+        :param spread_a: spread over a
+        :param spread_b: spread over b
+        :param bias_a: bias over a (0-1)
+        :param bias_b: bias over b (0-1)
+        :param border: minimum border towards element edges (relative to element => 1).
+            Random generated points outside that border get re-generated.
+        :param scroll_to: whether to scroll to the element
+        :param move_to: whether to move the mouse to the element
+        :param ensure_clickable: whether to ensure that the element is clickable. Not reliable in on every webpage
+
+        .. note::
+            a spread of 1 is equivalent to 6 std.
+            relative to the element.
+            (=> 99.7 %)
+        """
+        if scroll_to:
+            await self.scroll_to()
+        cords = None
+        start = time.perf_counter()
+        while not cords:
+            try:
+                cords = await self.mid_location(spread_a, spread_b, bias_a, bias_b, border)
+            except CDPError as e:
+                if e.code == -32000 and 'Could not compute box model.' in e.message:
+                    await asyncio.sleep(0.1)
+                else:
+                    raise e
+            if (time.perf_counter() - start) > visible_timeout:
+                raise asyncio.TimeoutError(f"Couldn't compute element location within {visible_timeout} seconds")
+        x, y = cords
+        if ensure_clickable:
+            is_clickable = await self.is_clickable()
+            if not is_clickable:
+                raise ElementNotClickable(x, y)
 
-    async def get_history(self) -> TypedDict('NavigationHistory', {'currentIndex': int, 'entries': list}):
-        """returns the history data
+        await self.__target__.pointer.click(x, y=y, click_kwargs={"timeout": timeout}, move_to=move_to)
 
-        see `Page.getNavigationHistory <https://chromedevtools.github.io/devtools-protocol/tot/Page/#method-getNavigationHistory>`__
+    async def write(self, text: str,click_kwargs=None, click_on:bool=True):
         """
-        return await self.execute_cdp_cmd("Page.getNavigationHistory")
+        inserts literal text to the element
 
-    # Navigation
-    async def back(self) -> None:
-        """Goes one step backward in the browser history.
+        .. warning::
+
+            This method is generally detectable.
+            You might consider using :func:`Elem.send_keys <selenium_driverless.types.webelement.WebElement.send_keys>` instead.
+
+        :param text: the text to send
+        :param click_kwargs: arguments to pass for :func:`Elem.send_keys <selenium_driverless.types.webelement.WebElement.send_keys>`
+        :param click_on: whether to click on the element before inserting the text
+        """
+        if click_kwargs is None:
+            click_kwargs = {}
+        if click_on:
+            await self.click(**click_kwargs)
+        else:
+            await self.focus()
+        await self.__target__.execute_cdp_cmd("Input.insertText", {"text": text})
+
+    async def set_file(self, path: str):
         """
-        history = await self.get_history()
-        entry = history["entries"][history['currentIndex'] - 1]["id"]
-        await self.execute_cdp_cmd("Page.navigateToHistoryEntry", {"entryId": entry})
-        await self._on_loaded()
+        sets the file on the current element (has to accept files)
 
-    async def forward(self) -> None:
-        """Goes one step forward in the browser history.
+        :param path: the absolute path to the file
         """
-        history = await self.get_history()
-        entry = history["entries"][history["currentIndex"] + 1]["id"]
-        await self.execute_cdp_cmd("Page.navigateToHistoryEntry", {"entryId": entry})
-        await self._on_loaded()
+        await self.set_files([path])
 
-    async def refresh(self) -> None:
-        """Refreshes the page.
+    async def set_files(self, paths: typing.List[str]):
         """
-        await self.execute_cdp_cmd("Page.reload")
-        await self._on_loaded()
+        sets files on the current element (has to accept files)
 
-    # Options
-    async def get_cookies(self) -> List[dict]:
-        """Returns a set of dictionaries, corresponding to cookies visible in
-        the current context.
+        :param paths: the absolute paths to the files
         """
-        return await get_cookies(self)
+        args = {"files": paths}
+        args.update(self._args_builder)
+        await self.__target__.execute_cdp_cmd("DOM.setFileInputFiles", args)
 
-    async def get_cookie(self, name) -> typing.Optional[typing.Dict]:
-        """Get a single cookie by name. Returns the cookie if found, None if
-        not.
+    async def send_keys(self, text: str, click_kwargs:dict=None, click_on:bool=True) -> None:
         """
-        return await get_cookie(target=self, name=name)
+        send text & keys to the target
 
-    async def delete_cookie(self, name: str, url: str = None, domain: str = None, path: str = None) -> None:
-        """Deletes a single cookie with the given name.
+        :param text: the text to send to the target
+        :param click_kwargs: arguments to pass for :func:`Elem.send_keys <selenium_driverless.types.webelement.WebElement.send_keys>`
+        :param click_on: whether to click on the element before sending the keys
         """
-        return await delete_cookie(target=self, url=url, name=name, domain=domain, path=path)
+        if click_kwargs is None:
+            click_kwargs = {}
+        if click_on:
+            await self.click(**click_kwargs)
+        else:
+            await self.focus()
+        await self.__target__.send_keys(text)
 
-    async def delete_all_cookies(self) -> None:
-        """Delete all cookies in the scope of the context.
+    async def mid_location(self, spread_a: float = 1, spread_b: float = 1, bias_a: float = 0.5, bias_b: float = 0.5, border:float=0.05) -> typing.List[int]:
         """
-        return await delete_all_cookies(self)
+        returns random location in the element with probability close to the middle
 
-    # noinspection GrazieInspection
-    async def add_cookie(self, cookie_dict) -> None:
-        """Adds a cookie in the current (incognito-) context
+        :param spread_a: spread over a
+        :param spread_b: spread over b
+        :param bias_a: bias over a (0-1)
+        :param bias_b: bias over b (0-1)
+        :param border: minimum border towards element edges (relative to the element => 1).
+            Random generated points outside that border get re-generated.
 
-        :param cookie_dict: see `Network.CookieParam <https://chromedevtools.github.io/devtools-protocol/tot/Network/#type-CookieParam>`__
+        .. note::
+            a spread of 1 is equivalent to 6 std.
+            relative to the element.
+            (=> 99.7 %)
         """
-        if not (cookie_dict.get("url") or cookie_dict.get("domain") or cookie_dict.get("path")):
-            cookie_dict["url"] = await self.current_url
-        return await add_cookie(target=self, cookie_dict=cookie_dict)
 
-    @property
-    async def _document_elem(self) -> WebElement:
-        if not self._document_elem_:
-            res = await self.execute_cdp_cmd("DOM.getDocument", {"pierce": True})
-            node_id = res["root"]["nodeId"]
-            frame = await self.base_frame
-            frame_id = frame["id"]
-            if self._loop:
-                self._document_elem_ = await SyncWebElement(target=self, node_id=node_id, loop=self._loop,
-                                                            isolated_exec_id=None, frame_id=frame_id)
-            else:
-                self._document_elem_ = await WebElement(target=self, node_id=node_id, loop=self._loop,
-                                                        isolated_exec_id=None, frame_id=frame_id)
-        return self._document_elem_
+        box = await self.box_model
+        vertices = box["content"]
+        point = rand_mid_loc(vertices, spread_a, spread_b, bias_a, bias_b, border)
 
-    # noinspection PyUnusedLocal
-    async def find_element(self, by: str, value: str, parent=None, timeout: int or None = None) -> WebElement:
-        start = time.perf_counter()
-        elem = None
-        while not elem:
-            parent = await self._document_elem
-            try:
-                elem = await parent.find_element(by=by, value=value, timeout=None)
-            except (StaleElementReferenceException, NoSuchElementException, StaleJSRemoteObjReference):
-                await self._on_loaded()
-            if (not timeout) or (time.perf_counter() - start) > timeout:
-                break
-            await asyncio.sleep(0.01)
-        if not elem:
-            raise NoSuchElementException()
-        return elem
-
-    async def find_elements(self, by: str, value: str, parent=None) -> typing.List[WebElement]:
-        if not parent:
-            parent = await self._document_elem
-        return await parent.find_elements(by=by, value=value)
+        # noinspection PyUnboundLocalVariable
+        x = int(point[0])
+        y = int(point[1])
+        return [x, y]
 
-    async def set_source(self, source: str, timeout: float = 15):
-        start = time.perf_counter()
-        while (time.perf_counter() - start) < timeout:
-            try:
-                document = await self._document_elem
-                await document.set_source(source)
-                return
-            except StaleElementReferenceException:
-                await self._on_loaded()
-                await asyncio.sleep(0)
-        raise TimeoutError("Couldn't get document element to not be stale")
-
-    async def search_elements(self, query: str) -> typing.List[WebElement]:
-        """
-        query:str | Plain text or query selector or XPath search query.
-        """
-        # ensure DOM is enabled
-        if not self._dom_enabled:
-            await self.execute_cdp_cmd("DOM.enable")
+    async def submit(self):
+        """Submits a form.
 
-        # ensure DOM.getDocument got called
-        await self._document_elem
+        .. warning::
+            the current implementation likely is detectable. It's recommended to use click instead if possible
+        """
+        script = (
+            "/* submitForm */var form = this;\n"
+            'while (form.nodeName != "FORM" && form.parentNode) {\n'
+            "  form = form.parentNode;\n"
+            "}\n"
+            "if (!form) { throw Error('Unable to find containing form element'); }\n"
+            "if (!form.ownerDocument) { throw Error('Unable to find owning document'); }\n"
+            "var e = form.ownerDocument.createEvent('Event');\n"
+            "e.initEvent('submit', true, true);\n"
+            "if (form.dispatchEvent(e)) { HTMLFormElement.prototype.submit.call(form) }\n"
+        )
+        return await self.execute_script(script, unique_context=True)
 
-        elems = []
-        res = await self.execute_cdp_cmd("DOM.performSearch",
-                                         {"includeUserAgentShadowDOM": True, "query": query})
-        search_id = res["searchId"]
-        elem_count = res["resultCount"]
-        if elem_count <= 0:
-            return []
-
-        res = await self.execute_cdp_cmd("DOM.getSearchResults",
-                                         {"searchId": search_id, "fromIndex": 0, "toIndex": elem_count})
-        for node_id in res["nodeIds"]:
-            if self._loop:
-                elem = await SyncWebElement(target=self, node_id=node_id, loop=self._loop, isolated_exec_id=None,
-                                            frame_id=None)
-            else:
-                elem = await WebElement(target=self, node_id=node_id, loop=self._loop, isolated_exec_id=None,
-                                        frame_id=None)
-            elems.append(elem)
-        return elems
-
-    async def get_screenshot_as_file(self, filename) -> bool:
-        # noinspection GrazieInspection
-        """Saves a screenshot of the current window to a PNG image file.
-                Returns False if there is any IOError, else returns True. Use full
-                paths in your filename.
-
-                :Args:
-                 - filename: The full path you wish to save your screenshot to. This
-                   should end with a `.png` extension.
-
-                :Usage:
-                    ::
-
-                        target.get_screenshot_as_file('/Screenshots/foo.png')
-                """
-        if not str(filename).lower().endswith(".png"):
-            warnings.warn(
-                "name used for saved screenshot does not match file " "type. It should end with a `.png` extension",
-                UserWarning,
-            )
-        png = await self.get_screenshot_as_png()
+    @property
+    async def dom_attributes(self) -> dict:
         try:
-            async with aiofiles.open(filename, "wb") as f:
-                await f.write(png)
-        except OSError:
-            return False
-        finally:
-            del png
-        return True
+            res = await self.__target__.execute_cdp_cmd("DOM.getAttributes", {"nodeId": await self.node_id})
+            attr_list = res["attributes"]
+            attributes_dict = defaultdict(lambda: None)
+
+            for i in range(0, len(attr_list), 2):
+                key = attr_list[i]
+                value = attr_list[i + 1]
+                attributes_dict[key] = value
+            return attributes_dict
+        except CDPError as e:
+            if not (e.code == -32000 and 'Node is not an Element' in e.message):
+                raise e
 
-    async def save_screenshot(self, filename) -> bool:
-        # noinspection GrazieInspection
-        """Saves a screenshot of the current window to a PNG image file.
-                Returns False if there is any IOError, else returns True. Use full
-                paths in your filename.
-
-                :Args:
-                 - filename: The full path you wish to save your screenshot to. This
-                   should end with a `.png` extension.
-
-                :Usage:
-                    ::
-
-                        target.save_screenshot('/Screenshots/foo.png')
-                """
-        return await self.get_screenshot_as_file(filename)
+    async def get_dom_attribute(self, name: str) -> str or None:
+        """Gets the given attribute of the element. Unlike
+        :func:`~selenium.webdriver.remote.BaseWebElement.get_attribute`, this
+        method only returns attributes declared in the element's HTML markup.
 
-    async def get_screenshot_as_png(self) -> bytes:
-        """Gets the screenshot of the current window as a binary data.
+        :Args:
+            - name - Name of the attribute to retrieve.
 
         :Usage:
             ::
 
-                target.get_screenshot_as_png()
+                text_length = target_element.get_dom_attribute("class")
         """
-        base_64 = await self.get_screenshot_as_base64()
-        return b64decode(base_64.encode("ascii"))
+        attrs = await self.dom_attributes
+        return attrs[name]
 
-    async def get_screenshot_as_base64(self) -> str:
-        """Gets the screenshot of the current window as a base64 encoded string
-        which is useful in embedded images in HTML.
+    async def set_dom_attribute(self, name: str, value: str):
+        await self.__target__.execute_cdp_cmd("DOM.setAttributeValue", {"nodeId": await self.node_id,
+                                                                        "name": name, "value": value})
 
-        :Usage:
-            ::
+    async def get_attribute(self, name):
+        """Alias to WebElement.get_property.
 
-                target.get_screenshot_as_base64()
+        .. warning::
+            do not use! This method might change in future
         """
-        res = await self.execute_cdp_cmd("Page.captureScreenshot", {"format": "png"}, timeout=30)
-        return res["data"]
+        return await self.get_property(name)
 
-    async def get_network_conditions(self):
-        """Gets Chromium network emulation settings.
+    async def is_selected(self) -> bool:
+        """Returns whether the element is selected.
 
-        :Returns:
-            A dict. For example:
-            {'latency': 4, 'download_throughput': 2, 'upload_throughput': 2,
-            'offline': False}
-        """
-        raise NotImplementedError("not started with chromedriver")
-
-    async def set_network_conditions(self, offline: bool, latency: int, download_throughput: int,
-                                     upload_throughput: int,
-                                     connection_type: typing.Literal[
-                                         "none", "cellular2g", "cellular3g", "cellular4g", "bluetooth", "ethernet", "wifi", "wimax", "other"]) -> None:
-        """Sets Chromium network emulation settings.
+        Can be used to check if a checkbox or radio button is selected.
+        """
+        result = await self.get_property("checked")
+        if result:
+            return True
+        else:
+            return False
 
-        :Args:
-         - network_conditions: A dict with conditions specification.
+    async def is_enabled(self) -> bool:
+        """Returns whether the element is enabled."""
+        return not await self.get_property("disabled")
 
-        :Usage:
-            ::
+    @property
+    async def shadow_root(self):
+        """the shadowRoot of the element
 
-                target.set_network_conditions(
-                    offline=False,
-                    latency=5,  # additional latency (ms)
-                    download_throughput=500 * 1024,  # maximal throughput
-                    upload_throughput=500 * 1024,  # maximal throughput
-                    connection_type="wifi")
-
-            Note: 'throughput' can be used to set both (for download and upload).
-        """
-        args = {"offline": offline, "latency": latency,
-                "downloadThroughput": download_throughput,
-                "uploadThroughput": upload_throughput}
-
-        conn_types = ["none", "cellular2g", "cellular3g", "cellular4g", "bluetooth", "ethernet", "wifi", "wimax",
-                      "other"]
-        if connection_type:
-            if connection_type not in conn_types:
-                raise ValueError(f"expected {conn_types} for connection_type,  but got {connection_type}")
-            args["connectionType"] = connection_type
-
-        await self.execute_cdp_cmd("Network.emulateNetworkConditions", args)
-
-    async def delete_network_conditions(self) -> None:
-        """Resets Chromium network emulation settings."""
-        raise NotImplementedError("not started with chromedriver")
-
-    async def wait_for_cdp(self, event: str, timeout: float or None = None):
-        if not self.socket:
-            await self._init()
-        return await self.socket.wait_for(event, timeout=timeout)
-
-    async def add_cdp_listener(self, event: str, callback: callable):
-        if not self.socket:
-            await self._init()
-        self.socket.add_listener(method=event, callback=callback)
-
-    async def remove_cdp_listener(self, event: str, callback: callable):
-        if not self.socket:
-            await self._init()
-        self.socket.remove_listener(method=event, callback=callback)
-
-    async def get_cdp_event_iter(self, event: str):
-        if not self.socket:
-            await self._init()
-        return self.socket.method_iterator(method=event)
-
-    async def execute_cdp_cmd(self, cmd: str, cmd_args: dict or None = None,
-                              timeout: float or None = 10) -> dict:
-        """Execute Chrome Devtools Protocol command and get returned result The
-        command and command args should follow chrome devtools protocol
-        domains/commands, refer to link
-        https://chromedevtools.github.io/devtools-protocol/
+        .. warning::
+            this does not support (yet) closed shadow-DOM elements
+        """
+        # todo: move to CDP
+        return await self.execute_script("return obj.shadowRoot")
 
-        :Args:
-         - cmd: A str, command name
-         - cmd_args: A dict, command args. empty dict {} if there is no command args
-        :Usage:
-            ::
+    # RenderedWebElement Items
+    async def is_displayed(self) -> bool:
 
-                target.execute_cdp_cmd('Network.getResponseBody', {'requestId': requestId})
-        :Returns:
-            A dict, empty dict {} if there is no result to return.
-            For example to getResponseBody:
-            {'base64Encoded': False, 'body': 'response body string'}
-        """
-        if not self.socket:
-            await self._init()
-        result = await self.socket.exec(method=cmd, params=cmd_args, timeout=timeout)
-        if cmd == "Page.enable":
-            self._page_enabled = True
-        elif cmd == "Page.disable":
-            self._page_enabled = False
-
-        elif cmd == "DOM.enable":
-            self._dom_enabled = True
-        elif cmd == "DOM.disable":
-            self._dom_enabled = False
-        return result
+        """Whether the element is visible to a user."""
+        try:
+            # Only go into this conditional for browsers that don't use the atom themselves
+            size = await self.size
+            return not (size["height"] == 0 or size["width"] == 0)
+        except CDPError as e:
+            if e.code == -32000 and 'Could not compute box model.' in e.message:
+                return False
+            else:
+                raise e
 
-    # noinspection PyTypeChecker
-    async def get_sinks(self) -> list:
+
+    @property
+    async def location_once_scrolled_into_view(self) -> dict:
         """
-        :Returns: A list of sinks available for Cast.
+        scrolls to the element and returns the coordinates of it
         """
-        await self.execute_cdp_cmd("Cast.enable")
-        raise NotImplementedError("not started with chromedriver")
+        await self.scroll_to()
+        result = await self.rect
+        return {"x": round(result["x"]), "y": round(result["y"])}
 
-    async def get_issue_message(self):
+    async def scroll_to(self, rect: dict = None):
         """
-        :Returns: An error message when there is any issue in a Cast session.
+        scroll to the element
+
+        .. note::
+            this isn't properly implemented yet and might be detectable
         """
-        raise NotImplementedError("not started with chromedriver")
+        args = self._args_builder
+        if rect:
+            args["rect"] = rect
+        try:
+            await self.__target__.execute_cdp_cmd("DOM.scrollIntoViewIfNeeded", args)
+            return True
+        except CDPError as e:
+            if e.code == -32000 and 'Node is detached from document' in e.message:
+                return False
 
-    async def set_sink_to_use(self, sink_name: str) -> dict:
-        """Sets a specific sink, using its name, as a Cast session receiver
-        target.
+    @property
+    async def size(self) -> dict:
+        """**async** The size of the element."""
+        box_model = await self.box_model
+        return {"height": box_model["height"], "width": box_model["width"]}
 
-        :Args:
-         - sink_name: Name of the sink to use as the target.
+    async def value_of_css_property(self, property_name) -> str:
         """
-        return await self.execute_cdp_cmd("Cast.setSinkToUse", {"sinkName": sink_name})
-
-    async def start_desktop_mirroring(self, sink_name: str) -> dict:
-        """Starts a desktop mirroring session on a specific receiver target.
+        .. warning::
+            NotImplemented
 
-        :Args:
-         - sink_name: Name of the sink to use as the target.
         """
-        return await self.execute_cdp_cmd("Cast.startDesktopMirrorin", {"sinkName": sink_name})
+        raise NotImplementedError("you might use javascript instead")
 
-    async def start_tab_mirroring(self, sink_name: str) -> dict:
-        """Starts a tab mirroring session on a specific receiver target.
+    @property
+    async def location(self) -> dict:
+        """The location of the element in the renderable canvas."""
+        result = await self.rect
+        return {"x": round(result["x"]), "y": round(result["y"])}
 
-        :Args:
-         - sink_name: Name of the sink to use as the target.
+    @property
+    async def rect(self) -> dict:
+        """A dictionary with the size and location of the element."""
+        # todo: calculate form DOM.getBoxModel
+        result = await self.execute_script("return obj.getClientRects()[0].toJSON()", serialization="json",
+                                           unique_context=True)
+        return result
+
+    @property
+    async def css_metrics(self):
+        script = """
+            function getRotationAngle(target) 
+                {
+                  const _obj = window.getComputedStyle(target, null);
+                  const matrix = _obj.getPropertyValue('transform');
+                  let angle = 0; 
+                  if (matrix !== 'none') 
+                  {
+                    const values = matrix.split('(')[1].split(')')[0].split(',');
+                    const a = values[0];
+                    const b = values[1];
+                    angle = Math.round(Math.atan2(b, a) * (180/Math.PI));
+                  } 
+                
+                  return (angle < 0) ? angle +=360 : angle;
+                }
+            var _rects = obj.getClientRects()
+            var rects = []
+            for(let i = 0; i < _rects.length; i++){
+                rects.push(_rects[i].toJSON())
+            }
+            var rotation = getRotationAngle(obj)
+            return [rects, rotation]
         """
-        return await self.execute_cdp_cmd("Cast.startTabMirroring", {"sinkName": sink_name})
+        return await self.execute_script(script, max_depth=4)
 
-    async def stop_casting(self, sink_name: str) -> dict:
-        """Stops the existing Cast session on a specific receiver target.
+    @property
+    async def box_model(self) -> dict:
+        """**async** returns the box model of the element. see `DOM.BoxModel <https://vanilla.aslushnikov.com/?DOM.BoxModel>`_
+        """
+        args = self._args_builder
+        try:
+            res = await self.__target__.execute_cdp_cmd("DOM.getBoxModel", args)
+        except CDPError as e:
+            if e.code == -32000 and e.message == 'Cannot find context with specified id':
+                raise StaleElementReferenceException(self)
+            else:
+                raise e
+        model = res['model']
+        keys = ['content', 'padding', 'border', 'margin']
+        for key in keys:
+            quad = model[key]
+            model[key] = np.array([[quad[0], quad[1]], [quad[2], quad[3]], [quad[4], quad[5]], [quad[6], quad[7]]])
+        return model
+
+    @property
+    async def aria_role(self) -> str:
+        """**async** Returns the ARIA role of the current web element."""
+        # todo: move to CDP
+        return await self.get_property("ariaRoleDescription")
+
+    @property
+    async def accessible_name(self) -> str:
+        """**async** Returns the ARIA Level of the current webelement."""
+        # todo: move to CDP
+        return await self.get_property("ariaLevel")
+
+    @property
+    async def screenshot_as_base64(self) -> str:
+        """**async** gets a screenshot as Base64 from the element
+        """
+        element_data = await self.box_model
+
+        x = element_data["content"][0][0]
+        y = element_data["content"][0][1]
+        width = element_data["width"]
+        height = element_data["height"]
+
+        get_image_bas64 = await self.__target__.execute_cdp_cmd("Page.captureScreenshot", {
+            "clip": {
+                "x": int(x),
+                "y": int(y),
+                "width": int(width),
+                "height": int(height),
+                "scale": 1
+            }
+        })
+        return get_image_bas64["data"]
 
-        :Args:
-         - sink_name: Name of the sink to stop the Cast session.
+    @property
+    async def screenshot_as_png(self) -> bytes:
+        """**async** Gets the screenshot of the current element as a binary data.
+        (PNG format)
         """
-        return await self.execute_cdp_cmd("Cast.stopCasting", {"sinkName": sink_name})
+        res = await self.screenshot_as_base64
+        return b64decode(res.encode("ascii"))
 
+    async def screenshot(self, filename) -> bool:
+        """Saves a screenshot of the current element to a PNG image file.
 
-class TargetInfo:
-    """
-    Info for a Target
+        :param filename: path to save the png to
+        """
+        if not filename.lower().endswith(".png"):
+            warnings.warn(
+                "name used for saved screenshot does not match file " "type. It should end with a `.png` extension",
+                UserWarning,
+            )
+        png = await self.screenshot_as_png
+        try:
+            async with aiofiles.open(filename, "wb") as f:
+                await f.write(png)
+        except OSError:
+            return False
+        finally:
+            del png
+        return True
 
-    .. note::
+    @property
+    async def parent(self) -> WebElement:
+        """The parent element this element"""
+        args = {}
+        if self._node_id:
+            args["nodeId"] = self._node_id
+        else:
+            args["objectId"] = await self.obj_id
+        node: dict = await self._describe()
+        node_id = node.get("parentId")
+        if node_id:
+            if self._loop:
+                # noinspection PyUnresolvedReferences
+                return SyncWebElement(node_id=node_id, target=self.__target__, context_id=self.__context_id__,
+                                      isolated_exec_id=self.___isolated_exec_id__, frame_id=await self.__frame_id__)
+            else:
+                # noinspection PyUnresolvedReferences
+                return WebElement(node_id=node_id, target=self.__target__, context_id=self.__context_id__,
+                                  isolated_exec_id=self.___isolated_exec_id__, frame_id=await self.__frame_id__)
 
-        the infos are not dynamic
-    """
+    @property
+    def children(self):
+        return self.find_elements(By.CSS_SELECTOR, "*")
 
-    def __init__(self, target_info: dict, target_getter: asyncio.Future or Target):
-        self._id = target_info.get('targetId')
-        self._type = target_info.get("type")
-        self._title = target_info.get("title")
-        self._url = target_info.get("url")
-        self._attached = target_info.get("attached")
-        self._opener_id = target_info.get("openerId")
-        self._can_access_opener = target_info.get('canAccessOpener')
-        self._opener_frame_id = target_info.get("openerFrameId")
-        self._browser_context_id = target_info.get('browserContextId')
-        self._subtype = target_info.get("subtype")
+    async def execute_raw_script(self, script: str, *args, await_res: bool = False, serialization: str = None,
+                                 max_depth: int = 2, timeout: float = 2, execution_context_id: str = None,
+                                 unique_context: bool = True):
+        return await self.__exec_raw__(script, *args, await_res=await_res, serialization=serialization,
+                                       max_depth=max_depth, timeout=timeout,
+                                       execution_context_id=execution_context_id,
+                                       unique_context=unique_context)
 
-        self._target = target_getter
-        self._started = False
+    async def execute_script(self, script: str, *args, max_depth: int = 2, serialization: str = None,
+                             timeout: float = 2, execution_context_id: str = None, unique_context: bool = True):
+        """executes JavaScript synchronously
 
-    def __await__(self):
-        return self._init().__await__()
+        .. code-block:: js
 
-    async def _init(self):
-        if not self._started:
-            self._started = True
-        return self
+            return document
 
-    # noinspection PyPep8Naming
-    @property
-    def Target(self) -> Target:
-        """
-        the Target itself
+        ``this`` and ``obj`` refers to the element here
+
+        see :func:`Target.execute_raw_script <selenium_driverless.types.target.Target.execute_raw_script>` for argument descriptions
         """
-        return self._target
+        return await self.__exec__(script, *args, max_depth=max_depth, serialization=serialization,
+                                   timeout=timeout, unique_context=unique_context,
+                                   execution_context_id=execution_context_id)
 
-    @property
-    def id(self) -> str:
-        """the ``Target.TargetID``"""
-        return self._id
+    async def execute_async_script(self, script: str, *args, max_depth: int = 2, serialization: str = None,
+                                   timeout: float = 2, execution_context_id: str = None, unique_context: bool = True):
+        """executes JavaScript asynchronously
 
-    @property
-    def type(self) -> str:
-        return self._type
+        .. warning::
+            using execute_async_script is not recommended as it doesn't handle exceptions correctly.
+            Use :func:`Chrome.eval_async <selenium_driverless.webdriver.Chrome.eval_async>`
 
-    @property
-    def title(self) -> str:
-        return self._title
+        .. code-block:: js
 
-    @property
-    def url(self) -> str:
-        return self._url
+            resolve = arguments[arguments.length-1]
 
-    @property
-    def attached(self) -> str:
-        """Whether the target has an attached client."""
-        return self._attached
+        ``this`` refers to ``globalThis`` (=> window)
 
-    @property
-    def opener_id(self) -> str:
-        """Opener ``Target.TargetId``"""
-        return self._opener_id
+        see :func:`Target.execute_raw_script <selenium_driverless.types.target.Target.execute_raw_script>` for argument descriptions
+        """
+        return await self.__exec_async__(script, *args, max_depth=max_depth, serialization=serialization,
+                                         timeout=timeout, unique_context=unique_context,
+                                         execution_context_id=execution_context_id)
 
-    @property
-    def can_access_opener(self):
-        """Whether the target has access to the originating window."""
-        return self._can_access_opener
+    async def eval_async(self, script: str, *args, max_depth: int = 2, serialization: str = None,
+                         timeout: float = None, execution_context_id: str = None,
+                         unique_context: bool = None):
+        """executes JavaScript asynchronously
 
-    @property
-    def opener_frame_id(self):
-        """``Page.FrameId`` of originating window (is only set if target has an opener)."""
-        return self._opener_frame_id
+        .. code-block:: js
 
-    @property
-    def browser_context_id(self):
-        """``Browser.BrowserContextID``"""
-        return self._browser_context_id
+            res = await fetch("https://httpbin.org/get");
+            // mind CORS!
+            json = await res.json()
+            return json
 
-    @property
-    def subtype(self):
-        """Provides additional details for specific target types. For example, for the type of "page", this may be set to "portal" or "prerender"""
-        return self._subtype
+        ``this`` refers to the element
+
+        see :func:`Target.execute_raw_script <selenium_driverless.types.target.Target.execute_raw_script>` for argument descriptions
+        """
+        return await self.__eval_async__(script, *args, max_depth=max_depth, serialization=serialization,
+                                         timeout=timeout, unique_context=unique_context,
+                                         execution_context_id=execution_context_id)
 
     def __repr__(self):
-        return f'{self.__class__.__name__}(type="{self.type}",title="{self.title})"'
+        return (f'{self.__class__.__name__}("{self.class_name}", '
+                f'obj_id={self.__obj_id__}, node_id="{self._node_id}", backend_node_id={self._backend_node_id}, '
+                f'context_id={self.__context_id__})')
+
+    def __eq__(self, other):
+        if isinstance(other, WebElement):
+            if other.__target__ == self.__target__:
+                if other.__obj_id__ and self.__obj_id__:
+                    return other.__obj_id__.split(".")[0] == self.__obj_id__.split(".")[0]
+                elif other._backend_node_id == self._backend_node_id:
+                    return True
+                elif other._node_id == self._node_id:
+                    return True
+        return False
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
```

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/utils/utils.py` & `selenium_driverless-1.9/src/selenium_driverless/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         s.bind((host, 0))
         s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         return s.getsockname()[1]
 
 
 def check_timeout(start_monotonic: float, timeout: float):
     if (time.perf_counter() - start_monotonic) > timeout:
-        raise TimeoutError(f"driver.quit took longer than timeout: {timeout}")
+        raise asyncio.TimeoutError(f"driver.quit took longer than timeout: {timeout}")
 
 
 async def is_first_run():
     path = DATA_DIR + "/is_first_run"
     if os.path.isfile(path):
         res = await read(path, sel_root=False)
         if res == __version__:
```

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless/webdriver.py` & `selenium_driverless-1.9/src/selenium_driverless/webdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,16 +287,14 @@
                     def remove_context():
                         if _id in self._contexts:
                             del self._contexts[_id]
                         self._base_context = None
 
                     # noinspection PyProtectedMember
                     context._closed_callbacks.append(remove_context)
-                    self.base_target.socket.on_closed.append(
-                        lambda code, reason: self.quit(clean_dirs=self._options.auto_clean_dirs))
                     self._current_context = context
                     self._base_context = context
                     self._contexts[_id] = context
                     break
             await self.execute_cdp_cmd("Emulation.setFocusEmulationEnabled", {"enabled": True})
             if self._options.single_proxy:
                 await self.set_single_proxy(self._options.single_proxy)
@@ -487,15 +485,15 @@
                                 r"chrome-extension://(.*)/"
                                 r"driverless_background_mv3_243ffdd55e32a012b4f253b2879af978\.js",
                                 target.url):
                             extension_target = target.Target
                             break
                 if not extension_target:
                     if (time.perf_counter() - start) > timeout:
-                        raise TimeoutError(f"Couldn't find mv3 extension within {timeout} seconds")
+                        raise asyncio.TimeoutError(f"Couldn't find mv3 extension within {timeout} seconds")
             while True:
                 try:
                     # fix WebRTC leak
                     await extension_target.execute_script(
                         "chrome.privacy.network.webRTCIPHandlingPolicy.set(arguments[0])",
                         {"value": "disable_non_proxied_udp"}, timeout=2)
                 except (asyncio.TimeoutError, TimeoutError):
@@ -662,21 +660,27 @@
     @property
     async def title(self) -> str:
         """**async** the title of the current target"""
         target = await self.current_target_info
         return target.title
 
     @property
-    async def current_pointer(self) -> Pointer:
-        """
-        **async** the Pointer of the current Target
-        """
+    def current_pointer(self) -> Pointer:
+        """the :class:`Pointer <selenium_driverless.input.pointer.Pointer>` for this target"""
         target = self.current_target
         return target.pointer
 
+    async def send_keys(self, text: str):
+        """
+        send text & keys to the current target
+
+        :param text: the text to send
+        """
+        await self.current_target.send_keys(text)
+
     async def execute_raw_script(self, script: str, *args, await_res: bool = False,
                                  serialization: typing.Literal["deep", "json", "idOnly"] = "deep",
                                  max_depth: int = None, timeout: int = 2, execution_context_id: str = None,
                                  unique_context: bool = False):
         """executes a JavaScript on ``GlobalThis`` such as
 
         .. code-block:: js
@@ -1432,67 +1436,67 @@
         # provide auth
         mv3_target = await self.mv3_extension
         script = "chrome.webRequest.onAuthRequired.removeListener(globalThis.onAuth);"
         self._auth = {}
         await mv3_target.execute_script(script)
         self._auth_interception_enabled = False
 
-    async def wait_for_cdp(self, event: str, timeout: float or None = None):
+    async def wait_for_cdp(self, event: str, timeout: float or None = None) -> dict:
         """
-        wait for a CDP-event (current target)
-
-        :param event: an even such as ``Page.windowOpen``
-        :param timeout: timeout to wait for the event
+        wait for an event on the current target
+        see :func:`Target.wait_for_cdp <selenium_driverless.types.target.Target.wait_for_cdp>` for reference
         """
         return await self.current_target.wait_for_cdp(event=event, timeout=timeout)
 
     async def add_cdp_listener(self, event: str, callback: typing.Callable[[dict], any]):
-        """add a listener on a CDP event (current target)
-
-        :param event: the name of the event
-        :param callback: the callback on the event
-            has to accept one parameter (event data as json)
+        """
+        add a listener for a CDP event on the current target
+        see :func:`Target.add_cdp_listener <selenium_driverless.types.target.Target.add_cdp_listener>` for reference
         """
         return await self.current_target.add_cdp_listener(event=event, callback=callback)
 
-    async def remove_cdp_listener(self, event: str, callback: callable):
-        """remove a listener for CDP-event (current target)
-
-        :param event: the name of the event
-        :param callback: the callback function to remove
+    async def remove_cdp_listener(self, event: str, callback: typing.Callable[[dict], any]):
+        """
+        remove a listener for a CDP event on the current target
+        see :func:`Target.remove_cdp_listener <selenium_driverless.types.target.Target.remove_cdp_listener>` for reference
         """
-        # todo: documentation from here on
         return await self.current_target.remove_cdp_listener(event=event, callback=callback)
 
-    async def get_cdp_event_iter(self, event: str, target_id: str = None):
+    async def get_cdp_event_iter(self, event: str, target_id: str = None) -> typing.AsyncIterable[dict]:
+        """
+        iterate over CDP events on the current target
+        see :func:`Target.get_cdp_event_iter <selenium_driverless.types.target.Target.get_cdp_event_iter>` for reference
+        """
         target = await self.get_target(target_id=target_id)
         return await target.get_cdp_event_iter(event=event)
 
     async def execute_cdp_cmd(self, cmd: str, cmd_args: dict or None = None,
                               timeout: float or None = 10, target_id: str = None) -> dict:
-        """Execute Chrome Devtools Protocol command and get returned result The
-        command and command args should follow chrome devtools protocol
-        domains/commands, refer to link
-        https://chromedevtools.github.io/devtools-protocol/
-
-        :Args:
-         - cmd: A str, command name
-         - cmd_args: A dict, command args. empty dict {} if there is no command args
-        :Usage:
-            ::
-
-                target.execute_cdp_cmd('Network.getResponseBody', {'requestId': requestId})
-        :Returns:
-            A dict, empty dict {} if there is no result to return.
-            For example to getResponseBody:
-            {'base64Encoded': False, 'body': 'response body string'}
+        """Execute Chrome Devtools Protocol command on the current target
+        executes it on :class:`Target.execute_cdp_cmd <selenium_driverless.types.base_target.BaseTarget>`
+        if ``message:'Not allowed'`` received
+        see :func:`Target.execute_cdp_cmd <selenium_driverless.types.target.Target.execute_cdp_cmd>` for reference
         """
         return await self.current_context.execute_cdp_cmd(cmd=cmd, cmd_args=cmd_args, timeout=timeout,
                                                           target_id=target_id)
 
+    async def fetch(self, *args, **kwargs) -> dict:
+        """
+        executes a JS ``fetch`` request within the current target
+        see :func:`Target.fetch <selenium_driverless.types.target.Target.fetch>` for reference
+        """
+        return await self.current_target.fetch(*args, **kwargs)
+
+    async def xhr(self, *args, **kwargs) -> dict:
+        """
+        executes a JS ``XMLHttpRequest`` request within the current target
+        see :func:`Target.fetch <selenium_driverless.types.target.Target.fetch>` for reference
+        """
+        return await self.current_target.xhr(*args, **kwargs)
+
     # noinspection PyTypeChecker
     async def get_sinks(self, target_id: str = None) -> list:
         """
         :Returns: A list of sinks available for Cast.
         """
         target = await self.get_target(target_id=target_id)
         return await target.get_sinks()
```

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless.egg-info/PKG-INFO` & `selenium_driverless-1.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,48 @@
-Metadata-Version: 2.1
-Name: selenium_driverless
-Version: 1.8.0.2
-Summary: Undetected selenium without chromedriver usage (Non-commercial use only!)
-Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
-Author: Aurin Aegerter
-Author-email: aurinliun@gmx.ch
-License: CC BY-NC-SA 4.0
-Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
-Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
-Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
-Keywords: Selenium,webautomation
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: Free for non-commercial use
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Internet :: Proxy Servers
-Classifier: Topic :: Internet
-Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: selenium~=4.6
-Requires-Dist: cdp-socket>=1.2.5
-Requires-Dist: numpy
-Requires-Dist: matplotlib~=3.5
-Requires-Dist: scipy~=1.7
-Requires-Dist: aiofiles
-Requires-Dist: platformdirs
-Provides-Extra: dev
-Requires-Dist: check-manifest; extra == "dev"
-
-# Selenium-Driverless (Non-commercial use only!)
+# Driverless (Non-commercial use only!)
 
 [![Downloads](https://static.pepy.tech/badge/selenium-driverless)](https://pepy.tech/project/selenium-driverless) [![](https://img.shields.io/pypi/v/selenium-driverless.svg?color=3399EE)](https://pypi.org/project/selenium-driverless/)
 [Documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/#)
 
 
 - Use Selenium __without chromedriver__
 - Currently passes __Cloudflare__, __Bet365__, [Turnstile](https://github.com/kaliiiiiiiiii/Selenium-Driverless/tree/master/dev#bypass-turnstile), and others
 - Multiple tabs simultaneously
-- Multiple Incognito-contexts with individual proxy & cookies
-- Async (`asyncio`) and sync (experimental) support
-- Proxy-auth support (experimental, [example code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/dev/examples/proxy_with_auth.py))
-- Network-interception
-- headless supported
+- Multiple Incognito-contexts with isolated cookies & local storage
+- Proxy-auth support ([example code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/dev/examples/proxy_with_auth.py))
+- Network-interception ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Chrome/RequestInterception/))
+- Single requests ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Target/#selenium_driverless.types.target.Target.fetch))
 
 ### Questions? 
 Feel free to join the [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on **Discord**:)
 
 Also, see [dev-branch](https://github.com/kaliiiiiiiiii/Selenium-Driverless/tree/dev) for the latest implementations.
 <details>
 <summary>dev-installation (click to expand)</summary>
 
 ```shell
 pip uninstall -y selenium-driverless
 pip install https://github.com/kaliiiiiiiiii/Selenium-Driverless/archive/refs/heads/dev.zip
 ```
 </details>
 
-### Still getting detected?
-Feel free to give me a feedback! \
-You're a company and looking for another solution? Maybe **[undetect.io](https://undetect.io/partner/steve)** is smth for you
+<!---
+
+## Sponsors
+
+### [Capsolver](https://capsolver.com/?utm_source=github&utm_medium=banner_github&utm_campaign=selenium-driverless)
+
+[![img.png](assets/capsolver.png)](https://capsolver.com/?utm_source=github&utm_medium=banner_github&utm_campaign=selenium-driverless)
+
+an AI-powered service that provides **automatic captcha solving** capabilities. It supports a range of captcha types,
+including `reCAPTCHA`, `hCaptcha`, and `FunCaptcha`, `AWS Captcha`, `Geetest` and image captcha among others.
+Capsolver offers browser-extensions for ease of use, API integration for developers, and various pricing packages to suit
+different needs.
+
+-->
 
 #### Also, feel free to
 <a href="https://www.buymeacoffee.com/kaliiii">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="https://www.buymeacoffee.com/assets/img/custom_images/black_img.png" />
     <source media="(prefers-color-scheme: light)" srcset="https://www.buymeacoffee.com/assets/img/custom_images/white_img.png" />
     <img alt="Star History Chart" src="https://www.buymeacoffee.com/assets/img/custom_images/black_img.png" />
@@ -97,15 +68,15 @@
 from selenium_driverless.types.by import By
 import asyncio
 
 
 async def main():
     options = webdriver.ChromeOptions()
     async with webdriver.Chrome(options=options) as driver:
-        await driver.get('http://nowsecure.nl#relax')
+        await driver.get('http://nowsecure.nl#relax', wait_load=True)
         await driver.sleep(0.5)
         await driver.wait_for_cdp("Page.domContentEventFired", timeout=15)
         
         # wait 10s for elem to exist
         elem = await driver.find_element(By.XPATH, '/html/body/div[2]/div/main/p[2]/a', timeout=10)
         await elem.click(move_to=True)
 
@@ -148,91 +119,14 @@
 # specify if you don't want to run remote
 # options.add_argument("--remote-debugging-port=2005")
 
 async with webdriver.Chrome(options=options) as driver:
   await driver.get('http://nowsecure.nl#relax', wait_load=True)
 ```
 
-### Network-Interception
-- use CDP events (see [chrome-developer-protocoll](https://chromedevtools.github.io/devtools-protocol/) for possible events) 
-
-**Notes**: synchronous might not work properly
-
-<details>
-<summary>Example Code (Click to expand)</summary>
-
-warning: network interception with `Fetch.enable` might have issues with cross-domain iframes, maximum websocket message size or Font requests.\
-You might try using [`Network.setRequestInterception](https://chromedevtools.github.io/devtools-protocol/tot/Network/#method-setRequestInterception) (officially deprecated) or narrowing the pattern
-
-```python
-import asyncio
-import base64
-import sys
-import time
-import traceback
-
-from cdp_socket.exceptions import CDPError
-from selenium_driverless import webdriver
-
-
-async def on_request(params, global_conn):
-    url = params["request"]["url"]
-    _params = {"requestId": params['requestId']}
-    if params.get('responseStatusCode') in [301, 302, 303, 307, 308]:
-        # redirected request
-        return await global_conn.execute_cdp_cmd("Fetch.continueResponse", _params)
-    else:
-        try:
-            body = await global_conn.execute_cdp_cmd("Fetch.getResponseBody", _params, timeout=1)
-        except CDPError as e:
-            if e.code == -32000 and e.message == 'Can only get response body on requests captured after headers received.':
-                print(params, "\n", file=sys.stderr)
-                traceback.print_exc()
-                await global_conn.execute_cdp_cmd("Fetch.continueResponse", _params)
-            else:
-                raise e
-        else:
-            start = time.perf_counter()
-            body_decoded = base64.b64decode(body['body'])
-
-            # modify body here
-
-            body_modified = base64.b64encode(body_decoded).decode("ascii")
-            fulfill_params = {"responseCode": 200, "body": body_modified, "responseHeaders": params["responseHeaders"]}
-            fulfill_params.update(_params)
-            if params["responseStatusText"] != "":
-                # empty string throws "Invalid http status code or phrase"
-                fulfill_params["responsePhrase"] = params["responseStatusText"]
-
-            _time = time.perf_counter() - start
-            if _time > 0.01:
-                print(f"decoding took long: {_time} s")
-            await global_conn.execute_cdp_cmd("Fetch.fulfillRequest", fulfill_params)
-            print("Mocked response", url)
-
-
-async def main():
-    async with webdriver.Chrome(max_ws_size=2 ** 30) as driver:
-        driver.base_target.socket.on_closed.append(lambda code, reason: print(f"chrome exited"))
-
-        global_conn = driver.base_target
-        await global_conn.execute_cdp_cmd("Fetch.enable",
-                                          cmd_args={"patterns": [{"requestStage": "Response", "urlPattern": "*"}]})
-        await global_conn.add_cdp_listener("Fetch.requestPaused", lambda data: on_request(data, global_conn))
-
-        await driver.get("https://nowsecure.nl/#relax", timeout=60, wait_load=False)
-        while True:
-            # time.sleep(10) # no. cloudflare would hang
-            await asyncio.sleep(10)
-
-
-asyncio.run(main())
-```
-</details>
-
 ## Multiple tabs simultaneously
 Note: asyncio is recommended, threading only works on independent webdriver.Chrome instances.
 
 <details>
 <summary>Example Code (Click to expand)</summary>
 
 ```python
@@ -311,15 +205,15 @@
 
 </details>
 
 ### Pointer Interaction
 see [@master/dev/show_mousemove.py](https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/master/dev/show_mousemove.py) for visualization
 
 ```python
-pointer = await driver.current_pointer
+pointer = driver.current_pointer
 move_kwargs = {"total_time": 0.7, "accel": 2, "smooth_soft": 20}
 
 await pointer.move_to(100, 500)
 await pointer.click(500, 50, move_kwargs=move_kwargs, move_to=True)
 ```
 ### Iframes
 - switch and interact with iframes
```

#### html2text {}

```diff
@@ -1,109 +1,52 @@
-Metadata-Version: 2.1 Name: selenium_driverless Version: 1.8.0.2 Summary:
-Undetected selenium without chromedriver usage (Non-commercial use only!) Home-
-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless Author: Aurin
-Aegerter Author-email: aurinliun@gmx.ch License: CC BY-NC-SA 4.0 Project-URL:
-Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless Project-
-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
-Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
-Keywords: Selenium,webautomation Classifier: Development Status :: 2 - Pre-
-Alpha Classifier: Intended Audience :: Developers Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: License :: Free
-for non-commercial use Classifier: Natural Language :: English Classifier:
-Operating System :: OS Independent Classifier: Topic :: Internet :: Proxy
-Servers Classifier: Topic :: Internet Classifier: Topic :: Internet :: WWW/HTTP
-:: Browsers Requires-Python: >=3.7 Description-Content-Type: text/markdown
-License-File: LICENSE.md Requires-Dist: selenium~=4.6 Requires-Dist: cdp-
-socket>=1.2.5 Requires-Dist: numpy Requires-Dist: matplotlib~=3.5 Requires-
-Dist: scipy~=1.7 Requires-Dist: aiofiles Requires-Dist: platformdirs Provides-
-Extra: dev Requires-Dist: check-manifest; extra == "dev" # Selenium-Driverless
-(Non-commercial use only!) [![Downloads](https://static.pepy.tech/badge/
-selenium-driverless)](https://pepy.tech/project/selenium-driverless) [![]
+# Driverless (Non-commercial use only!) [![Downloads](https://static.pepy.tech/
+badge/selenium-driverless)](https://pepy.tech/project/selenium-driverless) [![]
 (https://img.shields.io/pypi/v/selenium-driverless.svg?color=3399EE)](https://
 pypi.org/project/selenium-driverless/) [Documentation](https://
 kaliiiiiiiiii.github.io/Selenium-Driverless/#) - Use Selenium __without
 chromedriver__ - Currently passes __Cloudflare__, __Bet365__, [Turnstile]
 (https://github.com/kaliiiiiiiiii/Selenium-Driverless/tree/master/dev#bypass-
 turnstile), and others - Multiple tabs simultaneously - Multiple Incognito-
-contexts with individual proxy & cookies - Async (`asyncio`) and sync
-(experimental) support - Proxy-auth support (experimental, [example code]
-(https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/dev/examples/
-proxy_with_auth.py)) - Network-interception - headless supported ### Questions?
-Feel free to join the [Driverless-Community](https://discord.com/invite/
-MzZZjr2ZM3) on **Discord**:) Also, see [dev-branch](https://github.com/
+contexts with isolated cookies & local storage - Proxy-auth support ([example
+code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/dev/examples/
+proxy_with_auth.py)) - Network-interception ([documentation](https://
+kaliiiiiiiiii.github.io/Selenium-Driverless/api/Chrome/RequestInterception/)) -
+Single requests ([documentation](https://kaliiiiiiiiii.github.io/Selenium-
+Driverless/api/Target/#selenium_driverless.types.target.Target.fetch)) ###
+Questions? Feel free to join the [Driverless-Community](https://discord.com/
+invite/MzZZjr2ZM3) on **Discord**:) Also, see [dev-branch](https://github.com/
 kaliiiiiiiiii/Selenium-Driverless/tree/dev) for the latest implementations.
 dev-installation (click to expand) ```shell pip uninstall -y selenium-
 driverless pip install https://github.com/kaliiiiiiiiii/Selenium-Driverless/
-archive/refs/heads/dev.zip ``` ### Still getting detected? Feel free to give me
-a feedback! \ You're a company and looking for another solution? Maybe **
-[undetect.io](https://undetect.io/partner/steve)** is smth for you #### Also,
-feel free to _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]### Dependencies * [Python >= 3.7](https://
-www.python.org/downloads/) * [Google-Chrome](https://www.google.de/chrome/
-) installed (Chromium not tested) ### Installing * Install [Google-Chrome]
-(https://www.google.de/chrome/) * ```pip install selenium-driverless``` ###
-Usage ### with asyncio ```python from selenium_driverless import webdriver from
-selenium_driverless.types.by import By import asyncio async def main(): options
-= webdriver.ChromeOptions() async with webdriver.Chrome(options=options) as
-driver: await driver.get('http://nowsecure.nl#relax') await driver.sleep(0.5)
-await driver.wait_for_cdp("Page.domContentEventFired", timeout=15) # wait 10s
-for elem to exist elem = await driver.find_element(By.XPATH, '/html/body/div
-[2]/div/main/p[2]/a', timeout=10) await elem.click(move_to=True) alert = await
+archive/refs/heads/dev.zip ``` #### Also, feel free to _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]###
+Dependencies * [Python >= 3.7](https://www.python.org/downloads/) * [Google-
+Chrome](https://www.google.de/chrome/) installed (Chromium not tested) ###
+Installing * Install [Google-Chrome](https://www.google.de/chrome/) * ```pip
+install selenium-driverless``` ### Usage ### with asyncio ```python from
+selenium_driverless import webdriver from selenium_driverless.types.by import
+By import asyncio async def main(): options = webdriver.ChromeOptions() async
+with webdriver.Chrome(options=options) as driver: await driver.get('http://
+nowsecure.nl#relax', wait_load=True) await driver.sleep(0.5) await
+driver.wait_for_cdp("Page.domContentEventFired", timeout=15) # wait 10s for
+elem to exist elem = await driver.find_element(By.XPATH, '/html/body/div[2]/
+div/main/p[2]/a', timeout=10) await elem.click(move_to=True) alert = await
 driver.switch_to.alert print(alert.text) await alert.accept() print(await
 driver.title) asyncio.run(main()) ``` ### synchronous asyncified, might be
 buggy ```python from selenium_driverless.sync import webdriver options =
 webdriver.ChromeOptions() with webdriver.Chrome(options=options) as driver:
 driver.get('http://nowsecure.nl#relax') driver.sleep(0.5) driver.wait_for_cdp
 ("Page.domContentEventFired", timeout=15) title = driver.title url =
 driver.current_url source = driver.page_source print(title) ``` ### custom
 debugger address ```python from selenium_driverless import webdriver options =
 webdriver.ChromeOptions() options.debugger_address = "127.0.0.1:2005" # specify
 if you don't want to run remote # options.add_argument("--remote-debugging-
 port=2005") async with webdriver.Chrome(options=options) as driver: await
-driver.get('http://nowsecure.nl#relax', wait_load=True) ``` ### Network-
-Interception - use CDP events (see [chrome-developer-protocoll](https://
-chromedevtools.github.io/devtools-protocol/) for possible events) **Notes**:
-synchronous might not work properly Example Code (Click to expand) warning:
-network interception with `Fetch.enable` might have issues with cross-domain
-iframes, maximum websocket message size or Font requests.\ You might try using
-[`Network.setRequestInterception](https://chromedevtools.github.io/devtools-
-protocol/tot/Network/#method-setRequestInterception) (officially deprecated) or
-narrowing the pattern ```python import asyncio import base64 import sys import
-time import traceback from cdp_socket.exceptions import CDPError from
-selenium_driverless import webdriver async def on_request(params, global_conn):
-url = params["request"]["url"] _params = {"requestId": params['requestId']} if
-params.get('responseStatusCode') in [301, 302, 303, 307, 308]: # redirected
-request return await global_conn.execute_cdp_cmd("Fetch.continueResponse",
-_params) else: try: body = await global_conn.execute_cdp_cmd
-("Fetch.getResponseBody", _params, timeout=1) except CDPError as e: if e.code
-== -32000 and e.message == 'Can only get response body on requests captured
-after headers received.': print(params, "\n", file=sys.stderr)
-traceback.print_exc() await global_conn.execute_cdp_cmd
-("Fetch.continueResponse", _params) else: raise e else: start =
-time.perf_counter() body_decoded = base64.b64decode(body['body']) # modify body
-here body_modified = base64.b64encode(body_decoded).decode("ascii")
-fulfill_params = {"responseCode": 200, "body": body_modified,
-"responseHeaders": params["responseHeaders"]} fulfill_params.update(_params) if
-params["responseStatusText"] != "": # empty string throws "Invalid http status
-code or phrase" fulfill_params["responsePhrase"] = params["responseStatusText"]
-_time = time.perf_counter() - start if _time > 0.01: print(f"decoding took
-long: {_time} s") await global_conn.execute_cdp_cmd("Fetch.fulfillRequest",
-fulfill_params) print("Mocked response", url) async def main(): async with
-webdriver.Chrome(max_ws_size=2 ** 30) as driver:
-driver.base_target.socket.on_closed.append(lambda code, reason: print(f"chrome
-exited")) global_conn = driver.base_target await global_conn.execute_cdp_cmd
-("Fetch.enable", cmd_args={"patterns": [{"requestStage": "Response",
-"urlPattern": "*"}]}) await global_conn.add_cdp_listener("Fetch.requestPaused",
-lambda data: on_request(data, global_conn)) await driver.get("https://
-nowsecure.nl/#relax", timeout=60, wait_load=False) while True: # time.sleep(10)
-# no. cloudflare would hang await asyncio.sleep(10) asyncio.run(main()) ``` ##
-Multiple tabs simultaneously Note: asyncio is recommended, threading only works
-on independent webdriver.Chrome instances. Example Code (Click to expand)
+driver.get('http://nowsecure.nl#relax', wait_load=True) ``` ## Multiple tabs
+simultaneously Note: asyncio is recommended, threading only works on
+independent webdriver.Chrome instances. Example Code (Click to expand)
 ```python from selenium_driverless.sync import webdriver from
 selenium_driverless.utils.utils import read from selenium_driverless import
 webdriver import asyncio async def target_1_handler(target): await target.get
 ('https://abrahamjuliot.github.io/creepjs/') print(await target.title) async
 def target_2_handler(target): await target.get("about:blank") await
 target.execute_script(script=read("/files/js/show_mousemove.js")) await
 target.pointer.move_to(500, 500, total_time=2) async def main(): options =
@@ -123,15 +66,15 @@
 Object.defineProperty(document, "documentElement", { value: proxy }) """ await
 driver.execute_script(script) src = await driver.execute_script("return
 document.documentElement.outerHTML", unique_context=True) mocked = await
 driver.execute_script("return document.documentElement.outerHTML",
 unique_context=False) print(src, mocked) asyncio.run(main()) ``` ### Pointer
 Interaction see [@master/dev/show_mousemove.py](https://github.com/
 kaliiiiiiiiii/Selenium-Driverless/blob/master/dev/show_mousemove.py) for
-visualization ```python pointer = await driver.current_pointer move_kwargs =
+visualization ```python pointer = driver.current_pointer move_kwargs =
 {"total_time": 0.7, "accel": 2, "smooth_soft": 20} await pointer.move_to(100,
 500) await pointer.click(500, 50, move_kwargs=move_kwargs, move_to=True) ```
 ### Iframes - switch and interact with iframes ```python iframes = await
 driver.find_elements(By.TAG_NAME, "iframe") await asyncio.sleep(0.5)
 iframe_document = await iframes[0].content_document #
 iframe_document.find_elements(...) ``` ### use preferences ```python from
 selenium_driverless import webdriver options = webdriver.ChromeOptions() #
```

### Comparing `selenium_driverless-1.8.0.2/src/selenium_driverless.egg-info/SOURCES.txt` & `selenium_driverless-1.9/src/selenium_driverless.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 setup.cfg
 setup.py
 sync_main.py
 .github/dependabot.yml
 .github/workflows/dependency-review.yml
 dev/README.md
 dev/human_like_path.py
-dev/new_elem_calc.py
-dev/random_point_heatmap.py
 dev/assets/bypass_turnstile.mp4
 dev/assets/events_mouse.png
 dev/assets/events_mousepad.png
 dev/assets/heatmap.png
 dev/assets/mouse_path_gen.png
 dev/assets/mousemove_events_gen.png
 dev/assets/mousemove_events_test_sample_based.png
@@ -25,22 +23,18 @@
 dev/assets/real_mouse_path.png
 docs/.buildinfo
 docs/index.html
 docs/objects.inv
 docs/searchindex.js
 docs/.doctrees/environment.pickle
 docs/.doctrees/index.doctree
-docs/.doctrees/classes/Chrome.doctree
-docs/.doctrees/classes/ChromeOptions.doctree
 docs/_modules/index.html
 docs/_modules/selenium_driverless/types/options/index.html
 docs/_modules/selenium_driverless/webdriver/index.html
 docs/_sources/index.rst.txt
-docs/_sources/classes/Chrome.rst.txt
-docs/_sources/classes/ChromeOptions.rst.txt
 docs/_static/_sphinx_javascript_frameworks_compat.js
 docs/_static/basic.css
 docs/_static/doctools.js
 docs/_static/documentation_options.js
 docs/_static/file.png
 docs/_static/jquery.js
 docs/_static/language_data.js
@@ -68,22 +62,18 @@
 docs/_static/css/fonts/lato-normal-italic.woff2
 docs/_static/css/fonts/lato-normal.woff
 docs/_static/css/fonts/lato-normal.woff2
 docs/_static/js/badge_only.js
 docs/_static/js/html5shiv-printshiv.min.js
 docs/_static/js/html5shiv.min.js
 docs/_static/js/theme.js
-docs/classes/Chrome/index.html
-docs/classes/ChromeOptions/index.html
 docs/genindex/index.html
 docs/search/index.html
 docs_source/conf.py
 docs_source/index.rst
-docs_source/classes/Chrome.rst
-docs_source/classes/ChromeOptions.rst
 examples/proxy_with_auth.py
 src/selenium_driverless/__init__.py
 src/selenium_driverless/webdriver.py
 src/selenium_driverless.egg-info/PKG-INFO
 src/selenium_driverless.egg-info/SOURCES.txt
 src/selenium_driverless.egg-info/dependency_links.txt
 src/selenium_driverless.egg-info/requires.txt
@@ -93,14 +83,15 @@
 src/selenium_driverless/files/mv3_extension/driverless_background_mv3_243ffdd55e32a012b4f253b2879af978.js
 src/selenium_driverless/files/mv3_extension/manifest.json
 src/selenium_driverless/input/__init__.py
 src/selenium_driverless/input/pointer.py
 src/selenium_driverless/scripts/__init__.py
 src/selenium_driverless/scripts/driver_utils.py
 src/selenium_driverless/scripts/geometry.py
+src/selenium_driverless/scripts/network_interceptor.py
 src/selenium_driverless/scripts/prefs.py
 src/selenium_driverless/scripts/switch_to.py
 src/selenium_driverless/sync/__init__.py
 src/selenium_driverless/sync/alert.py
 src/selenium_driverless/sync/base_target.py
 src/selenium_driverless/sync/context.py
 src/selenium_driverless/sync/executor.py
```

### Comparing `selenium_driverless-1.8.0.2/tests/bypass_turnstile.py` & `selenium_driverless-1.9/tests/bypass_turnstile.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,45 +9,37 @@
     options = webdriver.ChromeOptions()
     # options.add_argument("--headless=new")
     async with webdriver.Chrome(options=options) as driver:
         await driver.get("https://nopecha.com/demo/turnstile")
         await asyncio.sleep(0.5)
 
         # some random mouse-movements over iframes
-        pointer = await driver.current_pointer
+        pointer = driver.current_pointer
         await pointer.move_to(500, 200, smooth_soft=60, total_time=0.5)
         await pointer.move_to(20, 50, smooth_soft=60, total_time=0.5)
         await pointer.move_to(8, 45, smooth_soft=60, total_time=0.5)
         await pointer.move_to(500, 200, smooth_soft=60, total_time=0.5)
         await pointer.move_to(166, 206, smooth_soft=60, total_time=0.5)
         await pointer.move_to(200, 205, smooth_soft=60, total_time=0.5)
 
         iframes = await driver.find_elements(By.TAG_NAME, "iframe")
         await asyncio.sleep(0.5)
 
         iframe_document = None
         for iframe in iframes:
             # filter out correct iframe document
             iframe_document = await iframe.content_document
-            text = None
             try:
-                elem = await iframe_document.find_element(By.CSS_SELECTOR, "body > div.overlay")
-                text = await elem.text
+                checkbox = await iframe_document.find_element(By.CSS_SELECTOR,
+                                                              "#challenge-stage > div > label > input[type=checkbox]",
+                                                              timeout=5)
             except NoSuchElementException:
                 pass
-            finally:
-                if text:  # 'Only a test.' text
-                    break
-        if not iframe_document:
-            raise Exception("correct target for iframe not found")
-
-        src = await driver.page_source
-        checkbox = await iframe_document.find_element(By.CSS_SELECTOR,
-                                                      "#challenge-stage > div > label > input[type=checkbox]",
-                                                      timeout=20)
-        await checkbox.click(move_to=True)
-        await asyncio.sleep(5)
+            else:
+                await checkbox.click(move_to=True)
+                await asyncio.sleep(1)
+        await asyncio.sleep(2)
         print("saving screenshot")
         await driver.save_screenshot("turnstile_captcha.png")
 
 
 asyncio.run(main())
```

### Comparing `selenium_driverless-1.8.0.2/tests/selenium_detector/selenium_detector.py` & `selenium_driverless-1.9/tests/selenium_detector/selenium_detector.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 async def main():
     options = webdriver.ChromeOptions()
     options.add_argument("--headless=new")
     async with webdriver.Chrome(options=options) as driver:
         await driver.get('https://hmaker.github.io/selenium-detector/')
         elem = await driver.find_element(By.CSS_SELECTOR, "#chromedriver-token")
-        await elem.write(await driver.execute_script('return window.token'))
+        await elem.send_keys(await driver.execute_script('return window.token'))
         elem2 = await driver.find_element(By.CSS_SELECTOR, "#chromedriver-asynctoken")
         async_token = await driver.eval_async('return await window.getAsyncToken()')
-        await elem2.write(async_token)
+        await elem2.send_keys(async_token)
         elem3 = await driver.find_element(By.CSS_SELECTOR, "#chromedriver-test")
         await elem3.click()
         passed = await driver.find_element(By.XPATH, '//*[@id="chromedriver-test-container"]/span')
         text = await passed.text
         assert text == "Passed!"
         print(text)
```

### Comparing `selenium_driverless-1.8.0.2/tests/selenium_detector/sync_selenium_detector.py` & `selenium_driverless-1.9/tests/selenium_detector/sync_selenium_detector.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 options = webdriver.ChromeOptions()
 options.add_argument("--headless=new")
 with webdriver.Chrome(options=options) as driver:
     driver.get('https://hmaker.github.io/selenium-detector/')
     elem = driver.find_element(By.CSS_SELECTOR, "#chromedriver-token")
 
-    elem.write(driver.execute_script('return window.token'))
+    elem.send_keys(driver.execute_script('return window.token'))
     elem2 = driver.find_element(By.CSS_SELECTOR, "#chromedriver-asynctoken")
     async_token = driver.eval_async('return await window.getAsyncToken()')
-    elem2.write(async_token)
+    elem2.send_keys(async_token)
     elem3 = driver.find_element(By.CSS_SELECTOR, "#chromedriver-test")
     elem.execute_script("console.log(arguments); try{throw new Error()} catch(e){console.error(e)}", elem, elem2, elem3, unique_context=False)
     driver.sleep(0.2)
     elem3.click()
     passed = driver.find_element(By.XPATH, '//*[@id="chromedriver-test-container"]/span')
     text = passed.text
     assert text == "Passed!"
```

### Comparing `selenium_driverless-1.8.0.2/tests/show_mousemove.py` & `selenium_driverless-1.9/tests/show_mousemove.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from selenium_driverless import webdriver
 from selenium_driverless.utils.utils import read
 from selenium_driverless.types.by import By
 import asyncio
+import aiodebug.log_slow_callbacks
+
+aiodebug.log_slow_callbacks.enable(0.05)
 
 
 async def main():
     options = webdriver.ChromeOptions()
     async with webdriver.Chrome(options=options) as driver:
         await driver.get("about:blank")
         await driver.execute_script(script=await read("/files/js/show_mousemove.js", sel_root=True))
         elem = await driver.find_element(By.ID, "clear")
-        pointer = await driver.current_pointer
+        pointer = driver.current_pointer
 
         move_kwargs = {"total_time": 0.7, "accel": 2, "smooth_soft": 20}
         await driver.execute_cdp_cmd("Emulation.setFocusEmulationEnabled", {"enabled": True})
 
         for _ in range(50):
             await pointer.click(100, 500, move_kwargs=move_kwargs, move_to=True)
             await asyncio.sleep(0)
```

### Comparing `selenium_driverless-1.8.0.2/tests/target_interception.py` & `selenium_driverless-1.9/tests/target_interception.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import asyncio
 from selenium_driverless import webdriver
 import sys
+import aiodebug.log_slow_callbacks
+
+aiodebug.log_slow_callbacks.enable(0.05)
 
 global driver
 
 handler = (lambda e: print(f'Exception in event-handler:\n{e.__class__.__module__}.{e.__class__.__name__}: {e}',
                            file=sys.stderr))
 sys.modules["selenium_driverless"].EXC_HANDLER = handler
 sys.modules["cdp_socket"].EXC_HANDLER = handler
@@ -27,11 +30,13 @@
         await driver.base_target.execute_cdp_cmd("Target.setAutoAttach",
                                                  {"autoAttach": True, "waitForDebuggerOnStart": True, "flatten": True})
         await driver.base_target.add_cdp_listener("Target.attachedToTarget", attached_callback)
         await driver.base_target.add_cdp_listener("Target.targetDestroyed", print)
         url = "https://abrahamjuliot.github.io/creepjs/tests/workers.html"
         await driver.get(url)
         await driver.switch_to.new_window(url=url)
-        input("press ENTER to exit: ")
+        a = True
+        while a:
+            await asyncio.sleep(2)
 
 
 asyncio.run(main())
```

### Comparing `selenium_driverless-1.8.0.2/tests/test_driverless.py` & `selenium_driverless-1.9/tests/test_driverless.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 loop = asyncio.get_event_loop()
 
 
 async def make_driver():
     options = webdriver.ChromeOptions()
     # options.add_argument("--headless=new")
+    # options.binary_location = "D:/System/Lib/Chrome/chrome.exe"
     return await webdriver.Chrome(options, debug=True)
 
 
 async def nowsecure(driver):
     async def get_elem():
         return await driver.find_element(By.XPATH, "/html/body/div[2]/div/main/p[2]/a", timeout=2)
     await driver.focus()
@@ -61,18 +62,18 @@
     await click_login()
 
 
 async def selenium_detector(driver):
     await driver.get('https://hmaker.github.io/selenium-detector/')
     await asyncio.sleep(1)
     elem = await driver.find_element(By.CSS_SELECTOR, "#chromedriver-token")
-    await elem.write(await driver.execute_script('return window.token'))
+    await elem.send_keys(await driver.execute_script('return window.token'))
     elem2 = await driver.find_element(By.CSS_SELECTOR, "#chromedriver-asynctoken")
     async_token = await driver.eval_async('return await window.getAsyncToken()')
-    await elem2.write(async_token)
+    await elem2.send_keys(async_token)
     elem3 = await driver.find_element(By.CSS_SELECTOR, "#chromedriver-test")
     await elem3.click()
     passed = await driver.find_element(By.XPATH, '//*[@id="chromedriver-test-container"]/span')
     text = await passed.text
     assert text == "Passed!"
```

