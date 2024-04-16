# Comparing `tmp/gen3_tracker-0.0.3rc7.tar.gz` & `tmp/gen3_tracker-0.0.3rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_tracker-0.0.3rc7.tar", last modified: Sun Apr 14 02:19:47 2024, max compression
+gzip compressed data, was "gen3_tracker-0.0.3rc8.tar", last modified: Tue Apr 16 23:30:02 2024, max compression
```

## Comparing `gen3_tracker-0.0.3rc7.tar` & `gen3_tracker-0.0.3rc8.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.697534 gen3_tracker-0.0.3rc7/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_tracker-0.0.3rc7/LICENSE
--rw-r--r--   0 walsbr   (320923486) 1971611142     2415 2024-04-14 02:19:47.697146 gen3_tracker-0.0.3rc7/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1338 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc7/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.696661 gen3_tracker-0.0.3rc7/gen3_tracker.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2415 2024-04-14 02:19:47.000000 gen3_tracker-0.0.3rc7/gen3_tracker.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     2904 2024-04-14 02:19:47.000000 gen3_tracker-0.0.3rc7/gen3_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2024-04-14 02:19:47.000000 gen3_tracker-0.0.3rc7/gen3_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       47 2024-04-14 02:19:47.000000 gen3_tracker-0.0.3rc7/gen3_tracker.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      186 2024-04-14 02:19:47.000000 gen3_tracker-0.0.3rc7/gen3_tracker.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       16 2024-04-14 02:19:47.000000 gen3_tracker-0.0.3rc7/gen3_tracker.egg-info/top_level.txt
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.663041 gen3_tracker-0.0.3rc7/gen3_util/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2885 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc7/gen3_util/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.669694 gen3_tracker-0.0.3rc7/gen3_util/access/
--rw-r--r--   0 walsbr   (320923486) 1971611142     3307 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4706 2024-04-13 10:20:22.000000 gen3_tracker-0.0.3rc7/gen3_util/access/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.673147 gen3_tracker-0.0.3rc7/gen3_util/access/policies/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_tracker-0.0.3rc7/gen3_util/access/policies/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      189 2024-02-29 16:26:49.000000 gen3_tracker-0.0.3rc7/gen3_util/access/policies/add-project-default.yaml
--rw-r--r--   0 walsbr   (320923486) 1971611142       77 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc7/gen3_util/access/policies/add-user-delete.yaml
--rw-r--r--   0 walsbr   (320923486) 1971611142       76 2024-02-26 20:40:22.000000 gen3_tracker-0.0.3rc7/gen3_util/access/policies/add-user-read.yaml
--rw-r--r--   0 walsbr   (320923486) 1971611142      199 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc7/gen3_util/access/policies/add-user-write.yaml
--rw-r--r--   0 walsbr   (320923486) 1971611142     6732 2024-04-13 10:20:42.000000 gen3_tracker-0.0.3rc7/gen3_util/access/requestor.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1052 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/access/submitter.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.674836 gen3_tracker-0.0.3rc7/gen3_util/buckets/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1211 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      883 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/buckets/lister.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.677930 gen3_tracker-0.0.3rc7/gen3_util/common/
--rw-r--r--   0 walsbr   (320923486) 1971611142    13758 2024-04-13 10:20:22.000000 gen3_tracker-0.0.3rc7/gen3_util/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.679545 gen3_tracker-0.0.3rc7/gen3_util/config/
--rw-r--r--   0 walsbr   (320923486) 1971611142    10225 2024-04-13 10:20:22.000000 gen3_tracker-0.0.3rc7/gen3_util/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      876 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/config/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      137 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/config.yaml
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.681472 gen3_tracker-0.0.3rc7/gen3_util/files/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1457 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/files/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    12297 2024-04-14 02:18:50.000000 gen3_tracker-0.0.3rc7/gen3_util/files/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3751 2024-03-01 20:19:22.000000 gen3_tracker-0.0.3rc7/gen3_util/files/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    13433 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc7/gen3_util/files/manifest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1503 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc7/gen3_util/files/middleware.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      634 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/files/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5194 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/files/uploader.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.682193 gen3_tracker-0.0.3rc7/gen3_util/jobs/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-10-19 18:01:08.000000 gen3_tracker-0.0.3rc7/gen3_util/jobs/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2618 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/jobs/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/jobs/lister.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.684448 gen3_tracker-0.0.3rc7/gen3_util/meta/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4438 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc7/gen3_util/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1415 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc7/gen3_util/meta/bundler.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     8981 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      687 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/meta/delta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2894 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/meta/differ.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      326 2023-10-19 18:01:08.000000 gen3_tracker-0.0.3rc7/gen3_util/meta/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2204 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/meta/importer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1655 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/meta/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2932 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc7/gen3_util/meta/publisher.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    15266 2024-04-14 02:18:50.000000 gen3_tracker-0.0.3rc7/gen3_util/meta/skeleton.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.684650 gen3_tracker-0.0.3rc7/gen3_util/meta/tabular/
--rw-r--r--   0 walsbr   (320923486) 1971611142    11706 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc7/gen3_util/meta/tabular/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4660 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/meta/uploader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4477 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc7/gen3_util/meta/validator.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.685432 gen3_tracker-0.0.3rc7/gen3_util/projects/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2778 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3696 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc7/gen3_util/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2341 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1496 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc7/gen3_util/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.687288 gen3_tracker-0.0.3rc7/gen3_util/repo/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4557 2024-04-11 18:50:38.000000 gen3_tracker-0.0.3rc7/gen3_util/repo/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    17870 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc7/gen3_util/repo/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3726 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/repo/cloner.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     9643 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc7/gen3_util/repo/committer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/repo/history.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1427 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc7/gen3_util/repo/initializer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3629 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc7/gen3_util/repo/puller.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4405 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc7/gen3_util/repo/pusher.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2959 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/gen3_util/repo/status.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.687643 gen3_tracker-0.0.3rc7/gen3_util/users/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-10-19 18:09:26.000000 gen3_tracker-0.0.3rc7/gen3_util/users/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1761 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc7/gen3_util/users/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2024-04-14 02:19:47.697600 gen3_tracker-0.0.3rc7/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5581 2024-04-14 02:17:55.000000 gen3_tracker-0.0.3rc7/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.645746 gen3_tracker-0.0.3rc7/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.690564 gen3_tracker-0.0.3rc7/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_tracker-0.0.3rc7/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1091 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1066 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/integration/test_access.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      454 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/integration/test_buckets.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    12460 2024-04-13 10:20:22.000000 gen3_tracker-0.0.3rc7/tests/integration/test_commit.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      257 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/integration/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4867 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc7/tests/integration/test_foreign_bucket.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2182 2024-04-13 10:20:22.000000 gen3_tracker-0.0.3rc7/tests/integration/test_init.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     9506 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/integration/test_meta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     8848 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/integration/test_meta_skeleton.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5763 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc7/tests/integration/test_no_bucket.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1321 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc7/tests/integration/test_project.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.693752 gen3_tracker-0.0.3rc7/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_tracker-0.0.3rc7/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      464 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/unit/conftest.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.693965 gen3_tracker-0.0.3rc7/tests/unit/plugins/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:45:48.000000 gen3_tracker-0.0.3rc7/tests/unit/plugins/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.694280 gen3_tracker-0.0.3rc7/tests/unit/plugins/gen3_util_plugin_foo/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1450 2023-07-07 00:45:48.000000 gen3_tracker-0.0.3rc7/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-14 02:19:47.696392 gen3_tracker-0.0.3rc7/tests/unit/tabular/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/unit/tabular/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    16696 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc7/tests/unit/tabular/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1172 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/unit/tabular/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     7826 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc7/tests/unit/tabular/test_default_columns.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1035 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/unit/tabular/test_dir_to_tabular.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1888 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/unit/tabular/test_from_tabular.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3779 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc7/tests/unit/tabular/test_to_tabular.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      737 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/unit/tabular/test_validate.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3841 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc7/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4881 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc7/tests/unit/test_coding.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_tracker-0.0.3rc7/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      532 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/unit/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1417 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/unit/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      445 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc7/tests/unit/test_job_dependencies.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      734 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/unit/test_manifest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/unit/test_validate_directory.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      625 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc7/tests/unit/test_version.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.472102 gen3_tracker-0.0.3rc8/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_tracker-0.0.3rc8/LICENSE
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2415 2024-04-16 23:30:02.471618 gen3_tracker-0.0.3rc8/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1338 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc8/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.470992 gen3_tracker-0.0.3rc8/gen3_tracker.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2415 2024-04-16 23:30:02.000000 gen3_tracker-0.0.3rc8/gen3_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2904 2024-04-16 23:30:02.000000 gen3_tracker-0.0.3rc8/gen3_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2024-04-16 23:30:02.000000 gen3_tracker-0.0.3rc8/gen3_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       47 2024-04-16 23:30:02.000000 gen3_tracker-0.0.3rc8/gen3_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      186 2024-04-16 23:30:02.000000 gen3_tracker-0.0.3rc8/gen3_tracker.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       16 2024-04-16 23:30:02.000000 gen3_tracker-0.0.3rc8/gen3_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.407915 gen3_tracker-0.0.3rc8/gen3_util/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2885 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc8/gen3_util/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.439551 gen3_tracker-0.0.3rc8/gen3_util/access/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3307 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4974 2024-04-16 23:28:35.000000 gen3_tracker-0.0.3rc8/gen3_util/access/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.441460 gen3_tracker-0.0.3rc8/gen3_util/access/policies/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_tracker-0.0.3rc8/gen3_util/access/policies/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      189 2024-02-29 16:26:49.000000 gen3_tracker-0.0.3rc8/gen3_util/access/policies/add-project-default.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142       77 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc8/gen3_util/access/policies/add-user-delete.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142       76 2024-02-26 20:40:22.000000 gen3_tracker-0.0.3rc8/gen3_util/access/policies/add-user-read.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142      199 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc8/gen3_util/access/policies/add-user-write.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6732 2024-04-13 10:20:42.000000 gen3_tracker-0.0.3rc8/gen3_util/access/requestor.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1052 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/access/submitter.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.442749 gen3_tracker-0.0.3rc8/gen3_util/buckets/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1211 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      883 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/buckets/lister.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.443133 gen3_tracker-0.0.3rc8/gen3_util/common/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13758 2024-04-13 10:20:22.000000 gen3_tracker-0.0.3rc8/gen3_util/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.444027 gen3_tracker-0.0.3rc8/gen3_util/config/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    10225 2024-04-13 10:20:22.000000 gen3_tracker-0.0.3rc8/gen3_util/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      876 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/config/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      137 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/config.yaml
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.447804 gen3_tracker-0.0.3rc8/gen3_util/files/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1457 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/files/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    12297 2024-04-16 23:15:38.000000 gen3_tracker-0.0.3rc8/gen3_util/files/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3751 2024-03-01 20:19:22.000000 gen3_tracker-0.0.3rc8/gen3_util/files/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13433 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc8/gen3_util/files/manifest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1503 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc8/gen3_util/files/middleware.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      634 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/files/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5194 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/files/uploader.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.448762 gen3_tracker-0.0.3rc8/gen3_util/jobs/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-10-19 18:01:08.000000 gen3_tracker-0.0.3rc8/gen3_util/jobs/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2618 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/jobs/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/jobs/lister.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.452781 gen3_tracker-0.0.3rc8/gen3_util/meta/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4438 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc8/gen3_util/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1415 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc8/gen3_util/meta/bundler.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     8981 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      687 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/meta/delta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2894 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/meta/differ.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      326 2023-10-19 18:01:08.000000 gen3_tracker-0.0.3rc8/gen3_util/meta/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2204 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/meta/importer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1655 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/meta/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2932 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc8/gen3_util/meta/publisher.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    15444 2024-04-16 23:23:47.000000 gen3_tracker-0.0.3rc8/gen3_util/meta/skeleton.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.453205 gen3_tracker-0.0.3rc8/gen3_util/meta/tabular/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    11706 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc8/gen3_util/meta/tabular/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4660 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/meta/uploader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4477 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc8/gen3_util/meta/validator.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.454636 gen3_tracker-0.0.3rc8/gen3_util/projects/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2778 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3696 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc8/gen3_util/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2341 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1496 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc8/gen3_util/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.458022 gen3_tracker-0.0.3rc8/gen3_util/repo/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4557 2024-04-11 18:50:38.000000 gen3_tracker-0.0.3rc8/gen3_util/repo/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    17870 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc8/gen3_util/repo/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3726 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/repo/cloner.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     9643 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc8/gen3_util/repo/committer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/repo/history.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1427 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc8/gen3_util/repo/initializer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3629 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc8/gen3_util/repo/puller.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4405 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc8/gen3_util/repo/pusher.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2959 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/gen3_util/repo/status.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.458577 gen3_tracker-0.0.3rc8/gen3_util/users/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-10-19 18:09:26.000000 gen3_tracker-0.0.3rc8/gen3_util/users/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1761 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc8/gen3_util/users/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2024-04-16 23:30:02.472185 gen3_tracker-0.0.3rc8/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5581 2024-04-16 23:29:38.000000 gen3_tracker-0.0.3rc8/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.400196 gen3_tracker-0.0.3rc8/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.462871 gen3_tracker-0.0.3rc8/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_tracker-0.0.3rc8/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1091 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1066 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/integration/test_access.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      454 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/integration/test_buckets.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    12460 2024-04-13 10:20:22.000000 gen3_tracker-0.0.3rc8/tests/integration/test_commit.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      257 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/integration/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4867 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc8/tests/integration/test_foreign_bucket.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2182 2024-04-13 10:20:22.000000 gen3_tracker-0.0.3rc8/tests/integration/test_init.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     9506 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/integration/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     8848 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/integration/test_meta_skeleton.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5763 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc8/tests/integration/test_no_bucket.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1321 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc8/tests/integration/test_project.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.467242 gen3_tracker-0.0.3rc8/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_tracker-0.0.3rc8/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      464 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/unit/conftest.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.467691 gen3_tracker-0.0.3rc8/tests/unit/plugins/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:45:48.000000 gen3_tracker-0.0.3rc8/tests/unit/plugins/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.467977 gen3_tracker-0.0.3rc8/tests/unit/plugins/gen3_util_plugin_foo/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1450 2023-07-07 00:45:48.000000 gen3_tracker-0.0.3rc8/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-16 23:30:02.470656 gen3_tracker-0.0.3rc8/tests/unit/tabular/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/unit/tabular/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    16696 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc8/tests/unit/tabular/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1172 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/unit/tabular/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     7826 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc8/tests/unit/tabular/test_default_columns.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1035 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/unit/tabular/test_dir_to_tabular.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1888 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/unit/tabular/test_from_tabular.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3779 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc8/tests/unit/tabular/test_to_tabular.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      737 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/unit/tabular/test_validate.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3841 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc8/tests/unit/test_cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4881 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc8/tests/unit/test_coding.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_tracker-0.0.3rc8/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      532 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/unit/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1417 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/unit/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      445 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc8/tests/unit/test_job_dependencies.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      734 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/unit/test_manifest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/unit/test_validate_directory.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      625 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc8/tests/unit/test_version.py
```

### Comparing `gen3_tracker-0.0.3rc7/LICENSE` & `gen3_tracker-0.0.3rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/PKG-INFO` & `gen3_tracker-0.0.3rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_tracker
-Version: 0.0.3rc7
+Version: 0.0.3rc8
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gen3_tracker-0.0.3rc7/README.md` & `gen3_tracker-0.0.3rc8/README.md`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_tracker.egg-info/PKG-INFO` & `gen3_tracker-0.0.3rc8/gen3_tracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3-tracker
-Version: 0.0.3rc7
+Version: 0.0.3rc8
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gen3_tracker-0.0.3rc7/gen3_tracker.egg-info/SOURCES.txt` & `gen3_tracker-0.0.3rc8/gen3_tracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/__init__.py` & `gen3_tracker-0.0.3rc8/gen3_util/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/access/__init__.py` & `gen3_tracker-0.0.3rc8/gen3_util/access/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/access/cli.py` & `gen3_tracker-0.0.3rc8/gen3_util/access/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,23 +69,28 @@
             output.update(LogAccess(**{
                 'msg': "No unsigned requests found"
             }))
         else:
             msg = f"Signing {len(unsigned_requests)} requests."
 
             signed_requests = []
+            problem_requests = []
             click.secho("signing requests...", fg='green')
             for request in unsigned_requests:
                 if request_id and request['request_id'] != request_id:
                     continue
-                signed_requests.append(
-                    update(config, request_id=request['request_id'], status='SIGNED', auth=auth).request
-                )
+                try:
+                    signed_requests.append(
+                        update(config, request_id=request['request_id'], status='SIGNED', auth=auth).request
+                    )
+                except Exception as e:
+                    print(f"Error signing request {request}: {e}")
+                    problem_requests.append(request)
 
-            msg = f"Signed {len(unsigned_requests)} requests.  System administrators will create new projects."
+            msg = f"Signed {len(signed_requests)} requests. There were {len(problem_requests)} problems. System administrators will create new projects."
 
             output.update(LogAccess(**{
                 'msg': msg,
                 'requests': signed_requests,
             }))
```

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/access/requestor.py` & `gen3_tracker-0.0.3rc8/gen3_util/access/requestor.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/access/submitter.py` & `gen3_tracker-0.0.3rc8/gen3_util/access/submitter.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/buckets/__init__.py` & `gen3_tracker-0.0.3rc8/gen3_util/buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/buckets/cli.py` & `gen3_tracker-0.0.3rc8/gen3_util/buckets/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/buckets/lister.py` & `gen3_tracker-0.0.3rc8/gen3_util/buckets/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/common/__init__.py` & `gen3_tracker-0.0.3rc8/gen3_util/common/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/config/__init__.py` & `gen3_tracker-0.0.3rc8/gen3_util/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/config/cli.py` & `gen3_tracker-0.0.3rc8/gen3_util/config/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/files/__init__.py` & `gen3_tracker-0.0.3rc8/gen3_util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/files/cli.py` & `gen3_tracker-0.0.3rc8/gen3_util/files/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/files/lister.py` & `gen3_tracker-0.0.3rc8/gen3_util/files/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/files/manifest.py` & `gen3_tracker-0.0.3rc8/gen3_util/files/manifest.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/files/middleware.py` & `gen3_tracker-0.0.3rc8/gen3_util/files/middleware.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/files/remover.py` & `gen3_tracker-0.0.3rc8/gen3_util/files/remover.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/files/uploader.py` & `gen3_tracker-0.0.3rc8/gen3_util/files/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/jobs/cli.py` & `gen3_tracker-0.0.3rc8/gen3_util/jobs/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/jobs/lister.py` & `gen3_tracker-0.0.3rc8/gen3_util/jobs/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/meta/__init__.py` & `gen3_tracker-0.0.3rc8/gen3_util/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/meta/bundler.py` & `gen3_tracker-0.0.3rc8/gen3_util/meta/bundler.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/meta/cli.py` & `gen3_tracker-0.0.3rc8/gen3_util/meta/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/meta/delta.py` & `gen3_tracker-0.0.3rc8/gen3_util/meta/delta.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/meta/differ.py` & `gen3_tracker-0.0.3rc8/gen3_util/meta/differ.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/meta/importer.py` & `gen3_tracker-0.0.3rc8/gen3_util/meta/importer.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/meta/lister.py` & `gen3_tracker-0.0.3rc8/gen3_util/meta/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/meta/publisher.py` & `gen3_tracker-0.0.3rc8/gen3_util/meta/publisher.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/meta/skeleton.py` & `gen3_tracker-0.0.3rc8/gen3_util/meta/skeleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,21 @@
     """Update document reference with index record."""
     assert document_reference.resource_type == 'DocumentReference'
     assert 'did' in index_record, f"index_record missing did: {index_record}"
     assert index_record['did'] == document_reference.id, f"{index_record['did']} != {document_reference.id}"
     assert 'created_date' in index_record, f"index_record missing created_date: {index_record}"
     document_reference.docStatus = 'final'
     document_reference.status = 'current'
-    if 'T' not in index_record['created_date']:
-        document_reference.date = index_record['created_date'] + "Z"
-    else:
-        document_reference.date = index_record['created_date']
+
+    assert 'T' in index_record['created_date'], f"created_date must be in ISO8601 format: {index_record['created_date']}"
+    time_part = index_record['created_date'].split('T')[-1]
+    if not ('-' in time_part or '+' in time_part):
+        index_record['created_date'] = index_record['created_date'] + "Z"
+    document_reference.date = index_record['created_date']
+
     attachment = Attachment()
     attachment.extension = [
         {
             "url": "http://aced-idp.org/fhir/StructureDefinition/md5",
             "valueString": index_record['hashes']['md5']
         },
         {
```

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/meta/tabular/__init__.py` & `gen3_tracker-0.0.3rc8/gen3_util/meta/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/meta/uploader.py` & `gen3_tracker-0.0.3rc8/gen3_util/meta/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/meta/validator.py` & `gen3_tracker-0.0.3rc8/gen3_util/meta/validator.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/projects/__init__.py` & `gen3_tracker-0.0.3rc8/gen3_util/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/projects/cli.py` & `gen3_tracker-0.0.3rc8/gen3_util/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/projects/lister.py` & `gen3_tracker-0.0.3rc8/gen3_util/projects/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/projects/remover.py` & `gen3_tracker-0.0.3rc8/gen3_util/projects/remover.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/repo/__init__.py` & `gen3_tracker-0.0.3rc8/gen3_util/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/repo/cli.py` & `gen3_tracker-0.0.3rc8/gen3_util/repo/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/repo/cloner.py` & `gen3_tracker-0.0.3rc8/gen3_util/repo/cloner.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/repo/committer.py` & `gen3_tracker-0.0.3rc8/gen3_util/repo/committer.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/repo/initializer.py` & `gen3_tracker-0.0.3rc8/gen3_util/repo/initializer.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/repo/puller.py` & `gen3_tracker-0.0.3rc8/gen3_util/repo/puller.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/repo/pusher.py` & `gen3_tracker-0.0.3rc8/gen3_util/repo/pusher.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/repo/status.py` & `gen3_tracker-0.0.3rc8/gen3_util/repo/status.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/gen3_util/users/cli.py` & `gen3_tracker-0.0.3rc8/gen3_util/users/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/setup.py` & `gen3_tracker-0.0.3rc8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='gen3_tracker',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.3rc7',  # Required
+    version='0.0.3rc8',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Commons utilities',
     # Optional
```

### Comparing `gen3_tracker-0.0.3rc7/tests/integration/conftest.py` & `gen3_tracker-0.0.3rc8/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/integration/test_access.py` & `gen3_tracker-0.0.3rc8/tests/integration/test_access.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/integration/test_commit.py` & `gen3_tracker-0.0.3rc8/tests/integration/test_commit.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/integration/test_foreign_bucket.py` & `gen3_tracker-0.0.3rc8/tests/integration/test_foreign_bucket.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/integration/test_init.py` & `gen3_tracker-0.0.3rc8/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/integration/test_meta.py` & `gen3_tracker-0.0.3rc8/tests/integration/test_meta.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/integration/test_meta_skeleton.py` & `gen3_tracker-0.0.3rc8/tests/integration/test_meta_skeleton.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/integration/test_no_bucket.py` & `gen3_tracker-0.0.3rc8/tests/integration/test_no_bucket.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/integration/test_project.py` & `gen3_tracker-0.0.3rc8/tests/integration/test_project.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/plugins/gen3_util_plugin_foo/__init__.py` & `gen3_tracker-0.0.3rc8/tests/unit/plugins/gen3_util_plugin_foo/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/tabular/conftest.py` & `gen3_tracker-0.0.3rc8/tests/unit/tabular/conftest.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/tabular/test_config.py` & `gen3_tracker-0.0.3rc8/tests/unit/tabular/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/tabular/test_default_columns.py` & `gen3_tracker-0.0.3rc8/tests/unit/tabular/test_default_columns.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/tabular/test_dir_to_tabular.py` & `gen3_tracker-0.0.3rc8/tests/unit/tabular/test_dir_to_tabular.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/tabular/test_from_tabular.py` & `gen3_tracker-0.0.3rc8/tests/unit/tabular/test_from_tabular.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/tabular/test_to_tabular.py` & `gen3_tracker-0.0.3rc8/tests/unit/tabular/test_to_tabular.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/tabular/test_validate.py` & `gen3_tracker-0.0.3rc8/tests/unit/tabular/test_validate.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/test_cli.py` & `gen3_tracker-0.0.3rc8/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/test_coding.py` & `gen3_tracker-0.0.3rc8/tests/unit/test_coding.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/test_coding_conventions.py` & `gen3_tracker-0.0.3rc8/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/test_config.py` & `gen3_tracker-0.0.3rc8/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/test_files.py` & `gen3_tracker-0.0.3rc8/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/test_manifest.py` & `gen3_tracker-0.0.3rc8/tests/unit/test_manifest.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/test_validate_directory.py` & `gen3_tracker-0.0.3rc8/tests/unit/test_validate_directory.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc7/tests/unit/test_version.py` & `gen3_tracker-0.0.3rc8/tests/unit/test_version.py`

 * *Files identical despite different names*

