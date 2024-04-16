# Comparing `tmp/pins-0.8.4.tar.gz` & `tmp/pins-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pins-0.8.4.tar", last modified: Wed Jan  3 22:19:26 2024, max compression
+gzip compressed data, was "pins-0.8.5.tar", last modified: Tue Apr 16 23:17:09 2024, max compression
```

## Comparing `pins-0.8.4.tar` & `pins-0.8.5.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.993070 pins-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-03 22:19:19.000000 pins-0.8.4/.env.dev
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-01-03 22:19:19.000000 pins-0.8.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-01-03 22:19:19.000000 pins-0.8.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-01-03 22:19:19.000000 pins-0.8.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-01-03 22:19:19.000000 pins-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-03 22:19:19.000000 pins-0.8.4/MAINTAINERS.md
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-03 22:19:19.000000 pins-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-01-03 22:19:19.000000 pins-0.8.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-01-03 22:19:26.993070 pins-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-01-03 22:19:19.000000 pins-0.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-01-03 22:19:19.000000 pins-0.8.4/README.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.977070 pins-0.8.4/binder/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-03 22:19:19.000000 pins-0.8.4/binder/postBuild
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-01-03 22:19:19.000000 pins-0.8.4/binder/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-03 22:19:19.000000 pins-0.8.4/binder/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-03 22:19:19.000000 pins-0.8.4/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.977070 pins-0.8.4/pins/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-03 22:19:19.000000 pins-0.8.4/pins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-03 22:19:19.000000 pins-0.8.4/pins/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    39285 2024-01-03 22:19:19.000000 pins-0.8.4/pins/boards.py
--rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-01-03 22:19:19.000000 pins-0.8.4/pins/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-01-03 22:19:19.000000 pins-0.8.4/pins/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    21110 2024-01-03 22:19:19.000000 pins-0.8.4/pins/constructors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.977070 pins-0.8.4/pins/data/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-01-03 22:19:19.000000 pins-0.8.4/pins/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-01-03 22:19:19.000000 pins-0.8.4/pins/data/mtcars.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-01-03 22:19:19.000000 pins-0.8.4/pins/drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-03 22:19:19.000000 pins-0.8.4/pins/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8503 2024-01-03 22:19:19.000000 pins-0.8.4/pins/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.977070 pins-0.8.4/pins/rsconnect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:19.000000 pins-0.8.4/pins/rsconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13785 2024-01-03 22:19:19.000000 pins-0.8.4/pins/rsconnect/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-01-03 22:19:19.000000 pins-0.8.4/pins/rsconnect/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.977070 pins-0.8.4/pins/rsconnect/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.981070 pins-0.8.4/pins/rsconnect/html/highlight.js-9.15.9/
--rw-r--r--   0 runner    (1001) docker     (127)    31530 2024-01-03 22:19:19.000000 pins-0.8.4/pins/rsconnect/html/highlight.js-9.15.9/highlight.js
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-03 22:19:19.000000 pins-0.8.4/pins/rsconnect/html/highlight.js-9.15.9/qtcreator_light.css
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-01-03 22:19:19.000000 pins-0.8.4/pins/rsconnect/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.981070 pins-0.8.4/pins/rsconnect/html/pagedtable-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-01-03 22:19:19.000000 pins-0.8.4/pins/rsconnect/html/pagedtable-1.1/pagedtable.css
--rw-r--r--   0 runner    (1001) docker     (127)    34769 2024-01-03 22:19:19.000000 pins-0.8.4/pins/rsconnect/html/pagedtable-1.1/pagedtable.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.981070 pins-0.8.4/pins/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.969070 pins-0.8.4/pins/tests/_snapshots/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.981070 pins-0.8.4/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/data.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.981070 pins-0.8.4/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/
--rw-r--r--   0 runner    (1001) docker     (127)    31530 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/highlight.js
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/qtcreator_light.css
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.981070 pins-0.8.4/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.css
--rw-r--r--   0 runner    (1001) docker     (127)    34769 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.js
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/test_rsc_pin.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.985070 pins-0.8.4/pins/tests/example-bundle/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/example-bundle/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/example-bundle/data_frame.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/example-bundle/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/example-bundle/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.985070 pins-0.8.4/pins/tests/pin-board/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pin-board/_pins.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.969070 pins-0.8.4/pins/tests/pin-board/x/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.985070 pins-0.8.4/pins/tests/pin-board/x/20221215T180351Z-c3943/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pin-board/x/20221215T180351Z-c3943/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pin-board/x/20221215T180351Z-c3943/x.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.969070 pins-0.8.4/pins/tests/pin-board/y/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.985070 pins-0.8.4/pins/tests/pin-board/y/20221215T180357Z-9ae7a/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pin-board/y/20221215T180357Z-9ae7a/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pin-board/y/20221215T180357Z-9ae7a/y.rds
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.985070 pins-0.8.4/pins/tests/pin-board/y/20221215T180400Z-b81d5/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pin-board/y/20221215T180400Z-b81d5/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pin-board/y/20221215T180400Z-b81d5/y.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.973070 pins-0.8.4/pins/tests/pins-compat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.973070 pins-0.8.4/pins/tests/pins-compat/df_arrow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.985070 pins-0.8.4/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/df_arrow.arrow
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.973070 pins-0.8.4/pins/tests/pins-compat/df_csv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.985070 pins-0.8.4/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/df_csv.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.985070 pins-0.8.4/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/df_csv.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.973070 pins-0.8.4/pins/tests/pins-compat/df_rds/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.985070 pins-0.8.4/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/df_rds.rds
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.973070 pins-0.8.4/pins/tests/pins-compat/df_unversioned/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.985070 pins-0.8.4/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/df_unversioned.rds
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.973070 pins-0.8.4/pins/tests/pins-old-types/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.973070 pins-0.8.4/pins/tests/pins-old-types/a-table/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.985070 pins-0.8.4/pins/tests/pins-old-types/a-table/v/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pins-old-types/a-table/v/data.csv
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pins-old-types/a-table/v/data.rds
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/pins-old-types/a-table/v/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20389 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/test_boards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/test_compat_old_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/test_constructors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/test_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    14589 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/test_rsconnect_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-01-03 22:19:19.000000 pins-0.8.4/pins/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-01-03 22:19:19.000000 pins-0.8.4/pins/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-01-03 22:19:19.000000 pins-0.8.4/pins/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.989070 pins-0.8.4/pins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-01-03 22:19:26.000000 pins-0.8.4/pins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-01-03 22:19:26.000000 pins-0.8.4/pins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 22:19:26.000000 pins-0.8.4/pins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-01-03 22:19:26.000000 pins-0.8.4/pins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-03 22:19:26.000000 pins-0.8.4/pins.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-03 22:19:19.000000 pins-0.8.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.989070 pins-0.8.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-01-03 22:19:19.000000 pins-0.8.4/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-03 22:19:19.000000 pins-0.8.4/requirements/minimum.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.989070 pins-0.8.4/script/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.989070 pins-0.8.4/script/ci-compat-check/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-03 22:19:19.000000 pins-0.8.4/script/ci-compat-check/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-03 22:19:19.000000 pins-0.8.4/script/ci-compat-check/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-03 22:19:19.000000 pins-0.8.4/script/ci-compat-check/dump_py_pins.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-03 22:19:19.000000 pins-0.8.4/script/ci-compat-check/dump_r_pins.R
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-01-03 22:19:19.000000 pins-0.8.4/script/ci-compat-check/validate_py_to_r.R
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-01-03 22:19:19.000000 pins-0.8.4/script/ci-compat-check/validate_r_to_py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 22:19:26.989070 pins-0.8.4/script/setup-rsconnect/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-03 22:19:19.000000 pins-0.8.4/script/setup-rsconnect/add-users.sh
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-01-03 22:19:19.000000 pins-0.8.4/script/setup-rsconnect/dump_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-01-03 22:19:19.000000 pins-0.8.4/script/setup-rsconnect/rstudio-connect.gcfg
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-03 22:19:19.000000 pins-0.8.4/script/setup-rsconnect/users.txt
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-01-03 22:19:19.000000 pins-0.8.4/script/stage_example_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-01-03 22:19:19.000000 pins-0.8.4/script/stage_r_pins.R
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-03 22:19:19.000000 pins-0.8.4/script/stage_r_pins_old_types.R
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-01-03 22:19:26.993070 pins-0.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.413551 pins-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-16 23:17:04.000000 pins-0.8.5/.env.dev
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-16 23:17:04.000000 pins-0.8.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-16 23:17:04.000000 pins-0.8.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-16 23:17:04.000000 pins-0.8.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-16 23:17:04.000000 pins-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-16 23:17:04.000000 pins-0.8.5/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 23:17:04.000000 pins-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-16 23:17:04.000000 pins-0.8.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-04-16 23:17:09.413551 pins-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-16 23:17:04.000000 pins-0.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-16 23:17:04.000000 pins-0.8.5/README.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.393551 pins-0.8.5/binder/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 23:17:04.000000 pins-0.8.5/binder/postBuild
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-16 23:17:04.000000 pins-0.8.5/binder/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 23:17:04.000000 pins-0.8.5/binder/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-16 23:17:04.000000 pins-0.8.5/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.397551 pins-0.8.5/pins/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-16 23:17:04.000000 pins-0.8.5/pins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-16 23:17:04.000000 pins-0.8.5/pins/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40269 2024-04-16 23:17:04.000000 pins-0.8.5/pins/boards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-04-16 23:17:04.000000 pins-0.8.5/pins/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-16 23:17:04.000000 pins-0.8.5/pins/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21110 2024-04-16 23:17:04.000000 pins-0.8.5/pins/constructors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.397551 pins-0.8.5/pins/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-16 23:17:04.000000 pins-0.8.5/pins/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-16 23:17:04.000000 pins-0.8.5/pins/data/mtcars.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-16 23:17:04.000000 pins-0.8.5/pins/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-16 23:17:04.000000 pins-0.8.5/pins/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8503 2024-04-16 23:17:04.000000 pins-0.8.5/pins/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.397551 pins-0.8.5/pins/rsconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13785 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.397551 pins-0.8.5/pins/rsconnect/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.397551 pins-0.8.5/pins/rsconnect/html/highlight.js-9.15.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    31530 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/html/highlight.js-9.15.9/highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/html/highlight.js-9.15.9/qtcreator_light.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.401551 pins-0.8.5/pins/rsconnect/html/pagedtable-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/html/pagedtable-1.1/pagedtable.css
+-rw-r--r--   0 runner    (1001) docker     (127)    34769 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/html/pagedtable-1.1/pagedtable.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.401551 pins-0.8.5/pins/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.389551 pins-0.8.5/pins/tests/_snapshots/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.401551 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/data.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.401551 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    31530 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/qtcreator_light.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.401551 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.css
+-rw-r--r--   0 runner    (1001) docker     (127)    34769 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.js
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/test_rsc_pin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/example-bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/example-bundle/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/example-bundle/data_frame.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/example-bundle/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/example-bundle/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pin-board/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pin-board/_pins.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.389551 pins-0.8.5/pins/tests/pin-board/x/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pin-board/x/20221215T180351Z-c3943/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pin-board/x/20221215T180351Z-c3943/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pin-board/x/20221215T180351Z-c3943/x.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.389551 pins-0.8.5/pins/tests/pin-board/y/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pin-board/y/20221215T180357Z-9ae7a/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pin-board/y/20221215T180357Z-9ae7a/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pin-board/y/20221215T180357Z-9ae7a/y.rds
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pin-board/y/20221215T180400Z-b81d5/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pin-board/y/20221215T180400Z-b81d5/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pin-board/y/20221215T180400Z-b81d5/y.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.393551 pins-0.8.5/pins/tests/pins-compat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.389551 pins-0.8.5/pins/tests/pins-compat/df_arrow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/df_arrow.arrow
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.393551 pins-0.8.5/pins/tests/pins-compat/df_csv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/df_csv.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/df_csv.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.393551 pins-0.8.5/pins/tests/pins-compat/df_rds/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/df_rds.rds
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.393551 pins-0.8.5/pins/tests/pins-compat/df_unversioned/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/df_unversioned.rds
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.393551 pins-0.8.5/pins/tests/pins-old-types/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.393551 pins-0.8.5/pins/tests/pins-old-types/a-table/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pins-old-types/a-table/v/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-old-types/a-table/v/data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-old-types/a-table/v/data.rds
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-old-types/a-table/v/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21746 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_boards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_compat_old_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14589 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_rsconnect_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-16 23:17:04.000000 pins-0.8.5/pins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-04-16 23:17:04.000000 pins-0.8.5/pins/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.409551 pins-0.8.5/pins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-04-16 23:17:09.000000 pins-0.8.5/pins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-16 23:17:09.000000 pins-0.8.5/pins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 23:17:09.000000 pins-0.8.5/pins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-16 23:17:09.000000 pins-0.8.5/pins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 23:17:09.000000 pins-0.8.5/pins.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-16 23:17:04.000000 pins-0.8.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-04-16 23:17:04.000000 pins-0.8.5/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-16 23:17:04.000000 pins-0.8.5/requirements/minimum.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.409551 pins-0.8.5/script/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.409551 pins-0.8.5/script/ci-compat-check/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-16 23:17:04.000000 pins-0.8.5/script/ci-compat-check/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-16 23:17:04.000000 pins-0.8.5/script/ci-compat-check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-16 23:17:04.000000 pins-0.8.5/script/ci-compat-check/dump_py_pins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-16 23:17:04.000000 pins-0.8.5/script/ci-compat-check/dump_r_pins.R
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-16 23:17:04.000000 pins-0.8.5/script/ci-compat-check/validate_py_to_r.R
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-16 23:17:04.000000 pins-0.8.5/script/ci-compat-check/validate_r_to_py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.409551 pins-0.8.5/script/setup-rsconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 23:17:04.000000 pins-0.8.5/script/setup-rsconnect/add-users.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-16 23:17:04.000000 pins-0.8.5/script/setup-rsconnect/dump_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 23:17:04.000000 pins-0.8.5/script/setup-rsconnect/rstudio-connect.gcfg
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 23:17:04.000000 pins-0.8.5/script/setup-rsconnect/users.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-16 23:17:04.000000 pins-0.8.5/script/stage_example_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-16 23:17:04.000000 pins-0.8.5/script/stage_r_pins.R
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-16 23:17:04.000000 pins-0.8.5/script/stage_r_pins_old_types.R
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-16 23:17:09.413551 pins-0.8.5/setup.cfg
```

### Comparing `pins-0.8.4/.env.dev` & `pins-0.8.5/.env.dev`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/.gitignore` & `pins-0.8.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/CONTRIBUTING.md` & `pins-0.8.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/LICENSE` & `pins-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/Makefile` & `pins-0.8.5/Makefile`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/PKG-INFO` & `pins-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pins
-Version: 0.8.4
+Version: 0.8.5
 Summary: Publish data sets, models, and other python objects, making it easy to share them across projects and with your colleagues.
 Home-page: https://github.com/rstudio/pins-python
 Author: Isabel Zimmerman
 Author-email: isabel.zimmerman@posit.co
 License: MIT
 Project-URL: Documentation, https://rstudio.github.io/pins-python
 Keywords: data,tidyverse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pins Version: 0.8.4 Summary: Publish data sets,
+Metadata-Version: 2.1 Name: pins Version: 0.8.5 Summary: Publish data sets,
 models, and other python objects, making it easy to share them across projects
 and with your colleagues. Home-page: https://github.com/rstudio/pins-python
 Author: Isabel Zimmerman Author-email: isabel.zimmerman@posit.co License: MIT
 Project-URL: Documentation, https://rstudio.github.io/pins-python Keywords:
 data,tidyverse Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
```

### Comparing `pins-0.8.4/README.md` & `pins-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/README.qmd` & `pins-0.8.5/README.qmd`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/binder/requirements.txt` & `pins-0.8.5/binder/requirements.txt`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/boards.py` & `pins-0.8.5/pins/boards.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from io import IOBase
 from pathlib import Path
 from importlib_resources import files
 from datetime import datetime, timedelta
 
 from typing import Sequence, Optional, Mapping
 
-from .versions import VersionRaw, guess_version
+from .versions import VersionRaw, guess_version, version_setup
 from .meta import Meta, MetaRaw, MetaFactory
-from .errors import PinsError
+from .errors import PinsError, PinsVersionError
 from .drivers import load_data, save_data, load_file, default_title
 from .utils import inform, warn_deprecated, ExtendMethodDoc
 from .config import get_allow_rsc_short_name
 from .cache import PinsCache
 
 
 _log = logging.getLogger(__name__)
@@ -86,34 +86,33 @@
 
         Parameters
         ----------
         name:
             Pin name.
 
         """
-        if not self.versioned:
-            raise NotImplementedError(
-                "Cannot show versions for a board type that does not support versioning."
-            )
 
         if not self.pin_exists(name):
             raise PinsError("Cannot check version, since pin %s does not exist" % name)
 
-        versions_raw = self.fs.ls(self.construct_path([self.path_to_pin(name)]))
+        detail = isinstance(self, BoardRsConnect)
+
+        versions_raw = self.fs.ls(
+            self.construct_path([self.path_to_pin(name)]), detail=detail
+        )
 
         # get a list of Version(Raw) objects
         all_versions = []
         for full_path in versions_raw:
             version = self.keep_final_path_component(full_path)
             all_versions.append(guess_version(version))
 
         # sort them, with latest last
         sorted_versions = self.sort_pin_versions(all_versions)
 
-        # TODO(defer): this deviates from R pins, which returns a df by default
         if as_df:
             import pandas as pd
 
             return pd.DataFrame([v.to_dict() for v in sorted_versions])
 
         return sorted_versions
 
@@ -175,15 +174,15 @@
 
         Notes
         -----
         This is a low-level function; use [](`~pins.boards.BaseBoard.pin_search`) to get more data about
         each pin in a convenient form.
         """
 
-        full_paths = self.fs.ls(self.board)
+        full_paths = self.fs.ls(self.board, detail=False)
         pin_names = map(self.keep_final_path_component, full_paths)
 
         return [name for name in pin_names if name not in self.reserved_pin_names]
 
     def pin_fetch(self, name: str, version: Optional[str] = None) -> Meta:
         meta = self.pin_meta(name, version)
 
@@ -235,19 +234,14 @@
         title: Optional[str] = None,
         description: Optional[str] = None,
         metadata: Optional[Mapping] = None,
         versioned: Optional[bool] = None,
         created: Optional[datetime] = None,
     ) -> Meta:
 
-        if not self.versioned:
-            raise NotImplementedError(
-                "Can only write pins with boards that support versioning."
-            )
-
         if type == "feather":
             warn_deprecated(
                 'Writing pin type "feather" is unsupported. Switching type to "arrow".'
                 " This produces the exact same behavior, and also works with R pins."
                 ' Please switch to pin_write using type="arrow".'
             )
             type = "arrow"
@@ -354,19 +348,14 @@
         versioned:
             Whether the pin should be versioned. Defaults to versioning.
         created:
             A date to store in the Meta.created field. This field may be used as
             part of the pin version name.
         """
 
-        if not self.versioned:
-            raise NotImplementedError(
-                "Can only write pins with boards that support versioning."
-            )
-
         if type == "file":
             raise NotImplementedError(
                 ".pin_write() does not support type='file'. "
                 "Use .pin_upload() to save a file as a pin."
             )
 
         return self._pin_store(
@@ -457,18 +446,14 @@
         Parameters
         ----------
         name:
             Pin name.
         version:
             Version identifier.
         """
-        if not self.versioned:
-            raise NotImplementedError(
-                "Can only write pins with boards that support versioning."
-            )
 
         pin_name = self.path_to_pin(name)
 
         pin_version_path = self.construct_path([pin_name, version])
         self.fs.rm(pin_version_path, recursive=True)
 
     def pin_versions_prune(
@@ -610,15 +595,15 @@
     # pin name internal methods -----------------------------------------------
     # these methods are responsible for validating pin names, and converting
     # names to their ultimate path on the file system.
 
     def validate_pin_name(self, name: str) -> None:
         """Raise an error if a pin name is not valid."""
 
-        if "/" in name:
+        if name and "/" in name:
             raise ValueError(f"Invalid pin name: {name}")
         elif name in self.reserved_pin_names:
             raise ValueError(f"The pin name '{name}' is reserved for internal use.")
 
     def path_to_pin(self, name: str) -> str:
         self.validate_pin_name(name)
 
@@ -649,20 +634,48 @@
         title: Optional[str] = None,
         description: Optional[str] = None,
         metadata: Optional[Mapping] = None,
         versioned: Optional[bool] = None,
         created: Optional[datetime] = None,
         object_name: Optional[str] = None,
     ):
+        meta = self._create_meta(
+            pin_dir_path,
+            x,
+            name,
+            type,
+            title,
+            description,
+            metadata,
+            versioned,
+            created,
+            object_name,
+        )
+
+        # handle unversioned boards
+        version_setup(self, name, meta.version, versioned)
+
+        return meta
+
+    def _create_meta(
+        self,
+        pin_dir_path,
+        x,
+        name: Optional[str] = None,
+        type: Optional[str] = None,
+        title: Optional[str] = None,
+        description: Optional[str] = None,
+        metadata: Optional[Mapping] = None,
+        versioned: Optional[bool] = None,
+        created: Optional[datetime] = None,
+        object_name: Optional[str] = None,
+    ):
         if name is None:
             raise NotImplementedError("Name must be specified.")
 
-        if versioned is False:
-            raise NotImplementedError("Only writing versioned pins supported.")
-
         if type is None:
             raise NotImplementedError("Type argument is required.")
 
         if title is None:
             title = default_title(x, name)
 
         # create metadata from object on disk ---------------------------------
@@ -764,23 +777,14 @@
     # TODO(question): is this class worth it? Or should the user just use fsspec?
 
     def __init__(self, *args, pin_paths: dict, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.pin_paths = pin_paths
 
-    # def pin_read(self, *args, **kwargs):
-    #    if not get_feature_preview():
-    #        raise NotImplementedError(
-    #            "pin_read with BoardManual is currently unimplemented. "
-    #            "See https://github.com/machow/pins-python/issues/59."
-    #        )
-
-    #    return super().pin_read(*args, **kwargs)
-
     @ExtendMethodDoc
     def pin_list(self):
         return list(self.pin_paths)
 
     @ExtendMethodDoc
     def pin_versions(self, *args, **kwargs):
         raise NotImplementedError("This board does not support pin_versions.")
@@ -883,15 +887,17 @@
         paged_res = self.fs.api.misc_get_applications("content_type:pin")
         results = paged_res.results
 
         names = [f"{cont['owner_username']}/{cont['name']}" for cont in results]
         return names
 
     @ExtendMethodDoc
-    def pin_write(self, *args, access_type=None, **kwargs):
+    def pin_write(
+        self, *args, access_type=None, versioned: Optional[bool] = None, **kwargs
+    ):
         """Write a pin.
 
         Extends parent method in the following ways:
 
         * Modifies content item to include any title and description changes.
         * Adds access_type argument to specify who can see content. Defaults to "acl".
         """
@@ -909,27 +915,55 @@
             # but should also fix things downstream.
             raise PinsError(
                 f"You are connected as {self.user_name}, but you are trying to create a new piece"
                 f" of content for another user ({pin_name}). They must create the content before you"
                 " can write to it."
             )
 
+        # attempt to make the least number of API calls possible
+        if versioned or versioned is None and self.versioned:
+            # arbitrary number greater than 1
+            n_versions_before = 100
+        else:
+            try:
+                versions_df = self.pin_versions(pin_name, as_df=True)
+                versions = versions_df["version"].to_list()
+                n_versions_before = len(versions)
+            except PinsError:
+                # pin does not exist
+                n_versions_before = 0
+
+        if versioned is None:
+            versioned = True if n_versions_before > 1 else self.versioned
+
+        if versioned is False and n_versions_before > 1:
+            raise PinsVersionError(
+                "Pin is versioned, but you have requested a write without versions."
+                "To un-version a pin, you must delete it"
+            )
+
         # run parent function ---
         meta = f_super(*args, **kwargs)
 
         # update content title to reflect what's in metadata ----
         # TODO(question): R pins updates this info before writing the pin..?
         content = self.fs.info(pin_name)
         self.fs.api.patch_content_item(
             content["guid"],
             title=meta.title,
             description=meta.description or "",
             access_type=access_type or content["access_type"],
         )
 
+        # clean up non-active pins in the case of an unversioned board
+        # a pin existed before the latest pin
+        if versioned is False and n_versions_before == 1:
+            _log.info(f"Replacing version '{versions}' with '{meta.version.version}'")
+            self.pin_version_delete(pin_name, versions[0])
+
         return meta
 
     @ExtendMethodDoc
     def pin_search(self, search=None, as_df=True):
         from pins.rsconnect.api import RsConnectApiRequestError
 
         paged_res = self.fs.api.misc_get_applications("content_type:pin", search=search)
@@ -1061,15 +1095,15 @@
         # RSC pin names can have form <user_name>/<name>, but this will try to
         # create the object in a directory named <user_name>. So we grab just
         # the <name> part.
         short_name = name.split("/")[-1]
 
         # TODO(compat): py pins always uses the short name, R pins uses w/e the
         # user passed, but guessing people want the long name?
-        meta = super().prepare_pin_version(pin_dir_path, x, short_name, *args, **kwargs)
+        meta = super()._create_meta(pin_dir_path, x, short_name, *args, **kwargs)
         meta.name = name
 
         # copy in files needed by index.html ----------------------------------
         crnt_files = set([meta.file] if isinstance(meta.file, str) else meta.file)
         to_add = [str(p) for p in self.html_assets_dir.rglob("*")]
         overlap = set(to_add) & crnt_files
         if overlap:
```

### Comparing `pins-0.8.4/pins/cache.py` & `pins-0.8.5/pins/cache.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/config.py` & `pins-0.8.5/pins/config.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/constructors.py` & `pins-0.8.5/pins/constructors.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/data/mtcars.csv` & `pins-0.8.5/pins/data/mtcars.csv`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/drivers.py` & `pins-0.8.5/pins/drivers.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,14 +117,24 @@
 
         elif meta.type == "file":
             raise NotImplementedError(
                 "Methods like `.pin_read()` are not able to read 'file' type pins."
                 " Use `.pin_download()` to download the file."
             )
 
+        elif meta.type == "rds":
+            try:
+                import rdata
+
+                return rdata.read_rds(f)
+            except ModuleNotFoundError:
+                raise ModuleNotFoundError(
+                    "Install the 'rdata' package to attempt to convert 'rds' files into Python objects."
+                )
+
     raise NotImplementedError(f"No driver for type {meta.type}")
 
 
 def save_data(
     obj, fname, type=None, apply_suffix: bool = True
 ) -> "str | Sequence[str]":
     # TODO: extensible saving with deferred importing
```

### Comparing `pins-0.8.4/pins/meta.py` & `pins-0.8.5/pins/meta.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/rsconnect/api.py` & `pins-0.8.5/pins/rsconnect/api.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/rsconnect/fs.py` & `pins-0.8.5/pins/rsconnect/fs.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/rsconnect/html/highlight.js-9.15.9/highlight.js` & `pins-0.8.5/pins/rsconnect/html/highlight.js-9.15.9/highlight.js`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/rsconnect/html/highlight.js-9.15.9/qtcreator_light.css` & `pins-0.8.5/pins/rsconnect/html/highlight.js-9.15.9/qtcreator_light.css`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/rsconnect/html/index.html` & `pins-0.8.5/pins/rsconnect/html/index.html`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/rsconnect/html/pagedtable-1.1/pagedtable.css` & `pins-0.8.5/pins/rsconnect/html/pagedtable-1.1/pagedtable.css`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/rsconnect/html/pagedtable-1.1/pagedtable.js` & `pins-0.8.5/pins/rsconnect/html/pagedtable-1.1/pagedtable.js`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/highlight.js` & `pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/highlight.js`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/qtcreator_light.css` & `pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/qtcreator_light.css`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/index.html` & `pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/index.html`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.css` & `pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.css`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.js` & `pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.js`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/tests/conftest.py` & `pins-0.8.5/pins/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/tests/helpers.py` & `pins-0.8.5/pins/tests/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         value = os.environ.get(name, default)
 
         if callable(value):
             return value()
 
         return value
 
-    def create_tmp_board(self, src_board=None) -> BaseBoard:
+    def create_tmp_board(self, src_board=None, versioned=True) -> BaseBoard:
         if self.fs_name == "gcs":
             opts = {"cache_timeout": 0}
         else:
             opts = {"use_listings_cache": False}
 
         fs = filesystem(self.fs_name, **opts)
         temp_name = str(uuid.uuid4())
@@ -132,15 +132,15 @@
 
         if src_board is not None:
             fs.put(src_board, board_name, recursive=True)
         else:
             fs.mkdir(board_name)
 
         self.board_path_registry.append(board_name)
-        return BaseBoard(board_name, fs=fs)
+        return BaseBoard(board_name, fs=fs, versioned=versioned)
 
     def teardown_board(self, board):
         board.fs.rm(board.board, recursive=True)
 
     def teardown(self):
         # cleanup all temporary boards
         fs = filesystem(self.fs_name)
@@ -164,18 +164,18 @@
 
     # TODO: could loop back once initializing all boards is clear
 
     def __init__(self, fs_name, path=None, *args, **kwargs):
         self.fs_name = fs_name
         self.path = None
 
-    def create_tmp_board(self, src_board=None):
+    def create_tmp_board(self, src_board=None, versioned=True):
         from pins.rsconnect.fs import PinBundleManifest  # noqa
 
-        board = BoardRsConnect("", rsc_fs_from_key("derek"))
+        board = BoardRsConnect("", rsc_fs_from_key("derek"), versioned=versioned)
 
         if src_board is None:
             return board
 
         # otherwise, try to copy in existing board ---
         # we need to add a manifest to each pin, so copy contents into a tmp dir
         with TemporaryDirectory() as tmp_dir:
```

### Comparing `pins-0.8.4/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/df_arrow.arrow` & `pins-0.8.5/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/df_arrow.arrow`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/tests/test_boards.py` & `pins-0.8.5/pins/tests/test_boards.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import uuid
 import pandas as pd
 import pytest
 
 from pins.tests.helpers import DEFAULT_CREATION_DATE, rm_env
 from pins.config import PINS_ENV_INSECURE_READ
-from pins.errors import PinsError, PinsInsecureReadError
+from pins.errors import PinsError, PinsInsecureReadError, PinsVersionError
 from pins.meta import MetaRaw
 
 from datetime import datetime, timedelta
 from time import sleep
 from pathlib import Path
 
 # using pytest cases, so that we can pass in fixtures as parameters
@@ -28,14 +28,20 @@
 @fixture
 def board(backend):
     yield backend.create_tmp_board()
     backend.teardown()
 
 
 @fixture
+def board_unversioned(backend):
+    yield backend.create_tmp_board(versioned=False)
+    backend.teardown()
+
+
+@fixture
 def board_with_cache(backend):
     from pins.constructors import board as board_constructor, board_rsconnect
 
     board = backend.create_tmp_board()
 
     if backend.fs_name == "rsc":
         # The rsconnect board is special, in that it's slower to set up and tear down,
@@ -300,14 +306,44 @@
     with rm_env(PINS_ENV_INSECURE_READ):
         os.environ[PINS_ENV_INSECURE_READ] = "0"
         board.allow_pickle_read = True
         board.pin_write({"a": 1}, "test_pin", type="joblib", title="some title")
         board.pin_read("test_pin")
 
 
+# pin_write with unversioned boards ===========================================
+
+
+@pytest.mark.parametrize("versioned", [None, False])
+def test_board_unversioned_pin_write_unversioned(versioned, board_unversioned):
+    board_unversioned.pin_write({"a": 1}, "test_pin", type="json", versioned=versioned)
+    board_unversioned.pin_write({"a": 2}, "test_pin", type="json", versioned=versioned)
+
+    assert len(board_unversioned.pin_versions("test_pin")) == 1
+    assert board_unversioned.pin_read("test_pin") == {"a": 2}
+
+
+def test_board_unversioned_pin_write_versioned(board_unversioned):
+    board_unversioned.pin_write({"a": 1}, "test_pin", type="json", versioned=False)
+    board_unversioned.pin_write({"a": 2}, "test_pin", type="json", versioned=True)
+
+    assert len(board_unversioned.pin_versions("test_pin")) == 2
+
+
+def test_board_versioned_pin_write_unversioned(board):
+    # should fall back to the versioned setting of the board
+    board.pin_write({"a": 1}, "test_pin", type="json")
+    board.pin_write({"a": 2}, "test_pin", type="json")
+
+    with pytest.raises(PinsVersionError):
+        board.pin_write({"a": 3}, "test_pin", type="json", versioned=False)
+
+    assert len(board.pin_versions("test_pin")) == 2
+
+
 # pin_delete ==================================================================
 
 
 @pytest.fixture
 def pin_name():
     return str(uuid.uuid4())
```

### Comparing `pins-0.8.4/pins/tests/test_cache.py` & `pins-0.8.5/pins/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/tests/test_compat.py` & `pins-0.8.5/pins/tests/test_compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,17 +149,21 @@
     src_df = board.pin_read("df_csv")
     dst_df = pd.read_csv(p_data)
 
     assert isinstance(src_df, pd.DataFrame)
     assert src_df.equals(dst_df)
 
 
-def test_compat_pin_read_supported(board):
-    with pytest.raises(NotImplementedError):
-        board.pin_read("df_rds")
+def test_compat_pin_read_supported_rds(board):
+    pytest.importorskip("rdata")
+    import pandas as pd
+
+    src_df = board.pin_read("df_rds")
+
+    assert isinstance(src_df, pd.DataFrame)
 
 
 # pin_write ----
 
 # manifest -----
```

### Comparing `pins-0.8.4/pins/tests/test_config.py` & `pins-0.8.5/pins/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/tests/test_constructors.py` & `pins-0.8.5/pins/tests/test_constructors.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/tests/test_drivers.py` & `pins-0.8.5/pins/tests/test_drivers.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/tests/test_meta.py` & `pins-0.8.5/pins/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/tests/test_rsconnect_api.py` & `pins-0.8.5/pins/tests/test_rsconnect_api.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/tests/test_versions.py` & `pins-0.8.5/pins/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/utils.py` & `pins-0.8.5/pins/utils.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/pins/versions.py` & `pins-0.8.5/pins/versions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import logging
+
 from dataclasses import dataclass, asdict
 from datetime import datetime
 from xxhash import xxh64
 
 from typing import Union, Sequence, Mapping
-
 from .errors import PinsVersionError
 from ._types import StrOrFile, IOBase
 
+_log = logging.getLogger(__name__)
+
 VERSION_TIME_FORMAT = "%Y%m%dT%H%M%SZ"
 
 
 class _VersionBase:
     pass
 
 
@@ -112,7 +115,35 @@
 
 
 def guess_version(x: str):
     try:
         return Version.from_string(x)
     except PinsVersionError:
         return VersionRaw(x)
+
+
+def version_setup(board, name, new_version, versioned):
+    if board.pin_exists(name):
+        versions_df = board.pin_versions(name, as_df=True)
+        versions = versions_df["version"].to_list()
+        old_version = versions[-1]
+        n_versions = len(versions)
+
+    else:
+        n_versions = 0
+
+    # if pin does not have version specified, see if multiple pins on board/board's version
+    if versioned is None:
+        versioned = True if n_versions > 1 else board.versioned
+
+    if versioned or n_versions == 0:
+        _log.info(f"Creating new version '{new_version}'")
+    elif n_versions == 1:
+        _log.info(f"Replacing version '{old_version}' with '{new_version}'")
+        board.pin_version_delete(name, old_version)
+    else:
+        raise PinsVersionError(
+            "Pin is versioned, but you have requested a write without versions."
+            "To un-version a pin, you must delete it"
+        )
+
+    return new_version
```

### Comparing `pins-0.8.4/pins.egg-info/PKG-INFO` & `pins-0.8.5/pins.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pins
-Version: 0.8.4
+Version: 0.8.5
 Summary: Publish data sets, models, and other python objects, making it easy to share them across projects and with your colleagues.
 Home-page: https://github.com/rstudio/pins-python
 Author: Isabel Zimmerman
 Author-email: isabel.zimmerman@posit.co
 License: MIT
 Project-URL: Documentation, https://rstudio.github.io/pins-python
 Keywords: data,tidyverse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pins Version: 0.8.4 Summary: Publish data sets,
+Metadata-Version: 2.1 Name: pins Version: 0.8.5 Summary: Publish data sets,
 models, and other python objects, making it easy to share them across projects
 and with your colleagues. Home-page: https://github.com/rstudio/pins-python
 Author: Isabel Zimmerman Author-email: isabel.zimmerman@posit.co License: MIT
 Project-URL: Documentation, https://rstudio.github.io/pins-python Keywords:
 data,tidyverse Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
```

### Comparing `pins-0.8.4/pins.egg-info/SOURCES.txt` & `pins-0.8.5/pins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/requirements/dev.txt` & `pins-0.8.5/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/script/stage_example_bundle.py` & `pins-0.8.5/script/stage_example_bundle.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/script/stage_r_pins.R` & `pins-0.8.5/script/stage_r_pins.R`

 * *Files identical despite different names*

### Comparing `pins-0.8.4/setup.cfg` & `pins-0.8.5/setup.cfg`

 * *Files identical despite different names*

