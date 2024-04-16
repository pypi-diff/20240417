# Comparing `tmp/pyMetaheuristic-1.9.4.tar.gz` & `tmp/pyMetaheuristic-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyMetaheuristic-1.9.4.tar", last modified: Sat Dec 30 18:45:01 2023, max compression
+gzip compressed data, was "dist\pyMetaheuristic-1.9.5.tar", last modified: Tue Apr 16 23:42:05 2024, max compression
```

## Comparing `pyMetaheuristic-1.9.4.tar` & `pyMetaheuristic-1.9.5.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-12-30 18:45:01.000000 pyMetaheuristic-1.9.4/
--rw-rw-rw-   0        0        0      671 2022-03-18 23:04:07.000000 pyMetaheuristic-1.9.4/LICENSE
--rw-rw-rw-   0        0        0    19869 2023-12-30 18:45:01.000000 pyMetaheuristic-1.9.4/PKG-INFO
--rw-rw-rw-   0        0        0    19358 2023-12-05 21:20:46.000000 pyMetaheuristic-1.9.4/README.md
-drwxrwxrwx   0        0        0        0 2023-12-30 18:45:00.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/
--rw-rw-rw-   0        0        0        1 2022-03-18 23:04:07.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-30 18:45:01.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/
--rw-rw-rw-   0        0        0     2323 2023-12-04 18:54:02.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/__init__.py
--rw-rw-rw-   0        0        0     7910 2023-12-03 15:25:03.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/abco.py
--rw-rw-rw-   0        0        0     7045 2023-12-03 15:23:34.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/acgwo.py
--rw-rw-rw-   0        0        0     8368 2023-12-03 17:27:26.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/afsa.py
--rw-rw-rw-   0        0        0     6416 2023-12-03 16:32:11.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/alo.py
--rw-rw-rw-   0        0        0     4385 2023-12-03 17:27:26.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/aoa.py
--rw-rw-rw-   0        0        0     6145 2023-12-03 17:30:48.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/ars.py
--rw-rw-rw-   0        0        0     5468 2023-12-30 18:38:11.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/bat_a.py
--rw-rw-rw-   0        0        0     5235 2023-12-03 21:42:31.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/bbo.py
--rw-rw-rw-   0        0        0     4224 2023-12-03 21:42:57.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/ca.py
--rw-rw-rw-   0        0        0     4866 2023-12-03 22:08:55.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/cat_so.py
--rw-rw-rw-   0        0        0     4749 2023-12-03 22:21:52.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/cem.py
--rw-rw-rw-   0        0        0     6767 2023-12-03 22:28:13.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/chicken_so.py
--rw-rw-rw-   0        0        0     5384 2023-12-03 22:43:28.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/clonalg.py
--rw-rw-rw-   0        0        0     4114 2023-12-03 22:49:17.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/coati_oa.py
--rw-rw-rw-   0        0        0     5511 2023-12-03 23:16:01.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/cockroach_so.py
--rw-rw-rw-   0        0        0     4163 2023-12-03 23:27:10.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/csa.py
--rw-rw-rw-   0        0        0     5501 2023-12-03 23:42:49.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/cuckoo_s.py
--rw-rw-rw-   0        0        0     7814 2023-12-03 23:46:43.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/da.py
--rw-rw-rw-   0        0        0     4228 2023-12-04 13:24:50.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/de.py
--rw-rw-rw-   0        0        0     4146 2023-12-04 12:59:10.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/dfo.py
--rw-rw-rw-   0        0        0     6376 2023-12-04 13:16:29.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/dvba.py
--rw-rw-rw-   0        0        0     4611 2023-12-04 13:24:32.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/eho.py
--rw-rw-rw-   0        0        0     6679 2023-12-04 13:37:52.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/fda.py
--rw-rw-rw-   0        0        0     4797 2023-12-04 14:02:18.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/firefly_a.py
--rw-rw-rw-   0        0        0     5384 2023-12-04 14:19:54.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/fpa.py
--rw-rw-rw-   0        0        0     6579 2023-12-08 21:50:01.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/ga.py
--rw-rw-rw-   0        0        0     5936 2023-12-04 17:17:28.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/gmo.py
--rw-rw-rw-   0        0        0     4657 2023-12-04 17:33:35.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/goa.py
--rw-rw-rw-   0        0        0     6179 2023-12-04 17:58:44.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/gsa.py
--rw-rw-rw-   0        0        0     6451 2023-12-04 18:05:33.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/gwo.py
--rw-rw-rw-   0        0        0     8767 2023-12-04 18:45:58.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/hho.py
--rw-rw-rw-   0        0        0     4173 2023-12-04 18:50:36.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/hsa.py
--rw-rw-rw-   0        0        0     5068 2023-12-04 19:26:31.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/hus.py
--rw-rw-rw-   0        0        0     8175 2023-12-04 18:24:12.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/i_gwo.py
--rw-rw-rw-   0        0        0     7517 2023-12-08 21:10:56.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/i_woa.py
--rw-rw-rw-   0        0        0     5820 2023-12-04 19:43:45.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/jso.py
--rw-rw-rw-   0        0        0     4535 2023-12-07 23:50:47.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/jy.py
--rw-rw-rw-   0        0        0    11608 2023-12-05 13:08:16.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/kha.py
--rw-rw-rw-   0        0        0     6074 2023-12-05 16:23:18.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/mbo.py
--rw-rw-rw-   0        0        0     9263 2023-12-05 16:51:31.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/memetic_a.py
--rw-rw-rw-   0        0        0     4913 2023-12-05 17:14:24.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/mfa.py
--rw-rw-rw-   0        0        0     5668 2023-12-05 17:20:30.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/mvo.py
--rw-rw-rw-   0        0        0     4145 2023-12-05 17:27:47.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/pbil.py
--rw-rw-rw-   0        0        0     5612 2023-12-05 18:00:16.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/pfa.py
--rw-rw-rw-   0        0        0     4904 2023-12-05 18:37:34.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/pso.py
--rw-rw-rw-   0        0        0     3909 2023-12-05 18:49:32.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/random_s.py
--rw-rw-rw-   0        0        0     4266 2023-12-08 21:15:11.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/sa.py
--rw-rw-rw-   0        0        0     4067 2023-12-05 19:33:28.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/sine_cosine_a.py
--rw-rw-rw-   0        0        0     6706 2023-12-05 19:38:31.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/sos.py
--rw-rw-rw-   0        0        0     7655 2023-12-08 21:07:15.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/spbo.py
--rw-rw-rw-   0        0        0     4454 2023-12-05 20:21:52.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/ssa.py
--rw-rw-rw-   0        0        0     5414 2023-12-05 20:32:10.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/tlbo.py
--rw-rw-rw-   0        0        0     5134 2023-12-08 21:10:24.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/woa.py
-drwxrwxrwx   0        0        0        0 2023-12-30 18:45:01.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/test_function/
--rw-rw-rw-   0        0        0       22 2022-03-18 23:04:07.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/test_function/__init__.py
--rw-rw-rw-   0        0        0    11703 2022-05-07 19:26:33.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/test_function/single.py
-drwxrwxrwx   0        0        0        0 2023-12-30 18:45:01.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/utils/
--rw-rw-rw-   0        0        0       22 2022-03-18 23:04:07.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/utils/__init__.py
--rw-rw-rw-   0        0        0     7537 2022-03-18 23:04:07.000000 pyMetaheuristic-1.9.4/pyMetaheuristic/utils/graphs.py
-drwxrwxrwx   0        0        0        0 2023-12-30 18:45:00.000000 pyMetaheuristic-1.9.4/pyMetaheuristic.egg-info/
--rw-rw-rw-   0        0        0    19869 2023-12-30 18:44:59.000000 pyMetaheuristic-1.9.4/pyMetaheuristic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2251 2023-12-30 18:44:59.000000 pyMetaheuristic-1.9.4/pyMetaheuristic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-30 18:44:59.000000 pyMetaheuristic-1.9.4/pyMetaheuristic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-12-30 18:44:59.000000 pyMetaheuristic-1.9.4/pyMetaheuristic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-12-30 18:44:59.000000 pyMetaheuristic-1.9.4/pyMetaheuristic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-30 18:45:01.000000 pyMetaheuristic-1.9.4/setup.cfg
--rw-rw-rw-   0        0        0      663 2023-12-30 18:39:47.000000 pyMetaheuristic-1.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:42:05.000000 pyMetaheuristic-1.9.5/
+-rw-rw-rw-   0        0        0      671 2022-03-18 23:04:07.000000 pyMetaheuristic-1.9.5/LICENSE
+-rw-rw-rw-   0        0        0    19869 2024-04-16 23:42:05.000000 pyMetaheuristic-1.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0    19358 2023-12-05 21:20:46.000000 pyMetaheuristic-1.9.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 23:42:04.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/
+-rw-rw-rw-   0        0        0        1 2022-03-18 23:04:07.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:42:05.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/
+-rw-rw-rw-   0        0        0     2323 2023-12-04 18:54:02.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     7910 2023-12-03 15:25:03.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/abco.py
+-rw-rw-rw-   0        0        0     7045 2023-12-03 15:23:34.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/acgwo.py
+-rw-rw-rw-   0        0        0     8368 2023-12-03 17:27:26.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/afsa.py
+-rw-rw-rw-   0        0        0     6416 2023-12-03 16:32:11.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/alo.py
+-rw-rw-rw-   0        0        0     4385 2023-12-03 17:27:26.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/aoa.py
+-rw-rw-rw-   0        0        0     6145 2023-12-03 17:30:48.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/ars.py
+-rw-rw-rw-   0        0        0     5468 2023-12-30 18:38:11.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/bat_a.py
+-rw-rw-rw-   0        0        0     5235 2023-12-03 21:42:31.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/bbo.py
+-rw-rw-rw-   0        0        0     4224 2023-12-03 21:42:57.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/ca.py
+-rw-rw-rw-   0        0        0     4866 2023-12-03 22:08:55.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/cat_so.py
+-rw-rw-rw-   0        0        0     4749 2023-12-03 22:21:52.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/cem.py
+-rw-rw-rw-   0        0        0     6767 2023-12-03 22:28:13.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/chicken_so.py
+-rw-rw-rw-   0        0        0     5384 2023-12-03 22:43:28.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/clonalg.py
+-rw-rw-rw-   0        0        0     4114 2023-12-03 22:49:17.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/coati_oa.py
+-rw-rw-rw-   0        0        0     5511 2023-12-03 23:16:01.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/cockroach_so.py
+-rw-rw-rw-   0        0        0     4163 2023-12-03 23:27:10.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/csa.py
+-rw-rw-rw-   0        0        0     5501 2023-12-03 23:42:49.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/cuckoo_s.py
+-rw-rw-rw-   0        0        0     7814 2023-12-03 23:46:43.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/da.py
+-rw-rw-rw-   0        0        0     4228 2023-12-04 13:24:50.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/de.py
+-rw-rw-rw-   0        0        0     4146 2023-12-04 12:59:10.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/dfo.py
+-rw-rw-rw-   0        0        0     6376 2023-12-04 13:16:29.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/dvba.py
+-rw-rw-rw-   0        0        0     4611 2023-12-04 13:24:32.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/eho.py
+-rw-rw-rw-   0        0        0     6679 2023-12-04 13:37:52.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/fda.py
+-rw-rw-rw-   0        0        0     4797 2023-12-04 14:02:18.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/firefly_a.py
+-rw-rw-rw-   0        0        0     5384 2023-12-04 14:19:54.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/fpa.py
+-rw-rw-rw-   0        0        0     6579 2023-12-08 21:50:01.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/ga.py
+-rw-rw-rw-   0        0        0     5936 2023-12-04 17:17:28.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/gmo.py
+-rw-rw-rw-   0        0        0     5472 2024-04-16 23:39:48.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/goa.py
+-rw-rw-rw-   0        0        0     6179 2023-12-04 17:58:44.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/gsa.py
+-rw-rw-rw-   0        0        0     6451 2023-12-04 18:05:33.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/gwo.py
+-rw-rw-rw-   0        0        0     8767 2023-12-04 18:45:58.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/hho.py
+-rw-rw-rw-   0        0        0     4173 2023-12-04 18:50:36.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/hsa.py
+-rw-rw-rw-   0        0        0     5068 2023-12-04 19:26:31.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/hus.py
+-rw-rw-rw-   0        0        0     8175 2023-12-04 18:24:12.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/i_gwo.py
+-rw-rw-rw-   0        0        0     7517 2023-12-08 21:10:56.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/i_woa.py
+-rw-rw-rw-   0        0        0     5820 2023-12-04 19:43:45.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/jso.py
+-rw-rw-rw-   0        0        0     4535 2023-12-07 23:50:47.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/jy.py
+-rw-rw-rw-   0        0        0    11608 2023-12-05 13:08:16.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/kha.py
+-rw-rw-rw-   0        0        0     6074 2023-12-05 16:23:18.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/mbo.py
+-rw-rw-rw-   0        0        0     9263 2023-12-05 16:51:31.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/memetic_a.py
+-rw-rw-rw-   0        0        0     4913 2023-12-05 17:14:24.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/mfa.py
+-rw-rw-rw-   0        0        0     5668 2023-12-05 17:20:30.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/mvo.py
+-rw-rw-rw-   0        0        0     4145 2023-12-05 17:27:47.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/pbil.py
+-rw-rw-rw-   0        0        0     5612 2023-12-05 18:00:16.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/pfa.py
+-rw-rw-rw-   0        0        0     4904 2023-12-05 18:37:34.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/pso.py
+-rw-rw-rw-   0        0        0     3909 2023-12-05 18:49:32.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/random_s.py
+-rw-rw-rw-   0        0        0     4266 2023-12-08 21:15:11.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/sa.py
+-rw-rw-rw-   0        0        0     4067 2023-12-05 19:33:28.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/sine_cosine_a.py
+-rw-rw-rw-   0        0        0     6706 2023-12-05 19:38:31.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/sos.py
+-rw-rw-rw-   0        0        0     7655 2023-12-08 21:07:15.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/spbo.py
+-rw-rw-rw-   0        0        0     4454 2023-12-05 20:21:52.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/ssa.py
+-rw-rw-rw-   0        0        0     5414 2023-12-05 20:32:10.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/tlbo.py
+-rw-rw-rw-   0        0        0     5134 2023-12-08 21:10:24.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/woa.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:42:05.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/test_function/
+-rw-rw-rw-   0        0        0       22 2022-03-18 23:04:07.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/test_function/__init__.py
+-rw-rw-rw-   0        0        0    11703 2022-05-07 19:26:33.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/test_function/single.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:42:05.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/utils/
+-rw-rw-rw-   0        0        0       22 2022-03-18 23:04:07.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/utils/__init__.py
+-rw-rw-rw-   0        0        0     7537 2022-03-18 23:04:07.000000 pyMetaheuristic-1.9.5/pyMetaheuristic/utils/graphs.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:42:04.000000 pyMetaheuristic-1.9.5/pyMetaheuristic.egg-info/
+-rw-rw-rw-   0        0        0    19869 2024-04-16 23:42:03.000000 pyMetaheuristic-1.9.5/pyMetaheuristic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2251 2024-04-16 23:42:04.000000 pyMetaheuristic-1.9.5/pyMetaheuristic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 23:42:03.000000 pyMetaheuristic-1.9.5/pyMetaheuristic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-16 23:42:03.000000 pyMetaheuristic-1.9.5/pyMetaheuristic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-16 23:42:03.000000 pyMetaheuristic-1.9.5/pyMetaheuristic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 23:42:05.000000 pyMetaheuristic-1.9.5/setup.cfg
+-rw-rw-rw-   0        0        0      663 2024-04-16 23:41:07.000000 pyMetaheuristic-1.9.5/setup.py
```

### Comparing `pyMetaheuristic-1.9.4/LICENSE` & `pyMetaheuristic-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/PKG-INFO` & `pyMetaheuristic-1.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyMetaheuristic
-Version: 1.9.4
+Version: 1.9.5
 Summary: pyMetaheuristic: A Comprehensive Python Library for Optimization
 Home-page: https://github.com/Valdecy/pyMetaheuristic
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyMetaheuristic-1.9.4/README.md` & `pyMetaheuristic-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/__init__.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/abco.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/abco.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/acgwo.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/acgwo.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/afsa.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/afsa.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/alo.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/alo.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/aoa.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/aoa.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/ars.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/ars.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/bat_a.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/bat_a.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/bbo.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/bbo.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/ca.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/ca.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/cat_so.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/cat_so.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/cem.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/cem.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/chicken_so.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/chicken_so.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/clonalg.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/clonalg.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/coati_oa.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/coati_oa.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/cockroach_so.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/cockroach_so.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/csa.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/csa.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/cuckoo_s.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/cuckoo_s.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/da.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/da.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/de.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/de.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/dfo.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/dfo.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/dvba.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/dvba.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/eho.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/eho.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/fda.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/fda.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/firefly_a.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/firefly_a.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/fpa.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/fpa.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/ga.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/ga.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/gmo.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/gmo.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/goa.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/goa.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,33 +51,47 @@
    a = position[:,:-1]
    b = a.reshape(np.prod(a.shape[:-1]), 1, a.shape[-1])
    return np.sqrt(np.einsum('ijk,ijk->ij',  b - a,  b - a)).squeeze()
 
 # Function: Update Position
 def update_position(position, best_position, min_values, max_values, C, F, L, target_function):
     dim             = len(min_values)
+    size            = position.shape[0] - 1
     distance_matrix = build_distance_matrix(position)
     distance_matrix = 2 * (distance_matrix - np.min(distance_matrix)) / (np.ptp(distance_matrix) + 1e-8) + 1
     np.fill_diagonal(distance_matrix, 0)
     for j in range(dim):
         sum_grass = np.zeros(position.shape[0])
         for i in range(position.shape[0]):
             s_vals       = s_function(distance_matrix[:, i], F, L)
             denominator  = np.where(distance_matrix[:, i] == 0, 1, distance_matrix[:, i])
             sum_grass[i] = np.sum(C * ((max_values[j] - min_values[j]) / 2) * s_vals * ((position[:, j] - position[i, j]) / denominator))
         position[:, j] = np.clip(C * sum_grass + best_position[j], min_values[j], max_values[j])
-    position[:, -1] = np.apply_along_axis(target_function, 1, position[:, :-1])
+    position[:, -1]     = np.apply_along_axis(target_function, 1, position[:, :-1])
+    unique_rows, counts = np.unique(np.round(position[:, :-1], 4), axis = 0, return_counts = True)
+    max_count           = np.max(counts)
+    if (max_count / position.shape[0] >= 0.8):
+        majority_row   = unique_rows[np.argmax(counts)]
+        different_rows = position[~np.all(np.round(position[:, :-1], 4) == majority_row, axis = 1)]
+        num_new_rows   = position.shape[0] - different_rows.shape[0]
+        new_rows       = initial_variables(num_new_rows, min_values, max_values, target_function)
+        if (different_rows.shape[0] > 0):
+            position = np.vstack((different_rows, new_rows))
+        else:   
+            position = new_rows
+        position = position[:size, :]
+        position = np.vstack((best_position, position))
     return position
 
 ############################################################################
 
 # Function: GOA
 def grasshopper_optimization_algorithm(grasshoppers = 25, min_values = [-5,-5], max_values = [5,5], c_min = 0.00004, c_max = 1, iterations = 1000, F = 0.5, L = 1.5, target_function = target_function, verbose = True, start_init = None, target_value = None):
     position      = initial_variables(grasshoppers, min_values, max_values, target_function, start_init)
-    best_position =  np.copy(position[np.argmin(position[:,-1]),:]) 
+    best_position = np.copy(position[np.argmin(position[:,-1]),:]) 
     count         = 0
     while (count <= iterations): 
         if (verbose == True):
             print('Iteration = ', count,  ' f(x) = ', best_position[-1])
         C        = c_max - count*( (c_max - c_min)/iterations)
         position = update_position(position, best_position, min_values, max_values, C, F, L, target_function)
         if (np.amin(position[:,-1]) < best_position[-1]):
@@ -87,8 +101,8 @@
                 count = 2* iterations
             else:
                 count = count + 1
         else:
             count = count + 1 
     return best_position
 
-############################################################################
+############################################################################
```

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/gsa.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/gsa.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/gwo.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/gwo.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/hho.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/hho.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/hsa.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/hsa.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/hus.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/hus.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/i_gwo.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/i_gwo.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/i_woa.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/i_woa.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/jso.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/jso.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/jy.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/jy.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/kha.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/kha.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/mbo.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/mbo.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/memetic_a.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/memetic_a.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/mfa.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/mfa.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/mvo.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/mvo.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/pbil.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/pbil.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/pfa.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/pfa.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/pso.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/pso.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/random_s.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/random_s.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/sa.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/sa.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/sine_cosine_a.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/sine_cosine_a.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/sos.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/sos.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/spbo.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/spbo.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/ssa.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/ssa.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/tlbo.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/tlbo.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/algorithm/woa.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/algorithm/woa.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/test_function/single.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/test_function/single.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic/utils/graphs.py` & `pyMetaheuristic-1.9.5/pyMetaheuristic/utils/graphs.py`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic.egg-info/PKG-INFO` & `pyMetaheuristic-1.9.5/pyMetaheuristic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyMetaheuristic
-Version: 1.9.4
+Version: 1.9.5
 Summary: pyMetaheuristic: A Comprehensive Python Library for Optimization
 Home-page: https://github.com/Valdecy/pyMetaheuristic
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyMetaheuristic-1.9.4/pyMetaheuristic.egg-info/SOURCES.txt` & `pyMetaheuristic-1.9.5/pyMetaheuristic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyMetaheuristic-1.9.4/setup.py` & `pyMetaheuristic-1.9.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyMetaheuristic',
-    version='1.9.4',
+    version='1.9.5',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyMetaheuristic',
     packages=find_packages(),
     install_requires=[
         'numpy',
```

