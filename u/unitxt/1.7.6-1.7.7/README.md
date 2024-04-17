# Comparing `tmp/unitxt-1.7.6.tar.gz` & `tmp/unitxt-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitxt-1.7.6.tar", last modified: Mon Apr  8 17:50:17 2024, max compression
+gzip compressed data, was "unitxt-1.7.7.tar", last modified: Wed Apr 17 07:23:09 2024, max compression
```

## Comparing `unitxt-1.7.6.tar` & `unitxt-1.7.7.tar`

### file list

```diff
@@ -1,1083 +1,1102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.445190 unitxt-1.7.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 17:50:13.000000 unitxt-1.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 17:50:13.000000 unitxt-1.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-04-08 17:50:17.445190 unitxt-1.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-08 17:50:13.000000 unitxt-1.7.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-08 17:50:14.000000 unitxt-1.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:50:17.445190 unitxt-1.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-08 17:50:14.000000 unitxt-1.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.253187 unitxt-1.7.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.273187 unitxt-1.7.6/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.281187 unitxt-1.7.6/src/unitxt/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/card.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.261187 unitxt-1.7.6/src/unitxt/catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.285187 unitxt-1.7.6/src/unitxt/catalog/augmentors/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/augmentors/augment_whitespace_model_input.json
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/augmentors/augment_whitespace_prefix_and_suffix_task_input.json
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/augmentors/augment_whitespace_task_input.json
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/augmentors/no_augmentation.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.293187 unitxt-1.7.6/src/unitxt/catalog/cards/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.293187 unitxt-1.7.6/src/unitxt/catalog/cards/20_newsgroups/
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/20_newsgroups/sklearn.json
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/20_newsgroups.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.253187 unitxt-1.7.6/src/unitxt/catalog/cards/CFPB/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.297187 unitxt-1.7.6/src/unitxt/catalog/cards/CFPB/product/
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/CFPB/product/2023.json
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/CFPB/product/watsonx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ag_news.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.297187 unitxt-1.7.6/src/unitxt/catalog/cards/ai2_arc/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ai2_arc/arc_challenge.json
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ai2_arc/arc_easy.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.297187 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/de.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/en.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/es.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/fr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/it.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/nl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/pt.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.305187 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/af_ZA.json
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.305187 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/all_1/
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/all_1/1.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/am_ET.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ar_SA.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/az_AZ.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/bn_BD.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ca_ES.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/cy_GB.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/da_DK.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/de_DE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/el_GR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/en_US.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/es_ES.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/fa_IR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/fi_FI.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/fr_FR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/he_IL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/hi_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/hu_HU.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/hy_AM.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/id_ID.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/is_IS.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/it_IT.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ja_JP.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/jv_ID.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ka_GE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/km_KH.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/kn_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ko_KR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/lv_LV.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ml_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/mn_MN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ms_MY.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/my_MM.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/nb_NO.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/nl_NL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/pl_PL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/pt_PT.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ro_RO.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ru_RU.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sl_SL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sq_AL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sv_SE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sw_KE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ta_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/te_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/th_TH.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/tl_PH.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/tr_TR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ur_PK.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/vi_VN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/zh_CN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/zh_TW.json
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/argument_topic.json
--rw-r--r--   0 runner    (1001) docker     (127)    13266 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/atis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/atta_q.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.305187 unitxt-1.7.6/src/unitxt/catalog/cards/babi/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/babi/qa.json
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/banking77.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.325188 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/acm_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/afr_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/als_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/amh_ethi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/apc_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/arb_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/arb_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ars_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ary_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/arz_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/asm_beng.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/azj_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/bam_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ben_beng.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ben_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/bod_tibt.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/bul_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/cat_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ceb_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ces_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ckb_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/dan_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/deu_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ell_grek.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/eng_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/est_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/eus_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/fin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/fra_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/fuv_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/gaz_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/grn_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/guj_gujr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hat_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hau_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/heb_hebr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hin_deva.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hrv_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hun_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hye_armn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ibo_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ilo_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ind_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/isl_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ita_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/jav_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/jpn_jpan.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kac_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kan_knda.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kat_geor.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kaz_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kea_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/khk_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/khm_khmr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kir_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kor_hang.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lao_laoo.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lit_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lug_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/luo_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lvs_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mal_mlym.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mar_deva.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mkd_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mlt_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mri_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mya_mymr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nld_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nob_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/npi_deva.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/npi_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nso_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nya_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ory_orya.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pan_guru.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pbt_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pes_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/plt_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pol_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/por_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ron_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/rus_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/shn_mymr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sin_sinh.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/slk_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/slv_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sna_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/snd_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/som_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sot_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/spa_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/srp_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ssw_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sun_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/swe_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/swh_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tam_taml.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tel_telu.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tgk_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tgl_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tha_thai.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tir_ethi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tsn_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tso_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tur_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ukr_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/urd_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/urd_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/uzn_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/vie_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/war_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/wol_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/xho_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/yor_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zho_hans.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zho_hant.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zsm_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zul_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/bold.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.325188 unitxt-1.7.6/src/unitxt/catalog/cards/boolq/
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/boolq/classification.json
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/boolq/multiple_choice.json
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/claim_stance_topic.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.325188 unitxt-1.7.6/src/unitxt/catalog/cards/clinc_oos/
--rw-r--r--   0 runner    (1001) docker     (127)    12619 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/clinc_oos/imbalanced.json
--rw-r--r--   0 runner    (1001) docker     (127)    12613 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/clinc_oos/plus.json
--rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/clinc_oos/small.json
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cnn_dailymail.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.329188 unitxt-1.7.6/src/unitxt/catalog/cards/coedit/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coedit/paraphrase.json
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coedit/preference.json
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coedit/rewriting.json
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coedit/selection.json
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coedit_error_detection.json
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coedit_gec.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.253187 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.329188 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/eng.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/por.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tel.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tur.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/yor.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/zho.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.329188 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/fra.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/spa.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.329188 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/deu.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/eng.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/fra.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/jpn.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/por.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/spa.json
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/cola.json
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/copa.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.329188 unitxt-1.7.6/src/unitxt/catalog/cards/coqa/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coqa/completion.json
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/coqa/qa.json
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/dart.json
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/dbpedia_14.json
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ethos_binary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.329188 unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/16k.json
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/2k.json
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/4k.json
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/8k.json
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/financial_tweets.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.329188 unitxt-1.7.6/src/unitxt/catalog/cards/head_qa/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/head_qa/en.json
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/head_qa/es.json
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/hellaswag.json
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/hh_rlhf.json
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/human_eval.json
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/law_stack_exchange.json
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/ledgar.json
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mbpp.json
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/medical_abstracts.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.333188 unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/de.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/es.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/fr.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/tu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/abstract_algebra.json
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/anatomy.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/astronomy.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/business_ethics.json
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/clinical_knowledge.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_biology.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_chemistry.json
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_computer_science.json
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_mathematics.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_medicine.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_physics.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/computer_security.json
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/conceptual_physics.json
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/econometrics.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/electrical_engineering.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/elementary_mathematics.json
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/formal_logic.json
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/global_facts.json
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_biology.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_chemistry.json
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_european_history.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_geography.json
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_government_and_politics.json
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_macroeconomics.json
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_mathematics.json
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_physics.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_psychology.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_statistics.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_us_history.json
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_world_history.json
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/human_aging.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/human_sexuality.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/international_law.json
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/jurisprudence.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/logical_fallacies.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/machine_learning.json
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/management.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/marketing.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/medical_genetics.json
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/miscellaneous.json
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/moral_disputes.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/moral_scenarios.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/nutrition.json
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/philosophy.json
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/prehistory.json
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_accounting.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_law.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_medicine.json
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_psychology.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/public_relations.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/security_studies.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/sociology.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/us_foreign_policy.json
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/virology.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/world_religions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mnli.json
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/mrpc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/multidoc2dial/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/multidoc2dial/abstractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/multidoc2dial/extractive.json
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/news_category_classification_headline.json
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/openbook_qa.json
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/piqa.json
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/pop_qa.json
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/qnli.json
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/qqp.json
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/race_all.json
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/race_high.json
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/race_middle.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/reuters21578/
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/reuters21578/ModApte.json
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/reuters21578/ModHayes.json
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/reuters21578/ModLewis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/rte.json
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/sciq.json
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/squad.json
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/sst2.json
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/stsb.json
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/summarize_from_human_feedback.json
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/tab_fact.json
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/tablerow_classify.json
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/toxigen.json
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/trec.json
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/unfair_tos.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.257187 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/ceb/
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/ceb/gja.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/da/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/da/ddt.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/de/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/de/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/en/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/en/ewt.json
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/en/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/hr/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/hr/set.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/pt/
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/pt/bosque.json
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/pt/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/ru/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/ru/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sk/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sk/snk.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.341188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sr/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sr/set.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.345188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sv/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sv/pud.json
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sv/talbanken.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.345188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/tl/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/tl/trg.json
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.345188 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/zh/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/zh/gsd.json
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/zh/pud.json
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wiki_bio.json
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wikitq.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.345188 unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/debiased.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/l.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/m.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/s.json
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/xl.json
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/xs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.345188 unitxt-1.7.6/src/unitxt/catalog/cards/wmt/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wmt/en_de.json
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wmt/en_fr.json
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wmt/en_ro.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.345188 unitxt-1.7.6/src/unitxt/catalog/cards/wnli/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wnli/truthfulness.json
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wnli.json
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/wsc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.353188 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/amharic.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/arabic.json
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/azerbaijani.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/bengali.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/burmese.json
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/chinese_simplified.json
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/chinese_traditional.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/english.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/french.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/gujarati.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/hausa.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/hindi.json
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/igbo.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/indonesian.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/japanese.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/kirundi.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/korean.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/kyrgyz.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/marathi.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/nepali.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/oromo.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/pashto.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/persian.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/pidgin.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/portuguese.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/punjabi.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/russian.json
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/scottish_gaelic.json
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/serbian_cyrillic.json
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/serbian_latin.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/sinhala.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/somali.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/spanish.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/swahili.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/tamil.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/telugu.json
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/thai.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/tigrinya.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/turkish.json
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/ukrainian.json
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/urdu.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/uzbek.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/vietnamese.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/welsh.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/yoruba.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.357188 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/ar.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/bg.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/de.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/el.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/en.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/es.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/fr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/hi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/sw.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/th.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/tr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/ur.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/vi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xnli/zh.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xsum.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.357188 unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/en.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/jp.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/pt.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/zh.json
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/cards/yahoo_answers_topics.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.357188 unitxt-1.7.6/src/unitxt/catalog/formats/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/empty_input_output_separator.json
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/human_assistant.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/llama.json
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/llama2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.357188 unitxt-1.7.6/src/unitxt/catalog/formats/models/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/models/alpaca_instruct.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.357188 unitxt-1.7.6/src/unitxt/catalog/formats/models/flan/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/models/flan/exq_exa.json
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/models/flan/few_shot.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.361188 unitxt-1.7.6/src/unitxt/catalog/formats/models/labradorite/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/models/labradorite/few_shot.json
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/models/labradorite/zero_shot.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.361188 unitxt-1.7.6/src/unitxt/catalog/formats/models/mistral/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.361188 unitxt-1.7.6/src/unitxt/catalog/formats/models/mistral/instruction/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/models/mistral/instruction/with_system_prompt.json
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/models/mistral/instruction.json
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/textual_assistant.json
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/user_agent.json
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/formats/user_assistant.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.365188 unitxt-1.7.6/src/unitxt/catalog/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/accuracy_binary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.369188 unitxt-1.7.6/src/unitxt/catalog/metrics/bert_score/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/bert_score/deberta_base_mnli.json
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/bert_score/deberta_large_mnli.json
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/bert_score/deberta_xlarge_mnli.json
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/bert_score/distilbert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/bleu.json
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/char_edit_dist_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/char_edit_distance.json
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/f1_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/f1_macro.json
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/f1_macro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/f1_micro.json
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/f1_micro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/f1_weighted.json
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/kendalltau_b.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/kpa.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/map.json
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/matthews_correlation.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/max_accuracy_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/max_f1_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/mrr.json
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/ndcg.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/ner.json
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/normalized_sacrebleu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.369188 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity/flan_t5_small.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.369188 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity_a/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity_a/flan_t5_small.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.369188 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity_chat/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity_chat/flan_t5_small.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.369188 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity_q/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/perplexity_q/flan_t5_small.json
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/precision_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/precision_macro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/precision_micro_multi_label.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.369188 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/answer_correctness.json
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/answer_reward.json
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/bert_k_precision.json
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/bert_recall.json
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/context_correctness.json
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/context_perplexity.json
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/context_relevance.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.373189 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/correctness/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/correctness/llama_index_by_gpt_3_5_turbo.json
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/correctness/llama_index_by_mock.json
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/faithfulness.json
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/k_precision.json
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/map.json
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/mrr.json
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rag/recall.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/recall_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/recall_macro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/recall_micro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/regard.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rerank_recall.json
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/retrieval_at_k.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.373189 unitxt-1.7.6/src/unitxt/catalog/metrics/reward/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/reward/deberta_v3_large_v2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.373189 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_mean_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_mean_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/group_mean_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/group_mean_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/robustness/group_mean_token_overlap.json
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/roc_auc.json
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rouge.json
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/rouge_with_confidence_intervals.json
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/sacrebleu.json
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/safety.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.373189 unitxt-1.7.6/src/unitxt/catalog/metrics/sentence_bert/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/sentence_bert/mpnet_base_v2.json
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/spearman.json
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/squad.json
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/token_overlap.json
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/token_overlap_with_context.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/unsorted_list_exact_match.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/metrics/wer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.261187 unitxt-1.7.6/src/unitxt/catalog/operators/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.261187 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.377189 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/classification/by_label.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.377189 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/multi_label/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/multi_label/zero_vs_many_labels.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.377189 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/ner/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/ner/zero_vs_many_entities.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.377189 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/qa/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/operators/balancers/qa/by_answer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.381189 unitxt-1.7.6/src/unitxt/catalog/processors/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/capitalize.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/convert_to_boolean.json
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/dict_of_lists_to_value_key_pairs.json
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/first_character.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/get_string_after_colon.json
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/hate_speech_or_not_hate_speech.json
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/list_to_empty_entity_tuples.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/load_json.json
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/load_json_from_predictions.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/lower_case.json
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/lower_case_till_punc.json
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/match_closest_option.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/predictions_yes_1_else_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/remove_none_from_list.json
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/stance_to_pro_con.json
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/str_to_float_format.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/substring.json
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/take_first_non_empty_line.json
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/take_first_word.json
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/to_list_by_comma.json
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/to_span_label_pairs.json
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/to_string.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/to_string_stripped.json
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/to_yes_or_none.json
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/toxic_or_not_toxic.json
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/processors/yes_no_to_int.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.381189 unitxt-1.7.6/src/unitxt/catalog/splitters/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/splitters/default.json
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/splitters/diverse_labels_sampler.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/splitters/large_no_dev.json
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/splitters/large_no_test.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/splitters/small_no_dev.json
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/splitters/small_no_test.json
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/splitters/test_only.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.261187 unitxt-1.7.6/src/unitxt/catalog/system_prompt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.381189 unitxt-1.7.6/src/unitxt/catalog/system_prompt/models/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/system_prompt/models/japanese_llama.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.381189 unitxt-1.7.6/src/unitxt/catalog/system_prompts/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/system_prompts/empty.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.381189 unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/alpaca.json
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/labradorite.json
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/llama.json
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/llama2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/classification/binary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/classification/multi_class/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/classification/multi_class/relation.json
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/classification/multi_class.json
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/classification/multi_label.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/completion/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/completion/abstractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/completion/extractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/completion/multiple_choice.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/evaluation/preference.json
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/generation.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/grammatical_error_correction.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/ner/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/ner/all_entity_types.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/ner/single_entity_type.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/multiple_choice/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/multiple_choice/open.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/with_topic.json
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/multiple_choice/with_context.json
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/multiple_choice/with_topic.json
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/open.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/with_context/abstractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/qa/with_context/extractive.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.385189 unitxt-1.7.6/src/unitxt/catalog/tasks/regression/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/regression/single_text.json
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/regression/two_texts.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/tasks/rewriting/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/rewriting/by_attribute.json
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/rewriting/paraphrase.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/tasks/selection/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/selection/by_attribute.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/tasks/span_labeling/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/span_labeling/extraction.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/tasks/summarization/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/summarization/abstractive.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/tasks/targeted_sentiment_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/targeted_sentiment_extraction/all_sentiment_classes.json
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/targeted_sentiment_extraction/single_sentiment_class.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/tasks/translation/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/tasks/translation/directed.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.265187 unitxt-1.7.6/src/unitxt/catalog/templates/classification/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/instruction.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.389189 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/simple.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.393189 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_1.json
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_2.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_6.json
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_7.json
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.393189 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/instruction.json
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.265187 unitxt-1.7.6/src/unitxt/catalog/templates/completion/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.393189 unitxt-1.7.6/src/unitxt/catalog/templates/completion/abstractive/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/abstractive/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/abstractive/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/abstractive/standard.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.393189 unitxt-1.7.6/src/unitxt/catalog/templates/completion/multiple_choice/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/multiple_choice/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/multiple_choice/enumerated.json
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/multiple_choice/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/multiple_choice/standard.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/completion/multiple_choice/title.json
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/empty.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.265187 unitxt-1.7.6/src/unitxt/catalog/templates/evaluation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.393189 unitxt-1.7.6/src/unitxt/catalog/templates/evaluation/preference/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/evaluation/preference/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/evaluation/preference/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.393189 unitxt-1.7.6/src/unitxt/catalog/templates/generation/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/generation/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/generation/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.397189 unitxt-1.7.6/src/unitxt/catalog/templates/grammatical_error_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/grammatical_error_correction/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/grammatical_error_correction/simple.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.397189 unitxt-1.7.6/src/unitxt/catalog/templates/grammatical_error_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/grammatical_error_detection/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/grammatical_error_detection/yes_no.json
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/key_val.json
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/key_val_with_new_lines.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.269187 unitxt-1.7.6/src/unitxt/catalog/templates/qa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.397189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/match.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.397189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.397189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/de/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.397189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/es/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/es/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.401189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.401189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.401189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.401189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.401189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.401189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.405189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.405189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.405189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.405189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.409189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.409189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.409189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fm_eval.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.409189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.409189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/match.json
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.413189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.413189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.413189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.413189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fm_eval.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.413189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.417189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/match.json
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.417189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.417189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/open/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/open/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/open/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/open/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/open/simple2.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/open/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.417189 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/ffqa.json
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/question_first.json
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/simple2.json
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/title.json
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/qa/with_context/with_type.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.269187 unitxt-1.7.6/src/unitxt/catalog/templates/regression/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.417189 unitxt-1.7.6/src/unitxt/catalog/templates/regression/single_text/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/regression/single_text/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/regression/single_text/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/regression/single_text/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.421189 unitxt-1.7.6/src/unitxt/catalog/templates/regression/two_texts/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/regression/two_texts/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.421189 unitxt-1.7.6/src/unitxt/catalog/templates/regression/two_texts/similarity/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/regression/two_texts/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/regression/two_texts/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.269187 unitxt-1.7.6/src/unitxt/catalog/templates/rewriting/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.421189 unitxt-1.7.6/src/unitxt/catalog/templates/rewriting/by_attribute/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/rewriting/by_attribute/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/rewriting/by_attribute/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.421189 unitxt-1.7.6/src/unitxt/catalog/templates/rewriting/paraphrase/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/rewriting/paraphrase/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/rewriting/paraphrase/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.269187 unitxt-1.7.6/src/unitxt/catalog/templates/selection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.421189 unitxt-1.7.6/src/unitxt/catalog/templates/selection/by_attribute/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/selection/by_attribute/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/selection/by_attribute/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.269187 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.421189 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/carry.json
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/extract.json
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/having.json
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/identify.json
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/span_labeling/extraction/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.269187 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.425189 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/casual.json
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/formal.json
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/formal_without_label.json
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/full.json
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/instructive.json
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/one_sentence.json
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/passive.json
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/professional.json
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/title.json
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/write_succinct.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.425189 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.425189 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_explicit_keys.json
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_implicit_keys.json
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/carry_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/entities_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/extract_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/having_sentiment.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.425189 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/having_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/sentiment_extracted.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.429189 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/having_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/sentiment_extracted.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.429189 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/having_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/sentiment_extracted.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.269187 unitxt-1.7.6/src/unitxt/catalog/templates/translation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.429189 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/casual.json
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/formal.json
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/instructional.json
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/playful.json
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog/templates/translation/directed/title.json
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/collections_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/deprecation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/dialog_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    23755 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/eval_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/fusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/generator_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/hf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/instructions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17915 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/metric_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   133392 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/normalizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    21234 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    76915 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/parsing_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.429189 unitxt-1.7.6/src/unitxt/prepare_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/prepare_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/prepare_utils/card_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/prepare_utils/instructions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/random_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.429189 unitxt-1.7.6/src/unitxt/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.429189 unitxt-1.7.6/src/unitxt/service/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/service/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/service/metrics/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/service/metrics/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/settings_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/span_lableing_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/split_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/splitters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/string_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17231 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/struct_data_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/system_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    20524 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.433189 unitxt-1.7.6/src/unitxt/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/test_utils/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/test_utils/card.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/test_utils/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/test_utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/test_utils/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/test_utils/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/type_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.433189 unitxt-1.7.6/src/unitxt/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56810 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/gradio_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/load_catalog_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/ui_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/ui/ui_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 17:50:14.000000 unitxt-1.7.6/src/unitxt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:17.433189 unitxt-1.7.6/src/unitxt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-04-08 17:50:17.000000 unitxt-1.7.6/src/unitxt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    49194 2024-04-08 17:50:17.000000 unitxt-1.7.6/src/unitxt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:50:17.000000 unitxt-1.7.6/src/unitxt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-08 17:50:17.000000 unitxt-1.7.6/src/unitxt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 17:50:17.000000 unitxt-1.7.6/src/unitxt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 17:50:17.000000 unitxt-1.7.6/src/unitxt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.111134 unitxt-1.7.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 07:23:05.000000 unitxt-1.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 07:23:05.000000 unitxt-1.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-04-17 07:23:09.111134 unitxt-1.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-17 07:23:05.000000 unitxt-1.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-17 07:23:05.000000 unitxt-1.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:23:09.111134 unitxt-1.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-17 07:23:05.000000 unitxt-1.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.911133 unitxt-1.7.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.931133 unitxt-1.7.7/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.943133 unitxt-1.7.7/src/unitxt/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/card.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.923133 unitxt-1.7.7/src/unitxt/catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.947133 unitxt-1.7.7/src/unitxt/catalog/augmentors/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/augmentors/augment_whitespace_model_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/augmentors/augment_whitespace_prefix_and_suffix_task_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/augmentors/augment_whitespace_task_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/augmentors/no_augmentation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.955133 unitxt-1.7.7/src/unitxt/catalog/cards/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.955133 unitxt-1.7.7/src/unitxt/catalog/cards/20_newsgroups/
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/20_newsgroups/sklearn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/20_newsgroups.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.911133 unitxt-1.7.7/src/unitxt/catalog/cards/CFPB/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.955133 unitxt-1.7.7/src/unitxt/catalog/cards/CFPB/product/
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/CFPB/product/2023.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/CFPB/product/watsonx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/ag_news.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.955133 unitxt-1.7.7/src/unitxt/catalog/cards/ai2_arc/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/ai2_arc/arc_challenge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/ai2_arc/arc_easy.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.959133 unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/it.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/nl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/pt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.967133 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/af_ZA.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.967133 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/all_1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/all_1/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/am_ET.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ar_SA.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/az_AZ.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/bn_BD.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ca_ES.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/cy_GB.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/da_DK.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/de_DE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/el_GR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/en_US.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/es_ES.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/fa_IR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/fi_FI.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/fr_FR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/he_IL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/hi_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/hu_HU.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/hy_AM.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/id_ID.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/is_IS.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/it_IT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ja_JP.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/jv_ID.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ka_GE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/km_KH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/kn_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ko_KR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/lv_LV.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ml_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/mn_MN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ms_MY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/my_MM.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/nb_NO.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/nl_NL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/pl_PL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/pt_PT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ro_RO.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ru_RU.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/sl_SL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/sq_AL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/sv_SE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/sw_KE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ta_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/te_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/th_TH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/tl_PH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/tr_TR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ur_PK.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/vi_VN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/zh_CN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/zh_TW.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/argument_topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13266 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/atis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/atta_q.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.971133 unitxt-1.7.7/src/unitxt/catalog/cards/babi/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/babi/qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/banking77.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.991133 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/acm_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/afr_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/als_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/amh_ethi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/apc_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/arb_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/arb_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ars_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ary_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/arz_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/asm_beng.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/azj_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/bam_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ben_beng.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ben_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/bod_tibt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/bul_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/cat_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ceb_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ces_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ckb_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/dan_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/deu_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ell_grek.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/eng_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/est_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/eus_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/fin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/fra_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/fuv_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/gaz_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/grn_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/guj_gujr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/hat_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/hau_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/heb_hebr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/hin_deva.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/hin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/hrv_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/hun_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/hye_armn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ibo_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ilo_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ind_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/isl_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ita_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/jav_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/jpn_jpan.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kac_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kan_knda.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kat_geor.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kaz_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kea_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/khk_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/khm_khmr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kir_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kor_hang.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/lao_laoo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/lin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/lit_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/lug_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/luo_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/lvs_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/mal_mlym.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/mar_deva.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/mkd_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/mlt_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/mri_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/mya_mymr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/nld_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/nob_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/npi_deva.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/npi_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/nso_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/nya_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ory_orya.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/pan_guru.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/pbt_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/pes_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/plt_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/pol_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/por_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ron_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/rus_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/shn_mymr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/sin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/sin_sinh.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/slk_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/slv_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/sna_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/snd_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/som_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/sot_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/spa_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/srp_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ssw_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/sun_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/swe_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/swh_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tam_taml.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tel_telu.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tgk_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tgl_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tha_thai.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tir_ethi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tsn_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tso_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tur_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ukr_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/urd_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/urd_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/uzn_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/vie_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/war_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/wol_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/xho_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/yor_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/zho_hans.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/zho_hant.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/zsm_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/belebele/zul_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/bold.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.991133 unitxt-1.7.7/src/unitxt/catalog/cards/boolq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/boolq/classification.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/boolq/multiple_choice.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/claim_stance_topic.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.995133 unitxt-1.7.7/src/unitxt/catalog/cards/clinc_oos/
+-rw-r--r--   0 runner    (1001) docker     (127)    12619 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/clinc_oos/imbalanced.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12613 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/clinc_oos/plus.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/clinc_oos/small.json
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cnn_dailymail.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.995133 unitxt-1.7.7/src/unitxt/catalog/cards/coedit/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/coedit/paraphrase.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/coedit/preference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/coedit/rewriting.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/coedit/selection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/coedit_error_detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/coedit_gec.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.915133 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.995133 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/eng.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/por.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tel.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tur.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/yor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/zho.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.995133 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/fra.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/spa.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.995133 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/deu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/eng.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/fra.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/jpn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/por.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/spa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/cola.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/copa.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.999133 unitxt-1.7.7/src/unitxt/catalog/cards/coqa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/coqa/completion.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/coqa/qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/dart.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/dbpedia_14.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/ethos_binary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.999133 unitxt-1.7.7/src/unitxt/catalog/cards/ffqa_filtered/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/ffqa_filtered/16k.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/ffqa_filtered/2k.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/ffqa_filtered/4k.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/ffqa_filtered/8k.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/financial_tweets.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.999133 unitxt-1.7.7/src/unitxt/catalog/cards/head_qa/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/head_qa/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/head_qa/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/hellaswag.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/hh_rlhf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/human_eval.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/law_stack_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/ledgar.json
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mbpp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/medical_abstracts.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.999133 unitxt-1.7.7/src/unitxt/catalog/cards/mlsum/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mlsum/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mlsum/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mlsum/fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mlsum/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mlsum/tu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.011133 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/abstract_algebra.json
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/anatomy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/astronomy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/business_ethics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/clinical_knowledge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/college_biology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/college_chemistry.json
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/college_computer_science.json
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/college_mathematics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/college_medicine.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/college_physics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/computer_security.json
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/conceptual_physics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/econometrics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/electrical_engineering.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/elementary_mathematics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/formal_logic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/global_facts.json
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_biology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_chemistry.json
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_european_history.json
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_geography.json
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_government_and_politics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_macroeconomics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_mathematics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_physics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_psychology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_statistics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_us_history.json
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_world_history.json
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/human_aging.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/human_sexuality.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/international_law.json
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/jurisprudence.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/logical_fallacies.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/machine_learning.json
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/management.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/marketing.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/medical_genetics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/miscellaneous.json
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/moral_disputes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/moral_scenarios.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/nutrition.json
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/philosophy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/prehistory.json
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/professional_accounting.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/professional_law.json
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/professional_medicine.json
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/professional_psychology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/public_relations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/security_studies.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/sociology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/us_foreign_policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/virology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/world_religions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/mrpc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.011133 unitxt-1.7.7/src/unitxt/catalog/cards/multidoc2dial/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/multidoc2dial/abstractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/multidoc2dial/extractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/news_category_classification_headline.json
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/openbook_qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/piqa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/pop_qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/qnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/qqp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/race_all.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/race_high.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/race_middle.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.915133 unitxt-1.7.7/src/unitxt/catalog/cards/rag/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.011133 unitxt-1.7.7/src/unitxt/catalog/cards/rag/model_response_assessment/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/rag/model_response_assessment/llm_as_judge_using_mt_bench_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.011133 unitxt-1.7.7/src/unitxt/catalog/cards/reuters21578/
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/reuters21578/ModApte.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/reuters21578/ModHayes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/reuters21578/ModLewis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/rte.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/sciq.json
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/squad.json
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/sst2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/stsb.json
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/summarize_from_human_feedback.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/tab_fact.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/tablerow_classify.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/toxigen.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/trec.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/unfair_tos.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.919133 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.011133 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/ceb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/ceb/gja.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.011133 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/da/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/da/ddt.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.011133 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/de/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/de/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.011133 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/en/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/en/ewt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/en/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.011133 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/hr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/hr/set.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.011133 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/pt/bosque.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/pt/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.011133 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/ru/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.015133 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/sk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/sk/snk.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.015133 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/sr/set.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.015133 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/sv/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/sv/pud.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/sv/talbanken.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.015133 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/tl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/tl/trg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.015133 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/zh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/zh/gsd.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/zh/pud.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/wiki_bio.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/wikitq.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.015133 unitxt-1.7.7/src/unitxt/catalog/cards/winogrande/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/winogrande/debiased.json
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/winogrande/l.json
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/winogrande/m.json
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/winogrande/s.json
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/winogrande/xl.json
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/winogrande/xs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.015133 unitxt-1.7.7/src/unitxt/catalog/cards/wmt/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/wmt/en_de.json
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/wmt/en_fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/wmt/en_ro.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.015133 unitxt-1.7.7/src/unitxt/catalog/cards/wnli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/wnli/truthfulness.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/wnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/wsc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.023133 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/amharic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/arabic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/azerbaijani.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/bengali.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/burmese.json
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/chinese_simplified.json
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/chinese_traditional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/english.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/french.json
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/gujarati.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/hausa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/hindi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/igbo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/indonesian.json
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/japanese.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/kirundi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/korean.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/kyrgyz.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/marathi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/nepali.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/oromo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/pashto.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/persian.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/pidgin.json
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/portuguese.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/punjabi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/russian.json
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/scottish_gaelic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/serbian_cyrillic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/serbian_latin.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/sinhala.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/somali.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/spanish.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/swahili.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/tamil.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/telugu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/thai.json
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/tigrinya.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/turkish.json
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/ukrainian.json
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/urdu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/uzbek.json
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/vietnamese.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/welsh.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/yoruba.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.027133 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/ar.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/bg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/el.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/hi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/sw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/th.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/tr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/ur.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/vi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xnli/zh.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xsum.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.027133 unitxt-1.7.7/src/unitxt/catalog/cards/xwinogrande/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xwinogrande/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xwinogrande/jp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xwinogrande/pt.json
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xwinogrande/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/xwinogrande/zh.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/cards/yahoo_answers_topics.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.031133 unitxt-1.7.7/src/unitxt/catalog/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/formats/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/formats/empty_input_output_separator.json
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/formats/human_assistant.json
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/formats/llama.json
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/formats/llama2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.031133 unitxt-1.7.7/src/unitxt/catalog/formats/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/formats/models/alpaca_instruct.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.031133 unitxt-1.7.7/src/unitxt/catalog/formats/models/flan/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/formats/models/flan/exq_exa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/formats/models/flan/few_shot.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.031133 unitxt-1.7.7/src/unitxt/catalog/formats/models/labradorite/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/formats/models/labradorite/few_shot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/formats/models/labradorite/zero_shot.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.031133 unitxt-1.7.7/src/unitxt/catalog/formats/models/mistral/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.031133 unitxt-1.7.7/src/unitxt/catalog/formats/models/mistral/instruction/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/formats/models/mistral/instruction/with_system_prompt.json
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/formats/models/mistral/instruction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/formats/textual_assistant.json
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/formats/user_agent.json
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/formats/user_assistant.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.039133 unitxt-1.7.7/src/unitxt/catalog/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/accuracy_binary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.039133 unitxt-1.7.7/src/unitxt/catalog/metrics/bert_score/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/bert_score/deberta_base_mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/bert_score/deberta_large_mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/bert_score/deberta_v3_base_mnli_xnli_ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/bert_score/deberta_xlarge_mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/bert_score/distilbert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/bleu.json
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/char_edit_dist_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/char_edit_distance.json
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/f1_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/f1_macro.json
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/f1_macro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/f1_micro.json
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/f1_micro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/f1_weighted.json
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/kendalltau_b.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/kpa.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/map.json
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/matthews_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/max_accuracy_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/max_f1_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/mrr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/ndcg.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/ner.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/normalized_sacrebleu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.039133 unitxt-1.7.7/src/unitxt/catalog/metrics/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/perplexity/flan_t5_small.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.039133 unitxt-1.7.7/src/unitxt/catalog/metrics/perplexity_a/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/perplexity_a/flan_t5_small.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.039133 unitxt-1.7.7/src/unitxt/catalog/metrics/perplexity_chat/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/perplexity_chat/flan_t5_small.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.039133 unitxt-1.7.7/src/unitxt/catalog/metrics/perplexity_nli/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/perplexity_nli/t5_nli_mixture.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.039133 unitxt-1.7.7/src/unitxt/catalog/metrics/perplexity_q/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/perplexity_q/flan_t5_small.json
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/precision_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/precision_macro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/precision_micro_multi_label.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.043133 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/answer_correctness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/answer_inference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/answer_reward.json
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/bert_k_precision.json
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/bert_k_precision_ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/bert_recall.json
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/bert_recall_ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/context_correctness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/context_perplexity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/context_relevance.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.043133 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/correctness/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/correctness/llama_index_by_gpt_3_5_turbo.json
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/correctness/llama_index_by_mock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/faithfulness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/k_precision.json
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/map.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.043133 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/model_response_assessment/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/model_response_assessment/llm_as_judge_by_flan_t5_large_on_hf_pipeline_using_mt_bench_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/mrr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rag/recall.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/recall_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/recall_macro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/recall_micro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/regard.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rerank_recall.json
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/retrieval_at_k.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.043133 unitxt-1.7.7/src/unitxt/catalog/metrics/reward/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/reward/deberta_v3_large_v2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.047133 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_mean_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_mean_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/group_mean_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/group_mean_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/robustness/group_mean_token_overlap.json
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/roc_auc.json
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rouge.json
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/rouge_with_confidence_intervals.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/sacrebleu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/safety.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.047133 unitxt-1.7.7/src/unitxt/catalog/metrics/sentence_bert/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/sentence_bert/mpnet_base_v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/spearman.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/squad.json
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/token_overlap.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/token_overlap_with_context.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/unsorted_list_exact_match.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/metrics/wer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.919133 unitxt-1.7.7/src/unitxt/catalog/operators/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.919133 unitxt-1.7.7/src/unitxt/catalog/operators/balancers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.047133 unitxt-1.7.7/src/unitxt/catalog/operators/balancers/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/operators/balancers/classification/by_label.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.047133 unitxt-1.7.7/src/unitxt/catalog/operators/balancers/multi_label/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/operators/balancers/multi_label/zero_vs_many_labels.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.047133 unitxt-1.7.7/src/unitxt/catalog/operators/balancers/ner/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/operators/balancers/ner/zero_vs_many_entities.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.047133 unitxt-1.7.7/src/unitxt/catalog/operators/balancers/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/operators/balancers/qa/by_answer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.051133 unitxt-1.7.7/src/unitxt/catalog/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/capitalize.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/convert_to_boolean.json
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/dict_of_lists_to_value_key_pairs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/extract_mt_bench_judgment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/first_character.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/get_string_after_colon.json
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/hate_speech_or_not_hate_speech.json
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/list_to_empty_entity_tuples.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/load_json.json
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/load_json_from_predictions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/lower_case.json
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/lower_case_till_punc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/match_closest_option.json
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/predictions_yes_1_else_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/remove_none_from_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/stance_to_pro_con.json
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/str_to_float_format.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/substring.json
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/take_first_non_empty_line.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/take_first_word.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/to_list_by_comma.json
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/to_span_label_pairs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/to_string.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/to_string_stripped.json
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/to_yes_or_none.json
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/toxic_or_not_toxic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/processors/yes_no_to_int.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.055133 unitxt-1.7.7/src/unitxt/catalog/splitters/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/splitters/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/splitters/diverse_labels_sampler.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/splitters/large_no_dev.json
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/splitters/large_no_test.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/splitters/small_no_dev.json
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/splitters/small_no_test.json
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/splitters/test_only.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.923133 unitxt-1.7.7/src/unitxt/catalog/system_prompt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.055133 unitxt-1.7.7/src/unitxt/catalog/system_prompt/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/system_prompt/models/japanese_llama.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.055133 unitxt-1.7.7/src/unitxt/catalog/system_prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/system_prompts/empty.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.055133 unitxt-1.7.7/src/unitxt/catalog/system_prompts/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/system_prompts/models/alpaca.json
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/system_prompts/models/labradorite.json
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/system_prompts/models/llama.json
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/system_prompts/models/llama2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.055133 unitxt-1.7.7/src/unitxt/catalog/tasks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.055133 unitxt-1.7.7/src/unitxt/catalog/tasks/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/classification/binary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.055133 unitxt-1.7.7/src/unitxt/catalog/tasks/classification/multi_class/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/classification/multi_class/relation.json
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/classification/multi_class.json
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/classification/multi_label.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.055133 unitxt-1.7.7/src/unitxt/catalog/tasks/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/completion/abstractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/completion/extractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/completion/multiple_choice.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.055133 unitxt-1.7.7/src/unitxt/catalog/tasks/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/evaluation/preference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/generation.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/grammatical_error_correction.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.059133 unitxt-1.7.7/src/unitxt/catalog/tasks/ner/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/ner/all_entity_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/ner/single_entity_type.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.059133 unitxt-1.7.7/src/unitxt/catalog/tasks/qa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.059133 unitxt-1.7.7/src/unitxt/catalog/tasks/qa/multiple_choice/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/qa/multiple_choice/open.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.059133 unitxt-1.7.7/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/with_topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/qa/multiple_choice/with_context.json
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/qa/multiple_choice/with_topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/qa/open.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.059133 unitxt-1.7.7/src/unitxt/catalog/tasks/qa/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/qa/with_context/abstractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/qa/with_context/extractive.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.059133 unitxt-1.7.7/src/unitxt/catalog/tasks/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/rag/model_response_assessment.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.059133 unitxt-1.7.7/src/unitxt/catalog/tasks/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/regression/single_text.json
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/regression/two_texts.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.059133 unitxt-1.7.7/src/unitxt/catalog/tasks/rewriting/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/rewriting/by_attribute.json
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/rewriting/paraphrase.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.059133 unitxt-1.7.7/src/unitxt/catalog/tasks/selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/selection/by_attribute.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.059133 unitxt-1.7.7/src/unitxt/catalog/tasks/span_labeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/span_labeling/extraction.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.059133 unitxt-1.7.7/src/unitxt/catalog/tasks/summarization/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/summarization/abstractive.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.059133 unitxt-1.7.7/src/unitxt/catalog/tasks/targeted_sentiment_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/targeted_sentiment_extraction/all_sentiment_classes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/targeted_sentiment_extraction/single_sentiment_class.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.059133 unitxt-1.7.7/src/unitxt/catalog/tasks/translation/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/tasks/translation/directed.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.059133 unitxt-1.7.7/src/unitxt/catalog/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.923133 unitxt-1.7.7/src/unitxt/catalog/templates/classification/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.063133 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/instruction.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.063133 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/relation/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/relation/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/relation/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/relation/simple.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.063133 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_6.json
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_7.json
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.063133 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_label/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_label/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_label/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_label/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_label/instruction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_label/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.923133 unitxt-1.7.7/src/unitxt/catalog/templates/completion/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.067133 unitxt-1.7.7/src/unitxt/catalog/templates/completion/abstractive/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/completion/abstractive/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/completion/abstractive/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/completion/abstractive/standard.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.067133 unitxt-1.7.7/src/unitxt/catalog/templates/completion/multiple_choice/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/completion/multiple_choice/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/completion/multiple_choice/enumerated.json
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/completion/multiple_choice/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/completion/multiple_choice/standard.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/completion/multiple_choice/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/empty.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.923133 unitxt-1.7.7/src/unitxt/catalog/templates/evaluation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.067133 unitxt-1.7.7/src/unitxt/catalog/templates/evaluation/preference/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/evaluation/preference/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/evaluation/preference/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.067133 unitxt-1.7.7/src/unitxt/catalog/templates/generation/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/generation/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/generation/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.067133 unitxt-1.7.7/src/unitxt/catalog/templates/grammatical_error_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/grammatical_error_correction/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/grammatical_error_correction/simple.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.067133 unitxt-1.7.7/src/unitxt/catalog/templates/grammatical_error_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/grammatical_error_detection/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/grammatical_error_detection/yes_no.json
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/key_val.json
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/key_val_with_new_lines.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.927133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.067133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/match.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.067133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.071133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.071133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/es/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.071133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.071133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.071133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.071133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.075133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.075133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.075133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.075133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.075133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.079133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.079133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.079133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.079133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fm_eval.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.079133 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.083134 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/match.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.083134 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.083134 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.083134 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.083134 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fm_eval.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.087134 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.087134 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/match.json
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.087134 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.087134 unitxt-1.7.7/src/unitxt/catalog/templates/qa/open/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/open/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/open/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/open/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/open/simple2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/open/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.087134 unitxt-1.7.7/src/unitxt/catalog/templates/qa/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/with_context/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/with_context/ffqa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/with_context/question_first.json
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/with_context/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/with_context/simple2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/with_context/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/qa/with_context/with_type.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.927133 unitxt-1.7.7/src/unitxt/catalog/templates/rag/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.091133 unitxt-1.7.7/src/unitxt/catalog/templates/rag/model_response_assessment/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/rag/model_response_assessment/llm_as_judge_using_mt_bench_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.931133 unitxt-1.7.7/src/unitxt/catalog/templates/regression/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.091133 unitxt-1.7.7/src/unitxt/catalog/templates/regression/single_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/regression/single_text/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/regression/single_text/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/regression/single_text/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.091133 unitxt-1.7.7/src/unitxt/catalog/templates/regression/two_texts/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/regression/two_texts/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.091133 unitxt-1.7.7/src/unitxt/catalog/templates/regression/two_texts/similarity/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/regression/two_texts/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/regression/two_texts/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.931133 unitxt-1.7.7/src/unitxt/catalog/templates/rewriting/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.091133 unitxt-1.7.7/src/unitxt/catalog/templates/rewriting/by_attribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/rewriting/by_attribute/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/rewriting/by_attribute/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.091133 unitxt-1.7.7/src/unitxt/catalog/templates/rewriting/paraphrase/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/rewriting/paraphrase/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/rewriting/paraphrase/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.931133 unitxt-1.7.7/src/unitxt/catalog/templates/selection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.091133 unitxt-1.7.7/src/unitxt/catalog/templates/selection/by_attribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/selection/by_attribute/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/selection/by_attribute/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.931133 unitxt-1.7.7/src/unitxt/catalog/templates/span_labeling/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.091133 unitxt-1.7.7/src/unitxt/catalog/templates/span_labeling/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/span_labeling/extraction/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/span_labeling/extraction/carry.json
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/span_labeling/extraction/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/span_labeling/extraction/extract.json
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/span_labeling/extraction/having.json
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/span_labeling/extraction/identify.json
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/span_labeling/extraction/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.931133 unitxt-1.7.7/src/unitxt/catalog/templates/summarization/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.095133 unitxt-1.7.7/src/unitxt/catalog/templates/summarization/abstractive/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/summarization/abstractive/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/summarization/abstractive/casual.json
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/summarization/abstractive/formal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/summarization/abstractive/formal_without_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/summarization/abstractive/full.json
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/summarization/abstractive/instructive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/summarization/abstractive/one_sentence.json
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/summarization/abstractive/passive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/summarization/abstractive/professional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/summarization/abstractive/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/summarization/abstractive/write_succinct.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.095133 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.095133 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_explicit_keys.json
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_implicit_keys.json
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/carry_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/entities_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/extract_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/having_sentiment.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.095133 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/having_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/sentiment_extracted.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.099134 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/having_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/sentiment_extracted.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.099134 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/having_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/sentiment_extracted.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:08.931133 unitxt-1.7.7/src/unitxt/catalog/templates/translation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.099134 unitxt-1.7.7/src/unitxt/catalog/templates/translation/directed/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/translation/directed/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/translation/directed/casual.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/translation/directed/formal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/translation/directed/instructional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/translation/directed/playful.json
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/translation/directed/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog/templates/translation/directed/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/collections_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/deprecation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/dialog_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23755 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/fusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/generator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/hf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/llm_as_judge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17915 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/metric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136915 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/normalizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21477 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77719 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/parsing_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.099134 unitxt-1.7.7/src/unitxt/prepare_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/prepare_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/prepare_utils/card_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/prepare_utils/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/random_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.099134 unitxt-1.7.7/src/unitxt/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.099134 unitxt-1.7.7/src/unitxt/service/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/service/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/service/metrics/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/service/metrics/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/settings_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/span_lableing_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/split_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/string_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17231 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/struct_data_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/system_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20524 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.103134 unitxt-1.7.7/src/unitxt/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/test_utils/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/test_utils/card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/test_utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/test_utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/test_utils/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/test_utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30249 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/type_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.103134 unitxt-1.7.7/src/unitxt/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56810 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/ui/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/ui/gradio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/ui/load_catalog_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/ui/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/ui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/ui/ui_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/ui/ui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 07:23:05.000000 unitxt-1.7.7/src/unitxt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:23:09.103134 unitxt-1.7.7/src/unitxt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-04-17 07:23:08.000000 unitxt-1.7.7/src/unitxt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    49989 2024-04-17 07:23:08.000000 unitxt-1.7.7/src/unitxt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:23:08.000000 unitxt-1.7.7/src/unitxt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-17 07:23:08.000000 unitxt-1.7.7/src/unitxt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-17 07:23:08.000000 unitxt-1.7.7/src/unitxt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 07:23:08.000000 unitxt-1.7.7/src/unitxt.egg-info/top_level.txt
```

### Comparing `unitxt-1.7.6/LICENSE` & `unitxt-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/PKG-INFO` & `unitxt-1.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitxt
-Version: 1.7.6
+Version: 1.7.7
 Summary: Load any mixture of text to text data in one line of code
 Home-page: https://github.com/ibm/unitxt
 Author: IBM Research
 Author-email: elron.bandel@ibm.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -36,14 +36,15 @@
 Requires-Dist: nltk; extra == "docs"
 Requires-Dist: sacrebleu; extra == "docs"
 Requires-Dist: absl-py; extra == "docs"
 Requires-Dist: rouge_score; extra == "docs"
 Requires-Dist: scikit-learn; extra == "docs"
 Requires-Dist: jiwer; extra == "docs"
 Requires-Dist: editdistance; extra == "docs"
+Provides-Extra: helm
 Provides-Extra: ui
 Requires-Dist: gradio; extra == "ui"
 Requires-Dist: transformers; extra == "ui"
 Provides-Extra: tests
 Requires-Dist: bert_score; extra == "tests"
 Requires-Dist: transformers; extra == "tests"
 Requires-Dist: sentence_transformers; extra == "tests"
@@ -57,57 +58,59 @@
 Requires-Dist: sacrebleu[ko]; extra == "tests"
 Requires-Dist: scikit-learn; extra == "tests"
 Requires-Dist: jiwer; extra == "tests"
 Requires-Dist: conllu; extra == "tests"
 Requires-Dist: llama-index-core; extra == "tests"
 Requires-Dist: llama-index-llms-openai; extra == "tests"
 Requires-Dist: pytrec-eval; extra == "tests"
+Requires-Dist: SentencePiece; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tomli; extra == "dev"
 Requires-Dist: codespell; extra == "dev"
 Provides-Extra: all
-Requires-Dist: fastapi==0.109.0; extra == "all"
+Requires-Dist: gradio; extra == "all"
 Requires-Dist: sphinxext-opengraph; extra == "all"
+Requires-Dist: conllu; extra == "all"
+Requires-Dist: torch==1.12.1; extra == "all"
 Requires-Dist: datasets; extra == "all"
-Requires-Dist: ruff; extra == "all"
-Requires-Dist: gradio; extra == "all"
-Requires-Dist: sphinx_rtd_theme; extra == "all"
+Requires-Dist: jiwer; extra == "all"
+Requires-Dist: pre-commit; extra == "all"
+Requires-Dist: pytrec-eval; extra == "all"
+Requires-Dist: sacrebleu; extra == "all"
 Requires-Dist: python-jose[cryptography]==3.3.0; extra == "all"
-Requires-Dist: sentence_transformers; extra == "all"
+Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "all"
 Requires-Dist: nltk; extra == "all"
-Requires-Dist: codespell; extra == "all"
-Requires-Dist: llama-index-core; extra == "all"
-Requires-Dist: rouge_score; extra == "all"
-Requires-Dist: rouge-score; extra == "all"
-Requires-Dist: pytrec-eval; extra == "all"
-Requires-Dist: evaluate; extra == "all"
-Requires-Dist: opendatasets; extra == "all"
 Requires-Dist: ibm-cos-sdk; extra == "all"
-Requires-Dist: mecab-python3; extra == "all"
 Requires-Dist: ipadic; extra == "all"
-Requires-Dist: jiwer; extra == "all"
-Requires-Dist: conllu; extra == "all"
-Requires-Dist: llama-index-llms-openai; extra == "all"
+Requires-Dist: ruff; extra == "all"
+Requires-Dist: SentencePiece; extra == "all"
+Requires-Dist: tomli; extra == "all"
+Requires-Dist: fastapi==0.109.0; extra == "all"
+Requires-Dist: rouge_score; extra == "all"
+Requires-Dist: codespell; extra == "all"
 Requires-Dist: scikit-learn; extra == "all"
-Requires-Dist: pre-commit; extra == "all"
-Requires-Dist: scipy; extra == "all"
-Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "all"
-Requires-Dist: sacrebleu[ko]; extra == "all"
-Requires-Dist: piccolo_theme; extra == "all"
-Requires-Dist: sacrebleu; extra == "all"
-Requires-Dist: editdistance; extra == "all"
-Requires-Dist: httpretty~=1.1.4; extra == "all"
-Requires-Dist: transformers; extra == "all"
+Requires-Dist: opendatasets; extra == "all"
 Requires-Dist: datasets>=2.16.0; extra == "all"
-Requires-Dist: tomli; extra == "all"
-Requires-Dist: torch==1.12.1; extra == "all"
+Requires-Dist: transformers; extra == "all"
 Requires-Dist: absl-py; extra == "all"
+Requires-Dist: llama-index-llms-openai; extra == "all"
+Requires-Dist: editdistance; extra == "all"
+Requires-Dist: httpretty~=1.1.4; extra == "all"
 Requires-Dist: bert_score; extra == "all"
+Requires-Dist: llama-index-core; extra == "all"
+Requires-Dist: scipy; extra == "all"
+Requires-Dist: evaluate; extra == "all"
+Requires-Dist: sacrebleu[ko]; extra == "all"
+Requires-Dist: piccolo_theme; extra == "all"
+Requires-Dist: sentence_transformers; extra == "all"
+Requires-Dist: sphinx_rtd_theme; extra == "all"
+Requires-Dist: rouge-score; extra == "all"
+Requires-Dist: mecab-python3; extra == "all"
 
 <div align="center">
     <img src="./assets/banner.png" alt="Image Description" width="100%" />
 </div>
 
 [![Button](https://img.shields.io/badge/Video-pink?style=for-the-badge)](https://unitxt.readthedocs.io/)
 [![Button](https://img.shields.io/badge/Demo-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/demo.html)
```

### Comparing `unitxt-1.7.6/README.md` & `unitxt-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/pyproject.toml` & `unitxt-1.7.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/setup.py` & `unitxt-1.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/__init__.py` & `unitxt-1.7.7/src/unitxt/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
 
-from .api import evaluate, load, load_dataset
+from .api import evaluate, load, load_dataset, produce
 from .catalog import add_to_catalog, get_from_catalog
 from .logging_utils import get_logger
 from .register import register_all_artifacts, register_local_catalog
 from .settings_utils import get_constants, get_settings
 
 register_all_artifacts()
 random.seed(0)
```

### Comparing `unitxt-1.7.6/src/unitxt/artifact.py` & `unitxt-1.7.7/src/unitxt/artifact.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,22 @@
 import json
 import os
 import pkgutil
 from abc import abstractmethod
 from copy import deepcopy
 from typing import Dict, List, Optional, Union, final
 
-from .dataclass import AbstractField, Dataclass, Field, InternalField, fields
+from .dataclass import (
+    AbstractField,
+    Dataclass,
+    Field,
+    InternalField,
+    NonPositionalField,
+    fields,
+)
 from .logging_utils import get_logger
 from .parsing_utils import (
     separate_inside_and_outside_square_brackets,
 )
 from .settings_utils import get_settings
 from .text_utils import camel_to_snake_case, is_camel_case
 from .type_utils import issubtype
@@ -110,18 +117,18 @@
         super().__init__(message)
 
 
 class Artifact(Dataclass):
     _class_register = {}
 
     type: str = Field(default=None, final=True, init=False)
-    __description__: str = InternalField(
+    __description__: str = NonPositionalField(
         default=None, required=False, also_positional=False
     )
-    __tags__: Dict[str, str] = InternalField(
+    __tags__: Dict[str, str] = NonPositionalField(
         default_factory=dict, required=False, also_positional=False
     )
     __id__: str = InternalField(default=None, required=False, also_positional=False)
 
     @classmethod
     def is_artifact_dict(cls, d):
         return isinstance(d, dict) and "type" in d
```

### Comparing `unitxt-1.7.6/src/unitxt/blocks.py` & `unitxt-1.7.7/src/unitxt/blocks.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/card.py` & `unitxt-1.7.7/src/unitxt/card.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/20_newsgroups/sklearn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/20_newsgroups/sklearn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/20_newsgroups.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/20_newsgroups.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/CFPB/product/2023.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/CFPB/product/2023.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/CFPB/product/watsonx.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/CFPB/product/watsonx.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/ag_news.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/ag_news.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/ai2_arc/arc_challenge.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/ai2_arc/arc_challenge.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/ai2_arc/arc_easy.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/ai2_arc/arc_easy.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/de.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/de.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/en.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/en.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/es.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/es.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/fr.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/fr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/it.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/it.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/nl.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/nl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/pt.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/pt.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil/ru.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil/ru.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/almost_evil.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/almost_evil.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/af_ZA.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/af_ZA.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/all.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/all_1/1.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/all_1/1.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/am_ET.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/am_ET.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ar_SA.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ar_SA.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/az_AZ.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/az_AZ.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/bn_BD.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/bn_BD.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ca_ES.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ca_ES.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/cy_GB.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/cy_GB.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/da_DK.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/da_DK.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/de_DE.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/de_DE.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/el_GR.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/el_GR.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/en_US.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/en_US.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/es_ES.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/es_ES.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/fa_IR.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/fa_IR.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/fi_FI.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/fi_FI.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/fr_FR.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/fr_FR.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/he_IL.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/he_IL.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/hi_IN.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/hi_IN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/hu_HU.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/hu_HU.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/hy_AM.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/hy_AM.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/id_ID.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/id_ID.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/is_IS.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/is_IS.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/it_IT.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/it_IT.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ja_JP.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ja_JP.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/jv_ID.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/jv_ID.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ka_GE.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ka_GE.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/km_KH.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/km_KH.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/kn_IN.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/kn_IN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ko_KR.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ko_KR.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/lv_LV.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/lv_LV.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ml_IN.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ml_IN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/mn_MN.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/mn_MN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ms_MY.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ms_MY.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/my_MM.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/my_MM.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/nb_NO.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/nb_NO.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/nl_NL.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/nl_NL.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/pl_PL.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/pl_PL.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/pt_PT.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/pt_PT.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ro_RO.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ro_RO.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ru_RU.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ru_RU.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sl_SL.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/sl_SL.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sq_AL.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/sq_AL.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sv_SE.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/sv_SE.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/sw_KE.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/sw_KE.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ta_IN.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ta_IN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/te_IN.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/te_IN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/th_TH.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/th_TH.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/tl_PH.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/tl_PH.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/tr_TR.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/tr_TR.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/ur_PK.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/ur_PK.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/vi_VN.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/vi_VN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/zh_CN.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/zh_CN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/amazon_mass/zh_TW.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/amazon_mass/zh_TW.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/argument_topic.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/argument_topic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/atis.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/atis.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/atta_q.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/atta_q.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/babi/qa.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/babi/qa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/banking77.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/banking77.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/acm_arab.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/acm_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/afr_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/afr_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/als_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/als_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/amh_ethi.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/amh_ethi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/apc_arab.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/apc_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/arb_arab.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/arb_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/arb_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/arb_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ars_arab.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ars_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ary_arab.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ary_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/arz_arab.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/arz_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/asm_beng.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/asm_beng.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/azj_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/azj_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/bam_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/bam_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ben_beng.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ben_beng.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ben_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ben_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/bod_tibt.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/bod_tibt.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/bul_cyrl.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/bul_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/cat_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/cat_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ceb_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ceb_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ces_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ces_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ckb_arab.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ckb_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/dan_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/dan_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/deu_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/deu_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ell_grek.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ell_grek.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/eng_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/eng_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/est_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/est_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/eus_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/eus_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/fin_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/fin_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/fra_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/fra_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/fuv_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/fuv_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/gaz_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/gaz_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/grn_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/grn_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/guj_gujr.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/guj_gujr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hat_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/hat_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hau_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/hau_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/heb_hebr.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/heb_hebr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hin_deva.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/hin_deva.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hin_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/hin_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hrv_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/hrv_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hun_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/hun_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/hye_armn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/hye_armn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ibo_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ibo_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ilo_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ilo_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ind_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ind_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/isl_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/isl_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ita_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ita_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/jav_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/jav_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/jpn_jpan.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/jpn_jpan.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kac_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kac_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kan_knda.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kan_knda.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kat_geor.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kat_geor.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kaz_cyrl.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kaz_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kea_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kea_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/khk_cyrl.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/khk_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/khm_khmr.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/khm_khmr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kin_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kin_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kir_cyrl.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kir_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/kor_hang.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/kor_hang.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lao_laoo.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/lao_laoo.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lin_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/lin_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lit_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/lit_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lug_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/lug_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/luo_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/luo_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/lvs_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/lvs_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mal_mlym.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/mal_mlym.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mar_deva.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/mar_deva.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mkd_cyrl.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/mkd_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mlt_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/mlt_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mri_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/mri_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/mya_mymr.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/mya_mymr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nld_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/nld_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nob_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/nob_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/npi_deva.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/npi_deva.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/npi_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/npi_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nso_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/nso_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/nya_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/nya_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ory_orya.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ory_orya.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pan_guru.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/pan_guru.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pbt_arab.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/pbt_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pes_arab.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/pes_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/plt_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/plt_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/pol_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/pol_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/por_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/por_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ron_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ron_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/rus_cyrl.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/rus_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/shn_mymr.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/shn_mymr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sin_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/sin_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sin_sinh.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/sin_sinh.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/slk_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/slk_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/slv_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/slv_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sna_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/sna_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/snd_arab.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/snd_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/som_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/som_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sot_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/sot_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/spa_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/spa_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/srp_cyrl.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/srp_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ssw_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ssw_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/sun_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/sun_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/swe_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/swe_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/swh_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/swh_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tam_taml.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tam_taml.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tel_telu.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tel_telu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tgk_cyrl.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tgk_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tgl_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tgl_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tha_thai.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tha_thai.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tir_ethi.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tir_ethi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tsn_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tsn_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tso_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tso_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/tur_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/tur_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/ukr_cyrl.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/ukr_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/urd_arab.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/urd_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/urd_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/urd_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/uzn_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/uzn_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/vie_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/vie_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/war_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/war_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/wol_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/wol_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/xho_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/xho_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/yor_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/yor_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zho_hans.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/zho_hans.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zho_hant.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/zho_hant.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zsm_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/zsm_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/belebele/zul_latn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/belebele/zul_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/bold.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/bold.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/boolq/classification.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/boolq/classification.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/boolq/multiple_choice.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/boolq/multiple_choice.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/claim_stance_topic.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/claim_stance_topic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/clinc_oos/imbalanced.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/clinc_oos/imbalanced.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/clinc_oos/plus.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/clinc_oos/plus.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/clinc_oos/small.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/clinc_oos/small.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cnn_dailymail.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cnn_dailymail.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/coedit/paraphrase.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/coedit/paraphrase.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/coedit/preference.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/coedit/preference.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/coedit/rewriting.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/coedit/rewriting.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/coedit/selection.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/coedit/selection.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/coedit_error_detection.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/coedit_error_detection.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/coedit_gec.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/coedit_gec.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/eng.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/eng.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/por.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/por.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tel.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tel.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tur.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tur.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/yor.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/yor.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/zho.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/zho.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/fra.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/fra.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/spa.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/spa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/deu.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/deu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/eng.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/eng.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/fra.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/fra.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/jpn.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/jpn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/por.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/por.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/spa.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/spa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/cola.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/cola.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/copa.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/copa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/coqa/completion.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/coqa/completion.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/coqa/qa.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/coqa/qa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/dart.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/dart.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/dbpedia_14.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/dbpedia_14.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/ethos_binary.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/ethos_binary.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/16k.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/ffqa_filtered/16k.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/2k.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/ffqa_filtered/2k.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/4k.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/ffqa_filtered/4k.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/ffqa_filtered/8k.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/ffqa_filtered/8k.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/financial_tweets.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/financial_tweets.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/head_qa/en.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/head_qa/en.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/head_qa/es.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/head_qa/es.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/hellaswag.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/hellaswag.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/hh_rlhf.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/hh_rlhf.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/human_eval.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/human_eval.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/law_stack_exchange.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/law_stack_exchange.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/ledgar.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/ledgar.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mbpp.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mbpp.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/medical_abstracts.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/medical_abstracts.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/de.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mlsum/de.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/es.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mlsum/es.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/fr.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mlsum/fr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/ru.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mlsum/ru.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mlsum/tu.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mlsum/tu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/abstract_algebra.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/abstract_algebra.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/anatomy.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/anatomy.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/astronomy.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/astronomy.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/business_ethics.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/business_ethics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/clinical_knowledge.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/clinical_knowledge.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_biology.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/college_biology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_chemistry.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/college_chemistry.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_computer_science.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/college_computer_science.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_mathematics.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/college_mathematics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_medicine.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/college_medicine.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/college_physics.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/college_physics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/computer_security.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/computer_security.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/conceptual_physics.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/conceptual_physics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/econometrics.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/econometrics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/electrical_engineering.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/electrical_engineering.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/elementary_mathematics.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/elementary_mathematics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/formal_logic.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/formal_logic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/global_facts.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/global_facts.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_biology.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_biology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_chemistry.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_chemistry.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_european_history.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_european_history.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_geography.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_geography.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_government_and_politics.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_government_and_politics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_macroeconomics.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_macroeconomics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_mathematics.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_mathematics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_physics.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_physics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_psychology.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_psychology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_statistics.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_statistics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_us_history.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_us_history.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/high_school_world_history.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/high_school_world_history.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/human_aging.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/human_aging.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/human_sexuality.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/human_sexuality.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/international_law.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/international_law.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/jurisprudence.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/jurisprudence.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/logical_fallacies.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/logical_fallacies.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/machine_learning.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/machine_learning.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/management.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/management.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/marketing.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/marketing.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/medical_genetics.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/medical_genetics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/miscellaneous.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/miscellaneous.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/moral_disputes.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/moral_disputes.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/moral_scenarios.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/moral_scenarios.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/nutrition.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/nutrition.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/philosophy.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/philosophy.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/prehistory.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/prehistory.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_accounting.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/professional_accounting.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_law.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/professional_law.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_medicine.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/professional_medicine.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/professional_psychology.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/professional_psychology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/public_relations.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/public_relations.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/security_studies.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/security_studies.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/sociology.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/sociology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/us_foreign_policy.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/us_foreign_policy.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/virology.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/virology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mmlu/world_religions.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mmlu/world_religions.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mnli.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mnli.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/mrpc.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/mrpc.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/multidoc2dial/abstractive.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/multidoc2dial/abstractive.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/multidoc2dial/extractive.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/multidoc2dial/extractive.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/news_category_classification_headline.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/news_category_classification_headline.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/openbook_qa.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/openbook_qa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/piqa.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/piqa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/pop_qa.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/pop_qa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/qnli.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/qnli.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/qqp.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/qqp.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/race_all.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/race_all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/race_high.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/race_high.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/race_middle.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/race_middle.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/reuters21578/ModApte.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/reuters21578/ModApte.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/reuters21578/ModHayes.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/reuters21578/ModHayes.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/reuters21578/ModLewis.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/reuters21578/ModLewis.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/rte.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/rte.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/sciq.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/sciq.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/squad.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/squad.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/sst2.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/sst2.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/stsb.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/stsb.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/summarize_from_human_feedback.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/summarize_from_human_feedback.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/tab_fact.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/tab_fact.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/tablerow_classify.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/tablerow_classify.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/toxigen.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/toxigen.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/trec.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/trec.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/unfair_tos.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/unfair_tos.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/ceb/gja.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/ceb/gja.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/da/ddt.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/da/ddt.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/de/pud.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/de/pud.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/en/ewt.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/en/ewt.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/en/pud.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/en/pud.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/hr/set.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/hr/set.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/pt/bosque.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/pt/bosque.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/pt/pud.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/pt/pud.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/ru/pud.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/ru/pud.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sk/snk.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/sk/snk.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sr/set.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/sr/set.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sv/pud.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/sv/pud.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/sv/talbanken.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/sv/talbanken.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/tl/trg.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/tl/trg.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/zh/gsd.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/zh/gsd.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/universal_ner/zh/pud.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/universal_ner/zh/pud.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/wiki_bio.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/wiki_bio.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/wikitq.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/winogrande/xs.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6875%*

 * *Differences: {"'loader'": "{'path': 'winogrande', 'name': 'winogrande_xs'}",*

 * * "'preprocess_steps'": "{2: {'type': 'cast_fields', 'fields': {replace: OrderedDict([('answer', "*

 * *                       "'int')])}}, 3: {'type': 'add_constant', 'field': 'answer', 'add': -1, "*

 * *                       "delete: ['rows_to_keep']}, 4: {'type': 'rename_fields', 'field_to_field': "*

 * *                       "{replace: OrderedDict([('sentence', 'question')])}}, insert: [(1, "*

 * *                       "OrderedDict([('type', 'list_field_valu […]*

```diff
@@ -1,38 +1,38 @@
 {
     "loader": {
-        "path": "wikitablequestions",
+        "name": "winogrande_xs",
+        "path": "winogrande",
         "type": "load_hf"
     },
     "preprocess_steps": [
         "splitters.small_no_test",
         {
-            "fields": {
-                "context_type": "table"
-            },
-            "type": "add_fields"
+            "fields": [
+                "option1",
+                "option2"
+            ],
+            "to_field": "choices",
+            "type": "list_field_values"
         },
         {
-            "max_length": 15,
-            "table": "table",
-            "text_output": "answers",
-            "type": "truncate_table_cells"
+            "fields": {
+                "answer": "int"
+            },
+            "type": "cast_fields"
         },
         {
-            "field": "table",
-            "rows_to_keep": 50,
-            "type": "truncate_table_rows"
+            "add": -1,
+            "field": "answer",
+            "type": "add_constant"
         },
         {
-            "field_to_field": [
-                [
-                    "table",
-                    "context"
-                ]
-            ],
-            "type": "serialize_table_as_indexed_row_major"
+            "field_to_field": {
+                "sentence": "question"
+            },
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.with_context.extractive",
-    "templates": "templates.qa.with_context.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/debiased.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/winogrande/debiased.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/l.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/winogrande/l.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/m.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/winogrande/m.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/s.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/winogrande/s.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/xl.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/winogrande/xl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/winogrande/xs.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/wnli/truthfulness.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6916666666666667%*

 * *Differences: {"'loader'": "{'path': 'glue', 'name': 'wnli'}",*

 * * "'preprocess_steps'": "{1: {'field_to_field': {replace: OrderedDict([('sentence1', 'text_a'), "*

 * *                       "('sentence2', 'text_b')])}}, insert: [(2, OrderedDict([('type', "*

 * *                       "'map_instance_values'), ('mappers', OrderedDict([('label', "*

 * *                       "OrderedDict([('0', 'yes'), ('1', 'no')]))]))])), (3, OrderedDict([('type', "*

 * *                       "'add_fields'), ('fields', OrderedDict([('classes', ['yes', 'no']), […]*

```diff
@@ -1,38 +1,41 @@
 {
     "loader": {
-        "name": "winogrande_xs",
-        "path": "winogrande",
+        "name": "wnli",
+        "path": "glue",
         "type": "load_hf"
     },
     "preprocess_steps": [
         "splitters.small_no_test",
         {
-            "fields": [
-                "option1",
-                "option2"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "fields": {
-                "answer": "int"
+            "field_to_field": {
+                "sentence1": "text_a",
+                "sentence2": "text_b"
             },
-            "type": "cast_fields"
+            "type": "rename_fields"
         },
         {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "mappers": {
+                "label": {
+                    "0": "yes",
+                    "1": "no"
+                }
+            },
+            "type": "map_instance_values"
         },
         {
-            "field_to_field": {
-                "sentence": "question"
+            "fields": {
+                "classes": [
+                    "yes",
+                    "no"
+                ],
+                "text_a_type": "premise",
+                "text_b_type": "hypothesis",
+                "type_of_relation": "truthfulness"
             },
-            "type": "rename_fields"
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
+    "task": "tasks.classification.multi_class.relation",
+    "templates": "templates.classification.multi_class.relation.truthfulness.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/wmt/en_de.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/wmt/en_de.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/wmt/en_fr.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/wmt/en_fr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/wmt/en_ro.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/wmt/en_ro.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/wnli/truthfulness.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xnli/ar.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8387499999999999%*

 * *Differences: {"'loader'": "{'path': 'xnli', 'name': 'ar'}",*

 * * "'preprocess_steps'": "{2: {'field_to_field': {replace: OrderedDict([('premise', 'text_a'), "*

 * *                       "('hypothesis', 'text_b')])}}, 3: {'mappers': {'label': {'0': 'entailment', "*

 * *                       "'1': 'neutral', '2': 'contradiction'}}}, 4: {'fields': {'classes': "*

 * *                       "['entailment', 'neutral', 'contradiction'], 'type_of_relation': "*

 * *                       "'entailment'}}, insert: [(0, OrderedDict([('type', 'rename_spl […]*

```diff
@@ -1,41 +1,49 @@
 {
     "loader": {
-        "name": "wnli",
-        "path": "glue",
+        "name": "ar",
+        "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        {
+            "mapper": {
+                "validation_matched": "validation"
+            },
+            "type": "rename_splits"
+        },
         "splitters.small_no_test",
         {
             "field_to_field": {
-                "sentence1": "text_a",
-                "sentence2": "text_b"
+                "hypothesis": "text_b",
+                "premise": "text_a"
             },
             "type": "rename_fields"
         },
         {
             "mappers": {
                 "label": {
-                    "0": "yes",
-                    "1": "no"
+                    "0": "entailment",
+                    "1": "neutral",
+                    "2": "contradiction"
                 }
             },
             "type": "map_instance_values"
         },
         {
             "fields": {
                 "classes": [
-                    "yes",
-                    "no"
+                    "entailment",
+                    "neutral",
+                    "contradiction"
                 ],
                 "text_a_type": "premise",
                 "text_b_type": "hypothesis",
-                "type_of_relation": "truthfulness"
+                "type_of_relation": "entailment"
             },
             "type": "add_fields"
         }
     ],
     "task": "tasks.classification.multi_class.relation",
-    "templates": "templates.classification.multi_class.relation.truthfulness.all",
+    "templates": "templates.classification.multi_class.relation.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/wnli.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/wnli.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/wsc.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/wsc.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/amharic.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/amharic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/arabic.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/arabic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/azerbaijani.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/azerbaijani.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/bengali.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/bengali.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/burmese.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/burmese.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/chinese_simplified.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/chinese_simplified.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/chinese_traditional.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/chinese_traditional.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/english.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/english.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/french.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/french.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/gujarati.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/gujarati.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/hausa.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/hausa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/hindi.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/hindi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/igbo.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/igbo.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/indonesian.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/indonesian.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/japanese.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/japanese.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/kirundi.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/kirundi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/korean.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/korean.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/kyrgyz.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/kyrgyz.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/marathi.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/marathi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/nepali.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/nepali.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/oromo.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/oromo.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/pashto.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/pashto.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/persian.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/persian.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/pidgin.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/pidgin.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/portuguese.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/portuguese.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/punjabi.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/punjabi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/russian.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/russian.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/scottish_gaelic.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/scottish_gaelic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/serbian_cyrillic.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/serbian_cyrillic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/serbian_latin.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/serbian_latin.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/sinhala.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/sinhala.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/somali.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/somali.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/spanish.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/spanish.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/swahili.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/swahili.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/tamil.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/tamil.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/telugu.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/telugu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/thai.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/thai.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/tigrinya.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/tigrinya.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/turkish.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/turkish.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/ukrainian.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/ukrainian.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/urdu.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/urdu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/uzbek.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/uzbek.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/vietnamese.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/vietnamese.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/welsh.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/welsh.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xlsum/yoruba.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xlsum/yoruba.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/ar.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xnli/en.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'en'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "ar",
+        "name": "en",
         "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
                 "validation_matched": "validation"
```

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/bg.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xnli/bg.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/de.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xnli/de.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/el.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xnli/el.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/en.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xnli/fr.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'fr'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "en",
+        "name": "fr",
         "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
                 "validation_matched": "validation"
```

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/es.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xnli/es.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/fr.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xnli/hi.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'hi'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "fr",
+        "name": "hi",
         "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
                 "validation_matched": "validation"
```

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/hi.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xnli/zh.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'loader'": "{'name': 'zh'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "loader": {
-        "name": "hi",
+        "name": "zh",
         "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
                 "validation_matched": "validation"
```

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/ru.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xnli/ru.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/sw.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xnli/sw.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/th.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xnli/th.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/tr.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xnli/tr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/ur.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xnli/ur.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xnli/vi.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xnli/vi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/en.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xwinogrande/en.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/jp.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xwinogrande/jp.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/pt.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xwinogrande/pt.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/ru.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xwinogrande/ru.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/xwinogrande/zh.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/xwinogrande/zh.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/cards/yahoo_answers_topics.json` & `unitxt-1.7.7/src/unitxt/catalog/cards/yahoo_answers_topics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/normalized_sacrebleu.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/normalized_sacrebleu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/answer_correctness.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/rag/answer_correctness.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/answer_reward.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/rag/answer_reward.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/bert_k_precision.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/rag/bert_k_precision.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/bert_recall.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/rag/bert_recall.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/context_correctness.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/rag/context_correctness.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/context_perplexity.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/rag/context_perplexity.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/context_relevance.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/rag/context_relevance.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/faithfulness.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/rag/faithfulness.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/k_precision.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/rag/k_precision.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/map.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/rag/map.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/mrr.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/rag/mrr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/rag/recall.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/rag/recall.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/sacrebleu.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/sacrebleu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/spearman.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/spearman.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/squad.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/squad.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/metrics/token_overlap_with_context.json` & `unitxt-1.7.7/src/unitxt/catalog/metrics/token_overlap_with_context.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/processors/to_span_label_pairs.json` & `unitxt-1.7.7/src/unitxt/catalog/processors/to_span_label_pairs.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json` & `unitxt-1.7.7/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/labradorite.json` & `unitxt-1.7.7/src/unitxt/catalog/system_prompts/models/labradorite.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/llama.json` & `unitxt-1.7.7/src/unitxt/catalog/system_prompts/models/llama.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/system_prompts/models/llama2.json` & `unitxt-1.7.7/src/unitxt/catalog/system_prompts/models/llama2.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json` & `unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/default.json` & `unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_label/default.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/instruction.json` & `unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_label/instruction.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/templates/classification/multi_label/title.json` & `unitxt-1.7.7/src/unitxt/catalog/templates/classification/multi_label/title.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/templates/evaluation/preference/default.json` & `unitxt-1.7.7/src/unitxt/catalog/templates/evaluation/preference/default.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json` & `unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json` & `unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/match.json` & `unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/match.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/title.json` & `unitxt-1.7.7/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/title.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json` & `unitxt-1.7.7/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'postprocessors'": "['processors.take_first_non_empty_line']"}*

```diff
@@ -1,7 +1,10 @@
 {
     "input_format": "Sentence 1: {text1} Sentence 2: {text2}",
     "instruction": "Evaluate the similarity between them and classify them into classes from 0-5 as follows:\n0 : The two sentences are completely dissimilar.\n1 : The two sentences are not equivalent, but are on the same topic.\n2 : The two sentences are not equivalent, but share some details.\n3 : The two sentences are roughly equivalent, but some important information differs/missing.\n4 : The two sentences are mostly equivalent, but some unimportant details differ.\n5 : The two sentences are completely equivalent, as they mean the same thing.",
     "output_format": "{attribute_value}",
+    "postprocessors": [
+        "processors.take_first_non_empty_line"
+    ],
     "quantum": 1,
     "type": "output_quantizing_template"
 }
```

### Comparing `unitxt-1.7.6/src/unitxt/catalog/templates/selection/by_attribute/default.json` & `unitxt-1.7.7/src/unitxt/catalog/templates/selection/by_attribute/default.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/templates/summarization/abstractive/all.json` & `unitxt-1.7.7/src/unitxt/catalog/templates/summarization/abstractive/all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json` & `unitxt-1.7.7/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/catalog.py` & `unitxt-1.7.7/src/unitxt/catalog.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/collections.py` & `unitxt-1.7.7/src/unitxt/collections.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/collections_operators.py` & `unitxt-1.7.7/src/unitxt/collections_operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/dataclass.py` & `unitxt-1.7.7/src/unitxt/dataclass.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/dataset.py` & `unitxt-1.7.7/src/unitxt/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 
 import datasets
 
+from .api import __file__ as _
 from .artifact import __file__ as _
 from .blocks import __file__ as _
 from .card import __file__ as _
 from .catalog import __file__ as _
 from .collections import __file__ as _
 from .collections_operators import __file__ as _
 from .dataclass import __file__ as _
@@ -15,15 +16,17 @@
 from .dict_utils import __file__ as _
 from .eval_utils import __file__ as _
 from .file_utils import __file__ as _
 from .formats import __file__ as _
 from .fusion import __file__ as _
 from .generator_utils import __file__ as _
 from .hf_utils import verify_versions_compatibility
+from .inference import __file__ as _
 from .instructions import __file__ as _
+from .llm_as_judge import __file__ as _
 from .loaders import __file__ as _
 from .logging_utils import get_logger
 from .metric import __file__ as _
 from .metric_utils import __file__ as _
 from .metrics import __file__ as _
 from .normalizers import __file__ as _
 from .operator import __file__ as _
```

### Comparing `unitxt-1.7.6/src/unitxt/dataset_utils.py` & `unitxt-1.7.7/src/unitxt/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/deprecation_utils.py` & `unitxt-1.7.7/src/unitxt/deprecation_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/dialog_operators.py` & `unitxt-1.7.7/src/unitxt/dialog_operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/dict_utils.py` & `unitxt-1.7.7/src/unitxt/dict_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/eval_utils.py` & `unitxt-1.7.7/src/unitxt/eval_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/file_utils.py` & `unitxt-1.7.7/src/unitxt/file_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/formats.py` & `unitxt-1.7.7/src/unitxt/formats.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/fusion.py` & `unitxt-1.7.7/src/unitxt/fusion.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/generator_utils.py` & `unitxt-1.7.7/src/unitxt/generator_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/hf_utils.py` & `unitxt-1.7.7/src/unitxt/hf_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/loaders.py` & `unitxt-1.7.7/src/unitxt/loaders.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/logging_utils.py` & `unitxt-1.7.7/src/unitxt/logging_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/metric.py` & `unitxt-1.7.7/src/unitxt/metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Dict, Iterable, List
 
 import evaluate
 
+from .api import __file__ as _
 from .artifact import __file__ as _
 from .blocks import __file__ as _
 from .card import __file__ as _
 from .catalog import __file__ as _
 from .collections import __file__ as _
 from .collections_operators import __file__ as _
 from .dataclass import __file__ as _
@@ -15,15 +16,17 @@
 from .dict_utils import __file__ as _
 from .eval_utils import __file__ as _
 from .file_utils import __file__ as _
 from .formats import __file__ as _
 from .fusion import __file__ as _
 from .generator_utils import __file__ as _
 from .hf_utils import verify_versions_compatibility
+from .inference import __file__ as _
 from .instructions import __file__ as _
+from .llm_as_judge import __file__ as _
 from .loaders import __file__ as _
 from .logging_utils import __file__ as _
 from .metric_utils import UNITXT_METRIC_SCHEMA, _compute
 from .metrics import __file__ as _
 from .normalizers import __file__ as _
 from .operator import __file__ as _
 from .operators import __file__ as _
```

### Comparing `unitxt-1.7.6/src/unitxt/metric_utils.py` & `unitxt-1.7.7/src/unitxt/metric_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/metrics.py` & `unitxt-1.7.7/src/unitxt/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1875,22 +1875,25 @@
 class BertScore(HuggingfaceBulkMetric):
     hf_metric_name = "bertscore"
     main_score = "f1"
     reduction_map = {"mean": ["f1", "precision", "recall"]}
     hf_metric_fields = ["f1", "precision", "recall"]
     ci_scores = ["f1", "precision", "recall"]
     model_name: str
+    model_layer: int = None
 
     prediction_type = "str"
 
     _requirements_list: List[str] = ["bert_score"]
 
     def prepare(self):
         super().prepare()
-        self.hf_compute_args = {"model_type": self.model_name, "batch_size": 16}
+        self.hf_compute_args = {"model_type": self.model_name, "batch_size": 32}
+        if self.model_layer:
+            self.hf_compute_args["num_layers"] = self.model_layer
 
 
 class SentenceBert(BulkInstanceMetric):
     reduction_map = {"mean": ["score"]}
     main_score = "score"
     batch_size: int = 32
 
@@ -1943,14 +1946,17 @@
 class Reward(BulkInstanceMetric):
     reduction_map = {"mean": ["score"]}
     main_score = "score"
     batch_size: int = 32
 
     model_name: str
 
+    prediction_type = "str"
+    single_reference_per_prediction = True
+
     _requirements_list: List[str] = ["transformers", "torch"]
 
     def prepare(self):
         super().prepare()
         import torch
         from transformers import pipeline
 
@@ -2137,17 +2143,21 @@
 class Perplexity(BulkInstanceMetric):
     """Computes the likelihood of generating text Y after text X - P(Y|X)."""
 
     main_score = "perplexity"
     reduction_map = {"mean": ["perplexity"]}
     prediction_type = "str"
 
-    perplexity_prompt: str
+    source_template: str
+    target_template: str
     batch_size: int = 32
     model_name: str
+    single_token_mode: bool = False
+
+    lm = None
 
     _requirements_list: List[str] = ["transformers", "torch"]
 
     def compute(
         self,
         references: List[List[Any]],
         predictions: List[Any],
@@ -2156,32 +2166,49 @@
         """Computes the likelihood of generating text Y after text X - P(Y|X).
 
         :param predictions: the list of Y texts = the targets of the generation
         :param references: the list of list of X texts = the sources of the generation
 
         :return: the likelihood of generating text Y_i after each text X_i_j = P(Y_i|X_i_1), ..., P(Y_i|X_i_n)  for every i.
         """
+        if self.lm is None:
+            from transformers import AutoConfig
+
+            config = AutoConfig.from_pretrained(self.model_name, trust_remote_code=True)
+            self.lm = (
+                self.EncoderDecoderLM(
+                    model_name=self.model_name, single_token_mode=self.single_token_mode
+                )
+                if config.is_encoder_decoder is True
+                else self.DecoderOnlyLM(
+                    model_name=self.model_name, single_token_mode=self.single_token_mode
+                )
+            )
+
         sources = []
         targets = []
         for prediction, instance_references in zip(predictions, references):
             for instance_reference in instance_references:
-                sources.append(f"{self.perplexity_prompt} {instance_reference}")
-                targets.append(prediction)
-
-        from transformers import AutoConfig
-
-        config = AutoConfig.from_pretrained(self.model_name, trust_remote_code=True)
-        lm = (
-            self.EncoderDecoderLM(model_name=self.model_name)
-            if config.is_encoder_decoder is True
-            else self.DecoderOnlyLM(model_name=self.model_name)
-        )
+                sources.append(
+                    self.Template.apply(
+                        self.source_template,
+                        prediction=prediction,
+                        reference=instance_reference,
+                    )
+                )
+                targets.append(
+                    self.Template.apply(
+                        self.target_template,
+                        prediction=prediction,
+                        reference=instance_reference,
+                    )
+                )
 
         # compute P(Q|P) and store in queue
-        scores = lm.compute_lm(
+        scores = self.lm.compute_lm(
             source=sources, target=targets, batch_size=self.batch_size
         )
 
         index = 0
         all_instances_scores = []
         for instance_references in references:
             instance_scores = {}
@@ -2196,25 +2223,43 @@
             # is at least one good result in the context. Using mean will
             # bring the score down due to bad contexts at the tail.
             instance_scores[self.main_score] = max(instance_scores_list)
             all_instances_scores.append(instance_scores)
 
         return all_instances_scores
 
+    class Template:
+        regex = re.compile(r"\{(\w+)}")
+
+        @classmethod
+        def apply(cls, template, **kwargs):
+            matches = Perplexity.Template.regex.finditer(template)
+            output = []
+            cursor = 0
+            for match in matches:
+                start = match.start()
+                end = match.end()
+                output.append(template[cursor:start])
+                output.append(kwargs[match.group(1)])
+                cursor = end
+            output.append(template[cursor:])
+            return "".join(output)
+
     class AbstractLM(ABC):
-        def __init__(self, model_name):
+        def __init__(self, model_name, single_token_mode):
             import torch
             from transformers import AutoTokenizer
 
             self.model_name = model_name
             self.device = "cuda:0" if torch.cuda.is_available() else "cpu"
             self.model = (
                 self.model_class().from_pretrained(self.model_name).to(self.device)
             )
             self.tokenizer = AutoTokenizer.from_pretrained(self.model_name)
+            self.single_token_mode = single_token_mode
 
         def compute_lm(
             self, source: List[str], target: List[str], batch_size: int
         ) -> List[float]:
             import torch
 
             scores = []
@@ -2228,15 +2273,18 @@
                     batch_target = target[batch * batch_size : (batch + 1) * batch_size]
                     if len(batch_source) > 0:
                         # tokenize the source and target
                         tokens_source = self.tokenizer(
                             batch_source, padding=True, return_tensors="pt"
                         )
                         tokens_target = self.tokenizer(
-                            batch_target, padding=True, return_tensors="pt"
+                            batch_target,
+                            padding=True,
+                            return_tensors="pt",
+                            add_special_tokens=not self.single_token_mode,
                         )
 
                         # compute the logits
                         logits, labels = self.compute_batch(
                             tokens_source, tokens_target
                         )
 
@@ -3349,40 +3397,69 @@
 
     prediction_type = "str"
     single_reference_per_prediction = True
 
     def compute(
         self,
         references: List[List[str]],
-        predictions: List[List[str]],
+        predictions: List[str],
         task_data: List[Dict],
     ) -> dict:
         float_predictions = [to_float_or_default(p) for p in predictions]
         references = [
             ["1"] if r[0].lower() in self.pos_classes else ["0"] for r in references
         ]
 
-        best_thr = -1
-        best_acc = -1
-        for thr in set(float_predictions):
-            new_predictions = [
-                "1" if float_prediction >= thr else "0"
-                for float_prediction in float_predictions
-            ]
-            acc = np.mean(
-                [
-                    [prediction] == reference
-                    for prediction, reference in zip(new_predictions, references)
-                ]
-            )
-            if acc > best_acc:
-                best_acc = acc
-                best_thr = thr
+        # Sticking to the test >= thr, accuracy induced by threshold thr is the number of float predictions
+        # that pass the test (are >= thr) and are paired with reference "1" plus the number of float predictions that
+        # fail the test (are < thr) and are paired with reference "0".
+        # A given threshold thr induces the same partition over the float predictions into passing and failing
+        # as threshold thr' induces, with thr' being the smallest among the ones passing the test of thr.
+        # Hence, we only need to review thresholds being float predictions, plus a threshold being larger than
+        # the largest float predictions, to induce the partition into all-failing , none-passing.
+
+        fp = [
+            (float_predictions[i], i, -1 if references[i][0] == "1" else +1)
+            for i in range(len(float_predictions))
+        ]
+        fp.sort()
+        # each triplet above: float-prediction f; f's ordinal position in float_predictions, which is also
+        # a means to obtain distinct triplets; and: the change in number of predictions that the test sends
+        # to the reference they are paired with, a change implied by a move of thr that transfers f
+        # from the set of passing the test to the set of failing it.
+
+        rightmost_thr = 1.0 if fp[-1][0] < 1 else fp[-1][0] + 0.01
+        # trying to be esthetic, have the threshold within [0,1], although this is not a requirement,
+        # and even the float predictions are not guaranteed to be within the range [0,1]
+
+        current_thr = fp[0][0]
+        # partition float_predictions into all-passing, none-failing
+        current_acc = sum(r[0] == "1" for r in references)
+        # number of predictions that thr sends to the reference they are paired with
+
+        best_acc = current_acc
+        best_thr = current_thr
+
+        i = 0
+        while (i < len(predictions)) and (best_acc < len(predictions)):
+            # best_acc can not exceed len(predictions)
+            delta = fp[i][2]
+            i += 1
+            while i < len(predictions) and fp[i][0] <= fp[i - 1][0]:
+                delta += fp[i][2]
+                i += 1
+            current_acc += delta
+            if current_acc > best_acc:
+                best_acc = current_acc
+                best_thr = fp[i][0] if i < len(predictions) else rightmost_thr
 
-        return {self.main_score: best_acc, "best_thr_max_acc": best_thr}
+        return {
+            self.main_score: float(best_acc) / len(predictions),
+            "best_thr_max_acc": best_thr,
+        }
 
 
 ######################
 # RerankRecallMetric #
 
 
 def pytrec_eval_at_k(results, qrels, at_k, metric_name):
```

### Comparing `unitxt-1.7.6/src/unitxt/normalizers.py` & `unitxt-1.7.7/src/unitxt/normalizers.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/operator.py` & `unitxt-1.7.7/src/unitxt/operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,22 @@
         return self.process(*args, **kwargs)
 
     @abstractmethod
     def process(self, *args, **kwargs) -> MultiStream:
         pass
 
 
+def instance_generator(instance):
+    yield instance
+
+
+def stream_single(instance: Dict[str, Any]) -> Stream:
+    return Stream(generator=instance_generator, gen_kwargs={"instance": instance})
+
+
 class MultiStreamOperator(StreamingOperator):
     """A class representing a multi-stream operator in the streaming system.
 
     A multi-stream operator is a type of `StreamingOperator` that operates on an entire MultiStream object at once. It takes a `MultiStream` as input and produces a `MultiStream` as output. The `process` method should be implemented by subclasses to define the specific operations to be performed on the input `MultiStream`.
     """
 
     caching: bool = NonPositionalField(default=None)
@@ -194,15 +202,15 @@
         return result
 
     @abstractmethod
     def process(self, multi_stream: MultiStream) -> MultiStream:
         pass
 
     def process_instance(self, instance, stream_name="tmp"):
-        multi_stream = MultiStream({stream_name: [instance]})
+        multi_stream = MultiStream({stream_name: stream_single(instance)})
         processed_multi_stream = self(multi_stream)
         return next(iter(processed_multi_stream[stream_name]))
 
 
 class SingleStreamOperator(MultiStreamOperator):
     """A class representing a single-stream operator in the streaming system.
 
@@ -265,15 +273,17 @@
         yield from self.process(stream, stream_name)
 
     @abstractmethod
     def process(self, stream: Stream, stream_name: Optional[str] = None) -> Generator:
         pass
 
     def process_instance(self, instance, stream_name="tmp"):
-        processed_stream = self._process_single_stream([instance], stream_name)
+        processed_stream = self._process_single_stream(
+            stream_single(instance), stream_name
+        )
         return next(iter(processed_stream))
 
 
 class PagedStreamOperator(SingleStreamOperator):
     """A class representing a paged-stream operator in the streaming system.
 
     A paged-stream operator is a type of `SingleStreamOperator` that operates on a page of instances
```

### Comparing `unitxt-1.7.6/src/unitxt/operators.py` & `unitxt-1.7.7/src/unitxt/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1158,28 +1158,33 @@
 
         # we now have a list of nanes of operators, each is equipped with process_instance method.
         operator = SequentialOperator(steps=operator_names)
         return operator.process_instance(instance)
 
 
 class FilterByCondition(SingleStreamOperator):
-    """Filters a stream, yielding only instances for which the required values follows the required condition operator.
+    """Filters a stream, yielding only instances in which the values in required fields follow the required condition operator.
 
-    Raises an error if a required key is missing.
+    Raises an error if a required field name is missing from the input instance.
 
     Args:
-       values (Dict[str, Any]): Values that instances must match using the condition to be included in the output.
-       condition: the name of the desired condition operator between the key and the value in values ("gt", "ge", "lt", "le", "ne", "eq")
+       values (Dict[str, Any]): Field names and respective Values that instances must match according the condition, to be included in the output.
+       condition: the name of the desired condition operator between the specified (sub) field's value  and the provided constant value.  Supported conditions are  ("gt", "ge", "lt", "le", "ne", "eq", "in","not in")
        error_on_filtered_all (bool, optional): If True, raises an error if all instances are filtered out. Defaults to True.
 
     Examples:
-       FilterByCondition(values = {"a":4}, condition = "gt") will yield only instances where "a">4
+       FilterByCondition(values = {"a":4}, condition = "gt") will yield only instances where field "a" contains a value > 4
        FilterByCondition(values = {"a":4}, condition = "le") will yield only instances where "a"<=4
        FilterByCondition(values = {"a":[4,8]}, condition = "in") will yield only instances where "a" is 4 or 8
        FilterByCondition(values = {"a":[4,8]}, condition = "not in") will yield only instances where "a" different from 4 or 8
+       FilterByCondition(values = {"a/b":[4,8]}, condition = "not in") will yield only instances where "a" is
+            a dict in which key "b" is mapped to a value that is neither 4 nor 8
+       FilterByCondition(values = {"a[2]":4}, condition = "le") will yield only instances where "a" is a list whose 3-rd
+            element is <= 4
+
 
     """
 
     values: Dict[str, Any]
     condition: str
     condition_to_func = {
         "gt": operator.gt,
@@ -1216,31 +1221,33 @@
                 raise ValueError(
                     f"The filter for key ('{key}') in FilterByCondition with condition '{self.condition}' must be list but is not : '{value}'"
                 )
         return super().verify()
 
     def _is_required(self, instance: dict) -> bool:
         for key, value in self.values.items():
-            if key not in instance:
+            try:
+                instance_key = dict_get(instance, key)
+            except ValueError as ve:
                 raise ValueError(
                     f"Required filter field ('{key}') in FilterByCondition is not found in {instance}"
-                )
+                ) from ve
             if self.condition == "in":
-                if instance[key] not in value:
+                if instance_key not in value:
                     return False
             elif self.condition == "not in":
-                if instance[key] in value:
+                if instance_key in value:
                     return False
             else:
                 func = self.condition_to_func[self.condition]
                 if func is None:
                     raise ValueError(
                         f"Function not defined for condition '{self.condition}'"
                     )
-                if not func(instance[key], value):
+                if not func(instance_key, value):
                     return False
         return True
 
 
 class ComputeExpressionMixin(Artifact):
     """Computes an expression expressed over fields of an instance.
 
@@ -1281,14 +1288,16 @@
        error_on_filtered_all (bool, optional): If True, raises an error if all instances are filtered out. Defaults to True.
 
     Examples:
        FilterByExpression(expression = "a > 4") will yield only instances where "a">4
        FilterByExpression(expression = "a <= 4 and b > 5") will yield only instances where the value of field "a" is not exceeding 4 and in field "b" -- greater than 5
        FilterByExpression(expression = "a in [4, 8]") will yield only instances where "a" is 4 or 8
        FilterByExpression(expression = "a not in [4, 8]") will yield only instances where "a" is neither 4 nor 8
+       FilterByExpression(expression = "a['b'] not in [4, 8]") will yield only instances where "a" is a dict in
+                                        which key 'b' is mapped to a value that is neither 4 nor 8
 
     """
 
     error_on_filtered_all: bool = True
 
     def process(self, stream: Stream, stream_name: Optional[str] = None) -> Generator:
         yielded = False
```

### Comparing `unitxt-1.7.6/src/unitxt/parsing_utils.py` & `unitxt-1.7.7/src/unitxt/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/prepare_utils/card_types.py` & `unitxt-1.7.7/src/unitxt/prepare_utils/card_types.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/processors.py` & `unitxt-1.7.7/src/unitxt/processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,7 +211,16 @@
 
     def process_value(self, text: Any) -> Any:
         if "not " + self.string.lower() in text.lower():
             return "not " + self.string.lower()
         if self.string.lower() in text.lower():
             return self.string.lower()
         return text
+
+
+class ExtractMtBenchJudgment(FieldOperator):
+    def process_value(self, text: Any) -> Any:
+        match = re.search(r"\[\[([\d]+\.?[\d]*)\]\]", text)
+        try:
+            return float(match.group(1)) / 10
+        except:
+            return 0.0
```

### Comparing `unitxt-1.7.6/src/unitxt/random_utils.py` & `unitxt-1.7.7/src/unitxt/random_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/register.py` & `unitxt-1.7.7/src/unitxt/register.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/schema.py` & `unitxt-1.7.7/src/unitxt/schema.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/service/metrics/main.py` & `unitxt-1.7.7/src/unitxt/service/metrics/main.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/service/metrics/tokens.py` & `unitxt-1.7.7/src/unitxt/service/metrics/tokens.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/settings_utils.py` & `unitxt-1.7.7/src/unitxt/settings_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/span_lableing_operators.py` & `unitxt-1.7.7/src/unitxt/span_lableing_operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/split_utils.py` & `unitxt-1.7.7/src/unitxt/split_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/splitters.py` & `unitxt-1.7.7/src/unitxt/splitters.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/standard.py` & `unitxt-1.7.7/src/unitxt/standard.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import List
 
 from .card import TaskCard
 from .dataclass import Field, InternalField, NonPositionalField, OptionalField
 from .formats import Format, SystemFormat
 from .logging_utils import get_logger
-from .operator import SourceSequentialOperator, StreamingOperator
+from .operator import SequentialOperator, SourceSequentialOperator, StreamingOperator
 from .operators import AddFields, Augmentor, NullAugmentor, StreamRefiner
 from .recipe import Recipe
 from .schema import ToUnitxtGroup
 from .splitters import Sampler, SeparateSplit, SpreadSplit
+from .stream import MultiStream
 from .system_prompts import EmptySystemPrompt, SystemPrompt
 from .templates import Template
 
 logger = get_logger()
 
 
 # Used to give meaningful name to recipe steps
@@ -95,67 +96,136 @@
                 raise ValueError(
                     f"max_train_instances should not exceed loader_limit ({self.loader_limit}), Got max_train_instances={self.max_train_instances}"
                 )
 
     def prepare_refiners(self):
         self.train_refiner.max_instances = self.max_train_instances
         self.train_refiner.apply_to_streams = ["train"]
-        self.steps.append(self.train_refiner)
+        self.processing.steps.append(self.train_refiner)
 
         self.validation_refiner.max_instances = self.max_validation_instances
         self.validation_refiner.apply_to_streams = ["validation"]
-        self.steps.append(self.validation_refiner)
+        self.processing.steps.append(self.validation_refiner)
 
         self.test_refiner.max_instances = self.max_test_instances
         self.test_refiner.apply_to_streams = ["test"]
-        self.steps.append(self.test_refiner)
+        self.processing.steps.append(self.test_refiner)
 
     def prepare_metrics_and_postprocessors(self):
         if self.postprocessors is None:
             postprocessors = self.template.get_postprocessors()
         else:
             postprocessors = self.postprocessors
 
         if self.metrics is None:
             metrics = self.card.task.metrics
         else:
             metrics = self.metrics
         return metrics, postprocessors
 
-    def prepare(self):
+    def set_pipelines(self):
+        self.loading = SequentialOperator()
+        self.metadata = SequentialOperator()
+        self.standardization = SequentialOperator()
+        self.processing = SequentialOperator()
+        self.verblization = SequentialOperator()
+        self.finalize = SequentialOperator()
+
         self.steps = [
-            self.card.loader,
+            self.loading,
+            self.metadata,
+            self.standardization,
+            self.processing,
+            self.verblization,
+            self.finalize,
+        ]
+
+        self.inference_instance = SequentialOperator()
+
+        self.inference_instance.steps = [
+            self.metadata,
+            self.processing,
+        ]
+
+        self.inference_demos = SourceSequentialOperator()
+
+        self.inference_demos.steps = [
+            self.loading,
+            self.metadata,
+            self.standardization,
+            self.processing,
+        ]
+
+        self.inference = SequentialOperator()
+
+        self.inference.steps = [self.verblization, self.finalize]
+
+        self._demos_pool_cache = None
+
+    def production_preprocess(self, task_instances):
+        ms = MultiStream.from_iterables({"__inference__": task_instances})
+        return list(self.inference_instance(ms)["__inference__"])
+
+    def production_demos_pool(self):
+        if self.num_demos > 0:
+            if self._demos_pool_cache is None:
+                self._demos_pool_cache = list(
+                    self.inference_demos()[self.demos_pool_name]
+                )
+            return self._demos_pool_cache
+        return []
+
+    def produce(self, task_instances):
+        """Use the recipe in production to produce model ready query from standard task instance."""
+        self.before_process_multi_stream()
+        multi_stream = MultiStream.from_iterables(
+            {
+                "__inference__": self.production_preprocess(task_instances),
+                self.demos_pool_name: self.production_demos_pool(),
+            }
+        )
+        multi_stream = self.inference(multi_stream)
+        return list(multi_stream["__inference__"])
+
+    def prepare(self):
+        self.set_pipelines()
+
+        loader = self.card.loader
+        if self.loader_limit:
+            loader.loader_limit = self.loader_limit
+            logger.info(f"Loader line limit was set to  {self.loader_limit}")
+        self.loading.steps.append(loader)
+
+        # This is required in case loader_limit is not enforced by the loader
+        if self.loader_limit:
+            self.loading.steps.append(StreamRefiner(max_instances=self.loader_limit))
+
+        self.metadata.steps.append(
             AddFields(
                 fields={
                     "recipe_metadata": {
                         "card": self.card,
                         "template": self.template,
                         "system_prompt": self.system_prompt,
                         "format": self.format,
                     }
                 }
-            ),
-        ]
-
-        if self.loader_limit:
-            self.card.loader.loader_limit = self.loader_limit
-            logger.info(f"Loader line limit was set to  {self.loader_limit}")
-            self.steps.append(StreamRefiner(max_instances=self.loader_limit))
+            )
+        )
 
-        if self.card.preprocess_steps is not None:
-            self.steps.extend(self.card.preprocess_steps)
+        self.standardization.steps.extend(self.card.preprocess_steps)
 
-        self.steps.append(self.card.task)
+        self.processing.steps.append(self.card.task)
 
         if self.augmentor.augment_task_input:
             self.augmentor.set_task_input_fields(self.card.task.augmentable_inputs)
-            self.steps.append(self.augmentor)
+            self.processing.steps.append(self.augmentor)
 
         if self.demos_pool_size is not None:
-            self.steps.append(
+            self.processing.steps.append(
                 CreateDemosPool(
                     from_split=self.demos_taken_from,
                     to_split_names=[self.demos_pool_name, self.demos_taken_from],
                     to_split_sizes=[int(self.demos_pool_size)],
                     remove_targets_from_source_split=self.demos_removed_from_data,
                 )
             )
@@ -169,31 +239,31 @@
                     )
                 self.sampler = self.card.sampler
 
             self.sampler.set_size(self.num_demos)
 
         self.prepare_refiners()
 
-        self.steps.append(self.template)
+        self.verblization.steps.append(self.template)
         if self.num_demos > 0:
-            self.steps.append(
+            self.verblization.steps.append(
                 AddDemosField(
                     source_stream=self.demos_pool_name,
                     target_field=self.demos_field,
                     sampler=self.sampler,
                 )
             )
-        self.steps.append(self.system_prompt)
-        self.steps.append(self.format)
+        self.verblization.steps.append(self.system_prompt)
+        self.verblization.steps.append(self.format)
         if self.augmentor.augment_model_input:
-            self.steps.append(self.augmentor)
+            self.verblization.steps.append(self.augmentor)
 
         metrics, postprocessors = self.prepare_metrics_and_postprocessors()
 
-        self.steps.append(
+        self.finalize.steps.append(
             ToUnitxtGroup(
                 group="unitxt",
                 metrics=metrics,
                 postprocessors=postprocessors,
             )
         )
```

### Comparing `unitxt-1.7.6/src/unitxt/stream.py` & `unitxt-1.7.7/src/unitxt/stream.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/string_operators.py` & `unitxt-1.7.7/src/unitxt/string_operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/struct_data_operators.py` & `unitxt-1.7.7/src/unitxt/struct_data_operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/system_prompts.py` & `unitxt-1.7.7/src/unitxt/system_prompts.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/task.py` & `unitxt-1.7.7/src/unitxt/task.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/templates.py` & `unitxt-1.7.7/src/unitxt/templates.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/test_utils/artifact.py` & `unitxt-1.7.7/src/unitxt/test_utils/artifact.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/test_utils/card.py` & `unitxt-1.7.7/src/unitxt/test_utils/card.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/test_utils/catalog.py` & `unitxt-1.7.7/src/unitxt/test_utils/catalog.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/test_utils/metrics.py` & `unitxt-1.7.7/src/unitxt/test_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/test_utils/operators.py` & `unitxt-1.7.7/src/unitxt/test_utils/operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/text_utils.py` & `unitxt-1.7.7/src/unitxt/text_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/type_utils.py` & `unitxt-1.7.7/src/unitxt/type_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,146 @@
+import ast
 import collections.abc
 import io
 import itertools
 import re
 import typing
 
 from .utils import safe_eval
 
 
+def convert_union_type(type_string: str) -> str:
+    """Converts Python 3.10 union type hints into form compatible with Python 3.9 version.
+
+    Args:
+        type_string (str): A string representation of a Python type hint. It can be any
+                           valid Python type, which does not contain strings (e.g. 'Literal').
+                           Examples include 'List[int|float]', 'str|float|bool' etc.
+
+        Formally, the function depends on the input string adhering to the following rules.
+        Assuming that the input is a valid type hint the function does not check that 'word' is
+        'str', 'bool', 'List' etc. It just depends on the following general structure (spaces ignored):
+        type -> word OR type( | type)* OR word[type( , type)*]
+        word is a sequence of (0 or more) chars, each being any char but: [ ] , |
+        This implies that if any of these 4 chars shows not as a meta char of the input
+        type_string, but inside some constant string (of Literal, for example), the scheme
+        will not work.
+
+        Cases like Literal, that might contain occurrences of the four chars above not as meta chars
+        in the type string, must be handled as special cases by this function, as shown for Literal,
+        as an example. Because 'format_type_string' serves as preprocessing for 'parse_type_string',
+        which has a list of allowed types, of which Literal is not a member, Literal and such are not
+        relevant at all now; and the case is brought here just for an example for future use.
+
+
+    Returns:
+        str: A type string with converted union types, which is compatible with typing module.
+
+    Examples:
+        convert_union_type('List[int|float]') -> 'List[Union[int,float]]'
+        convert_union_type('Optional[int|float|bool]') -> 'Optional[Union[int,float,bool]]'
+
+    """
+
+    def consume_literal(string: str) -> str:
+        # identifies the prefix of string that matches a full Literal typing, with all its constants, including
+        # constants that contain [ ] , etc. on which construct_union_part depends.
+        # string starts with the [ that follows 'Literal'
+        candidate_end = string.find("]")
+        while candidate_end != -1:
+            try:
+                ast.literal_eval(string[: candidate_end + 1])
+                break
+            except Exception:
+                candidate_end = string.find("]", candidate_end + 1)
+
+        if candidate_end == -1:
+            raise ValueError("invalid Literal in input type_string")
+        return string[: candidate_end + 1]
+
+    stack = [""]  # the start of a type
+    input = type_string.strip()
+    next_word = re.compile(r"([^\[\],|]*)([\[\],|]|$)")
+    while len(input) > 0:
+        word = next_word.match(input)
+        input = input[len(word.group(0)) :].strip()
+        stack[-1] += word.group(1)
+        if word.group(2) in ["]", ",", ""]:  # "" for eol:$
+            # top of stack is now complete to a whole type
+            lwt = stack.pop()
+            if (
+                "|" in lwt
+            ):  # the | -s are only at the top level of lwt, not inside any subtype
+                lwt = "Union[" + lwt.replace("|", ",") + "]"
+            lwt += word.group(2)
+            if len(stack) > 0:
+                stack[-1] += lwt
+            else:
+                stack = [lwt]
+            if word.group(2) == ",":
+                stack.append("")  # to start the expected next type
+
+        elif word.group(2) in ["|"]:
+            # top of stack is the last whole element(s) to be union-ed,
+            # and more are expected
+            stack[-1] += "|"
+
+        else:  # "["
+            if word.group(1) == "Literal":
+                literal_ops = consume_literal("[" + input)
+                stack[-1] += literal_ops
+                input = input[len(literal_ops) - 1 :]
+            else:
+                stack[-1] += "["
+                stack.append("")
+                # start type (,type)*  inside the []
+
+    assert len(stack) == 1
+    if "|" in stack[0]:  # these belong to the top level only
+        stack[0] = "Union[" + stack[0].replace("|", ",") + "]"
+    return stack[0]
+
+
+def format_type_string(type_string: str) -> str:
+    """Formats a string representing a valid Python type hint so that it is compatible with Python 3.9 notation.
+
+    Args:
+        type_string (str): A string representation of a Python type hint. This can be any
+                           valid type, which does not contain strings (e.g. 'Literal').
+                           Examples include 'List[int]', 'Dict[str, Any]', 'Optional[List[str]]', etc.
+
+    Returns:
+        str: A formatted type string.
+
+    Examples:
+        format_type_string('list[int | float]') -> 'List[Union[int,float]]'
+        format_type_string('dict[str, Optional[str]]') -> 'Dict[str,Optional[str]]'
+
+    The function formats valid type string (either after or before Python 3.10) into a
+    form compatible with 3.9. This is done by captilizing the first letter of a lower-cased
+    type name and transferring the 'bitwise or operator' into 'Union' notation. The function
+    also removes whitespaces and redundant module name in type names imported from 'typing'
+    module, e.g. 'typing.Tuple' -> 'Tuple'.
+
+    Currently, the capitalization is applied only to types which unitxt allows, i.e.
+    'list', 'dict', 'tuple'. Moreover, the function expects the input to not contain types
+    which contain strings, for example 'Literal'.
+    """
+    types_map = {
+        "list": "List",
+        "tuple": "Tuple",
+        "dict": "Dict",
+        "typing.": "",
+        " ": "",
+    }
+    for old_type, new_type in types_map.items():
+        type_string = type_string.replace(old_type, new_type)
+    return convert_union_type(type_string)
+
+
 def parse_type_string(type_string: str) -> typing.Any:
     """Parses a string representing a Python type hint and evaluates it to return the corresponding type object.
 
     This function uses a safe evaluation context
     to mitigate the risks of executing arbitrary code.
 
     Args:
@@ -20,14 +150,19 @@
     Returns:
         typing.Any: The Python type object corresponding to the given type string.
 
     Raises:
         ValueError: If the type string contains elements not allowed in the safe context
                     or tokens list.
 
+    The function formats the string first if it represents a new Python type hint
+    (i.e. valid since Python 3.10), which uses lowercased names for some types and
+    'bitwise or operator' instead of 'Union', for example: 'list[int|float]' instead
+    of 'List[Union[int,float]]' etc.
+
     The function uses a predefined safe context with common types from the `typing` module
     and basic Python data types. It also defines a list of safe tokens that are allowed
     in the type string.
     """
     safe_context = {
         "Any": typing.Any,
         "List": typing.List,
@@ -37,14 +172,16 @@
         "int": int,
         "str": str,
         "float": float,
         "bool": bool,
         "Optional": typing.Optional,
     }
 
+    type_string = format_type_string(type_string)
+
     safe_tokens = ["[", "]", ",", " "]
     return safe_eval(type_string, safe_context, safe_tokens)
 
 
 def infer_type(obj) -> typing.Any:
     return parse_type_string(infer_type_string(obj))
```

### Comparing `unitxt-1.7.6/src/unitxt/ui/__init__.py` & `unitxt-1.7.7/src/unitxt/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/ui/banner.png` & `unitxt-1.7.7/src/unitxt/ui/banner.png`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/ui/gradio_utils.py` & `unitxt-1.7.7/src/unitxt/ui/gradio_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/ui/load_catalog_data.py` & `unitxt-1.7.7/src/unitxt/ui/load_catalog_data.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/ui/run.py` & `unitxt-1.7.7/src/unitxt/ui/run.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/ui/settings.py` & `unitxt-1.7.7/src/unitxt/ui/settings.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/ui/ui_tester.py` & `unitxt-1.7.7/src/unitxt/ui/ui_tester.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/ui/ui_utils.py` & `unitxt-1.7.7/src/unitxt/ui/ui_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/utils.py` & `unitxt-1.7.7/src/unitxt/utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt/validate.py` & `unitxt-1.7.7/src/unitxt/validate.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.6/src/unitxt.egg-info/PKG-INFO` & `unitxt-1.7.7/src/unitxt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitxt
-Version: 1.7.6
+Version: 1.7.7
 Summary: Load any mixture of text to text data in one line of code
 Home-page: https://github.com/ibm/unitxt
 Author: IBM Research
 Author-email: elron.bandel@ibm.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -36,14 +36,15 @@
 Requires-Dist: nltk; extra == "docs"
 Requires-Dist: sacrebleu; extra == "docs"
 Requires-Dist: absl-py; extra == "docs"
 Requires-Dist: rouge_score; extra == "docs"
 Requires-Dist: scikit-learn; extra == "docs"
 Requires-Dist: jiwer; extra == "docs"
 Requires-Dist: editdistance; extra == "docs"
+Provides-Extra: helm
 Provides-Extra: ui
 Requires-Dist: gradio; extra == "ui"
 Requires-Dist: transformers; extra == "ui"
 Provides-Extra: tests
 Requires-Dist: bert_score; extra == "tests"
 Requires-Dist: transformers; extra == "tests"
 Requires-Dist: sentence_transformers; extra == "tests"
@@ -57,57 +58,59 @@
 Requires-Dist: sacrebleu[ko]; extra == "tests"
 Requires-Dist: scikit-learn; extra == "tests"
 Requires-Dist: jiwer; extra == "tests"
 Requires-Dist: conllu; extra == "tests"
 Requires-Dist: llama-index-core; extra == "tests"
 Requires-Dist: llama-index-llms-openai; extra == "tests"
 Requires-Dist: pytrec-eval; extra == "tests"
+Requires-Dist: SentencePiece; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tomli; extra == "dev"
 Requires-Dist: codespell; extra == "dev"
 Provides-Extra: all
-Requires-Dist: fastapi==0.109.0; extra == "all"
+Requires-Dist: gradio; extra == "all"
 Requires-Dist: sphinxext-opengraph; extra == "all"
+Requires-Dist: conllu; extra == "all"
+Requires-Dist: torch==1.12.1; extra == "all"
 Requires-Dist: datasets; extra == "all"
-Requires-Dist: ruff; extra == "all"
-Requires-Dist: gradio; extra == "all"
-Requires-Dist: sphinx_rtd_theme; extra == "all"
+Requires-Dist: jiwer; extra == "all"
+Requires-Dist: pre-commit; extra == "all"
+Requires-Dist: pytrec-eval; extra == "all"
+Requires-Dist: sacrebleu; extra == "all"
 Requires-Dist: python-jose[cryptography]==3.3.0; extra == "all"
-Requires-Dist: sentence_transformers; extra == "all"
+Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "all"
 Requires-Dist: nltk; extra == "all"
-Requires-Dist: codespell; extra == "all"
-Requires-Dist: llama-index-core; extra == "all"
-Requires-Dist: rouge_score; extra == "all"
-Requires-Dist: rouge-score; extra == "all"
-Requires-Dist: pytrec-eval; extra == "all"
-Requires-Dist: evaluate; extra == "all"
-Requires-Dist: opendatasets; extra == "all"
 Requires-Dist: ibm-cos-sdk; extra == "all"
-Requires-Dist: mecab-python3; extra == "all"
 Requires-Dist: ipadic; extra == "all"
-Requires-Dist: jiwer; extra == "all"
-Requires-Dist: conllu; extra == "all"
-Requires-Dist: llama-index-llms-openai; extra == "all"
+Requires-Dist: ruff; extra == "all"
+Requires-Dist: SentencePiece; extra == "all"
+Requires-Dist: tomli; extra == "all"
+Requires-Dist: fastapi==0.109.0; extra == "all"
+Requires-Dist: rouge_score; extra == "all"
+Requires-Dist: codespell; extra == "all"
 Requires-Dist: scikit-learn; extra == "all"
-Requires-Dist: pre-commit; extra == "all"
-Requires-Dist: scipy; extra == "all"
-Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "all"
-Requires-Dist: sacrebleu[ko]; extra == "all"
-Requires-Dist: piccolo_theme; extra == "all"
-Requires-Dist: sacrebleu; extra == "all"
-Requires-Dist: editdistance; extra == "all"
-Requires-Dist: httpretty~=1.1.4; extra == "all"
-Requires-Dist: transformers; extra == "all"
+Requires-Dist: opendatasets; extra == "all"
 Requires-Dist: datasets>=2.16.0; extra == "all"
-Requires-Dist: tomli; extra == "all"
-Requires-Dist: torch==1.12.1; extra == "all"
+Requires-Dist: transformers; extra == "all"
 Requires-Dist: absl-py; extra == "all"
+Requires-Dist: llama-index-llms-openai; extra == "all"
+Requires-Dist: editdistance; extra == "all"
+Requires-Dist: httpretty~=1.1.4; extra == "all"
 Requires-Dist: bert_score; extra == "all"
+Requires-Dist: llama-index-core; extra == "all"
+Requires-Dist: scipy; extra == "all"
+Requires-Dist: evaluate; extra == "all"
+Requires-Dist: sacrebleu[ko]; extra == "all"
+Requires-Dist: piccolo_theme; extra == "all"
+Requires-Dist: sentence_transformers; extra == "all"
+Requires-Dist: sphinx_rtd_theme; extra == "all"
+Requires-Dist: rouge-score; extra == "all"
+Requires-Dist: mecab-python3; extra == "all"
 
 <div align="center">
     <img src="./assets/banner.png" alt="Image Description" width="100%" />
 </div>
 
 [![Button](https://img.shields.io/badge/Video-pink?style=for-the-badge)](https://unitxt.readthedocs.io/)
 [![Button](https://img.shields.io/badge/Demo-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/demo.html)
```

### Comparing `unitxt-1.7.6/src/unitxt.egg-info/SOURCES.txt` & `unitxt-1.7.7/src/unitxt.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 src/unitxt/dict_utils.py
 src/unitxt/eval_utils.py
 src/unitxt/file_utils.py
 src/unitxt/formats.py
 src/unitxt/fusion.py
 src/unitxt/generator_utils.py
 src/unitxt/hf_utils.py
+src/unitxt/inference.py
 src/unitxt/instructions.py
+src/unitxt/llm_as_judge.py
 src/unitxt/loaders.py
 src/unitxt/logging_utils.py
 src/unitxt/metric.py
 src/unitxt/metric_utils.py
 src/unitxt/metrics.py
 src/unitxt/normalizers.py
 src/unitxt/operator.py
@@ -400,14 +402,15 @@
 src/unitxt/catalog/cards/mmlu/security_studies.json
 src/unitxt/catalog/cards/mmlu/sociology.json
 src/unitxt/catalog/cards/mmlu/us_foreign_policy.json
 src/unitxt/catalog/cards/mmlu/virology.json
 src/unitxt/catalog/cards/mmlu/world_religions.json
 src/unitxt/catalog/cards/multidoc2dial/abstractive.json
 src/unitxt/catalog/cards/multidoc2dial/extractive.json
+src/unitxt/catalog/cards/rag/model_response_assessment/llm_as_judge_using_mt_bench_template.json
 src/unitxt/catalog/cards/reuters21578/ModApte.json
 src/unitxt/catalog/cards/reuters21578/ModHayes.json
 src/unitxt/catalog/cards/reuters21578/ModLewis.json
 src/unitxt/catalog/cards/universal_ner/ceb/gja.json
 src/unitxt/catalog/cards/universal_ner/da/ddt.json
 src/unitxt/catalog/cards/universal_ner/de/pud.json
 src/unitxt/catalog/cards/universal_ner/en/ewt.json
@@ -555,34 +558,40 @@
 src/unitxt/catalog/metrics/string_containment.json
 src/unitxt/catalog/metrics/token_overlap.json
 src/unitxt/catalog/metrics/token_overlap_with_context.json
 src/unitxt/catalog/metrics/unsorted_list_exact_match.json
 src/unitxt/catalog/metrics/wer.json
 src/unitxt/catalog/metrics/bert_score/deberta_base_mnli.json
 src/unitxt/catalog/metrics/bert_score/deberta_large_mnli.json
+src/unitxt/catalog/metrics/bert_score/deberta_v3_base_mnli_xnli_ml.json
 src/unitxt/catalog/metrics/bert_score/deberta_xlarge_mnli.json
 src/unitxt/catalog/metrics/bert_score/distilbert_base_uncased.json
 src/unitxt/catalog/metrics/perplexity/flan_t5_small.json
 src/unitxt/catalog/metrics/perplexity_a/flan_t5_small.json
 src/unitxt/catalog/metrics/perplexity_chat/flan_t5_small.json
+src/unitxt/catalog/metrics/perplexity_nli/t5_nli_mixture.json
 src/unitxt/catalog/metrics/perplexity_q/flan_t5_small.json
 src/unitxt/catalog/metrics/rag/answer_correctness.json
+src/unitxt/catalog/metrics/rag/answer_inference.json
 src/unitxt/catalog/metrics/rag/answer_reward.json
 src/unitxt/catalog/metrics/rag/bert_k_precision.json
+src/unitxt/catalog/metrics/rag/bert_k_precision_ml.json
 src/unitxt/catalog/metrics/rag/bert_recall.json
+src/unitxt/catalog/metrics/rag/bert_recall_ml.json
 src/unitxt/catalog/metrics/rag/context_correctness.json
 src/unitxt/catalog/metrics/rag/context_perplexity.json
 src/unitxt/catalog/metrics/rag/context_relevance.json
 src/unitxt/catalog/metrics/rag/faithfulness.json
 src/unitxt/catalog/metrics/rag/k_precision.json
 src/unitxt/catalog/metrics/rag/map.json
 src/unitxt/catalog/metrics/rag/mrr.json
 src/unitxt/catalog/metrics/rag/recall.json
 src/unitxt/catalog/metrics/rag/correctness/llama_index_by_gpt_3_5_turbo.json
 src/unitxt/catalog/metrics/rag/correctness/llama_index_by_mock.json
+src/unitxt/catalog/metrics/rag/model_response_assessment/llm_as_judge_by_flan_t5_large_on_hf_pipeline_using_mt_bench_template.json
 src/unitxt/catalog/metrics/reward/deberta_v3_large_v2.json
 src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_accuracy.json
 src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_string_containment.json
 src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_accuracy.json
 src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_string_containment.json
 src/unitxt/catalog/metrics/robustness/fixed_group_mean_accuracy.json
 src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_accuracy.json
@@ -603,14 +612,15 @@
 src/unitxt/catalog/operators/balancers/classification/by_label.json
 src/unitxt/catalog/operators/balancers/multi_label/zero_vs_many_labels.json
 src/unitxt/catalog/operators/balancers/ner/zero_vs_many_entities.json
 src/unitxt/catalog/operators/balancers/qa/by_answer.json
 src/unitxt/catalog/processors/capitalize.json
 src/unitxt/catalog/processors/convert_to_boolean.json
 src/unitxt/catalog/processors/dict_of_lists_to_value_key_pairs.json
+src/unitxt/catalog/processors/extract_mt_bench_judgment.json
 src/unitxt/catalog/processors/first_character.json
 src/unitxt/catalog/processors/get_string_after_colon.json
 src/unitxt/catalog/processors/hate_speech_or_not_hate_speech.json
 src/unitxt/catalog/processors/list_to_empty_entity_tuples.json
 src/unitxt/catalog/processors/load_json.json
 src/unitxt/catalog/processors/load_json_from_predictions.json
 src/unitxt/catalog/processors/lower_case.json
@@ -659,14 +669,15 @@
 src/unitxt/catalog/tasks/qa/open.json
 src/unitxt/catalog/tasks/qa/multiple_choice/open.json
 src/unitxt/catalog/tasks/qa/multiple_choice/with_context.json
 src/unitxt/catalog/tasks/qa/multiple_choice/with_topic.json
 src/unitxt/catalog/tasks/qa/multiple_choice/with_context/with_topic.json
 src/unitxt/catalog/tasks/qa/with_context/abstractive.json
 src/unitxt/catalog/tasks/qa/with_context/extractive.json
+src/unitxt/catalog/tasks/rag/model_response_assessment.json
 src/unitxt/catalog/tasks/regression/single_text.json
 src/unitxt/catalog/tasks/regression/two_texts.json
 src/unitxt/catalog/tasks/rewriting/by_attribute.json
 src/unitxt/catalog/tasks/rewriting/paraphrase.json
 src/unitxt/catalog/tasks/selection/by_attribute.json
 src/unitxt/catalog/tasks/span_labeling/extraction.json
 src/unitxt/catalog/tasks/summarization/abstractive.json
@@ -830,14 +841,15 @@
 src/unitxt/catalog/templates/qa/with_context/all.json
 src/unitxt/catalog/templates/qa/with_context/ffqa.json
 src/unitxt/catalog/templates/qa/with_context/question_first.json
 src/unitxt/catalog/templates/qa/with_context/simple.json
 src/unitxt/catalog/templates/qa/with_context/simple2.json
 src/unitxt/catalog/templates/qa/with_context/title.json
 src/unitxt/catalog/templates/qa/with_context/with_type.json
+src/unitxt/catalog/templates/rag/model_response_assessment/llm_as_judge_using_mt_bench_template.json
 src/unitxt/catalog/templates/regression/single_text/all.json
 src/unitxt/catalog/templates/regression/single_text/simple.json
 src/unitxt/catalog/templates/regression/single_text/title.json
 src/unitxt/catalog/templates/regression/two_texts/all.json
 src/unitxt/catalog/templates/regression/two_texts/simple.json
 src/unitxt/catalog/templates/regression/two_texts/title.json
 src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json
```

### Comparing `unitxt-1.7.6/src/unitxt.egg-info/requires.txt` & `unitxt-1.7.7/src/unitxt.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 datasets>=2.16.0
 evaluate
 absl-py
 ipadic
 scipy
 
 [all]
-fastapi==0.109.0
+gradio
 sphinxext-opengraph
+conllu
+torch==1.12.1
 datasets
-ruff
-gradio
-sphinx_rtd_theme
+jiwer
+pre-commit
+pytrec-eval
+sacrebleu
 python-jose[cryptography]==3.3.0
-sentence_transformers
+uvicorn[standard]==0.27.0.post1
 nltk
-codespell
-llama-index-core
-rouge_score
-rouge-score
-pytrec-eval
-evaluate
-opendatasets
 ibm-cos-sdk
-mecab-python3
 ipadic
-jiwer
-conllu
-llama-index-llms-openai
+ruff
+SentencePiece
+tomli
+fastapi==0.109.0
+rouge_score
+codespell
 scikit-learn
-pre-commit
-scipy
-uvicorn[standard]==0.27.0.post1
-sacrebleu[ko]
-piccolo_theme
-sacrebleu
-editdistance
-httpretty~=1.1.4
-transformers
+opendatasets
 datasets>=2.16.0
-tomli
-torch==1.12.1
+transformers
 absl-py
+llama-index-llms-openai
+editdistance
+httpretty~=1.1.4
 bert_score
+llama-index-core
+scipy
+evaluate
+sacrebleu[ko]
+piccolo_theme
+sentence_transformers
+sphinx_rtd_theme
+mecab-python3
 
 [base]
 datasets>=2.16.0
 evaluate
 absl-py
 ipadic
 scipy
@@ -66,14 +66,16 @@
 sacrebleu
 absl-py
 rouge_score
 scikit-learn
 jiwer
 editdistance
 
+[helm]
+
 [service]
 torch==1.12.1
 fastapi==0.109.0
 uvicorn[standard]==0.27.0.post1
 python-jose[cryptography]==3.3.0
 transformers
 
@@ -91,11 +93,12 @@
 sacrebleu[ko]
 scikit-learn
 jiwer
 conllu
 llama-index-core
 llama-index-llms-openai
 pytrec-eval
+SentencePiece
 
 [ui]
 gradio
 transformers
```

