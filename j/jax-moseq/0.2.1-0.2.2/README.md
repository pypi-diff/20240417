# Comparing `tmp/jax-moseq-0.2.1.tar.gz` & `tmp/jax-moseq-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-moseq-0.2.1.tar", last modified: Mon Dec 18 20:35:51 2023, max compression
+gzip compressed data, was "jax-moseq-0.2.2.tar", last modified: Tue Apr 16 22:04:35 2024, max compression
```

## Comparing `jax-moseq-0.2.1.tar` & `jax-moseq-0.2.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-12-18 20:35:51.919590 jax-moseq-0.2.1/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8384 2023-10-25 15:56:05.000000 jax-moseq-0.2.1/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      300 2023-12-18 20:35:51.919725 jax-moseq-0.2.1/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      615 2023-10-25 15:56:05.000000 jax-moseq-0.2.1/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-12-18 20:35:51.920539 jax-moseq-0.2.1/jax_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      125 2023-12-14 14:49:37.000000 jax-moseq-0.2.1/jax_moseq/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-12-18 20:35:51.920620 jax-moseq-0.2.1/jax_moseq/_version.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-12-18 20:35:51.901928 jax-moseq-0.2.1/jax_moseq/models/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      128 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/__init__.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-12-18 20:35:51.904931 jax-moseq-0.2.1/jax_moseq/models/allo_dynamics/
--rw-r--r--   0 calebweinreb   (501) staff       (20)       95 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/allo_dynamics/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     3925 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/allo_dynamics/generate.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8176 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/allo_dynamics/gibbs.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     2589 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/allo_dynamics/initialize.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1594 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/allo_dynamics/log_prob.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-12-18 20:35:51.906838 jax-moseq-0.2.1/jax_moseq/models/allo_keypoint_slds/
--rw-r--r--   0 calebweinreb   (501) staff       (20)       71 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/allo_keypoint_slds/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    11801 2023-12-18 20:29:04.000000 jax-moseq-0.2.1/jax_moseq/models/allo_keypoint_slds/gibbs.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1224 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/allo_keypoint_slds/initialize.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     2626 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/allo_keypoint_slds/log_prob.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-12-18 20:35:51.909577 jax-moseq-0.2.1/jax_moseq/models/arhmm/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      183 2023-12-14 14:51:51.000000 jax-moseq-0.2.1/jax_moseq/models/arhmm/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     5396 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/arhmm/generate.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     7998 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/arhmm/gibbs.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     7853 2023-12-14 14:49:37.000000 jax-moseq-0.2.1/jax_moseq/models/arhmm/initialize.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     5852 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/arhmm/log_prob.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-12-18 20:35:51.912830 jax-moseq-0.2.1/jax_moseq/models/keypoint_slds/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      216 2023-12-14 14:53:08.000000 jax-moseq-0.2.1/jax_moseq/models/keypoint_slds/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    13737 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/keypoint_slds/alignment.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    13193 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/keypoint_slds/gibbs.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    14173 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/keypoint_slds/initialize.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4798 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/keypoint_slds/log_prob.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-12-18 20:35:51.915212 jax-moseq-0.2.1/jax_moseq/models/slds/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      134 2023-12-14 14:56:29.000000 jax-moseq-0.2.1/jax_moseq/models/slds/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    12866 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/models/slds/gibbs.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     9780 2023-12-14 14:49:37.000000 jax-moseq-0.2.1/jax_moseq/models/slds/initialize.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4066 2023-12-14 14:49:37.000000 jax-moseq-0.2.1/jax_moseq/models/slds/log_prob.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-12-18 20:35:51.918703 jax-moseq-0.2.1/jax_moseq/utils/
--rw-r--r--   0 calebweinreb   (501) staff       (20)       46 2023-12-14 14:49:37.000000 jax-moseq-0.2.1/jax_moseq/utils/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1133 2023-12-14 14:49:37.000000 jax-moseq-0.2.1/jax_moseq/utils/autoregression.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     9717 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/utils/debugging.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     2853 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/utils/distributions.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     6688 2023-12-15 15:04:36.000000 jax-moseq-0.2.1/jax_moseq/utils/kalman.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    13218 2023-12-14 14:49:37.000000 jax-moseq-0.2.1/jax_moseq/utils/transitions.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    16911 2023-12-15 15:10:52.000000 jax-moseq-0.2.1/jax_moseq/utils/utils.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-12-18 20:35:51.901600 jax-moseq-0.2.1/jax_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      300 2023-12-18 20:35:51.000000 jax-moseq-0.2.1/jax_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1425 2023-12-18 20:35:51.000000 jax-moseq-0.2.1/jax_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-12-18 20:35:51.000000 jax-moseq-0.2.1/jax_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      102 2023-12-18 20:35:51.000000 jax-moseq-0.2.1/jax_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       10 2023-12-18 20:35:51.000000 jax-moseq-0.2.1/jax_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      656 2023-12-18 20:35:51.920307 jax-moseq-0.2.1/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      242 2023-12-14 14:49:37.000000 jax-moseq-0.2.1/setup.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    84134 2023-12-14 14:49:38.000000 jax-moseq-0.2.1/versioneer.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-16 22:04:35.290272 jax-moseq-0.2.2/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8384 2023-10-25 15:56:05.000000 jax-moseq-0.2.2/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      300 2024-04-16 22:04:35.290562 jax-moseq-0.2.2/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      615 2023-10-25 15:56:05.000000 jax-moseq-0.2.2/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-16 22:04:35.292311 jax-moseq-0.2.2/jax_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      125 2023-12-14 14:49:37.000000 jax-moseq-0.2.2/jax_moseq/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2024-04-16 22:04:35.292472 jax-moseq-0.2.2/jax_moseq/_version.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-16 22:04:35.264339 jax-moseq-0.2.2/jax_moseq/models/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      128 2024-04-16 21:38:18.000000 jax-moseq-0.2.2/jax_moseq/models/__init__.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-16 22:04:35.269403 jax-moseq-0.2.2/jax_moseq/models/allo_dynamics/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       95 2023-12-15 15:04:36.000000 jax-moseq-0.2.2/jax_moseq/models/allo_dynamics/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     3925 2023-12-15 15:04:36.000000 jax-moseq-0.2.2/jax_moseq/models/allo_dynamics/generate.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8176 2023-12-15 15:04:36.000000 jax-moseq-0.2.2/jax_moseq/models/allo_dynamics/gibbs.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     2589 2024-04-16 21:38:18.000000 jax-moseq-0.2.2/jax_moseq/models/allo_dynamics/initialize.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1594 2023-12-15 15:04:36.000000 jax-moseq-0.2.2/jax_moseq/models/allo_dynamics/log_prob.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-16 22:04:35.271929 jax-moseq-0.2.2/jax_moseq/models/allo_keypoint_slds/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       71 2023-12-15 15:04:36.000000 jax-moseq-0.2.2/jax_moseq/models/allo_keypoint_slds/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    11801 2024-04-16 21:38:18.000000 jax-moseq-0.2.2/jax_moseq/models/allo_keypoint_slds/gibbs.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1224 2024-04-16 21:38:18.000000 jax-moseq-0.2.2/jax_moseq/models/allo_keypoint_slds/initialize.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     2626 2023-12-15 15:04:36.000000 jax-moseq-0.2.2/jax_moseq/models/allo_keypoint_slds/log_prob.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-16 22:04:35.274812 jax-moseq-0.2.2/jax_moseq/models/arhmm/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      183 2023-12-14 14:51:51.000000 jax-moseq-0.2.2/jax_moseq/models/arhmm/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     5396 2023-12-15 15:04:36.000000 jax-moseq-0.2.2/jax_moseq/models/arhmm/generate.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     7998 2023-12-15 15:04:36.000000 jax-moseq-0.2.2/jax_moseq/models/arhmm/gibbs.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     7853 2023-12-14 14:49:37.000000 jax-moseq-0.2.2/jax_moseq/models/arhmm/initialize.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     5714 2024-04-16 21:38:18.000000 jax-moseq-0.2.2/jax_moseq/models/arhmm/log_prob.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-16 22:04:35.277518 jax-moseq-0.2.2/jax_moseq/models/keypoint_slds/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      216 2023-12-14 14:53:08.000000 jax-moseq-0.2.2/jax_moseq/models/keypoint_slds/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    13737 2024-04-16 21:38:18.000000 jax-moseq-0.2.2/jax_moseq/models/keypoint_slds/alignment.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    13193 2023-12-15 15:04:36.000000 jax-moseq-0.2.2/jax_moseq/models/keypoint_slds/gibbs.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    14689 2024-04-16 22:04:26.000000 jax-moseq-0.2.2/jax_moseq/models/keypoint_slds/initialize.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4798 2023-12-15 15:04:36.000000 jax-moseq-0.2.2/jax_moseq/models/keypoint_slds/log_prob.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-16 22:04:35.280503 jax-moseq-0.2.2/jax_moseq/models/slds/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      134 2023-12-14 14:56:29.000000 jax-moseq-0.2.2/jax_moseq/models/slds/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    12866 2023-12-15 15:04:36.000000 jax-moseq-0.2.2/jax_moseq/models/slds/gibbs.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     9780 2023-12-14 14:49:37.000000 jax-moseq-0.2.2/jax_moseq/models/slds/initialize.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4066 2023-12-14 14:49:37.000000 jax-moseq-0.2.2/jax_moseq/models/slds/log_prob.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-16 22:04:35.288684 jax-moseq-0.2.2/jax_moseq/utils/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       46 2023-12-14 14:49:37.000000 jax-moseq-0.2.2/jax_moseq/utils/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1133 2023-12-14 14:49:37.000000 jax-moseq-0.2.2/jax_moseq/utils/autoregression.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     9721 2024-03-16 17:09:44.000000 jax-moseq-0.2.2/jax_moseq/utils/debugging.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     2853 2023-12-15 15:04:36.000000 jax-moseq-0.2.2/jax_moseq/utils/distributions.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     6688 2023-12-15 15:04:36.000000 jax-moseq-0.2.2/jax_moseq/utils/kalman.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    13218 2023-12-14 14:49:37.000000 jax-moseq-0.2.2/jax_moseq/utils/transitions.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    16911 2023-12-15 15:10:52.000000 jax-moseq-0.2.2/jax_moseq/utils/utils.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-16 22:04:35.263682 jax-moseq-0.2.2/jax_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      300 2024-04-16 22:04:35.000000 jax-moseq-0.2.2/jax_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1425 2024-04-16 22:04:35.000000 jax-moseq-0.2.2/jax_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2024-04-16 22:04:35.000000 jax-moseq-0.2.2/jax_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      102 2024-04-16 22:04:35.000000 jax-moseq-0.2.2/jax_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       10 2024-04-16 22:04:35.000000 jax-moseq-0.2.2/jax_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      656 2024-04-16 22:04:35.291813 jax-moseq-0.2.2/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      242 2023-12-14 14:49:37.000000 jax-moseq-0.2.2/setup.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    84134 2023-12-14 14:49:38.000000 jax-moseq-0.2.2/versioneer.py
```

### Comparing `jax-moseq-0.2.1/LICENSE.md` & `jax-moseq-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/README.md` & `jax-moseq-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/allo_dynamics/generate.py` & `jax-moseq-0.2.2/jax_moseq/models/allo_dynamics/generate.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/allo_dynamics/gibbs.py` & `jax-moseq-0.2.2/jax_moseq/models/allo_dynamics/gibbs.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/allo_dynamics/initialize.py` & `jax-moseq-0.2.2/jax_moseq/models/allo_dynamics/initialize.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/allo_dynamics/log_prob.py` & `jax-moseq-0.2.2/jax_moseq/models/allo_dynamics/log_prob.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/allo_keypoint_slds/gibbs.py` & `jax-moseq-0.2.2/jax_moseq/models/allo_keypoint_slds/gibbs.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/allo_keypoint_slds/initialize.py` & `jax-moseq-0.2.2/jax_moseq/models/allo_keypoint_slds/initialize.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/allo_keypoint_slds/log_prob.py` & `jax-moseq-0.2.2/jax_moseq/models/allo_keypoint_slds/log_prob.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/arhmm/generate.py` & `jax-moseq-0.2.2/jax_moseq/models/arhmm/generate.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/arhmm/gibbs.py` & `jax-moseq-0.2.2/jax_moseq/models/arhmm/gibbs.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/arhmm/initialize.py` & `jax-moseq-0.2.2/jax_moseq/models/arhmm/initialize.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/arhmm/log_prob.py` & `jax-moseq-0.2.2/jax_moseq/models/arhmm/log_prob.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,21 +95,16 @@
     ll["z"] = (log_pz * mask[..., nlags + 1 :]).sum()
     ll["x"] = (log_px * mask[..., nlags:]).sum()
     return ll
 
 
 def model_likelihood(data, states, params, hypparams=None, **kwargs):
     """
-<<<<<<< HEAD
     Convenience function that invokes :py:func:`jax_moseq.models.arhmm.log_prob.log_joint_likelihood`.
-    
-=======
-    Convenience class that invokes :py:func:`jax_moseq.models.arhmm.log_prob.log_joint_likelihood`.
 
->>>>>>> dev
     Parameters
     ----------
     data : dict
         Data dictionary containing the observations and mask.
     states : dict
         State values for each latent variable.
     params : dict
```

### Comparing `jax-moseq-0.2.1/jax_moseq/models/keypoint_slds/alignment.py` & `jax-moseq-0.2.2/jax_moseq/models/keypoint_slds/alignment.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/keypoint_slds/gibbs.py` & `jax-moseq-0.2.2/jax_moseq/models/keypoint_slds/gibbs.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/keypoint_slds/initialize.py` & `jax-moseq-0.2.2/jax_moseq/models/keypoint_slds/initialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     params,
     noise_prior,
     obs_hypparams,
     Y_flat=None,
     v=None,
     h=None,
     fix_heading=False,
-    **kwargs
+    **kwargs,
 ):
     """
     Initialize the latent states of the keypoint SLDS from the data,
     parameters, and hyperparameters.
 
     Parameters
     ----------
@@ -159,15 +159,15 @@
     trans_hypparams=None,
     ar_hypparams=None,
     obs_hypparams=None,
     cen_hypparams=None,
     verbose=False,
     exclude_outliers_for_pca=True,
     fix_heading=False,
-    **kwargs
+    **kwargs,
 ):
     """
     Initialize a keypoint SLDS model dict containing the
     hyperparameters, noise prior, and initial seed, states,
     and parameters.
 
     Parameters
@@ -448,7 +448,19 @@
         )
 
     if not (states and params) and (anterior_idxs is None or posterior_idxs is None):
         raise ValueError(
             "If `states` and `params` not provided, must "
             "provide `anterior_idxs` and `posterior_idxs`."
         )
+
+    if data:
+        if ar_hypparams:
+            latent_dim = ar_hypparams["latent_dim"]
+        else:
+            latent_dim = hypparams["ar_hypparams"]["latent_dim"]
+        max_dim = (data["Y"].shape[-2] - 1) * data["Y"].shape[-1]
+        if latent_dim > max_dim:
+            raise ValueError(
+                "`latent_dim` must be less than or equal to `(num_keypoints - 1) * keypoint_dim`. "
+                f"The current value of `latent_dim` ({latent_dim}) is above the maximum ({max_dim})"
+            )
```

### Comparing `jax-moseq-0.2.1/jax_moseq/models/keypoint_slds/log_prob.py` & `jax-moseq-0.2.2/jax_moseq/models/keypoint_slds/log_prob.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/slds/gibbs.py` & `jax-moseq-0.2.2/jax_moseq/models/slds/gibbs.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/slds/initialize.py` & `jax-moseq-0.2.2/jax_moseq/models/slds/initialize.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/models/slds/log_prob.py` & `jax-moseq-0.2.2/jax_moseq/models/slds/log_prob.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/utils/autoregression.py` & `jax-moseq-0.2.2/jax_moseq/utils/autoregression.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/utils/debugging.py` & `jax-moseq-0.2.2/jax_moseq/utils/debugging.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         if len(args_with_wrong_precision) > 0:
             msg = f'JAX is configured to use {"64" if x64 else "32"}-bit precision, '
             msg += (
                 f'but following arguments contain {"32" if x64 else "64"}-bit arrays: '
             )
             msg += ", ".join([f'"{name}"' for name in args_with_wrong_precision])
             msg += '. Either change the JAX config using `jax.config.update("jax_enable_x64", True/False)` '
-            msg += "or convert the arguments to the correct precision using `jax_moseq.utils.utils.convert_data_precision`."
+            msg += "or convert the arguments to the correct precision using `jax_moseq.utils.debugging.convert_data_precision`."
             raise ValueError(msg)
 
         return fn(*args, **kwargs)
 
     return wrapper
```

### Comparing `jax-moseq-0.2.1/jax_moseq/utils/distributions.py` & `jax-moseq-0.2.2/jax_moseq/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/utils/kalman.py` & `jax-moseq-0.2.2/jax_moseq/utils/kalman.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/utils/transitions.py` & `jax-moseq-0.2.2/jax_moseq/utils/transitions.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq/utils/utils.py` & `jax-moseq-0.2.2/jax_moseq/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/jax_moseq.egg-info/SOURCES.txt` & `jax-moseq-0.2.2/jax_moseq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/setup.cfg` & `jax-moseq-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.2.1/versioneer.py` & `jax-moseq-0.2.2/versioneer.py`

 * *Files identical despite different names*

