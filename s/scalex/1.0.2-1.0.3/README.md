# Comparing `tmp/scalex-1.0.2.tar.gz` & `tmp/scalex-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalex-1.0.2.tar", last modified: Tue Oct 25 14:43:24 2022, max compression
+gzip compressed data, was "scalex-1.0.3.tar", last modified: Tue Apr 16 23:10:20 2024, max compression
```

## Comparing `scalex-1.0.2.tar` & `scalex-1.0.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 leixiong   (501) staff       (20)        0 2022-10-25 14:43:24.627290 scalex-1.0.2/
--rw-r--r--   0 leixiong   (501) staff       (20)      121 2022-10-18 13:45:02.000000 scalex-1.0.2/.gitignore
--rw-r--r--   0 leixiong   (501) staff       (20)     1073 2022-10-18 13:45:02.000000 scalex-1.0.2/LICENSE.txt
--rw-r--r--   0 leixiong   (501) staff       (20)     6972 2022-10-25 14:43:24.627139 scalex-1.0.2/PKG-INFO
--rw-r--r--   0 leixiong   (501) staff       (20)     6217 2022-10-19 17:13:37.000000 scalex-1.0.2/README.md
--rwxr-xr-x   0 leixiong   (501) staff       (20)     3214 2022-10-25 14:37:34.000000 scalex-1.0.2/SCALEX.py
-drwxr-xr-x   0 leixiong   (501) staff       (20)        0 2022-10-25 14:43:24.616827 scalex-1.0.2/docs/
--rw-r--r--   0 leixiong   (501) staff       (20)      638 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/Makefile
--rw-r--r--   0 leixiong   (501) staff       (20)      799 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/make.bat
-drwxr-xr-x   0 leixiong   (501) staff       (20)        0 2022-10-25 14:43:24.617468 scalex-1.0.2/docs/source/
-drwxr-xr-x   0 leixiong   (501) staff       (20)        0 2022-10-25 14:43:24.617564 scalex-1.0.2/docs/source/_static/
--rw-r--r--   0 leixiong   (501) staff       (20)     6148 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/_static/.DS_Store
-drwxr-xr-x   0 leixiong   (501) staff       (20)        0 2022-10-25 14:43:24.619314 scalex-1.0.2/docs/source/_static/img/
--rw-r--r--   0 leixiong   (501) staff       (20)     6148 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/_static/img/.DS_Store
--rw-r--r--   0 leixiong   (501) staff       (20)    63250 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/_static/img/cross-modality_integration.png
--rw-r--r--   0 leixiong   (501) staff       (20)     2994 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/_static/img/logo_white.png
--rw-r--r--   0 leixiong   (501) staff       (20)   264528 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/_static/img/mouse_atlas_reference.png
--rw-r--r--   0 leixiong   (501) staff       (20)   249863 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/_static/img/pancreas_projection.png
--rw-r--r--   0 leixiong   (501) staff       (20)    49732 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/_static/img/pbmc_before_integration.png
--rw-r--r--   0 leixiong   (501) staff       (20)    80122 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/_static/img/pbmc_integration.png
--rw-r--r--   0 leixiong   (501) staff       (20)    60360 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/_static/img/query_kidney.png
--rw-r--r--   0 leixiong   (501) staff       (20)    54065 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/_static/img/query_tabula_muris_aging.png
--rw-r--r--   0 leixiong   (501) staff       (20)   103354 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/_static/img/scATAC_integration.png
--rw-r--r--   0 leixiong   (501) staff       (20)   379113 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/_static/img/scalex.jpg
-drwxr-xr-x   0 leixiong   (501) staff       (20)        0 2022-10-25 14:43:24.619624 scalex-1.0.2/docs/source/api/
--rw-r--r--   0 leixiong   (501) staff       (20)     1889 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/api/index.rst
--rw-r--r--   0 leixiong   (501) staff       (20)     3190 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/conf.py
--rw-r--r--   0 leixiong   (501) staff       (20)      192 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/contributors.rst
--rw-r--r--   0 leixiong   (501) staff       (20)     1236 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/index.rst
--rw-r--r--   0 leixiong   (501) staff       (20)     1054 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/installation.rst
--rw-r--r--   0 leixiong   (501) staff       (20)      264 2022-10-19 20:38:22.000000 scalex-1.0.2/docs/source/news.rst
-drwxr-xr-x   0 leixiong   (501) staff       (20)        0 2022-10-25 14:43:24.619819 scalex-1.0.2/docs/source/release/
--rw-r--r--   0 leixiong   (501) staff       (20)      167 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/release/1.0.0.rst
--rw-r--r--   0 leixiong   (501) staff       (20)       66 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/release/index.rst
-drwxr-xr-x   0 leixiong   (501) staff       (20)        0 2022-10-25 14:43:24.621795 scalex-1.0.2/docs/source/tutorial/
--rw-r--r--   0 leixiong   (501) staff       (20)   170454 2022-10-18 14:23:26.000000 scalex-1.0.2/docs/source/tutorial/Integration_PBMC.ipynb
--rw-r--r--   0 leixiong   (501) staff       (20)   435407 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/tutorial/Integration_cross-modality.ipynb
--rw-r--r--   0 leixiong   (501) staff       (20)   358829 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/tutorial/Integration_scATAC-seq.ipynb
--rw-r--r--   0 leixiong   (501) staff       (20)  1415270 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/tutorial/Projection_pancreas.ipynb
--rw-r--r--   0 leixiong   (501) staff       (20)     1856 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/tutorial/index.rst
--rw-r--r--   0 leixiong   (501) staff       (20)     3712 2022-10-18 13:45:02.000000 scalex-1.0.2/docs/source/usage.rst
-drwxr-xr-x   0 leixiong   (501) staff       (20)        0 2022-10-25 14:43:24.622676 scalex-1.0.2/experiments/
--rwxr-xr-x   0 leixiong   (501) staff       (20)     3342 2022-10-18 13:45:02.000000 scalex-1.0.2/experiments/LISI.ipynb
--rwxr-xr-x   0 leixiong   (501) staff       (20)   245692 2022-10-18 13:45:02.000000 scalex-1.0.2/experiments/NMI-ARI.ipynb
--rwxr-xr-x   0 leixiong   (501) staff       (20)    47829 2022-10-18 13:45:02.000000 scalex-1.0.2/experiments/Silhouette_score & batch_entropy_mixing_score.ipynb
--rwxr-xr-x   0 leixiong   (501) staff       (20)     9228 2022-10-18 13:45:02.000000 scalex-1.0.2/experiments/dirichlet_regression.ipynb
--rwxr-xr-x   0 leixiong   (501) staff       (20)    30433 2022-10-18 13:45:02.000000 scalex-1.0.2/experiments/overcorrection_score.ipynb
--rwxr-xr-x   0 leixiong   (501) staff       (20)  1084713 2022-10-18 13:45:02.000000 scalex-1.0.2/experiments/projection.ipynb
--rw-r--r--   0 leixiong   (501) staff       (20)      187 2022-10-18 13:45:02.000000 scalex-1.0.2/requirements.txt
-drwxr-xr-x   0 leixiong   (501) staff       (20)        0 2022-10-25 14:43:24.624132 scalex-1.0.2/scalex/
--rw-r--r--   0 leixiong   (501) staff       (20)      220 2022-10-25 14:42:37.000000 scalex-1.0.2/scalex/__init__.py
--rwxr-xr-x   0 leixiong   (501) staff       (20)    19141 2022-10-19 17:26:00.000000 scalex-1.0.2/scalex/data.py
--rwxr-xr-x   0 leixiong   (501) staff       (20)     9650 2022-10-25 14:34:58.000000 scalex-1.0.2/scalex/function.py
--rwxr-xr-x   0 leixiong   (501) staff       (20)      839 2022-10-19 15:59:06.000000 scalex-1.0.2/scalex/logger.py
--rwxr-xr-x   0 leixiong   (501) staff       (20)     2789 2022-10-18 13:45:02.000000 scalex-1.0.2/scalex/metrics.py
-drwxr-xr-x   0 leixiong   (501) staff       (20)        0 2022-10-25 14:43:24.625143 scalex-1.0.2/scalex/net/
--rw-r--r--   0 leixiong   (501) staff       (20)        0 2022-10-18 13:45:02.000000 scalex-1.0.2/scalex/net/__init__.py
--rwxr-xr-x   0 leixiong   (501) staff       (20)     5616 2022-10-18 13:45:02.000000 scalex-1.0.2/scalex/net/layer.py
--rwxr-xr-x   0 leixiong   (501) staff       (20)      514 2022-10-18 13:45:02.000000 scalex-1.0.2/scalex/net/loss.py
--rwxr-xr-x   0 leixiong   (501) staff       (20)     2324 2022-10-19 16:19:07.000000 scalex-1.0.2/scalex/net/utils.py
--rwxr-xr-x   0 leixiong   (501) staff       (20)     6650 2022-10-25 14:08:42.000000 scalex-1.0.2/scalex/net/vae.py
--rwxr-xr-x   0 leixiong   (501) staff       (20)    11068 2022-10-18 13:45:02.000000 scalex-1.0.2/scalex/plot.py
-drwxr-xr-x   0 leixiong   (501) staff       (20)        0 2022-10-25 14:43:24.624655 scalex-1.0.2/scalex.egg-info/
--rw-r--r--   0 leixiong   (501) staff       (20)     6972 2022-10-25 14:43:24.000000 scalex-1.0.2/scalex.egg-info/PKG-INFO
--rw-r--r--   0 leixiong   (501) staff       (20)     1913 2022-10-25 14:43:24.000000 scalex-1.0.2/scalex.egg-info/SOURCES.txt
--rw-r--r--   0 leixiong   (501) staff       (20)        1 2022-10-25 14:43:24.000000 scalex-1.0.2/scalex.egg-info/dependency_links.txt
--rw-r--r--   0 leixiong   (501) staff       (20)      187 2022-10-25 14:43:24.000000 scalex-1.0.2/scalex.egg-info/requires.txt
--rw-r--r--   0 leixiong   (501) staff       (20)        7 2022-10-25 14:43:24.000000 scalex-1.0.2/scalex.egg-info/top_level.txt
--rw-r--r--   0 leixiong   (501) staff       (20)       38 2022-10-25 14:43:24.627329 scalex-1.0.2/setup.cfg
--rwxr-xr-x   0 leixiong   (501) staff       (20)     1782 2022-10-18 13:45:02.000000 scalex-1.0.2/setup.py
-drwxr-xr-x   0 leixiong   (501) staff       (20)        0 2022-10-25 14:43:24.626902 scalex-1.0.2/third_parties/
--rwxr-xr-x   0 leixiong   (501) staff       (20)     2062 2022-10-18 13:45:02.000000 scalex-1.0.2/third_parties/BBKNN.py
--rwxr-xr-x   0 leixiong   (501) staff       (20)     3033 2022-10-18 13:45:02.000000 scalex-1.0.2/third_parties/Conos.R
--rwxr-xr-x   0 leixiong   (501) staff       (20)     2654 2022-10-18 13:45:02.000000 scalex-1.0.2/third_parties/DESC.py
--rwxr-xr-x   0 leixiong   (501) staff       (20)     2546 2022-10-18 13:45:02.000000 scalex-1.0.2/third_parties/FastMNN.R
--rwxr-xr-x   0 leixiong   (501) staff       (20)     2704 2022-10-18 13:45:02.000000 scalex-1.0.2/third_parties/Harmony.R
--rwxr-xr-x   0 leixiong   (501) staff       (20)     2792 2022-10-18 13:45:02.000000 scalex-1.0.2/third_parties/LIGER.R
--rwxr-xr-x   0 leixiong   (501) staff       (20)     2023 2022-10-18 13:45:02.000000 scalex-1.0.2/third_parties/Raw.py
--rwxr-xr-x   0 leixiong   (501) staff       (20)     2253 2022-10-18 13:45:02.000000 scalex-1.0.2/third_parties/Scanorama.py
--rwxr-xr-x   0 leixiong   (501) staff       (20)     3786 2022-10-18 13:45:02.000000 scalex-1.0.2/third_parties/Seurat_v3.R
--rwxr-xr-x   0 leixiong   (501) staff       (20)     2915 2022-10-18 13:45:02.000000 scalex-1.0.2/third_parties/online_iNMF.R
--rwxr-xr-x   0 leixiong   (501) staff       (20)     2738 2022-10-18 13:45:02.000000 scalex-1.0.2/third_parties/scVI.py
+drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.738808 scalex-1.0.3/
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)      121 2024-04-16 21:24:31.000000 scalex-1.0.3/.gitignore
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)     1073 2024-04-16 21:24:31.000000 scalex-1.0.3/LICENSE.txt
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)     7320 2024-04-16 23:10:20.736808 scalex-1.0.3/PKG-INFO
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)     6217 2024-04-16 22:10:50.000000 scalex-1.0.3/README.md
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     3779 2024-04-16 22:01:37.000000 scalex-1.0.3/SCALEX.py
+drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.505806 scalex-1.0.3/docs/
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)      638 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/Makefile
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)      799 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/make.bat
+drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.518806 scalex-1.0.3/docs/source/
+drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.520806 scalex-1.0.3/docs/source/_static/
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)     6148 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/.DS_Store
+drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.554807 scalex-1.0.3/docs/source/_static/img/
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)     6148 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/.DS_Store
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)    63250 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/cross-modality_integration.png
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)     2994 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/logo_white.png
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)   264528 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/mouse_atlas_reference.png
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)   249863 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/pancreas_projection.png
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)    49732 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/pbmc_before_integration.png
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)    80122 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/pbmc_integration.png
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)    60360 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/query_kidney.png
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)    54065 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/query_tabula_muris_aging.png
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)   103354 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/scATAC_integration.png
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)   379113 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/scalex.jpg
+drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.560807 scalex-1.0.3/docs/source/api/
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)     1889 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/api/index.rst
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)     3190 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/conf.py
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)      192 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/contributors.rst
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)     1236 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/index.rst
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)     1054 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/installation.rst
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)      267 2024-04-16 22:11:29.000000 scalex-1.0.3/docs/source/news.rst
+drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.565807 scalex-1.0.3/docs/source/release/
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)      167 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/release/1.0.0.rst
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)       66 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/release/index.rst
+drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.599807 scalex-1.0.3/docs/source/tutorial/
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)   170454 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/tutorial/Integration_PBMC.ipynb
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)   435407 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/tutorial/Integration_cross-modality.ipynb
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)   358829 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/tutorial/Integration_scATAC-seq.ipynb
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)  1415270 2024-04-16 21:24:32.000000 scalex-1.0.3/docs/source/tutorial/Projection_pancreas.ipynb
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)     1856 2024-04-16 21:24:32.000000 scalex-1.0.3/docs/source/tutorial/index.rst
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)     3712 2024-04-16 21:24:32.000000 scalex-1.0.3/docs/source/usage.rst
+drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.615807 scalex-1.0.3/experiments/
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     3342 2024-04-16 21:24:32.000000 scalex-1.0.3/experiments/LISI.ipynb
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)   245692 2024-04-16 21:24:32.000000 scalex-1.0.3/experiments/NMI-ARI.ipynb
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)    47829 2024-04-16 21:24:32.000000 scalex-1.0.3/experiments/Silhouette_score & batch_entropy_mixing_score.ipynb
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     9228 2024-04-16 21:24:32.000000 scalex-1.0.3/experiments/dirichlet_regression.ipynb
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)    30433 2024-04-16 21:24:32.000000 scalex-1.0.3/experiments/overcorrection_score.ipynb
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)  1084713 2024-04-16 21:24:32.000000 scalex-1.0.3/experiments/projection.ipynb
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)      188 2024-04-16 22:25:18.000000 scalex-1.0.3/requirements.txt
+drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.688808 scalex-1.0.3/scalex/
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)      220 2024-04-16 22:35:39.000000 scalex-1.0.3/scalex/__init__.py
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)    21827 2024-04-16 22:27:20.000000 scalex-1.0.3/scalex/data.py
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)    10508 2024-04-16 23:05:40.000000 scalex-1.0.3/scalex/function.py
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)      839 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/logger.py
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2789 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/metrics.py
+drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.709808 scalex-1.0.3/scalex/net/
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/net/__init__.py
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     5616 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/net/layer.py
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)      514 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/net/loss.py
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2324 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/net/utils.py
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     7093 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/net/vae.py
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)    11068 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/plot.py
+drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.734808 scalex-1.0.3/scalex.egg-info/
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)     7320 2024-04-16 23:10:19.000000 scalex-1.0.3/scalex.egg-info/PKG-INFO
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)     1913 2024-04-16 23:10:19.000000 scalex-1.0.3/scalex.egg-info/SOURCES.txt
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)        1 2024-04-16 23:10:19.000000 scalex-1.0.3/scalex.egg-info/dependency_links.txt
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)      188 2024-04-16 23:10:19.000000 scalex-1.0.3/scalex.egg-info/requires.txt
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)        7 2024-04-16 23:10:19.000000 scalex-1.0.3/scalex.egg-info/top_level.txt
+-rw-r--r--   0 leixiong  (1316) kundaje  (65541)       38 2024-04-16 23:10:20.738808 scalex-1.0.3/setup.cfg
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     1782 2024-04-16 21:24:32.000000 scalex-1.0.3/setup.py
+drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.732808 scalex-1.0.3/third_parties/
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2062 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/BBKNN.py
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     3033 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/Conos.R
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2654 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/DESC.py
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2546 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/FastMNN.R
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2704 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/Harmony.R
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2792 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/LIGER.R
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2023 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/Raw.py
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2253 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/Scanorama.py
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     3786 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/Seurat_v3.R
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2915 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/online_iNMF.R
+-rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2738 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/scVI.py
```

### Comparing `scalex-1.0.2/LICENSE.txt` & `scalex-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/PKG-INFO` & `scalex-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: scalex
-Version: 1.0.2
-Summary: Online single-cell data integration through projecting heterogeneous datasets into a common cell-embedding space
-Home-page: https://github.com/jsxlei/scalex
-Author: Lei Xiong
-Author-email: jsxlei@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >3.6.0
-License-File: LICENSE.txt
-
 [![Stars](https://img.shields.io/github/stars/jsxlei/scalex?logo=GitHub&color=yellow)](https://github.com/jsxlei/scalex/stargazers)
 [![PyPI](https://img.shields.io/pypi/v/scalex.svg)](https://pypi.org/project/scalex)
 [![Documentation Status](https://readthedocs.org/projects/scalex/badge/?version=latest)](https://scalex.readthedocs.io/en/latest/?badge=stable)
 [![Downloads](https://pepy.tech/badge/scalex)](https://pepy.tech/project/scalex)
 [![DOI](https://zenodo.org/badge/345941713.svg)](https://zenodo.org/badge/latestdoi/345941713)
 # [Online single-cell data integration through projecting heterogeneous datasets into a common cell-embedding space](https://www.nature.com/articles/s41467-022-33758-z)
 
@@ -172,9 +152,7 @@
     
     
 
     
     
 
 
-
-
```

### Comparing `scalex-1.0.2/SCALEX.py` & `scalex-1.0.3/SCALEX.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     parser.add_argument('--test_list', '-t', type=str, nargs='+', default=[])
     
     parser.add_argument('--min_features', type=int, default=None)
     parser.add_argument('--min_cells', type=int, default=3)
     parser.add_argument('--n_top_features', default=None)
     parser.add_argument('--target_sum', type=int, default=None)
     parser.add_argument('--processed', action='store_true', default=False)
+    parser.add_argument('--fraction', type=float, default=None)
+    parser.add_argument('--n_obs', type=int, default=None)
+    parser.add_argument('--use_layer', type=str, default='X')
+    parser.add_argument('--backed', action='store_true', default=False)
 
     parser.add_argument('--projection', '-p', default=None)
     parser.add_argument('--impute', type=str, default=None)
     parser.add_argument('--outdir', '-o', type=str, default='output/')
     
     parser.add_argument('--lr', type=float, default=2e-4)
     parser.add_argument('--batch_size', type=int, default=64)
@@ -38,14 +42,16 @@
     parser.add_argument('--max_iteration', type=int, default=30000)
     parser.add_argument('--seed', type=int, default=124)
     parser.add_argument('--chunk_size', type=int, default=20000)
     parser.add_argument('--ignore_umap', action='store_true')
     parser.add_argument('--repeat', action='store_true')
     parser.add_argument('--assess', action='store_true')
     parser.add_argument('--eval', action='store_true')
+    parser.add_argument('--num_workers', type=int, default=4)
+    parser.add_argument('--keep_mt', action='store_true')
     # parser.add_argument('--version', type=int, default=2)
     # parser.add_argument('--k', type=str, default=30)
     # parser.add_argument('--embed', type=str, default='UMAP')
 #     parser.add_argument('--beta', type=float, default=0.5)
 #     parser.add_argument('--hid_dim', type=int, default=1024)
 
 
@@ -58,15 +64,20 @@
         profile=args.profile,
         join=args.join, 
         batch_key=args.batch_key, 
         min_features=args.min_features, 
         min_cells=args.min_cells, 
         target_sum=args.target_sum,
         n_top_features=args.n_top_features, 
+        fraction=args.fraction,
+        n_obs=args.n_obs,
         processed=args.processed,
+        keep_mt=args.keep_mt,
+        use_layer=args.use_layer,
+        backed=args.backed,
         batch_size=args.batch_size, 
         lr=args.lr, 
         max_iteration=args.max_iteration, 
         impute=args.impute,
         batch_name=args.batch_name, 
         seed=args.seed, 
         gpu=args.gpu, 
@@ -74,10 +85,11 @@
         projection=args.projection, 
         chunk_size=args.chunk_size,
         ignore_umap=args.ignore_umap,
         repeat=args.repeat,
         verbose=True,
         assess=args.assess,
         eval=args.eval,
+        num_workers=args.num_workers,
         show=False,
     )
```

### Comparing `scalex-1.0.2/docs/Makefile` & `scalex-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/make.bat` & `scalex-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/_static/.DS_Store` & `scalex-1.0.3/docs/source/_static/.DS_Store`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/_static/img/.DS_Store` & `scalex-1.0.3/docs/source/_static/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/_static/img/cross-modality_integration.png` & `scalex-1.0.3/docs/source/_static/img/cross-modality_integration.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/_static/img/logo_white.png` & `scalex-1.0.3/docs/source/_static/img/logo_white.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/_static/img/mouse_atlas_reference.png` & `scalex-1.0.3/docs/source/_static/img/mouse_atlas_reference.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/_static/img/pancreas_projection.png` & `scalex-1.0.3/docs/source/_static/img/pancreas_projection.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/_static/img/pbmc_before_integration.png` & `scalex-1.0.3/docs/source/_static/img/pbmc_before_integration.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/_static/img/pbmc_integration.png` & `scalex-1.0.3/docs/source/_static/img/pbmc_integration.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/_static/img/query_kidney.png` & `scalex-1.0.3/docs/source/_static/img/query_kidney.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/_static/img/query_tabula_muris_aging.png` & `scalex-1.0.3/docs/source/_static/img/query_tabula_muris_aging.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/_static/img/scATAC_integration.png` & `scalex-1.0.3/docs/source/_static/img/scATAC_integration.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/_static/img/scalex.jpg` & `scalex-1.0.3/docs/source/_static/img/scalex.jpg`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/api/index.rst` & `scalex-1.0.3/docs/source/api/index.rst`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/conf.py` & `scalex-1.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/index.rst` & `scalex-1.0.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/installation.rst` & `scalex-1.0.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/tutorial/Integration_PBMC.ipynb` & `scalex-1.0.3/docs/source/tutorial/Integration_PBMC.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/tutorial/Integration_cross-modality.ipynb` & `scalex-1.0.3/docs/source/tutorial/Integration_cross-modality.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/tutorial/Integration_scATAC-seq.ipynb` & `scalex-1.0.3/docs/source/tutorial/Integration_scATAC-seq.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/tutorial/Projection_pancreas.ipynb` & `scalex-1.0.3/docs/source/tutorial/Projection_pancreas.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/tutorial/index.rst` & `scalex-1.0.3/docs/source/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/docs/source/usage.rst` & `scalex-1.0.3/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/experiments/LISI.ipynb` & `scalex-1.0.3/experiments/LISI.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/experiments/NMI-ARI.ipynb` & `scalex-1.0.3/experiments/NMI-ARI.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/experiments/Silhouette_score & batch_entropy_mixing_score.ipynb` & `scalex-1.0.3/experiments/Silhouette_score & batch_entropy_mixing_score.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/experiments/dirichlet_regression.ipynb` & `scalex-1.0.3/experiments/dirichlet_regression.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/experiments/overcorrection_score.ipynb` & `scalex-1.0.3/experiments/overcorrection_score.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/experiments/projection.ipynb` & `scalex-1.0.3/experiments/projection.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/scalex/data.py` & `scalex-1.0.3/scalex/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 from anndata import AnnData
 import scanpy as sc
 from sklearn.preprocessing import maxabs_scale, MaxAbsScaler
 
 from glob import glob
 
-np.warnings.filterwarnings('ignore')
 DATA_PATH = os.path.expanduser("~")+'/.scalex/'
 CHUNK_SIZE = 20000
 
 
 def read_mtx(path):
     """\
     Read mtx format data folder including: 
@@ -57,46 +56,60 @@
             adata.var = pd.DataFrame(index=gene)
         elif 'feature' in filename:
             gene = pd.read_csv(filename, sep='\t', header=None).iloc[:, 1].values
             adata.var = pd.DataFrame(index=gene)
     return adata
 
 
-def load_file(path):  
+def load_file(path, backed=False):  
     """
     Load single cell dataset from file
     
     Parameters
     ----------
     path
         the path store the file
         
     Return
     ------
     AnnData
     """
     if os.path.exists(DATA_PATH+path+'.h5ad'):
-        adata = sc.read_h5ad(DATA_PATH+path+'.h5ad')
+        adata = sc.read_h5ad(DATA_PATH+path+'.h5ad', backed=backed)
     elif os.path.isdir(path): # mtx format
         adata = read_mtx(path)
     elif os.path.isfile(path):
         if path.endswith(('.csv', '.csv.gz')):
             adata = sc.read_csv(path).T
         elif path.endswith(('.txt', '.txt.gz', '.tsv', '.tsv.gz')):
             df = pd.read_csv(path, sep='\t', index_col=0).T
             adata = AnnData(df.values, dict(obs_names=df.index.values), dict(var_names=df.columns.values))
         elif path.endswith('.h5ad'):
             adata = sc.read_h5ad(path)
+        # elif path.endswith('.h5mu'):
+        #     import muon as mu
+
+        #     mdata = mu.read(path)
+        #     rna = mdata.mod['rna']
+        #     atac = mdata.mod['atac']
+            
+            # gene_activity = gene_score(atac, rna_var=None, gene_region='combined')
+            
+            # rna.var_names_make_unique()
+            # gene_activity.var_names_make_unique()
+
+            # return AnnData.concatenate(rna, gene_activity, join='inner', batch_key='batch',
+            #                         batch_categories=['RNA', 'ATAC'], index_unique=None) 
     elif path.endswith(tuple(['.h5mu/rna', '.h5mu/atac'])):
         import muon as mu
-        adata = mu.read(path)
+        adata = mu.read(path, backed=backed) 
     else:
         raise ValueError("File {} not exists".format(path))
         
-    if not issparse(adata.X):
+    if not issparse(adata.X) and not backed:
         adata.X = scipy.sparse.csr_matrix(adata.X)
     adata.var_names_make_unique()
     return adata
 
 
 def load_files(root):
     """
@@ -180,23 +193,25 @@
 def preprocessing_rna(
         adata: AnnData, 
         min_features: int = 600, 
         min_cells: int = 3, 
         target_sum: int = 10000, 
         n_top_features = 2000, # or gene list
         chunk_size: int = CHUNK_SIZE,
+        keep_mt: bool = False,
+        backed: bool = False,
         log=None
     ):
     """
     Preprocessing single-cell RNA-seq data
     
     Parameters
     ----------
     adata
-        An AnnData matrice of shape n_obs × n_vars. Rows correspond to cells and columns to genes.
+        An AnnData matrice of shape n_obs x n_vars. Rows correspond to cells and columns to genes.
     min_features
         Filtered out cells that are detected in less than n genes. Default: 600.
     min_cells
         Filtered out genes that are detected in less than n cells. Default: 3.
     target_sum
         After normalization, each cell has a total count equal to target_sum. If None, total count of each cell equal to the median of total counts for cells before normalization.
     n_top_features
@@ -212,19 +227,21 @@
     """
     if min_features is None: min_features = 600
     if n_top_features is None: n_top_features = 2000
     if target_sum is None: target_sum = 10000
     
     if log: log.info('Preprocessing')
     # if not issparse(adata.X):
-    if type(adata.X) != csr.csr_matrix:
+    if type(adata.X) != csr.csr_matrix and (not backed) and (not adata.isbacked):
         adata.X = scipy.sparse.csr_matrix(adata.X)
     
-    adata = adata[:, [gene for gene in adata.var_names 
-                  if not str(gene).startswith(tuple(['ERCC', 'MT-', 'mt-']))]]
+    if not keep_mt:
+        if log: log.info('Filtering out MT genes')
+        adata = adata[:, [gene for gene in adata.var_names 
+                    if not str(gene).startswith(tuple(['ERCC', 'MT-', 'mt-']))]]
     
     if log: log.info('Filtering cells')
     sc.pp.filter_cells(adata, min_genes=min_features)
     
     if log: log.info('Filtering features')
     sc.pp.filter_genes(adata, min_cells=min_cells)
 
@@ -233,40 +250,43 @@
     
     if log: log.info('Log1p transforming')
     sc.pp.log1p(adata)
     
     adata.raw = adata
     if log: log.info('Finding variable features')
     if type(n_top_features) == int and n_top_features>0:
-        sc.pp.highly_variable_genes(adata, n_top_genes=n_top_features, batch_key='batch', inplace=False, subset=True)
+        sc.pp.highly_variable_genes(adata, n_top_genes=n_top_features, batch_key='batch') #, inplace=False, subset=True)
+        adata = adata[:, adata.var.highly_variable].copy()
     elif type(n_top_features) != int:
         adata = reindex(adata, n_top_features)
         
     if log: log.info('Batch specific maxabs scaling')
-    adata = batch_scale(adata, chunk_size=chunk_size)
+    # adata = batch_scale(adata, chunk_size=chunk_size)
+    adata.X = MaxAbsScaler().fit_transform(adata.X)
     if log: log.info('Processed dataset shape: {}'.format(adata.shape))
     return adata
 
 
 def preprocessing_atac(
         adata: AnnData, 
         min_features: int = 100, 
         min_cells: int = 3, 
         target_sum=None, 
         n_top_features = 100000, # or gene list
         chunk_size: int = CHUNK_SIZE,
+        backed: bool = False,
         log=None
     ):
     """
     Preprocessing single-cell ATAC-seq
     
     Parameters
     ----------
     adata
-        An AnnData matrice of shape n_obs × n_vars. Rows correspond to cells and columns to genes.
+        An AnnData matrice of shape n_obs x n_vars. Rows correspond to cells and columns to genes.
     min_features
         Filtered out cells that are detected in less than n genes. Default: 100.
     min_cells
         Filtered out genes that are detected in less than n cells. Default: 3.
     target_sum
         After normalization, each cell has a total count equal to target_sum. If None, total count of each cell equal to the median of total counts for cells before normalization. Default: None.
     n_top_features
@@ -283,63 +303,67 @@
     import episcanpy as epi
     
     if min_features is None: min_features = 100
     if n_top_features is None: n_top_features = 100000
     if target_sum is None: target_sum = 10000
     
     if log: log.info('Preprocessing')
-    # if not issparse(adata.X):
     if type(adata.X) != csr.csr_matrix:
         adata.X = scipy.sparse.csr_matrix(adata.X)
     
-    adata.X[adata.X>1] = 1
+    # adata.X[adata.X>1] = 1
+    sc.pp.normalize_total(adata, target_sum=target_sum)
+    sc.pp.log1p(adata)
     
     if log: log.info('Filtering cells')
     sc.pp.filter_cells(adata, min_genes=min_features)
     
     if log: log.info('Filtering features')
     sc.pp.filter_genes(adata, min_cells=min_cells)
     
 #     adata.raw = adata
     if log: log.info('Finding variable features')
-    if type(n_top_features) == int and n_top_features>0:
-        sc.pp.highly_variable_genes(adata, n_top_genes=n_top_features, batch_key='batch', inplace=False, subset=True)
-        # epi.pp.select_var_feature(adata, nb_features=n_top_features, show=False, copy=False)
+    if type(n_top_features) == int and n_top_features>0 and n_top_features < adata.shape[1]:
+        # sc.pp.highly_variable_genes(adata, n_top_genes=n_top_features, batch_key='batch', inplace=False, subset=True)
+        epi.pp.select_var_feature(adata, nb_features=n_top_features, show=False, copy=False)
     elif type(n_top_features) != int:
         adata = reindex(adata, n_top_features)
 
     
     # if log: log.info('Normalizing total per cell')
     # if target_sum != -1:
-        # sc.pp.normalize_total(adata, target_sum=target_sum)
+    
 
         
     if log: log.info('Batch specific maxabs scaling')
-    adata = batch_scale(adata, chunk_size=chunk_size)
+    # adata = batch_scale(adata, chunk_size=chunk_size)
+    adata.X = MaxAbsScaler().fit_transform(adata.X)
     if log: log.info('Processed dataset shape: {}'.format(adata.shape))
     return adata
 
 
 def preprocessing(
         adata: AnnData, 
         profile: str='RNA',
         min_features: int = 600, 
         min_cells: int = 3, 
         target_sum: int = None, 
         n_top_features = None, # or gene list
+        keep_mt: bool = False,
+        backed: bool = False,
         chunk_size: int = CHUNK_SIZE,
         log=None
     ):
     """
     Preprocessing single-cell data
     
     Parameters
     ----------
     adata
-        An AnnData matrice of shape n_obs × n_vars. Rows correspond to cells and columns to genes.
+        An AnnData matrice of shape n_obs x n_vars. Rows correspond to cells and columns to genes.
     profile
         Specify the single-cell profile type, RNA or ATAC, Default: RNA.
     min_features
         Filtered out cells that are detected in less than n genes. Default: 100.
     min_cells
         Filtered out genes that are detected in less than n cells. Default: 3.
     target_sum
@@ -359,25 +383,28 @@
     if profile == 'RNA':
         return preprocessing_rna(
                    adata, 
                    min_features=min_features, 
                    min_cells=min_cells, 
                    target_sum=target_sum,
                    n_top_features=n_top_features, 
+                   keep_mt=keep_mt,
+                   backed=backed,
                    chunk_size=chunk_size, 
                    log=log
                )
     elif profile == 'ATAC':
         return preprocessing_atac(
                    adata, 
                    min_features=min_features, 
                    min_cells=min_cells, 
                    target_sum=target_sum,
                    n_top_features=n_top_features, 
                    chunk_size=chunk_size, 
+                   backed=backed,
                    log=log
                )
     else:
         raise ValueError("Not support profile: `{}` yet".format(profile))
 
 def batch_scale(adata, chunk_size=CHUNK_SIZE):
     """
@@ -393,16 +420,17 @@
     Return
     ------
     AnnData
     """
     for b in adata.obs['batch'].unique():
         idx = np.where(adata.obs['batch']==b)[0]
         scaler = MaxAbsScaler(copy=False).fit(adata.X[idx])
-        for i in range(len(idx)//chunk_size+1):
-            adata.X[idx[i*chunk_size:(i+1)*chunk_size]] = scaler.transform(adata.X[idx[i*chunk_size:(i+1)*chunk_size]])
+        adata.X[idx] = scaler.transform(adata.X[idx])
+        # for i in range(len(idx)//chunk_size+1):
+            # adata.X[idx[i*chunk_size:(i+1)*chunk_size]] = scaler.transform(adata.X[idx[i*chunk_size:(i+1)*chunk_size]])
 
     return adata
         
 
 def reindex(adata, genes, chunk_size=CHUNK_SIZE):
     """
     Reindex AnnData with gene list
@@ -422,16 +450,17 @@
     """
     idx = [i for i, g in enumerate(genes) if g in adata.var_names]
     print('There are {} gene in selected genes'.format(len(idx)))
     if len(idx) == len(genes):
         adata = adata[:, genes]
     else:
         new_X = scipy.sparse.lil_matrix((adata.shape[0], len(genes)))
-        for i in range(new_X.shape[0]//chunk_size+1):
-            new_X[i*chunk_size:(i+1)*chunk_size, idx] = adata[i*chunk_size:(i+1)*chunk_size, genes[idx]].X
+        new_X[:, idx] = adata[:, genes[idx]].X
+        # for i in range(new_X.shape[0]//chunk_size+1):
+            # new_X[i*chunk_size:(i+1)*chunk_size, idx] = adata[i*chunk_size:(i+1)*chunk_size, genes[idx]].X
         adata = AnnData(new_X.tocsr(), obs=adata.obs, var={'var_names':genes}) 
     return adata
 
 
 class BatchSampler(Sampler):
     """
     Batch-specific Sampler
@@ -455,15 +484,15 @@
         self.drop_last = drop_last
         self.batch_id = batch_id
 
     def __iter__(self):
         batch = {}
         sampler = np.random.permutation(len(self.batch_id))
         for idx in sampler:
-            c = self.batch_id[idx]
+            c = self.batch_id.iloc[idx]
             if c not in batch:
                 batch[c] = []
             batch[c].append(idx)
 
             if len(batch[c]) == self.batch_size:
                 yield batch[c]
                 batch[c] = []
@@ -479,50 +508,67 @@
             return (len(self.batch_id)+self.batch_size-1) // self.batch_size
         
     
 class SingleCellDataset(Dataset):
     """
     Dataloader of single-cell data
     """
-    def __init__(self, adata):
+    def __init__(self, adata, use_layer='X'):
         """
         create a SingleCellDataset object
             
         Parameters
         ----------
         adata
             AnnData object wrapping the single-cell data matrix
         """
         self.adata = adata
         self.shape = adata.shape
+        self.use_layer = use_layer
         
     def __len__(self):
-        return self.adata.X.shape[0]
+        return self.adata.shape[0]
     
     def __getitem__(self, idx):
-        x = self.adata.X[idx].toarray().squeeze()
-        domain_id = self.adata.obs['batch'].cat.codes[idx]
+        if self.use_layer == 'X':
+            if isinstance(self.adata.X[idx], np.ndarray):
+                x = self.adata.X[idx].squeeze().astype(float)
+            else:
+                x = self.adata.X[idx].toarray().squeeze().astype(float)
+        else:
+            if self.use_layer in self.adata.layers:
+                x = self.adata.layers[self.use_layer][idx]
+            else:
+                x = self.adata.obsm[self.use_layer][idx]
+                
+        domain_id = self.adata.obs['batch'].cat.codes.iloc[idx]
         return x, domain_id, idx
 
 
 def load_data(
         data_list, 
         batch_categories=None, 
         profile='RNA',
         join='inner', 
         batch_key='batch', 
         batch_name='batch',
         min_features=600, 
         min_cells=3, 
         target_sum=None,
         n_top_features=None, 
+        keep_mt=False,
+        backed=False,
         batch_size=64, 
         chunk_size=CHUNK_SIZE,
+        fraction=None,
+        n_obs=None,
         processed=False,
         log=None,
+        num_workers=4,
+        use_layer='X',
     ):
     """
     Load dataset with preprocessing
     
     Parameters
     ----------
     data_list
@@ -556,42 +602,61 @@
         An iterable over the given dataset for training.
     testloader
         An iterable over the given dataset for testing
     """
     adata = concat_data(data_list, batch_categories, join=join, batch_key=batch_key)
     if log: log.info('Raw dataset shape: {}'.format(adata.shape))
     if batch_name!='batch':
-        adata.obs['batch'] = adata.obs[batch_name]
+        if ',' in batch_name:
+            names = batch_name.split(',')
+            adata.obs['batch'] = adata.obs[names[0]].astype(str)+'_'+adata.obs[names[1]].astype(str)
+        else:
+            adata.obs['batch'] = adata.obs[batch_name]
     if 'batch' not in adata.obs:
         adata.obs['batch'] = 'batch'
     adata.obs['batch'] = adata.obs['batch'].astype('category')
     if log: log.info('There are {} batches under batch_name: {}'.format(len(adata.obs['batch'].cat.categories), batch_name))
     
     if isinstance(n_top_features, str):
         if os.path.isfile(n_top_features):
             n_top_features = np.loadtxt(n_top_features, dtype=str)
         else:
             n_top_features = int(n_top_features)
     
-    if not processed:
+    if n_obs is not None or fraction is not None:
+        sc.pp.subsample(adata, fraction=fraction, n_obs=n_obs)
+
+    if not processed and use_layer == 'X':
         adata = preprocessing(
             adata, 
             profile=profile,
             min_features=min_features, 
             min_cells=min_cells, 
             target_sum=target_sum,
             n_top_features=n_top_features,
+            keep_mt=keep_mt,
             chunk_size=chunk_size,
+            backed=backed,
             log=log,
         )
-    scdata = SingleCellDataset(adata) # Wrap AnnData into Pytorch Dataset
+    else:
+        if use_layer in adata.layers:
+            adata.layers[use_layer] = MaxAbsScaler().fit_transform(adata.layers[use_layer])
+        elif use_layer in adata.obsm:
+            adata.obsm[use_layer] = MaxAbsScaler().fit_transform(adata.obsm[use_layer])
+        else:
+            raise ValueError("Not support use_layer: `{}` yet".format(use_layer))
+    scdata = SingleCellDataset(adata, use_layer=use_layer) # Wrap AnnData into Pytorch Dataset
     trainloader = DataLoader(
         scdata, 
         batch_size=batch_size, 
         drop_last=True, 
         shuffle=True, 
-        num_workers=4
+        num_workers=num_workers,
     )
+
     batch_sampler = BatchSampler(batch_size, adata.obs['batch'], drop_last=False)
-    testloader = DataLoader(scdata, batch_sampler=batch_sampler)
+    testloader = DataLoader(scdata, batch_sampler=batch_sampler, num_workers=num_workers)
     
-    return adata, trainloader, testloader 
+    return adata, trainloader, testloader 
+
+
```

### Comparing `scalex-1.0.2/scalex/function.py` & `scalex-1.0.3/scalex/function.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,19 @@
         min_features:int=600, 
         min_cells:int=3, 
         target_sum:int=None,
         n_top_features:int=None,
         join:str='inner', 
         batch_key:str='batch',  
         processed:bool=False,
+        fraction:float=None,
+        n_obs:int=None,
+        use_layer:str='X',
+        keep_mt:bool=False,
+        backed:bool=False,
         batch_size:int=64, 
         lr:float=2e-4, 
         max_iteration:int=30000,
         seed:int=124, 
         gpu:int=0, 
         outdir:str=None, 
         projection:str=None,
@@ -46,14 +51,16 @@
         impute:str=None, 
         chunk_size:int=20000,
         ignore_umap:bool=False,
         verbose:bool=False,
         assess:bool=False,
         show:bool=True,
         eval:bool=False,
+        num_workers:int=4,
+        cell_type:str='cell_type',
     ) -> AnnData:
     """
     Online single-cell data integration through projecting heterogeneous datasets into a common cell-embedding space
     
     Parameters
     ----------
     data_list
@@ -120,39 +127,46 @@
     if torch.cuda.is_available(): # cuda device
         device='cuda'
         torch.cuda.set_device(gpu)
     else:
         device='cpu'
     
     if outdir:
-        outdir = outdir+'/'
-        os.makedirs(outdir+'/checkpoint', exist_ok=True)
-        log = create_logger('SCALEX', fh=outdir+'log.txt', overwrite=True)
+        # outdir = outdir+'/'
+        os.makedirs(os.path.join(outdir, 'checkpoint'), exist_ok=True)
+        log = create_logger('SCALEX', fh=os.path.join(outdir, 'log.txt'), overwrite=True)
     else:
         log = create_logger('SCALEX')
 
     if not projection:
         adata, trainloader, testloader = load_data(
             data_list, batch_categories, 
             join=join,
             profile=profile,
             target_sum=target_sum,
             n_top_features=n_top_features,
             batch_size=batch_size, 
             chunk_size=chunk_size,
             min_features=min_features, 
             min_cells=min_cells,
+            fraction=fraction,
+            n_obs=n_obs,
             processed=processed,
+            use_layer=use_layer,
+            backed=backed,
             batch_name=batch_name, 
             batch_key=batch_key,
+            keep_mt=keep_mt,
             log=log,
+            num_workers=num_workers,
         )
         
-        early_stopping = EarlyStopping(patience=10, checkpoint_file=outdir+'/checkpoint/model.pt' if outdir else None)
-        x_dim, n_domain = adata.shape[1], len(adata.obs['batch'].cat.categories)
+        early_stopping = EarlyStopping(patience=10, checkpoint_file=os.path.join(outdir, 'checkpoint/model.pt') if outdir else None)
+        x_dim = adata.shape[1] if (use_layer == 'X' or use_layer in adata.layers) else adata.obsm[use_layer].shape[1]
+        n_domain = len(adata.obs['batch'].cat.categories)
         
         # model config
         enc = [['fc', 1024, 1, 'relu'],['fc', 10, '', '']]  # TO DO
         dec = [['fc', x_dim, n_domain, 'sigmoid']]
 
         model = VAE(enc, dec, n_domain=n_domain)
         
@@ -162,90 +176,97 @@
             lr=lr, 
             max_iteration=max_iteration, 
             device=device, 
             early_stopping=early_stopping, 
             verbose=verbose,
         )
         if outdir:
-            torch.save({'n_top_features':adata.var.index, 'enc':enc, 'dec':dec, 'n_domain':n_domain}, outdir+'/checkpoint/config.pt')
+            torch.save({'n_top_features':adata.var.index, 'enc':enc, 'dec':dec, 'n_domain':n_domain}, os.path.join(outdir, 'checkpoint/config.pt'))
     else:
-        state = torch.load(projection+'/checkpoint/config.pt')
+        state = torch.load(os.path.join(projection, 'checkpoint/config.pt'))
         n_top_features, enc, dec, n_domain = state['n_top_features'], state['enc'], state['dec'], state['n_domain']
         model = VAE(enc, dec, n_domain=n_domain)
-        model.load_model(projection+'/checkpoint/model.pt')
+        model.load_model(os.path.join(projection, 'checkpoint/model.pt'))
         model.to(device)
         
         adata, trainloader, testloader = load_data(
             data_list, batch_categories,  
             join='outer', 
             profile=profile,
             target_sum=target_sum,
             chunk_size=chunk_size,
             n_top_features=n_top_features, 
             min_cells=0,
             min_features=min_features,
             processed=processed,
             batch_name=batch_name,
             batch_key=batch_key,
-            log = log
+            # keep_mt=keep_mt,
+            log = log,
+            num_workers=num_workers,
         )
 #         log.info('Processed dataset shape: {}'.format(adata.shape))
         
     adata.obsm['latent'] = model.encodeBatch(testloader, device=device, eval=eval) # save latent rep
     if impute:
         adata.layers['impute'] = model.encodeBatch(testloader, out='impute', batch_id=impute, device=device, eval=eval)
     # log.info('Output dir: {}'.format(outdir))
     
     model.to('cpu')
     del model
     if projection and (not repeat):
-        ref = sc.read_h5ad(projection+'/adata.h5ad')
+        ref = sc.read_h5ad(os.path.join(projection, 'adata.h5ad'))
         adata = AnnData.concatenate(
             ref, adata, 
             batch_categories=['reference', 'query'], 
             batch_key='projection', 
             index_unique=None
         )
 
     if outdir is not None:
-        adata.write(outdir+'adata.h5ad', compression='gzip')  
+        adata.write(os.path.join(outdir, 'adata.h5ad'), compression='gzip')  
 
     if not ignore_umap: #and adata.shape[0]<1e6:
         log.info('Plot umap')
         sc.pp.neighbors(adata, n_neighbors=30, use_rep='latent')
         sc.tl.umap(adata, min_dist=0.1)
         sc.tl.leiden(adata)
         adata.obsm['X_scalex_umap'] = adata.obsm['X_umap']
         
         # UMAP visualization
         sc.set_figure_params(dpi=80, figsize=(3,3))
-        cols = ['batch', 'celltype', 'cell_type', 'leiden']
+        cols = [cell_type, 'leiden'] 
+        cols += ['batch'] if n_domain > 1 else []
         color = [c for c in cols if c in adata.obs]
         if outdir:
             sc.settings.figdir = outdir
             save = '.png'
         else:
             save = None
 
         if len(color) > 0:
             if projection and (not repeat):
                 embedding(adata, color='leiden', groupby='projection', save=save, show=show)
             else:
                 sc.pl.umap(adata, color=color, save=save, wspace=0.4, ncols=4, show=show)  
-        if assess:
-            if len(adata.obs['batch'].cat.categories) > 1:
-                entropy_score = batch_entropy_mixing_score(adata.obsm['X_umap'], adata.obs['batch'])
-                log.info('batch_entropy_mixing_score: {:.3f}'.format(entropy_score))
-
-            if 'celltype' in adata.obs:
-                sil_score = silhouette_score(adata.obsm['X_umap'], adata.obs['celltype'].cat.codes)
-                log.info("silhouette_score: {:.3f}".format(sil_score))
 
     if outdir is not None:
-        adata.write(outdir+'adata.h5ad', compression='gzip')
+        adata.write(os.path.join(outdir, 'adata.h5ad'), compression='gzip')
+
+    if assess:
+        if adata.shape[0] > 5e4:
+            log.info('Subsample cell numbers to 50,000 for entropy_batch_mixing_score calculation.')
+            sc.pp.subsample(adata, n_obs=int(5e4))
+        if len(adata.obs['batch'].cat.categories) > 1:
+            entropy_score = batch_entropy_mixing_score(adata.obsm['X_umap'], adata.obs['batch'])
+            log.info('batch_entropy_mixing_score: {:.3f}'.format(entropy_score))
+
+        if cell_type in adata.obs:
+            sil_score = silhouette_score(adata.obsm['X_umap'], adata.obs[cell_type].cat.codes)
+            log.info("silhouette_score: {:.3f}".format(sil_score))
     
     return adata
         
         
 
 def label_transfer(ref, query, rep='latent', label='celltype'):
     """
```

### Comparing `scalex-1.0.2/scalex/logger.py` & `scalex-1.0.3/scalex/logger.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/scalex/metrics.py` & `scalex-1.0.3/scalex/metrics.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/scalex/net/layer.py` & `scalex-1.0.3/scalex/net/layer.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/scalex/net/loss.py` & `scalex-1.0.3/scalex/net/loss.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/scalex/net/utils.py` & `scalex-1.0.3/scalex/net/utils.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/scalex/net/vae.py` & `scalex-1.0.3/scalex/net/vae.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 # Description:
 
 """
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import numpy as np
-from tqdm import tqdm
+from tqdm.autonotebook import trange
+from tqdm.contrib import tenumerate
 from collections import defaultdict
-import sys
 
 from .layer import *
 from .loss import *
 
 
 class VAE(nn.Module):
     """
@@ -151,44 +151,50 @@
         verbose
             Verbosity, True or False. Default: False.
         """
         self.to(device)
         optim = torch.optim.Adam(self.parameters(), lr=lr, weight_decay=5e-4)
         n_epoch = int(np.ceil(max_iteration/len(dataloader)))
         
-        with tqdm(range(n_epoch), total=n_epoch, desc='Epochs') as tq:       
+        with trange(n_epoch, total=n_epoch, desc='Epochs') as tq:
             for epoch in tq:
-                tk0 = tqdm(enumerate(dataloader), total=len(dataloader), leave=False, desc='Iterations', disable=(not verbose))
+                tk0 = tenumerate(dataloader, total=len(dataloader), leave=False, desc='Iterations', disable=(not verbose))
                 epoch_loss = defaultdict(float)
+                acc = []
                 for i, (x, y, idx) in tk0:
                     x, y = x.float().to(device), y.long().to(device)
 
                     # loss
                     z, mu, var = self.encoder(x)
                     recon_x = self.decoder(z, y)
                     recon_loss = F.binary_cross_entropy(recon_x, x) * x.size(-1)  ## TO DO
                     kl_loss = kl_div(mu, var) 
             
+                    # acc.append(pearson_corr_coef(recon_x, x))
                     loss = {'recon_loss':recon_loss, 'kl_loss':0.5*kl_loss} 
                     
                     optim.zero_grad()
                     sum(loss.values()).backward()
                     optim.step()
                     
                     for k,v in loss.items():
                         epoch_loss[k] += loss[k].item()
                         
                     info = ','.join(['{}={:.3f}'.format(k, v) for k,v in loss.items()])
-                    tk0.set_postfix_str(info)
+                    # tk0.set_postfix_str(info)
                     
 
                 epoch_loss = {k:v/(i+1) for k, v in epoch_loss.items()}
                 epoch_info = ','.join(['{}={:.3f}'.format(k, v) for k,v in epoch_loss.items()])
+                # epoch_info += ',acc={:.3f}'.format(torch.Tensor(acc).mean().item())
                 tq.set_postfix_str(epoch_info) 
                     
                 early_stopping(sum(epoch_loss.values()), self)
                 if early_stopping.early_stop:
                     print('EarlyStopping: run {} epoch'.format(epoch+1))
                     break       
                     
         
-                
+def pearson_corr_coef(x, y, dim = 1, reduce_dims = (-1,)):
+    x_centered = x - x.mean(dim = dim, keepdim = True)
+    y_centered = y - y.mean(dim = dim, keepdim = True)
+    return F.cosine_similarity(x_centered, y_centered, dim = dim).mean(dim = reduce_dims)
```

### Comparing `scalex-1.0.2/scalex/plot.py` & `scalex-1.0.3/scalex/plot.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/scalex.egg-info/PKG-INFO` & `scalex-1.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 Metadata-Version: 2.1
 Name: scalex
-Version: 1.0.2
+Version: 1.0.3
 Summary: Online single-cell data integration through projecting heterogeneous datasets into a common cell-embedding space
 Home-page: https://github.com/jsxlei/scalex
 Author: Lei Xiong
 Author-email: jsxlei@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >3.6.0
 License-File: LICENSE.txt
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: pandas>=2.2.2
+Requires-Dist: scipy>=1.13.0
+Requires-Dist: scikit-learn>=1.4.2
+Requires-Dist: torch>=2.2.2
+Requires-Dist: scanpy>=1.10.1
+Requires-Dist: tqdm>=4.66.2
+Requires-Dist: matplotlib>=3.8.4
+Requires-Dist: seaborn>=0.13.2
+Requires-Dist: leidenalg>=0.8.3
+Requires-Dist: sphinx_autodoc_typehints
+Requires-Dist: nbsphinx
 
 [![Stars](https://img.shields.io/github/stars/jsxlei/scalex?logo=GitHub&color=yellow)](https://github.com/jsxlei/scalex/stargazers)
 [![PyPI](https://img.shields.io/pypi/v/scalex.svg)](https://pypi.org/project/scalex)
 [![Documentation Status](https://readthedocs.org/projects/scalex/badge/?version=latest)](https://scalex.readthedocs.io/en/latest/?badge=stable)
 [![Downloads](https://pepy.tech/badge/scalex)](https://pepy.tech/project/scalex)
 [![DOI](https://zenodo.org/badge/345941713.svg)](https://zenodo.org/badge/latestdoi/345941713)
 # [Online single-cell data integration through projecting heterogeneous datasets into a common cell-embedding space](https://www.nature.com/articles/s41467-022-33758-z)
@@ -172,9 +183,7 @@
     
     
 
     
     
 
 
-
-
```

### Comparing `scalex-1.0.2/scalex.egg-info/SOURCES.txt` & `scalex-1.0.3/scalex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/setup.py` & `scalex-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/third_parties/BBKNN.py` & `scalex-1.0.3/third_parties/BBKNN.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/third_parties/Conos.R` & `scalex-1.0.3/third_parties/Conos.R`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/third_parties/DESC.py` & `scalex-1.0.3/third_parties/DESC.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/third_parties/FastMNN.R` & `scalex-1.0.3/third_parties/FastMNN.R`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/third_parties/Harmony.R` & `scalex-1.0.3/third_parties/Harmony.R`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/third_parties/LIGER.R` & `scalex-1.0.3/third_parties/LIGER.R`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/third_parties/Raw.py` & `scalex-1.0.3/third_parties/Raw.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/third_parties/Scanorama.py` & `scalex-1.0.3/third_parties/Scanorama.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/third_parties/Seurat_v3.R` & `scalex-1.0.3/third_parties/Seurat_v3.R`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/third_parties/online_iNMF.R` & `scalex-1.0.3/third_parties/online_iNMF.R`

 * *Files identical despite different names*

### Comparing `scalex-1.0.2/third_parties/scVI.py` & `scalex-1.0.3/third_parties/scVI.py`

 * *Files identical despite different names*

