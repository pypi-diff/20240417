# Comparing `tmp/aideml-0.0.1.tar.gz` & `tmp/aideml-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aideml-0.0.1.tar", last modified: Tue Jan 30 15:13:56 2024, max compression
+gzip compressed data, was "aideml-0.1.0.tar", last modified: Wed Apr 17 15:15:49 2024, max compression
```

## Comparing `aideml-0.0.1.tar` & `aideml-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,114 @@
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-01-30 15:13:56.100777 aideml-0.0.1/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      487 2024-01-30 15:13:56.100621 aideml-0.0.1/PKG-INFO
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      116 2024-01-30 15:13:14.000000 aideml-0.0.1/README.md
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-01-30 15:13:56.099924 aideml-0.0.1/aideml/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)        0 2024-01-30 15:13:14.000000 aideml-0.0.1/aideml/__init__.py
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-01-30 15:13:56.100472 aideml-0.0.1/aideml.egg-info/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      487 2024-01-30 15:13:56.000000 aideml-0.0.1/aideml.egg-info/PKG-INFO
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      172 2024-01-30 15:13:56.000000 aideml-0.0.1/aideml.egg-info/SOURCES.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)        1 2024-01-30 15:13:56.000000 aideml-0.0.1/aideml.egg-info/dependency_links.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)        7 2024-01-30 15:13:56.000000 aideml-0.0.1/aideml.egg-info/top_level.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      457 2024-01-30 15:13:42.000000 aideml-0.0.1/pyproject.toml
--rw-r--r--   0 yuxiangwu   (501) staff       (20)       38 2024-01-30 15:13:56.100814 aideml-0.0.1/setup.cfg
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      524 2024-01-30 15:13:51.000000 aideml-0.0.1/setup.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:15:49.441960 aideml-0.1.0/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3120 2024-04-17 15:10:16.000000 aideml-0.1.0/.gitignore
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1068 2024-04-17 15:10:16.000000 aideml-0.1.0/LICENSE
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    23814 2024-04-17 15:15:49.441798 aideml-0.1.0/PKG-INFO
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    23360 2024-04-17 15:10:16.000000 aideml-0.1.0/README.md
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:15:49.430269 aideml-0.1.0/aide/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1892 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/__init__.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    14729 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/agent.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:15:49.430768 aideml-0.1.0/aide/backend/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1941 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/backend/__init__.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1968 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/backend/backend_anthropic.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2272 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/backend/backend_openai.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1703 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/backend/utils.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:15:49.428579 aideml-0.1.0/aide/example_tasks/
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:15:49.430921 aideml-0.1.0/aide/example_tasks/bitcoin_price/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    41966 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/example_tasks/bitcoin_price/BTC-USD.csv
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:15:49.431796 aideml-0.1.0/aide/example_tasks/house_prices/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    13370 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/example_tasks/house_prices/data_description.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    31939 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/example_tasks/house_prices/sample_submission.csv
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)   451405 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/example_tasks/house_prices/test.csv
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)   460676 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/example_tasks/house_prices/train.csv
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    11106 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/interpreter.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     7065 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/journal.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1278 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/journal2report.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4059 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/run.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:15:49.432991 aideml-0.1.0/aide/utils/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3322 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/utils/__init__.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     5371 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/utils/config.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1376 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/utils/config.yaml
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     5266 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/utils/data_preview.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2284 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/utils/metric.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2755 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/utils/response.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1463 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/utils/serialize.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2406 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/utils/tree_export.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:15:49.433255 aideml-0.1.0/aide/utils/viz_templates/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1675 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/utils/viz_templates/template.html
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     8969 2024-04-17 15:10:16.000000 aideml-0.1.0/aide/utils/viz_templates/template.js
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:15:49.434058 aideml-0.1.0/aideml.egg-info/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    23814 2024-04-17 15:15:49.000000 aideml-0.1.0/aideml.egg-info/PKG-INFO
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4040 2024-04-17 15:15:49.000000 aideml-0.1.0/aideml.egg-info/SOURCES.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)        1 2024-04-17 15:15:49.000000 aideml-0.1.0/aideml.egg-info/dependency_links.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)       38 2024-04-17 15:15:49.000000 aideml-0.1.0/aideml.egg-info/entry_points.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      849 2024-04-17 15:15:49.000000 aideml-0.1.0/aideml.egg-info/requires.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)        5 2024-04-17 15:15:49.000000 aideml-0.1.0/aideml.egg-info/top_level.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1049 2024-04-17 15:10:16.000000 aideml-0.1.0/requirements.txt
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:15:49.441619 aideml-0.1.0/sample_results/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2086 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/bike-sharing-demand.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1649 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/career-con-2019.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2645 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/cat-in-the-dat-ii.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1822 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/cat-in-the-dat.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2150 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/ciphertext-challenge-ii.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1115 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/ciphertext-challenge-iii.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2560 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/competitive-data-science-predict-future-sales.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2451 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/digit-recognizer.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1657 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/dont-overfit-ii.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3290 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/facial-keypoints-detection.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1017 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/forest-cover-type-prediction.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2670 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/godaddy-microbusiness-density-forecasting.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2072 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/home-data-for-ml-course.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2574 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/house-prices-advanced-regression-techniques.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1928 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/icr-identify-age-related-conditions.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1206 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/jigsaw-toxic-comment-classification-challenge.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3571 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/new-york-city-taxi-fare-prediction.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1207 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/nlp-getting-started.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1857 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/optiver-trading-at-the-close.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1824 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e1.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      990 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e11.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2077 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e13.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2101 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e14.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1759 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e15.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2940 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e16.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2299 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e17.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3109 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e18.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2568 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e19.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2077 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e20.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2086 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e22.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2254 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e23.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3368 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e24.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2063 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e25.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2001 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e26.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2069 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e3.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1292 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e5.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1217 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e7.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1102 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s3e9.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1917 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s4e1.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2087 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/playground-series-s4e2.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3855 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/santa-2019-revenge-of-the-accountants.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1609 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/scrabble-player-rating.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1887 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/sentiment-analysis-on-movie-reviews.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2413 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/spaceship-titanic.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1868 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-apr-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1533 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-apr-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1370 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-aug-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2479 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-aug-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1114 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-dec-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2330 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-feb-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2088 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-feb-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1145 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-jan-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2594 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-jan-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3354 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-jul-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1506 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-jul-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1721 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-jun-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1397 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-jun-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1885 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-mar-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1740 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-mar-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1106 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-may-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1308 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-may-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1819 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-oct-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2421 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-oct-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1234 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-sep-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2244 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tabular-playground-series-sep-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3410 2024-04-17 15:10:16.000000 aideml-0.1.0/sample_results/tmdb-box-office-prediction.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)       38 2024-04-17 15:15:49.442005 aideml-0.1.0/setup.cfg
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1104 2024-04-17 15:14:42.000000 aideml-0.1.0/setup.py
```

