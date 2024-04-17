# Comparing `tmp/pyiron_base-0.8.1.tar.gz` & `tmp/pyiron_base-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_base-0.8.1.tar", last modified: Sat Apr 13 15:37:28 2024, max compression
+gzip compressed data, was "pyiron_base-0.8.2.tar", last modified: Wed Apr 17 17:00:59 2024, max compression
```

## Comparing `pyiron_base-0.8.1.tar` & `pyiron_base-0.8.2.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.735357 pyiron_base-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-13 15:37:28.735357 pyiron_base-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.715357 pyiron_base-0.8.1/pyiron_base/
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-13 15:37:28.735357 pyiron_base-0.8.1/pyiron_base/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.719357 pyiron_base-0.8.1/pyiron_base/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/cli/control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/cli/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/cli/reloadfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/cli/rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/cli/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.719357 pyiron_base-0.8.1/pyiron_base/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24876 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/database/filetable.py
--rw-r--r--   0 runner    (1001) docker     (127)    36818 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/database/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/database/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/database/jobtable.py
--rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/database/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/database/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/database/sqlcolumnlength.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/database/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.719357 pyiron_base-0.8.1/pyiron_base/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/interfaces/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/interfaces/has_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/interfaces/has_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/interfaces/has_hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11046 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/interfaces/lockable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/interfaces/object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/interfaces/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.719357 pyiron_base-0.8.1/pyiron_base/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29296 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/datamining.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.723357 pyiron_base-0.8.1/pyiron_base/jobs/flex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/flex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/flex/executablecontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/flex/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/flex/pythonfunctioncontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.723357 pyiron_base-0.8.1/pyiron_base/jobs/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38915 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.723357 pyiron_base-0.8.1/pyiron_base/jobs/job/extension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10855 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/extension/executable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/extension/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/extension/jobstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.723357 pyiron_base-0.8.1/pyiron_base/jobs/job/extension/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/extension/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22428 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/extension/server/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/extension/server/queuestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/extension/server/runmode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    61015 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/jobtype.py
--rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    29036 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/runfunction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)    19542 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/job/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.727357 pyiron_base-0.8.1/pyiron_base/jobs/master/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/master/flexible.py
--rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/master/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/master/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/master/list.py
--rw-r--r--   0 runner    (1001) docker     (127)    32984 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/master/submissionstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/script.py
--rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/jobs/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.727357 pyiron_base-0.8.1/pyiron_base/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.727357 pyiron_base-0.8.1/pyiron_base/project/archiving/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/archiving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/archiving/export_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/archiving/import_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/archiving/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/condaenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/external.py
--rw-r--r--   0 runner    (1001) docker     (127)    74335 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9360 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/jobloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/size.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.727357 pyiron_base-0.8.1/pyiron_base/project/update/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/project/update/pyiron_base_03x_to_04x.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.731357 pyiron_base-0.8.1/pyiron_base/state/
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/state/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/state/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/state/publications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/state/queue_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    25130 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/state/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/state/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/state/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.731357 pyiron_base-0.8.1/pyiron_base/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34122 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/storage/datacontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/storage/filedata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/storage/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)    43407 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/storage/flattenedstorage.py
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/storage/has_stored_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    49006 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/storage/hdfio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/storage/hdfstub.py
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/storage/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/storage/inputlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    33000 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/storage/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.735357 pyiron_base-0.8.1/pyiron_base/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/utils/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/utils/jedi.py
--rw-r--r--   0 runner    (1001) docker     (127)    29090 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/utils/safetar.py
--rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/pyiron_base/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.735357 pyiron_base-0.8.1/pyiron_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-13 15:37:28.000000 pyiron_base-0.8.1/pyiron_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-13 15:37:28.000000 pyiron_base-0.8.1/pyiron_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:37:28.000000 pyiron_base-0.8.1/pyiron_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-13 15:37:28.000000 pyiron_base-0.8.1/pyiron_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-13 15:37:28.000000 pyiron_base-0.8.1/pyiron_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 15:37:28.000000 pyiron_base-0.8.1/pyiron_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-13 15:37:26.000000 pyiron_base-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:37:28.735357 pyiron_base-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:37:28.735357 pyiron_base-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/tests/test_testwithproject.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-13 15:36:38.000000 pyiron_base-0.8.1/tests/test_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.565263 pyiron_base-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-04-17 17:00:59.565263 pyiron_base-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.545263 pyiron_base-0.8.2/pyiron_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-17 17:00:59.565263 pyiron_base-0.8.2/pyiron_base/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.549263 pyiron_base-0.8.2/pyiron_base/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/reloadfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.549263 pyiron_base-0.8.2/pyiron_base/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24876 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/filetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36818 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/jobtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/sqlcolumnlength.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.549263 pyiron_base-0.8.2/pyiron_base/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/has_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/has_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/has_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11046 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/lockable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.549263 pyiron_base-0.8.2/pyiron_base/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29296 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.553263 pyiron_base-0.8.2/pyiron_base/jobs/flex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/flex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/flex/executablecontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/flex/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/flex/pythonfunctioncontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.553263 pyiron_base-0.8.2/pyiron_base/jobs/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39577 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.553263 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10855 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/jobstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.553263 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22428 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/queuestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/runmode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61239 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/jobtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29036 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/runfunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19730 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.557263 pyiron_base-0.8.2/pyiron_base/jobs/master/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/master/flexible.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/master/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/master/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/master/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32984 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/master/submissionstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.557263 pyiron_base-0.8.2/pyiron_base/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.557263 pyiron_base-0.8.2/pyiron_base/project/archiving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/archiving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/archiving/export_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/archiving/import_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/archiving/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/condaenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74335 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9360 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/jobloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/size.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.557263 pyiron_base-0.8.2/pyiron_base/project/update/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/update/pyiron_base_03x_to_04x.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.561263 pyiron_base-0.8.2/pyiron_base/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/publications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/queue_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25130 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.561263 pyiron_base-0.8.2/pyiron_base/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34122 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/datacontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/filedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43875 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/flattenedstorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/has_stored_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49006 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/hdfio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/hdfstub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/inputlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33000 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.561263 pyiron_base-0.8.2/pyiron_base/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/jedi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29090 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/safetar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.565263 pyiron_base-0.8.2/pyiron_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-04-17 17:00:59.000000 pyiron_base-0.8.2/pyiron_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-17 17:00:59.000000 pyiron_base-0.8.2/pyiron_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 17:00:59.000000 pyiron_base-0.8.2/pyiron_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 17:00:59.000000 pyiron_base-0.8.2/pyiron_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-17 17:00:59.000000 pyiron_base-0.8.2/pyiron_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 17:00:59.000000 pyiron_base-0.8.2/pyiron_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-17 17:00:57.000000 pyiron_base-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 17:00:59.565263 pyiron_base-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.561263 pyiron_base-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/tests/test_testwithproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/tests/test_toolkit.py
```

### Comparing `pyiron_base-0.8.1/LICENSE` & `pyiron_base-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/PKG-INFO` & `pyiron_base-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_base
-Version: 0.8.1
+Version: 0.8.2
 Summary: Core components of the pyiron integrated development environment (IDE) for computational materials science
 Author-email: "Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department" <pyiron@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
         All rights reserved.
         
@@ -42,21 +42,21 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
+Requires-Python: <3.13,>=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: cloudpickle<=3.0.0,>=2.0.0
 Requires-Dist: gitpython<=3.1.43,>=3.1.23
-Requires-Dist: h5io_browser<=0.0.11,>=0.0.6
-Requires-Dist: h5py<=3.10.0,>=3.6.0
+Requires-Dist: h5io_browser<=0.0.12,>=0.0.6
+Requires-Dist: h5py<=3.11.0,>=3.6.0
 Requires-Dist: jinja2<=3.1.3,>=2.11.3
 Requires-Dist: numpy<=1.26.4,>=1.23.5
 Requires-Dist: monty<=2024.3.31,>=2021.3.3
 Requires-Dist: pandas<=2.2.2,>=2.0.0
 Requires-Dist: pint<=0.23,>=0.18
 Requires-Dist: psutil<=5.9.8,>=5.8.0
 Requires-Dist: pyfileindex<=0.0.24,>=0.0.16
```

### Comparing `pyiron_base-0.8.1/README.rst` & `pyiron_base-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/__init__.py` & `pyiron_base-0.8.2/pyiron_base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/_tests.py` & `pyiron_base-0.8.2/pyiron_base/_tests.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/cli/control.py` & `pyiron_base-0.8.2/pyiron_base/cli/control.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/cli/install.py` & `pyiron_base-0.8.2/pyiron_base/cli/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/cli/ls.py` & `pyiron_base-0.8.2/pyiron_base/cli/ls.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/cli/reloadfile.py` & `pyiron_base-0.8.2/pyiron_base/cli/reloadfile.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/cli/rm.py` & `pyiron_base-0.8.2/pyiron_base/cli/rm.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/cli/wrapper.py` & `pyiron_base-0.8.2/pyiron_base/cli/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/database/filetable.py` & `pyiron_base-0.8.2/pyiron_base/database/filetable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/database/generic.py` & `pyiron_base-0.8.2/pyiron_base/database/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/database/interface.py` & `pyiron_base-0.8.2/pyiron_base/database/interface.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/database/jobtable.py` & `pyiron_base-0.8.2/pyiron_base/database/jobtable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/database/manager.py` & `pyiron_base-0.8.2/pyiron_base/database/manager.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/database/performance.py` & `pyiron_base-0.8.2/pyiron_base/database/performance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/database/tables.py` & `pyiron_base-0.8.2/pyiron_base/database/tables.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/interfaces/factory.py` & `pyiron_base-0.8.2/pyiron_base/interfaces/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/interfaces/has_dict.py` & `pyiron_base-0.8.2/pyiron_base/interfaces/has_dict.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/interfaces/has_groups.py` & `pyiron_base-0.8.2/pyiron_base/interfaces/has_groups.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/interfaces/has_hdf.py` & `pyiron_base-0.8.2/pyiron_base/interfaces/has_hdf.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/interfaces/lockable.py` & `pyiron_base-0.8.2/pyiron_base/interfaces/lockable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/interfaces/object.py` & `pyiron_base-0.8.2/pyiron_base/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/interfaces/singleton.py` & `pyiron_base-0.8.2/pyiron_base/interfaces/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/datamining.py` & `pyiron_base-0.8.2/pyiron_base/jobs/datamining.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/dynamic.py` & `pyiron_base-0.8.2/pyiron_base/jobs/dynamic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/flex/executablecontainer.py` & `pyiron_base-0.8.2/pyiron_base/jobs/flex/executablecontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/flex/factory.py` & `pyiron_base-0.8.2/pyiron_base/jobs/flex/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/flex/pythonfunctioncontainer.py` & `pyiron_base-0.8.2/pyiron_base/jobs/flex/pythonfunctioncontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/core.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -205,14 +205,16 @@
         self._job_id = None
         self._parent_id = None
         self._master_id = None
         self._status = None
         self._import_directory = None
         self._database_property = DatabaseProperties()
         self._hdf5_content = HDF5Content(project_hdf5=self._hdf5)
+        self._files_to_remove = list()
+        self._files_to_compress = list()
 
     @property
     def content(self):
         return self._hdf5_content
 
     @property
     def files(self):
@@ -381,14 +383,22 @@
         Set the ProjectHDFio instance which points to the HDF5 file the job is stored in
 
         Args:
             project (ProjectHDFio): HDF5 project
         """
         self._hdf5 = project.copy()
 
+    @property
+    def files_to_compress(self):
+        return self._files_to_compress
+
+    @property
+    def files_to_remove(self):
+        return self._files_to_remove
+
     def relocate_hdf5(self, h5_path=None):
         """
         Relocate the hdf file. This function is needed when the child job is
         spawned by a parent job (cf. pyiron_base.jobs.master.generic)
         """
         if h5_path is None:
             h5_path = "/" + self.job_name
@@ -1057,22 +1067,30 @@
         Returns:
             list: list of nodes without childs
         """
         nodes = self.list_nodes()
         childs = self.list_childs()
         return list(set(childs) - set(nodes))
 
-    def compress(self, files_to_compress=None):
+    def compress(self, files_to_compress=None, files_to_remove=None):
         """
         Compress the output files of a job object.
 
         Args:
             files_to_compress (list):
         """
-        _job_compress(job=self, files_to_compress=files_to_compress)
+        if files_to_compress is None and len(self._files_to_compress) != 0:
+            files_to_compress = self._files_to_compress
+        elif files_to_compress is None:
+            files_to_compress = self.files.list()
+        if files_to_remove is None:
+            files_to_remove = self._files_to_remove
+        else:
+            files_to_remove = []
+        _job_compress(job=self, files_to_compress=files_to_compress, files_to_remove=files_to_remove)
 
     def decompress(self):
         """
         Decompress the output files of a compressed job object.
         """
         _job_decompress(job=self)
```

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/extension/executable.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/extension/executable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/extension/files.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/extension/files.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/extension/jobstatus.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/extension/jobstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/extension/server/generic.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/extension/server/queuestatus.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/queuestatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/extension/server/runmode.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/runmode.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/factory.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/generic.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1065,14 +1065,18 @@
         self._executable_activate_mpi()
         if self._executable is not None:
             data_dict["executable"] = self._executable.to_dict()
         if self._import_directory is not None:
             data_dict["import_directory"] = self._import_directory
         if self._executor_type is not None:
             data_dict["executor_type"] = self._executor_type
+        if len(self._files_to_compress) > 0:
+            data_dict["files_to_compress"] = self._files_to_compress
+        if len(self._files_to_remove) > 0:
+            data_dict["files_to_compress"] = self._files_to_remove
         return data_dict
 
     def from_dict(self, job_dict):
         self._type_from_dict(type_dict=job_dict)
         if "import_directory" in job_dict.keys():
             self._import_directory = job_dict["import_directory"]
         self._server.from_dict(server_dict=job_dict["server"])
```

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/interactive.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/jobtype.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/jobtype.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/path.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/runfunction.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/runfunction.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/template.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/template.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/toolkit.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/util.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,39 +271,45 @@
 def _get_compressed_job_name(working_directory):
     """Return the canonical file name of a compressed job from the working directory."""
     return os.path.join(
         working_directory, os.path.basename(working_directory) + ".tar.bz2"
     )
 
 
-def _job_compress(job, files_to_compress=None):
+def _job_compress(job, files_to_compress=[], files_to_remove=[]):
     """
     Compress the output files of a job object.
 
     Args:
         job (JobCore): job object to compress
         files_to_compress (list): list of files to compress
+        files_to_remove (list): list of files to remove
     """
+
+    def delete_file_or_folder(fullname):
+        if os.path.isfile(fullname):
+            os.remove(fullname)
+        elif os.path.isdir(fullname):
+            shutil.rmtree(fullname)
+
     if not _job_is_compressed(job):
-        if files_to_compress is None:
-            files_to_compress = job.files.list()
+        for name in files_to_remove:
+            delete_file_or_folder(fullname=os.path.join(job.working_directory, name))
         cwd = os.getcwd()
         try:
             os.chdir(job.working_directory)
             with tarfile.open(_job_compressed_name(job), "w:bz2") as tar:
                 for name in files_to_compress:
                     if "tar" not in name and not stat.S_ISFIFO(os.stat(name).st_mode):
                         tar.add(name)
             for name in files_to_compress:
-                if "tar" not in name:
-                    fullname = os.path.join(job.working_directory, name)
-                    if os.path.isfile(fullname):
-                        os.remove(fullname)
-                    elif os.path.isdir(fullname):
-                        shutil.rmtree(fullname)
+                if name != _job_compressed_name(job):
+                    delete_file_or_folder(
+                        fullname=os.path.join(job.working_directory, name)
+                    )
         finally:
             os.chdir(cwd)
     else:
         job.logger.info("The files are already compressed!")
 
 
 def _job_decompress(job):
```

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/job/wrapper.py` & `pyiron_base-0.8.2/pyiron_base/jobs/job/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/master/flexible.py` & `pyiron_base-0.8.2/pyiron_base/jobs/master/flexible.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/master/generic.py` & `pyiron_base-0.8.2/pyiron_base/jobs/master/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/master/interactivewrapper.py` & `pyiron_base-0.8.2/pyiron_base/jobs/master/interactivewrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/master/list.py` & `pyiron_base-0.8.2/pyiron_base/jobs/master/list.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/master/parallel.py` & `pyiron_base-0.8.2/pyiron_base/jobs/master/parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/master/submissionstatus.py` & `pyiron_base-0.8.2/pyiron_base/jobs/master/submissionstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/script.py` & `pyiron_base-0.8.2/pyiron_base/jobs/script.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/jobs/worker.py` & `pyiron_base-0.8.2/pyiron_base/jobs/worker.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/project/archiving/export_archive.py` & `pyiron_base-0.8.2/pyiron_base/project/archiving/export_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/project/archiving/import_archive.py` & `pyiron_base-0.8.2/pyiron_base/project/archiving/import_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/project/condaenv.py` & `pyiron_base-0.8.2/pyiron_base/project/condaenv.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/project/data.py` & `pyiron_base-0.8.2/pyiron_base/project/data.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/project/external.py` & `pyiron_base-0.8.2/pyiron_base/project/external.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/project/generic.py` & `pyiron_base-0.8.2/pyiron_base/project/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/project/gui.py` & `pyiron_base-0.8.2/pyiron_base/project/gui.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/project/jobloader.py` & `pyiron_base-0.8.2/pyiron_base/project/jobloader.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/project/maintenance.py` & `pyiron_base-0.8.2/pyiron_base/project/maintenance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/project/path.py` & `pyiron_base-0.8.2/pyiron_base/project/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/project/size.py` & `pyiron_base-0.8.2/pyiron_base/project/size.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/project/update/pyiron_base_03x_to_04x.py` & `pyiron_base-0.8.2/pyiron_base/project/update/pyiron_base_03x_to_04x.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/state/__init__.py` & `pyiron_base-0.8.2/pyiron_base/state/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/state/install.py` & `pyiron_base-0.8.2/pyiron_base/state/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/state/logger.py` & `pyiron_base-0.8.2/pyiron_base/state/logger.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/state/publications.py` & `pyiron_base-0.8.2/pyiron_base/state/publications.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/state/queue_adapter.py` & `pyiron_base-0.8.2/pyiron_base/state/queue_adapter.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/state/settings.py` & `pyiron_base-0.8.2/pyiron_base/state/settings.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/state/signal.py` & `pyiron_base-0.8.2/pyiron_base/state/signal.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/state/update.py` & `pyiron_base-0.8.2/pyiron_base/state/update.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/storage/datacontainer.py` & `pyiron_base-0.8.2/pyiron_base/storage/datacontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/storage/filedata.py` & `pyiron_base-0.8.2/pyiron_base/storage/filedata.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/storage/fileio.py` & `pyiron_base-0.8.2/pyiron_base/storage/fileio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/storage/flattenedstorage.py` & `pyiron_base-0.8.2/pyiron_base/storage/flattenedstorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,25 +25,30 @@
 import numpy as np
 import h5py
 import pandas as pd
 from pyiron_base.interfaces.has_hdf import HasHDF
 from pyiron_base.interfaces.lockable import Lockable, sentinel
 
 
+_CHARSIZE = np.dtype("U1").itemsize
+
+
 def _ensure_str_array_size(array, strlen):
     """
     Ensures that the given array can store at least string of length `strlen`.
 
     Args:
         array (ndarray): array of dtype <U
-        strlen (int): maximum length that should fit in it
+        strlen (int, ndarray): maximum length that should fit in it
     Returns:
         ndarray: either `array` or resized copy
     """
-    current_length = array.itemsize // np.dtype("1U").itemsize
+    current_length = array.itemsize // _CHARSIZE
+    if isinstance(strlen, np.ndarray):
+        strlen = strlen.itemsize // _CHARSIZE
     if current_length < strlen:
         return array.astype(f"{2 * strlen}U")
     else:
         return array
 
 
 class FlattenedStorage(Lockable, HasHDF):
@@ -934,24 +939,32 @@
                     a + self._per_chunk_arrays[k][last] + len_last
                 )  # no += to prevent inplace mutation
             if k not in self._per_chunk_arrays.keys():
                 dtype, fill = get_dtype_and_fill(storage=other, name=k)
                 self.add_array(
                     name=k, dtype=dtype, shape=a.shape[1:], fill=fill, per="chunk"
                 )
+            elif a.dtype.char == "U":
+                self._per_chunk_arrays[k] = _ensure_str_array_size(
+                    self._per_chunk_arrays[k], a
+                )
             self._per_chunk_arrays[k][self.num_chunks : combined_num_chunks] = a[
                 0 : other.num_chunks
             ]
 
         for k, a in other._per_element_arrays.items():
             if k not in self._per_element_arrays.keys():
                 dtype, fill = get_dtype_and_fill(storage=other, name=k)
                 self.add_array(
                     name=k, shape=a.shape[1:], dtype=dtype, fill=fill, per="element"
                 )
+            elif a.dtype.char == "U":
+                self._per_element_arrays[k] = _ensure_str_array_size(
+                    self._per_element_arrays[k], a
+                )
             self._per_element_arrays[k][self.num_elements : combined_num_elements] = a[
                 0 : other.num_elements
             ]
         self.num_elements = combined_num_elements
         self.num_chunks = combined_num_chunks
         self.current_chunk_index = self.num_chunks
         self.current_element_index = self.num_elements
```

### Comparing `pyiron_base-0.8.1/pyiron_base/storage/has_stored_traits.py` & `pyiron_base-0.8.2/pyiron_base/storage/has_stored_traits.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/storage/hdfio.py` & `pyiron_base-0.8.2/pyiron_base/storage/hdfio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/storage/hdfstub.py` & `pyiron_base-0.8.2/pyiron_base/storage/hdfstub.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/storage/helper_functions.py` & `pyiron_base-0.8.2/pyiron_base/storage/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/storage/parameters.py` & `pyiron_base-0.8.2/pyiron_base/storage/parameters.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/utils/deprecate.py` & `pyiron_base-0.8.2/pyiron_base/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/utils/error.py` & `pyiron_base-0.8.2/pyiron_base/utils/error.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/utils/instance.py` & `pyiron_base-0.8.2/pyiron_base/utils/instance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/utils/jedi.py` & `pyiron_base-0.8.2/pyiron_base/utils/jedi.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/utils/parser.py` & `pyiron_base-0.8.2/pyiron_base/utils/parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/utils/safetar.py` & `pyiron_base-0.8.2/pyiron_base/utils/safetar.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base/utils/units.py` & `pyiron_base-0.8.2/pyiron_base/utils/units.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyiron_base.egg-info/PKG-INFO` & `pyiron_base-0.8.2/pyiron_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_base
-Version: 0.8.1
+Version: 0.8.2
 Summary: Core components of the pyiron integrated development environment (IDE) for computational materials science
 Author-email: "Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department" <pyiron@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
         All rights reserved.
         
@@ -42,21 +42,21 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
+Requires-Python: <3.13,>=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: cloudpickle<=3.0.0,>=2.0.0
 Requires-Dist: gitpython<=3.1.43,>=3.1.23
-Requires-Dist: h5io_browser<=0.0.11,>=0.0.6
-Requires-Dist: h5py<=3.10.0,>=3.6.0
+Requires-Dist: h5io_browser<=0.0.12,>=0.0.6
+Requires-Dist: h5py<=3.11.0,>=3.6.0
 Requires-Dist: jinja2<=3.1.3,>=2.11.3
 Requires-Dist: numpy<=1.26.4,>=1.23.5
 Requires-Dist: monty<=2024.3.31,>=2021.3.3
 Requires-Dist: pandas<=2.2.2,>=2.0.0
 Requires-Dist: pint<=0.23,>=0.18
 Requires-Dist: psutil<=5.9.8,>=5.8.0
 Requires-Dist: pyfileindex<=0.0.24,>=0.0.16
```

### Comparing `pyiron_base-0.8.1/pyiron_base.egg-info/SOURCES.txt` & `pyiron_base-0.8.2/pyiron_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/pyproject.toml` & `pyiron_base-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 description = "Core components of the pyiron integrated development environment (IDE) for computational materials science"
 authors = [
     { name = "Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department", email = "pyiron@mpie.de" },
 ]
 readme = "README.rst"
 license = { file = "LICENSE" }
 keywords = ["pyiron"]
-requires-python = ">=3.8"
+requires-python = ">=3.9, <3.13"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Scientific/Engineering :: Physics",
     "License :: OSI Approved :: BSD License",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "cloudpickle>=2.0.0,<=3.0.0",
     "gitpython>=3.1.23,<=3.1.43",
-    "h5io_browser>=0.0.6,<=0.0.11",
-    "h5py>=3.6.0,<=3.10.0",
+    "h5io_browser>=0.0.6,<=0.0.12",
+    "h5py>=3.6.0,<=3.11.0",
     "jinja2>=2.11.3,<=3.1.3",
     "numpy>=1.23.5,<=1.26.4",
     "monty>=2021.3.3,<=2024.3.31",
     "pandas>=2.0.0,<=2.2.2",
     "pint>=0.18,<=0.23",
     "psutil>=5.8.0,<=5.9.8",
     "pyfileindex>=0.0.16,<=0.0.24",
```

### Comparing `pyiron_base-0.8.1/tests/test_testwithproject.py` & `pyiron_base-0.8.2/tests/test_testwithproject.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.1/tests/test_toolkit.py` & `pyiron_base-0.8.2/tests/test_toolkit.py`

 * *Files identical despite different names*

