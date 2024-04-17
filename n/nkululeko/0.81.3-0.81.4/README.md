# Comparing `tmp/nkululeko-0.81.3.tar.gz` & `tmp/nkululeko-0.81.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.81.3.tar", last modified: Tue Apr 16 14:07:48 2024, max compression
+gzip compressed data, was "nkululeko-0.81.4.tar", last modified: Wed Apr 17 14:41:08 2024, max compression
```

## Comparing `nkululeko-0.81.3.tar` & `nkululeko-0.81.4.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.790954 nkululeko-0.81.3/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16523 2024-04-16 12:34:42.000000 nkululeko-0.81.3/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.81.3/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34664 2024-04-16 14:07:48.790954 nkululeko-0.81.3/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16870 2024-03-18 08:28:24.000000 nkululeko-0.81.3/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.778954 nkululeko-0.81.3/data/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/aesdd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.81.3/data/aesdd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/androids/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.81.3/data/androids/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/androids_orig/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.81.3/data/androids_orig/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/androids_test/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.81.3/data/androids_test/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/ased/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/ased/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/asvp-esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.81.3/data/asvp-esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/baved/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.81.3/data/baved/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/cafe/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.81.3/data/cafe/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/clac/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.81.3/data/clac/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/cmu-mosei/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.81.3/data/cmu-mosei/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/crema-d/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3281 2023-06-13 12:24:10.000000 nkululeko-0.81.3/data/crema-d/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/demos/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/ekorpus/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.81.3/data/ekorpus/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/emns/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/emns/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/emofilm/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.81.3/data/emofilm/convert_to_16k.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.81.3/data/emofilm/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/emorynlp/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.81.3/data/emorynlp/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/emov-db/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.81.3/data/emov-db/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/emovo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/emovo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/emozionalmente/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.81.3/data/emozionalmente/create.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/enterface/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/enterface/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.81.3/data/esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/gerparas/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.81.3/data/gerparas/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/iemocap/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.81.3/data/iemocap/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/jl/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.81.3/data/jl/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/jtes/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.81.3/data/jtes/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/meld/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/meld/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/mesd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/mesd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/mess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/mess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/mlendsnd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.81.3/data/mlendsnd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/msp-improv/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.81.3/data/msp-improv/process_database2.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/msp-podcast/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.81.3/data/msp-podcast/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/oreau2/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/oreau2/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/portuguese/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.81.3/data/portuguese/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/ravdess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3327 2023-08-31 07:30:49.000000 nkululeko-0.81.3/data/ravdess/process_database.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.81.3/data/ravdess/process_database_speaker.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/savee/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/savee/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/shemo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/shemo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/subesco/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/subesco/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/tess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.81.3/data/tess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/thorsten-emotional/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.81.3/data/thorsten-emotional/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/urdu/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/urdu/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/vivae/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.81.3/data/vivae/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.778954 nkululeko-0.81.3/docs/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/docs/source/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3072 2024-03-13 09:14:20.000000 nkululeko-0.81.3/docs/source/conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.778954 nkululeko-0.81.3/meta/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/meta/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.81.3/meta/demos/demo_best_model.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/meta/demos/multiple_exeriments/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1043 2022-04-12 11:25:08.000000 nkululeko-0.81.3/meta/demos/multiple_exeriments/do_experiments.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3871 2022-08-30 17:14:03.000000 nkululeko-0.81.3/meta/demos/multiple_exeriments/parse_nkulu.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.81.3/meta/demos/my_experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.81.3/meta/demos/my_experiment_local.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.81.3/meta/demos/plot_faster_anim.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.786954 nkululeko-0.81.3/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.81.3/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.81.3/nkululeko/aug_train.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.81.3/nkululeko/augment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.786954 nkululeko-0.81.3/nkululeko/augmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.81.3/nkululeko/augmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.81.3/nkululeko/augmenting/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.81.3/nkululeko/augmenting/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.81.3/nkululeko/augmenting/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3335 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/augmenting/resampler.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.786954 nkululeko-0.81.3/nkululeko/autopredict/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.81.3/nkululeko/autopredict/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_age.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_arousal.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_dominance.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_gender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_pesq.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_sdr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_stoi.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_valence.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4818 2023-09-26 13:42:48.000000 nkululeko-0.81.3/nkululeko/autopredict/estimate_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.81.3/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-04-16 12:34:59.000000 nkululeko-0.81.3/nkululeko/constants.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.786954 nkululeko-0.81.3/nkululeko/data/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.81.3/nkululeko/data/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27265 2024-03-27 10:33:18.000000 nkululeko-0.81.3/nkululeko/data/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3407 2024-02-28 17:49:47.000000 nkululeko-0.81.3/nkululeko/data/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2500 2024-03-14 10:49:21.000000 nkululeko-0.81.3/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.81.3/nkululeko/demo_feats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4733 2024-04-15 11:33:44.000000 nkululeko-0.81.3/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    29575 2024-03-18 15:37:11.000000 nkululeko-0.81.3/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2250 2024-02-29 11:07:16.000000 nkululeko-0.81.3/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.81.3/nkululeko/export.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.786954 nkululeko-0.81.3/nkululeko/feat_extract/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.81.3/nkululeko/feat_extract/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3192 2024-03-12 12:44:04.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3346 2024-04-16 13:29:59.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_agender_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11399 2024-01-24 16:15:03.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3108 2024-03-12 12:44:04.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3078 2024-03-12 12:44:04.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3379 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5205 2023-10-20 09:59:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_hubert.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1598 2024-03-11 08:25:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4149 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4140 2023-10-16 17:04:58.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4734 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3039 2023-12-15 13:29:14.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2771 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3656 2023-11-16 12:12:10.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_spectra.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_spkrec.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4521 2024-02-20 12:42:26.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_squim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3211 2024-02-29 15:42:20.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5072 2024-02-15 14:59:43.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4683 2024-03-14 11:24:49.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_wavlm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1375 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.81.3/nkululeko/feat_extract/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7281 2023-12-19 11:16:14.000000 nkululeko-0.81.3/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.81.3/nkululeko/file_checker.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.81.3/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      453 2024-02-28 17:38:08.000000 nkululeko-0.81.3/nkululeko/glob_conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.786954 nkululeko-0.81.3/nkululeko/losses/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.81.3/nkululeko/losses/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.81.3/nkululeko/losses/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.81.3/nkululeko/losses/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9337 2024-02-26 18:28:01.000000 nkululeko-0.81.3/nkululeko/modelrunner.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.790954 nkululeko-0.81.3/nkululeko/models/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.81.3/nkululeko/models/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11648 2024-04-16 11:54:27.000000 nkululeko-0.81.3/nkululeko/models/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      378 2023-12-23 10:35:03.000000 nkululeko-0.81.3/nkululeko/models/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9726 2024-04-16 11:54:29.000000 nkululeko-0.81.3/nkululeko/models/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      645 2023-09-26 13:42:48.000000 nkululeko-0.81.3/nkululeko/models/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      573 2023-09-07 11:38:13.000000 nkululeko-0.81.3/nkululeko/models/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      580 2023-09-07 11:38:09.000000 nkululeko-0.81.3/nkululeko/models/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      392 2023-12-19 13:57:23.000000 nkululeko-0.81.3/nkululeko/models/model_lin_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9107 2024-04-16 11:54:31.000000 nkululeko-0.81.3/nkululeko/models/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10083 2024-04-16 13:48:13.000000 nkululeko-0.81.3/nkululeko/models/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      867 2024-03-21 10:56:45.000000 nkululeko-0.81.3/nkululeko/models/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      699 2024-03-21 10:56:18.000000 nkululeko-0.81.3/nkululeko/models/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      390 2023-09-07 11:38:37.000000 nkululeko-0.81.3/nkululeko/models/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      397 2023-09-07 11:38:33.000000 nkululeko-0.81.3/nkululeko/models/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-03-21 10:21:07.000000 nkululeko-0.81.3/nkululeko/models/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      227 2023-12-14 15:14:23.000000 nkululeko-0.81.3/nkululeko/models/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5732 2024-03-11 14:48:46.000000 nkululeko-0.81.3/nkululeko/multidb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1966 2024-02-28 17:41:34.000000 nkululeko-0.81.3/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23025 2024-02-01 14:55:26.000000 nkululeko-0.81.3/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1876 2023-12-19 11:16:14.000000 nkululeko-0.81.3/nkululeko/predict.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.790954 nkululeko-0.81.3/nkululeko/reporting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.81.3/nkululeko/reporting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.81.3/nkululeko/reporting/defines.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.81.3/nkululeko/reporting/latex_writer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/reporting/report.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.81.3/nkululeko/reporting/report_item.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12670 2024-04-16 13:43:47.000000 nkululeko-0.81.3/nkululeko/reporting/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.81.3/nkululeko/reporting/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2233 2024-03-14 15:08:12.000000 nkululeko-0.81.3/nkululeko/resample.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7461 2024-04-16 11:54:24.000000 nkululeko-0.81.3/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.81.3/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.81.3/nkululeko/segment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.790954 nkululeko-0.81.3/nkululeko/segmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.81.3/nkululeko/segmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.81.3/nkululeko/segmenting/seg_inaspeechsegmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/segmenting/seg_silero.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.81.3/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1486 2024-03-18 15:18:33.000000 nkululeko-0.81.3/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2695 2024-03-18 15:40:15.000000 nkululeko-0.81.3/nkululeko/test_predictor.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.790954 nkululeko-0.81.3/nkululeko/utils/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.81.3/nkululeko/utils/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.81.3/nkululeko/utils/files.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2788 2023-12-19 11:26:19.000000 nkululeko-0.81.3/nkululeko/utils/stats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12330 2024-03-21 11:06:05.000000 nkululeko-0.81.3/nkululeko/utils/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.790954 nkululeko-0.81.3/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34664 2024-04-16 14:07:48.000000 nkululeko-0.81.3/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5144 2024-04-16 14:07:48.000000 nkululeko-0.81.3/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-04-16 14:07:48.000000 nkululeko-0.81.3/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-04-16 14:07:48.000000 nkululeko-0.81.3/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-04-16 14:07:48.000000 nkululeko-0.81.3/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.81.3/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-04-16 14:07:48.790954 nkululeko-0.81.3/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.81.3/setup.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.778954 nkululeko-0.81.3/venv/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.790954 nkululeko-0.81.3/venv/bin/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.81.3/venv/bin/activate_this.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.208378 nkululeko-0.81.4/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16604 2024-04-17 13:03:49.000000 nkululeko-0.81.4/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.81.4/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34745 2024-04-17 14:41:08.208378 nkululeko-0.81.4/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16870 2024-03-18 08:28:24.000000 nkululeko-0.81.4/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.196378 nkululeko-0.81.4/data/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/aesdd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.81.4/data/aesdd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/androids/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.81.4/data/androids/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/androids_orig/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.81.4/data/androids_orig/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/androids_test/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.81.4/data/androids_test/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/ased/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.81.4/data/ased/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/asvp-esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.81.4/data/asvp-esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/baved/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.81.4/data/baved/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/cafe/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.81.4/data/cafe/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/clac/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.81.4/data/clac/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/cmu-mosei/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.81.4/data/cmu-mosei/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/crema-d/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3281 2023-06-13 12:24:10.000000 nkululeko-0.81.4/data/crema-d/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.81.4/data/demos/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/ekorpus/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.81.4/data/ekorpus/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/emns/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.81.4/data/emns/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/emofilm/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.81.4/data/emofilm/convert_to_16k.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.81.4/data/emofilm/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/emorynlp/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.81.4/data/emorynlp/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/emov-db/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.81.4/data/emov-db/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/emovo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.81.4/data/emovo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/emozionalmente/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.81.4/data/emozionalmente/create.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/enterface/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.81.4/data/enterface/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.81.4/data/esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/gerparas/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.81.4/data/gerparas/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/iemocap/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.81.4/data/iemocap/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/jl/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.81.4/data/jl/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/jtes/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.81.4/data/jtes/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/meld/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.81.4/data/meld/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/mesd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.81.4/data/mesd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/mess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.81.4/data/mess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/mlendsnd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.81.4/data/mlendsnd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/msp-improv/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.81.4/data/msp-improv/process_database2.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/msp-podcast/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.81.4/data/msp-podcast/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/oreau2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.81.4/data/oreau2/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/portuguese/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.81.4/data/portuguese/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/ravdess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3327 2023-08-31 07:30:49.000000 nkululeko-0.81.4/data/ravdess/process_database.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.81.4/data/ravdess/process_database_speaker.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/savee/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.81.4/data/savee/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/shemo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.81.4/data/shemo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/subesco/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.81.4/data/subesco/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/tess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.81.4/data/tess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/thorsten-emotional/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.81.4/data/thorsten-emotional/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/urdu/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.81.4/data/urdu/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/data/vivae/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.81.4/data/vivae/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.196378 nkululeko-0.81.4/docs/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/docs/source/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3072 2024-03-13 09:14:20.000000 nkululeko-0.81.4/docs/source/conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/meta/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/meta/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.81.4/meta/demos/demo_best_model.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.204378 nkululeko-0.81.4/meta/demos/multiple_exeriments/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1043 2022-04-12 11:25:08.000000 nkululeko-0.81.4/meta/demos/multiple_exeriments/do_experiments.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3871 2022-08-30 17:14:03.000000 nkululeko-0.81.4/meta/demos/multiple_exeriments/parse_nkulu.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.81.4/meta/demos/my_experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.81.4/meta/demos/my_experiment_local.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.81.4/meta/demos/plot_faster_anim.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.204378 nkululeko-0.81.4/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.81.4/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.81.4/nkululeko/aug_train.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.81.4/nkululeko/augment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.204378 nkululeko-0.81.4/nkululeko/augmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.81.4/nkululeko/augmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.81.4/nkululeko/augmenting/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.81.4/nkululeko/augmenting/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.81.4/nkululeko/augmenting/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3335 2023-12-19 11:16:16.000000 nkululeko-0.81.4/nkululeko/augmenting/resampler.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.204378 nkululeko-0.81.4/nkululeko/autopredict/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.81.4/nkululeko/autopredict/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.81.4/nkululeko/autopredict/ap_age.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.4/nkululeko/autopredict/ap_arousal.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.81.4/nkululeko/autopredict/ap_dominance.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.81.4/nkululeko/autopredict/ap_gender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.81.4/nkululeko/autopredict/ap_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.81.4/nkululeko/autopredict/ap_pesq.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.81.4/nkululeko/autopredict/ap_sdr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.81.4/nkululeko/autopredict/ap_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.81.4/nkululeko/autopredict/ap_stoi.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.4/nkululeko/autopredict/ap_valence.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4818 2023-09-26 13:42:48.000000 nkululeko-0.81.4/nkululeko/autopredict/estimate_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.81.4/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-04-17 13:48:24.000000 nkululeko-0.81.4/nkululeko/constants.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.204378 nkululeko-0.81.4/nkululeko/data/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.81.4/nkululeko/data/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27295 2024-04-17 13:34:27.000000 nkululeko-0.81.4/nkululeko/data/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3407 2024-02-28 17:49:47.000000 nkululeko-0.81.4/nkululeko/data/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2500 2024-03-14 10:49:21.000000 nkululeko-0.81.4/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.81.4/nkululeko/demo_feats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4733 2024-04-15 11:33:44.000000 nkululeko-0.81.4/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    29575 2024-04-17 13:01:44.000000 nkululeko-0.81.4/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2250 2024-02-29 11:07:16.000000 nkululeko-0.81.4/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.81.4/nkululeko/export.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.208378 nkululeko-0.81.4/nkululeko/feat_extract/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.81.4/nkululeko/feat_extract/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3192 2024-03-12 12:44:04.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3346 2024-04-16 13:29:59.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_agender_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11399 2024-01-24 16:15:03.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3108 2024-03-12 12:44:04.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3094 2024-04-17 13:43:57.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3379 2023-12-19 11:16:16.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5205 2023-10-20 09:59:16.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_hubert.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1598 2024-03-11 08:25:16.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4149 2023-12-19 11:16:16.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4140 2023-10-16 17:04:58.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4734 2023-12-19 11:16:16.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3039 2023-12-15 13:29:14.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2771 2023-12-19 11:16:16.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3656 2023-11-16 12:12:10.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_spectra.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_spkrec.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4521 2024-02-20 12:42:26.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_squim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3211 2024-02-29 15:42:20.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5072 2024-02-15 14:59:43.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4683 2024-03-14 11:24:49.000000 nkululeko-0.81.4/nkululeko/feat_extract/feats_wavlm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1375 2023-12-19 11:16:16.000000 nkululeko-0.81.4/nkululeko/feat_extract/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.81.4/nkululeko/feat_extract/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7281 2023-12-19 11:16:14.000000 nkululeko-0.81.4/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.81.4/nkululeko/file_checker.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.81.4/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      453 2024-02-28 17:38:08.000000 nkululeko-0.81.4/nkululeko/glob_conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.208378 nkululeko-0.81.4/nkululeko/losses/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.81.4/nkululeko/losses/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.81.4/nkululeko/losses/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.81.4/nkululeko/losses/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9335 2024-04-17 13:01:44.000000 nkululeko-0.81.4/nkululeko/modelrunner.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.208378 nkululeko-0.81.4/nkululeko/models/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.81.4/nkululeko/models/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11569 2024-04-17 13:01:47.000000 nkululeko-0.81.4/nkululeko/models/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      378 2023-12-23 10:35:03.000000 nkululeko-0.81.4/nkululeko/models/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9726 2024-04-16 11:54:29.000000 nkululeko-0.81.4/nkululeko/models/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      645 2023-09-26 13:42:48.000000 nkululeko-0.81.4/nkululeko/models/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      573 2023-09-07 11:38:13.000000 nkululeko-0.81.4/nkululeko/models/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      580 2023-09-07 11:38:09.000000 nkululeko-0.81.4/nkululeko/models/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      392 2023-12-19 13:57:23.000000 nkululeko-0.81.4/nkululeko/models/model_lin_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9107 2024-04-16 11:54:31.000000 nkululeko-0.81.4/nkululeko/models/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10083 2024-04-16 13:48:13.000000 nkululeko-0.81.4/nkululeko/models/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      914 2024-04-17 12:17:54.000000 nkululeko-0.81.4/nkululeko/models/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      699 2024-03-21 10:56:18.000000 nkululeko-0.81.4/nkululeko/models/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      390 2023-09-07 11:38:37.000000 nkululeko-0.81.4/nkululeko/models/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      397 2023-09-07 11:38:33.000000 nkululeko-0.81.4/nkululeko/models/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-03-21 10:21:07.000000 nkululeko-0.81.4/nkululeko/models/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      227 2023-12-14 15:14:23.000000 nkululeko-0.81.4/nkululeko/models/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5732 2024-03-11 14:48:46.000000 nkululeko-0.81.4/nkululeko/multidb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1966 2024-02-28 17:41:34.000000 nkululeko-0.81.4/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23025 2024-02-01 14:55:26.000000 nkululeko-0.81.4/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1924 2024-04-17 13:35:31.000000 nkululeko-0.81.4/nkululeko/predict.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.208378 nkululeko-0.81.4/nkululeko/reporting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.81.4/nkululeko/reporting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.81.4/nkululeko/reporting/defines.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.81.4/nkululeko/reporting/latex_writer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.81.4/nkululeko/reporting/report.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.81.4/nkululeko/reporting/report_item.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12670 2024-04-16 13:43:47.000000 nkululeko-0.81.4/nkululeko/reporting/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.81.4/nkululeko/reporting/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2233 2024-04-17 13:34:59.000000 nkululeko-0.81.4/nkululeko/resample.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7461 2024-04-16 11:54:24.000000 nkululeko-0.81.4/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.81.4/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.81.4/nkululeko/segment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.208378 nkululeko-0.81.4/nkululeko/segmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.81.4/nkululeko/segmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.81.4/nkululeko/segmenting/seg_inaspeechsegmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.81.4/nkululeko/segmenting/seg_silero.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.81.4/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1486 2024-03-18 15:18:33.000000 nkululeko-0.81.4/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2695 2024-03-18 15:40:15.000000 nkululeko-0.81.4/nkululeko/test_predictor.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.208378 nkululeko-0.81.4/nkululeko/utils/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.81.4/nkululeko/utils/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.81.4/nkululeko/utils/files.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2788 2023-12-19 11:26:19.000000 nkululeko-0.81.4/nkululeko/utils/stats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12330 2024-03-21 11:06:05.000000 nkululeko-0.81.4/nkululeko/utils/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.208378 nkululeko-0.81.4/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34745 2024-04-17 14:41:08.000000 nkululeko-0.81.4/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5144 2024-04-17 14:41:08.000000 nkululeko-0.81.4/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-04-17 14:41:08.000000 nkululeko-0.81.4/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-04-17 14:41:08.000000 nkululeko-0.81.4/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-04-17 14:41:08.000000 nkululeko-0.81.4/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.81.4/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-04-17 14:41:08.208378 nkululeko-0.81.4/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.81.4/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.200378 nkululeko-0.81.4/venv/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-17 14:41:08.208378 nkululeko-0.81.4/venv/bin/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.81.4/venv/bin/activate_this.py
```

### Comparing `nkululeko-0.81.3/CHANGELOG.md` & `nkululeko-0.81.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+Version 0.81.4
+--------------
+* fixed bug in demo module
+* removed [MODEL] save
+
 Version 0.81.3
 --------------
 * added confidence intervals to result reporting
 
 Version 0.81.2
 --------------
 * added a parselmouth.Praat error if pitch out of range
```

### Comparing `nkululeko-0.81.3/LICENSE` & `nkululeko-0.81.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/PKG-INFO` & `nkululeko-0.81.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.81.3
+Version: 0.81.4
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -319,14 +319,19 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.81.4
+--------------
+* fixed bug in demo module
+* removed [MODEL] save
+
 Version 0.81.3
 --------------
 * added confidence intervals to result reporting
 
 Version 0.81.2
 --------------
 * added a parselmouth.Praat error if pitch out of range
```

### Comparing `nkululeko-0.81.3/README.md` & `nkululeko-0.81.4/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/aesdd/process_database.py` & `nkululeko-0.81.4/data/aesdd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/androids/process_database.py` & `nkululeko-0.81.4/data/androids/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/androids_orig/process_database.py` & `nkululeko-0.81.4/data/androids_orig/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/androids_test/process_database.py` & `nkululeko-0.81.4/data/androids_test/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/ased/process_database.py` & `nkululeko-0.81.4/data/ased/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/asvp-esd/process_database.py` & `nkululeko-0.81.4/data/asvp-esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/baved/process_database.py` & `nkululeko-0.81.4/data/baved/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/cafe/process_database.py` & `nkululeko-0.81.4/data/cafe/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/clac/process_database.py` & `nkululeko-0.81.4/data/clac/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/cmu-mosei/process_database.py` & `nkululeko-0.81.4/data/cmu-mosei/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/crema-d/process_database.py` & `nkululeko-0.81.4/data/crema-d/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/demos/process_database.py` & `nkululeko-0.81.4/data/demos/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/ekorpus/process_database.py` & `nkululeko-0.81.4/data/ekorpus/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/emns/process_database.py` & `nkululeko-0.81.4/data/emns/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/emofilm/convert_to_16k.py` & `nkululeko-0.81.4/data/emofilm/convert_to_16k.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/emofilm/process_database.py` & `nkululeko-0.81.4/data/emofilm/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/emorynlp/process_database.py` & `nkululeko-0.81.4/data/emorynlp/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/emov-db/process_database.py` & `nkululeko-0.81.4/data/emov-db/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/emovo/process_database.py` & `nkululeko-0.81.4/data/emovo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/emozionalmente/create.py` & `nkululeko-0.81.4/data/emozionalmente/create.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/enterface/process_database.py` & `nkululeko-0.81.4/data/enterface/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/esd/process_database.py` & `nkululeko-0.81.4/data/esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/gerparas/process_database.py` & `nkululeko-0.81.4/data/gerparas/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/iemocap/process_database.py` & `nkululeko-0.81.4/data/iemocap/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/jl/process_database.py` & `nkululeko-0.81.4/data/jl/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/jtes/process_database.py` & `nkululeko-0.81.4/data/jtes/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/meld/process_database.py` & `nkululeko-0.81.4/data/meld/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/mesd/process_database.py` & `nkululeko-0.81.4/data/mesd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/mess/process_database.py` & `nkululeko-0.81.4/data/mess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/mlendsnd/process_database.py` & `nkululeko-0.81.4/data/mlendsnd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/msp-improv/process_database2.py` & `nkululeko-0.81.4/data/msp-improv/process_database2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/msp-podcast/process_database.py` & `nkululeko-0.81.4/data/msp-podcast/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/oreau2/process_database.py` & `nkululeko-0.81.4/data/oreau2/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/portuguese/process_database.py` & `nkululeko-0.81.4/data/portuguese/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/ravdess/process_database.py` & `nkululeko-0.81.4/data/ravdess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/ravdess/process_database_speaker.py` & `nkululeko-0.81.4/data/ravdess/process_database_speaker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/savee/process_database.py` & `nkululeko-0.81.4/data/savee/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/shemo/process_database.py` & `nkululeko-0.81.4/data/shemo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/subesco/process_database.py` & `nkululeko-0.81.4/data/subesco/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/tess/process_database.py` & `nkululeko-0.81.4/data/tess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/thorsten-emotional/process_database.py` & `nkululeko-0.81.4/data/thorsten-emotional/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/urdu/process_database.py` & `nkululeko-0.81.4/data/urdu/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/data/vivae/process_database.py` & `nkululeko-0.81.4/data/vivae/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/docs/source/conf.py` & `nkululeko-0.81.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/meta/demos/demo_best_model.py` & `nkululeko-0.81.4/meta/demos/demo_best_model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/meta/demos/multiple_exeriments/do_experiments.py` & `nkululeko-0.81.4/meta/demos/multiple_exeriments/do_experiments.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/meta/demos/multiple_exeriments/parse_nkulu.py` & `nkululeko-0.81.4/meta/demos/multiple_exeriments/parse_nkulu.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/meta/demos/my_experiment.py` & `nkululeko-0.81.4/meta/demos/my_experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/meta/demos/my_experiment_local.py` & `nkululeko-0.81.4/meta/demos/my_experiment_local.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/meta/demos/plot_faster_anim.py` & `nkululeko-0.81.4/meta/demos/plot_faster_anim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/aug_train.py` & `nkululeko-0.81.4/nkululeko/aug_train.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/augment.py` & `nkululeko-0.81.4/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/augmenting/augmenter.py` & `nkululeko-0.81.4/nkululeko/augmenting/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/augmenting/randomsplicer.py` & `nkululeko-0.81.4/nkululeko/augmenting/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/augmenting/randomsplicing.py` & `nkululeko-0.81.4/nkululeko/augmenting/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/augmenting/resampler.py` & `nkululeko-0.81.4/nkululeko/augmenting/resampler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/autopredict/ap_age.py` & `nkululeko-0.81.4/nkululeko/autopredict/ap_age.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/autopredict/ap_arousal.py` & `nkululeko-0.81.4/nkululeko/autopredict/ap_arousal.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/autopredict/ap_dominance.py` & `nkululeko-0.81.4/nkululeko/autopredict/ap_dominance.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/autopredict/ap_gender.py` & `nkululeko-0.81.4/nkululeko/autopredict/ap_gender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/autopredict/ap_mos.py` & `nkululeko-0.81.4/nkululeko/autopredict/ap_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/autopredict/ap_pesq.py` & `nkululeko-0.81.4/nkululeko/autopredict/ap_pesq.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/autopredict/ap_sdr.py` & `nkululeko-0.81.4/nkululeko/autopredict/ap_sdr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/autopredict/ap_snr.py` & `nkululeko-0.81.4/nkululeko/autopredict/ap_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/autopredict/ap_stoi.py` & `nkululeko-0.81.4/nkululeko/autopredict/ap_stoi.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/autopredict/ap_valence.py` & `nkululeko-0.81.4/nkululeko/autopredict/ap_valence.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/autopredict/estimate_snr.py` & `nkululeko-0.81.4/nkululeko/autopredict/estimate_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/cacheddataset.py` & `nkululeko-0.81.4/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/data/dataset.py` & `nkululeko-0.81.4/nkululeko/data/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,16 @@
             glob_conf.report.add_item(ReportItem("Data", "Load report", r_string))
             glob_conf.report.initial = False
 
     def load(self):
         """Load the dataframe with files, speakers and task labels"""
         # store the dataframe
         store = self.util.get_path("store")
-        store_file = f"{store}{self.name}"
         store_format = self.util.config_val("FEATS", "store_format", "pkl")
+        store_file = f"{store}{self.name}.{store_format}"
         self.root = self._load_db()
         if not self.start_fresh and os.path.isfile(store_file):
             self.util.debug(f"{self.name}: reusing previously stored file {store_file}")
             self.df = self.util.get_store(store_file, store_format)
             self.is_labeled = self.target in self.df
             self.got_gender = "gender" in self.df
             self.got_age = "age" in self.df
@@ -237,15 +237,15 @@
             self.df[self.target] = scaler.fit_transform(
                 self.df[self.target].values.reshape(-1, 1)
             )
 
         # store the dataframe
         store = self.util.get_path("store")
         store_format = self.util.config_val("FEATS", "store_format", "pkl")
-        store_file = f"{store}{self.name}"
+        store_file = f"{store}{self.name}.{store_format}"
         self.util.write_store(self.df, store_file, store_format)
 
     def _get_df_for_lists(self, db, df_files):
         is_labeled, got_speaker, got_gender, got_age = (
             False,
             False,
             False,
```

### Comparing `nkululeko-0.81.3/nkululeko/data/dataset_csv.py` & `nkululeko-0.81.4/nkululeko/data/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/demo.py` & `nkululeko-0.81.4/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/demo_feats.py` & `nkululeko-0.81.4/nkululeko/demo_feats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/demo_predictor.py` & `nkululeko-0.81.4/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/experiment.py` & `nkululeko-0.81.4/nkululeko/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -681,15 +681,15 @@
         f = open(filename, "rb")
         tmp_dict = pickle.load(f)
         f.close()
         self.__dict__.update(tmp_dict)
         glob_conf.set_labels(self.labels)
 
     def save(self, filename):
-        if self.runmgr.modelrunner.model.is_ANN():
+        if self.runmgr.modelrunner.model.is_ann():
             self.runmgr.modelrunner.model = None
             self.util.warn(
                 f"Save experiment: Can't pickle the learning model so saving without it."
             )
         try:
             f = open(filename, "wb")
             pickle.dump(self.__dict__, f)
@@ -704,15 +704,15 @@
             )
         except (AttributeError, RuntimeError) as error:
             self.util.warn(f"Save experiment: Can't pickle local object: {error}")
 
     def save_onnx(self, filename):
         # export the model to onnx
         model = self.runmgr.get_best_model()
-        if model.is_ANN():
+        if model.is_ann():
             print("converting to onnx from torch")
         else:
             from skl2onnx import to_onnx
 
             print("converting to onnx from sklearn")
         # save the rest
         f = open(filename, "wb")
```

### Comparing `nkululeko-0.81.3/nkululeko/explore.py` & `nkululeko-0.81.4/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/export.py` & `nkululeko-0.81.4/nkululeko/export.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_agender.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_agender_agender.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_agender_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_analyser.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_audmodel.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_audmodel_dim.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_audmodel_dim.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # feats_audmodel_dim.py
-from nkululeko.feat_extract.featureset import Featureset
 import os
+
+import numpy as np
 import pandas as pd
+import torch
+
 import audeer
-import nkululeko.glob_conf as glob_conf
-import audonnx
-import numpy as np
 import audinterface
+import audonnx
+
+from nkululeko.feat_extract.featureset import Featureset
+import nkululeko.glob_conf as glob_conf
 
 
 class AudModelDimSet(Featureset):
     """
     Emotional dimensions from the wav2vec2. based model finetuned on MSPPodcast emotions, described in the paper
     "Dawn of the transformer era in speech emotion recognition: closing the valence gap"
     https://arxiv.org/abs/2203.07378
```

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_clap.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_hubert.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_hubert.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_import.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_mld.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_mos.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_opensmile.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_oxbow.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_praat.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_snr.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_spectra.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_spectra.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_spkrec.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_spkrec.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_squim.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_squim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_trill.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_wav2vec2.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feats_wavlm.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feats_wavlm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/featureset.py` & `nkululeko-0.81.4/nkululeko/feat_extract/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feat_extract/feinberg_praat.py` & `nkululeko-0.81.4/nkululeko/feat_extract/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/feature_extractor.py` & `nkululeko-0.81.4/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/file_checker.py` & `nkululeko-0.81.4/nkululeko/file_checker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/filter_data.py` & `nkululeko-0.81.4/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/losses/loss_ccc.py` & `nkululeko-0.81.4/nkululeko/losses/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/losses/loss_softf1loss.py` & `nkululeko-0.81.4/nkululeko/losses/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/modelrunner.py` & `nkululeko-0.81.4/nkululeko/modelrunner.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     def do_epochs(self):
         # initialze results
         reports = []
         plot_epochs = self.util.config_val("PLOT", "epochs", False)
         only_test = self.util.config_val("MODEL", "only_test", False)
         epoch_num = int(self.util.config_val("EXP", "epochs", 1))
-        if not self.model.is_ANN() and epoch_num > 1:
+        if not self.model.is_ann() and epoch_num > 1:
             self.util.warn(f"setting epoch num to 1 (was {epoch_num}) if model not ANN")
             epoch_num = 1
             glob_conf.config["EXP"]["epochs"] = "1"
         patience = self.util.config_val("MODEL", "patience", False)
         patience_counter = -1
         if self.util.high_is_good():
             highest = 0
@@ -65,15 +65,15 @@
             self.util.debug(
                 f"run: {self.run} epoch: {epoch}: result: "
                 f"{reports[-1].get_result().get_test_result()}"
             )
             if plot_epochs:
                 self.util.debug(f"plotting conf matrix to {plot_name}")
                 report.plot_confmatrix(plot_name, epoch)
-            store_models = self.util.config_val("MODEL", "save", False)
+            store_models = self.util.config_val("EXP", "save", False)
             plot_best_model = self.util.config_val("PLOT", "best_model", False)
             if (store_models or plot_best_model) and (
                 not only_test
             ):  # in any case the model needs to be stored to disk.
                 self.model.store()
             if patience:
                 patience = int(patience)
```

### Comparing `nkululeko-0.81.3/nkululeko/models/model.py` & `nkululeko-0.81.4/nkululeko/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # model.py
-from nkululeko.utils.util import Util
-import pandas as pd
-import numpy as np
-import nkululeko.glob_conf as glob_conf
-import sklearn.utils
-from nkululeko.reporting.reporter import Reporter
 import ast
-from sklearn.model_selection import GridSearchCV
 import pickle
 import random
+
+import numpy as np
+import pandas as pd
+from sklearn.model_selection import GridSearchCV
 from sklearn.model_selection import LeaveOneGroupOut
 from sklearn.model_selection import StratifiedKFold
+import sklearn.utils
+
+import nkululeko.glob_conf as glob_conf
+from nkululeko.reporting.reporter import Reporter
+from nkululeko.utils.util import Util
 
 
 class Model:
-    """Generic model class for linear (non-neural) algorithms"""
+    """Generic model class for linear (non-neural) algorithms."""
 
     def __init__(self, df_train, df_test, feats_train, feats_test):
-        """Constructor taking the configuration and all dataframes"""
+        """Constructor taking the configuration and all dataframes."""
         self.df_train, self.df_test, self.feats_train, self.feats_test = (
             df_train,
             df_test,
             feats_train,
             feats_test,
         )
         self.model_type = "classic"
@@ -31,15 +33,15 @@
         self.epoch = 0
         self.logo = self.util.config_val("MODEL", "logo", False)
         self.xfoldx = self.util.config_val("MODEL", "k_fold_cross", False)
 
     def set_model_type(self, type):
         self.model_type = type
 
-    def is_ANN(self):
+    def is_ann(self):
         if self.model_type == "ann":
             return True
         else:
             return False
 
     def set_testdata(self, data_df, feats_df):
         self.df_test, self.feats_test = data_df, feats_df
@@ -273,16 +275,14 @@
         return "generic"
 
     def predict_sample(self, features):
         """Predict one sample"""
         prediction = {}
         if self.util.exp_is_classification():
             # get the class probabilities
-            if not self.get_type() == "xgb":
-                features = [features]
             predictions = self.clf.predict_proba(features)
             # pred = self.clf.predict(features)
             for i in range(len(self.clf.classes_)):
                 cat = self.clf.classes_[i]
                 prediction[cat] = predictions[0][i]
         else:
             predictions = self.clf.predict(features)
@@ -298,14 +298,14 @@
         dir = self.util.get_path("model_dir")
         name = f"{self.util.get_exp_name(only_train=True)}_{self.run}_{self.epoch:03d}.model"
         try:
             with open(dir + name, "rb") as handle:
                 self.clf = pickle.load(handle)
         except FileNotFoundError as fe:
             self.util.error(
-                f"did you forget to store your models? needs: \n[MODEL]\nsave=True\n{fe}"
+                f"Did you forget to store your models? needs: \n[MODEL]\nsave=True\n{fe}"
             )
 
     def load_path(self, path, run, epoch):
         self.set_id(run, epoch)
         with open(path, "rb") as handle:
             self.clf = pickle.load(handle)
```

### Comparing `nkululeko-0.81.3/nkululeko/models/model_cnn.py` & `nkululeko-0.81.4/nkululeko/models/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/models/model_gmm.py` & `nkululeko-0.81.4/nkululeko/models/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/models/model_knn.py` & `nkululeko-0.81.4/nkululeko/models/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/models/model_knn_reg.py` & `nkululeko-0.81.4/nkululeko/models/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/models/model_mlp.py` & `nkululeko-0.81.4/nkululeko/models/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/models/model_mlp_regression.py` & `nkululeko-0.81.4/nkululeko/models/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/models/model_svm.py` & `nkululeko-0.81.4/nkululeko/models/model_svm.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,10 +21,13 @@
             kernel=kernel,
             C=c,
             gamma="scale",
             probability=True,
             class_weight=class_weight,
         )  # set up the classifier
 
-    def set_C(self, c):
-        """Set the C parameter"""
+    def set_c(self, c):
+        """Set the C parameter."""
         self.clf.C = c
+
+    def get_type(self):
+        return "svm"
```

### Comparing `nkululeko-0.81.3/nkululeko/models/model_svr.py` & `nkululeko-0.81.4/nkululeko/models/model_svr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/multidb.py` & `nkululeko-0.81.4/nkululeko/multidb.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/nkululeko.py` & `nkululeko-0.81.4/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/plots.py` & `nkululeko-0.81.4/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/predict.py` & `nkululeko-0.81.4/nkululeko/predict.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,17 @@
         exit()
 
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
     # create a new experiment
     expr = Experiment(config)
-    util = Util("predict")
+    module = "predict"
+    expr.set_module(module)
+    util = Util(module)
     util.debug(
         f"running {expr.name} from config {config_file}, nkululeko version"
         f" {VERSION}"
     )
 
     # load the data
     expr.load_datasets()
```

### Comparing `nkululeko-0.81.3/nkululeko/reporting/defines.py` & `nkululeko-0.81.4/nkululeko/reporting/defines.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/reporting/latex_writer.py` & `nkululeko-0.81.4/nkululeko/reporting/latex_writer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/reporting/report.py` & `nkululeko-0.81.4/nkululeko/reporting/report.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/reporting/report_item.py` & `nkululeko-0.81.4/nkululeko/reporting/report_item.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/reporting/reporter.py` & `nkululeko-0.81.4/nkululeko/reporting/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/reporting/result.py` & `nkululeko-0.81.4/nkululeko/reporting/result.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/resample.py` & `nkululeko-0.81.4/nkululeko/resample.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/runmanager.py` & `nkululeko-0.81.4/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/scaler.py` & `nkululeko-0.81.4/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/segment.py` & `nkululeko-0.81.4/nkululeko/segment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/segmenting/seg_inaspeechsegmenter.py` & `nkululeko-0.81.4/nkululeko/segmenting/seg_inaspeechsegmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/segmenting/seg_silero.py` & `nkululeko-0.81.4/nkululeko/segmenting/seg_silero.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/syllable_nuclei.py` & `nkululeko-0.81.4/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/test.py` & `nkululeko-0.81.4/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/test_predictor.py` & `nkululeko-0.81.4/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/utils/files.py` & `nkululeko-0.81.4/nkululeko/utils/files.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/utils/stats.py` & `nkululeko-0.81.4/nkululeko/utils/stats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko/utils/util.py` & `nkululeko-0.81.4/nkululeko/utils/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.81.4/nkululeko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.81.3
+Version: 0.81.4
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -319,14 +319,19 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.81.4
+--------------
+* fixed bug in demo module
+* removed [MODEL] save
+
 Version 0.81.3
 --------------
 * added confidence intervals to result reporting
 
 Version 0.81.2
 --------------
 * added a parselmouth.Praat error if pitch out of range
```

### Comparing `nkululeko-0.81.3/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.81.4/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/setup.cfg` & `nkululeko-0.81.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.3/venv/bin/activate_this.py` & `nkululeko-0.81.4/venv/bin/activate_this.py`

 * *Files identical despite different names*

