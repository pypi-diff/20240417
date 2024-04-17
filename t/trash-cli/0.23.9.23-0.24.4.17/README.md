# Comparing `tmp/trash-cli-0.23.9.23.tar.gz` & `tmp/trash_cli-0.24.4.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trash-cli-0.23.9.23.tar", last modified: Sat Sep 23 12:47:29 2023, max compression
+gzip compressed data, was "trash_cli-0.24.4.17.tar", last modified: Wed Apr 17 19:18:15 2024, max compression
```

## Comparing `trash-cli-0.23.9.23.tar` & `trash_cli-0.24.4.17.tar`

### file list

```diff
@@ -1,192 +1,207 @@
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.743089 trash-cli-0.23.9.23/
--rw-r--r--   0 andrea     (501) staff       (20)    17992 2022-08-24 18:45:23.000000 trash-cli-0.23.9.23/COPYING
--rw-r--r--   0 andrea     (501) staff       (20)     7870 2023-09-23 12:47:29.743014 trash-cli-0.23.9.23/PKG-INFO
--rw-r--r--   0 andrea     (501) staff       (20)     7349 2023-04-18 09:13:51.000000 trash-cli-0.23.9.23/README.rst
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.656365 trash-cli-0.23.9.23/man/
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.668069 trash-cli-0.23.9.23/man/man1/
--rw-r--r--   0 andrea     (501) staff       (20)     2754 2022-08-24 18:45:23.000000 trash-cli-0.23.9.23/man/man1/trash-empty.1
--rw-r--r--   0 andrea     (501) staff       (20)     2386 2022-08-24 18:45:23.000000 trash-cli-0.23.9.23/man/man1/trash-list.1
--rw-r--r--   0 andrea     (501) staff       (20)     3270 2023-09-22 20:55:46.000000 trash-cli-0.23.9.23/man/man1/trash-put.1
--rw-r--r--   0 andrea     (501) staff       (20)     2399 2022-08-24 18:45:23.000000 trash-cli-0.23.9.23/man/man1/trash-restore.1
--rw-r--r--   0 andrea     (501) staff       (20)     1433 2022-08-24 18:45:23.000000 trash-cli-0.23.9.23/man/man1/trash-rm.1
--rw-r--r--   0 andrea     (501) staff       (20)     3270 2023-09-22 20:55:46.000000 trash-cli-0.23.9.23/man/man1/trash.1
--rw-r--r--   0 andrea     (501) staff       (20)       90 2022-10-04 20:03:09.000000 trash-cli-0.23.9.23/pyproject.toml
--rw-r--r--   0 andrea     (501) staff       (20)      996 2023-09-23 12:47:29.743527 trash-cli-0.23.9.23/setup.cfg
--rw-r--r--   0 andrea     (501) staff       (20)       99 2023-05-04 13:06:54.000000 trash-cli-0.23.9.23/setup.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.684809 trash-cli-0.23.9.23/tests/
--rw-r--r--   0 andrea     (501) staff       (20)     1428 2022-10-17 17:10:38.000000 trash-cli-0.23.9.23/tests/test_bump.py
--rw-r--r--   0 andrea     (501) staff       (20)     1774 2022-11-25 12:59:58.000000 trash-cli-0.23.9.23/tests/test_candidate_shrink_user.py
--rw-r--r--   0 andrea     (501) staff       (20)     1363 2022-08-24 18:45:23.000000 trash-cli-0.23.9.23/tests/test_fake_file_system.py
--rw-r--r--   0 andrea     (501) staff       (20)      728 2023-06-02 18:54:48.000000 trash-cli-0.23.9.23/tests/test_fake_fstab.py
--rw-r--r--   0 andrea     (501) staff       (20)     1255 2023-05-04 12:51:43.000000 trash-cli-0.23.9.23/tests/test_fake_ismount.py
--rw-r--r--   0 andrea     (501) staff       (20)     1780 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/tests/test_filesystem.py
--rw-r--r--   0 andrea     (501) staff       (20)     1126 2023-05-04 12:51:31.000000 trash-cli-0.23.9.23/tests/test_generate_scripts.py
--rw-r--r--   0 andrea     (501) staff       (20)      426 2022-08-24 18:45:23.000000 trash-cli-0.23.9.23/tests/test_joining_paths.py
--rw-r--r--   0 andrea     (501) staff       (20)     1662 2022-10-02 19:53:24.000000 trash-cli-0.23.9.23/tests/test_list_all_trashinfo_contents.py
--rw-r--r--   0 andrea     (501) staff       (20)     2056 2022-10-02 19:53:24.000000 trash-cli-0.23.9.23/tests/test_make_script.py
--rw-r--r--   0 andrea     (501) staff       (20)      893 2022-09-22 13:29:20.000000 trash-cli-0.23.9.23/tests/test_mock_dir_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)      355 2022-10-17 17:10:38.000000 trash-cli-0.23.9.23/tests/test_my_mock.py
--rw-r--r--   0 andrea     (501) staff       (20)     3760 2023-05-04 12:51:31.000000 trash-cli-0.23.9.23/tests/test_parsing_trashinfo_contents.py
--rw-r--r--   0 andrea     (501) staff       (20)      958 2023-06-02 18:54:48.000000 trash-cli-0.23.9.23/tests/test_partitions.py
--rw-r--r--   0 andrea     (501) staff       (20)     2645 2022-11-24 10:56:43.000000 trash-cli-0.23.9.23/tests/test_top_trash_dir_rules.py
--rw-r--r--   0 andrea     (501) staff       (20)      663 2023-05-01 16:33:41.000000 trash-cli-0.23.9.23/tests/test_trash_dir_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)      662 2022-11-03 21:54:36.000000 trash-cli-0.23.9.23/tests/test_trash_put_reporter.py
--rw-r--r--   0 andrea     (501) staff       (20)      665 2023-06-02 18:54:48.000000 trash-cli-0.23.9.23/tests/test_volume_of.py
--rwxr-xr-x   0 andrea     (501) staff       (20)      132 2023-09-23 12:47:02.000000 trash-cli-0.23.9.23/trash
--rwxr-xr-x   0 andrea     (501) staff       (20)      134 2023-09-23 12:47:02.000000 trash-cli-0.23.9.23/trash-empty
--rwxr-xr-x   0 andrea     (501) staff       (20)      133 2023-09-23 12:47:02.000000 trash-cli-0.23.9.23/trash-list
--rwxr-xr-x   0 andrea     (501) staff       (20)      132 2023-09-23 12:47:02.000000 trash-cli-0.23.9.23/trash-put
--rwxr-xr-x   0 andrea     (501) staff       (20)      136 2023-09-23 12:47:02.000000 trash-cli-0.23.9.23/trash-restore
--rwxr-xr-x   0 andrea     (501) staff       (20)      131 2023-09-23 12:47:02.000000 trash-cli-0.23.9.23/trash-rm
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.687331 trash-cli-0.23.9.23/trash_cli.egg-info/
--rw-r--r--   0 andrea     (501) staff       (20)     7870 2023-09-23 12:47:29.000000 trash-cli-0.23.9.23/trash_cli.egg-info/PKG-INFO
--rw-r--r--   0 andrea     (501) staff       (20)     5095 2023-09-23 12:47:29.000000 trash-cli-0.23.9.23/trash_cli.egg-info/SOURCES.txt
--rw-r--r--   0 andrea     (501) staff       (20)        1 2023-09-23 12:47:29.000000 trash-cli-0.23.9.23/trash_cli.egg-info/dependency_links.txt
--rw-r--r--   0 andrea     (501) staff       (20)       83 2023-09-23 12:47:29.000000 trash-cli-0.23.9.23/trash_cli.egg-info/requires.txt
--rw-r--r--   0 andrea     (501) staff       (20)        9 2023-09-23 12:47:29.000000 trash-cli-0.23.9.23/trash_cli.egg-info/top_level.txt
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.690276 trash-cli-0.23.9.23/trashcli/
--rw-r--r--   0 andrea     (501) staff       (20)       87 2022-10-02 19:52:17.000000 trash-cli-0.23.9.23/trashcli/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      223 2023-06-10 12:52:55.000000 trash-cli-0.23.9.23/trashcli/compat.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.698679 trash-cli-0.23.9.23/trashcli/empty/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2022-09-09 17:05:55.000000 trash-cli-0.23.9.23/trashcli/empty/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      642 2023-05-04 12:51:30.000000 trash-cli-0.23.9.23/trashcli/empty/clock.py
--rw-r--r--   0 andrea     (501) staff       (20)      655 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/empty/console.py
--rw-r--r--   0 andrea     (501) staff       (20)      952 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/empty/delete_according_date.py
--rw-r--r--   0 andrea     (501) staff       (20)      307 2022-09-06 20:19:17.000000 trash-cli-0.23.9.23/trashcli/empty/description.py
--rw-r--r--   0 andrea     (501) staff       (20)     2328 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/empty/emptier.py
--rw-r--r--   0 andrea     (501) staff       (20)     2959 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/empty/empty_action.py
--rw-r--r--   0 andrea     (501) staff       (20)     3298 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/empty/empty_cmd.py
--rw-r--r--   0 andrea     (501) staff       (20)      306 2022-09-16 20:46:37.000000 trash-cli-0.23.9.23/trashcli/empty/errors.py
--rw-r--r--   0 andrea     (501) staff       (20)      143 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/empty/existing_file_remover.py
--rw-r--r--   0 andrea     (501) staff       (20)      270 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/empty/file_system_dir_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)     1477 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/empty/guard.py
--rw-r--r--   0 andrea     (501) staff       (20)       64 2022-09-06 20:19:17.000000 trash-cli-0.23.9.23/trashcli/empty/is_input_interactive.py
--rw-r--r--   0 andrea     (501) staff       (20)     1361 2023-06-06 17:07:29.000000 trash-cli-0.23.9.23/trashcli/empty/main.py
--rw-r--r--   0 andrea     (501) staff       (20)      179 2022-09-06 20:19:17.000000 trash-cli-0.23.9.23/trashcli/empty/older_than.py
--rw-r--r--   0 andrea     (501) staff       (20)       61 2022-09-06 20:19:17.000000 trash-cli-0.23.9.23/trashcli/empty/parse_reply.py
--rw-r--r--   0 andrea     (501) staff       (20)     3509 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/empty/parser.py
--rw-r--r--   0 andrea     (501) staff       (20)      512 2022-09-13 17:23:47.000000 trash-cli-0.23.9.23/trashcli/empty/prepare_output_message.py
--rw-r--r--   0 andrea     (501) staff       (20)      589 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/empty/print_time_action.py
--rw-r--r--   0 andrea     (501) staff       (20)      257 2023-06-04 21:12:19.000000 trash-cli-0.23.9.23/trashcli/empty/top_trash_dir_rules_file_system_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)      494 2023-06-02 18:54:48.000000 trash-cli-0.23.9.23/trashcli/empty/user.py
--rw-r--r--   0 andrea     (501) staff       (20)      514 2023-06-05 17:05:16.000000 trash-cli-0.23.9.23/trashcli/file_system_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)     6321 2023-06-06 17:07:29.000000 trash-cli-0.23.9.23/trashcli/fs.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.701011 trash-cli-0.23.9.23/trashcli/fstab/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-05-04 12:51:43.000000 trash-cli-0.23.9.23/trashcli/fstab/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)     1797 2023-06-02 18:54:48.000000 trash-cli-0.23.9.23/trashcli/fstab/mount_points_listing.py
--rw-r--r--   0 andrea     (501) staff       (20)     1171 2023-06-02 18:54:48.000000 trash-cli-0.23.9.23/trashcli/fstab/volume_listing.py
--rw-r--r--   0 andrea     (501) staff       (20)      818 2023-06-02 18:54:48.000000 trash-cli-0.23.9.23/trashcli/fstab/volume_of.py
--rw-r--r--   0 andrea     (501) staff       (20)     1673 2023-06-02 18:54:48.000000 trash-cli-0.23.9.23/trashcli/fstab/volumes.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.704263 trash-cli-0.23.9.23/trashcli/lib/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2022-10-17 17:10:38.000000 trash-cli-0.23.9.23/trashcli/lib/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      145 2023-05-04 12:51:31.000000 trash-cli-0.23.9.23/trashcli/lib/dir_checker.py
--rw-r--r--   0 andrea     (501) staff       (20)      328 2023-06-06 17:07:29.000000 trash-cli-0.23.9.23/trashcli/lib/dir_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)      279 2023-05-04 12:51:31.000000 trash-cli-0.23.9.23/trashcli/lib/exit_codes.py
--rw-r--r--   0 andrea     (501) staff       (20)      207 2023-05-04 12:51:31.000000 trash-cli-0.23.9.23/trashcli/lib/logger.py
--rw-r--r--   0 andrea     (501) staff       (20)     1038 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/lib/my_input.py
--rw-r--r--   0 andrea     (501) staff       (20)      227 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/lib/my_permission_error.py
--rw-r--r--   0 andrea     (501) staff       (20)      281 2023-05-04 12:51:31.000000 trash-cli-0.23.9.23/trashcli/lib/path_of_backup_copy.py
--rw-r--r--   0 andrea     (501) staff       (20)      766 2023-06-05 12:04:25.000000 trash-cli-0.23.9.23/trashcli/lib/print_version.py
--rw-r--r--   0 andrea     (501) staff       (20)      919 2023-05-01 16:33:41.000000 trash-cli-0.23.9.23/trashcli/lib/trash_dir_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)      926 2023-06-02 18:54:48.000000 trash-cli-0.23.9.23/trashcli/lib/trash_dirs.py
--rw-r--r--   0 andrea     (501) staff       (20)      860 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/lib/user_info.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.707341 trash-cli-0.23.9.23/trashcli/list/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-04-27 14:26:42.000000 trash-cli-0.23.9.23/trashcli/list/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      691 2023-05-04 12:51:31.000000 trash-cli-0.23.9.23/trashcli/list/extractors.py
--rw-r--r--   0 andrea     (501) staff       (20)      336 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/list/fs.py
--rw-r--r--   0 andrea     (501) staff       (20)     5777 2023-06-05 17:05:16.000000 trash-cli-0.23.9.23/trashcli/list/list_trash_action.py
--rw-r--r--   0 andrea     (501) staff       (20)     3765 2023-06-05 12:01:41.000000 trash-cli-0.23.9.23/trashcli/list/main.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.708573 trash-cli-0.23.9.23/trashcli/list/minor_actions/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-05-01 16:33:40.000000 trash-cli-0.23.9.23/trashcli/list/minor_actions/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      636 2023-05-04 12:51:43.000000 trash-cli-0.23.9.23/trashcli/list/minor_actions/debug_volumes.py
--rw-r--r--   0 andrea     (501) staff       (20)     1344 2023-05-04 12:51:43.000000 trash-cli-0.23.9.23/trashcli/list/minor_actions/list_trash_dirs.py
--rw-r--r--   0 andrea     (501) staff       (20)      376 2023-05-04 12:51:43.000000 trash-cli-0.23.9.23/trashcli/list/minor_actions/list_volumes.py
--rw-r--r--   0 andrea     (501) staff       (20)      230 2023-05-04 12:51:43.000000 trash-cli-0.23.9.23/trashcli/list/minor_actions/print_python_executable.py
--rw-r--r--   0 andrea     (501) staff       (20)     5056 2023-09-21 16:32:21.000000 trash-cli-0.23.9.23/trashcli/list/parser.py
--rw-r--r--   0 andrea     (501) staff       (20)     2342 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/list/trash_dir_selector.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.710531 trash-cli-0.23.9.23/trashcli/parse_trashinfo/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-05-04 12:51:30.000000 trash-cli-0.23.9.23/trashcli/parse_trashinfo/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      200 2023-05-04 12:51:30.000000 trash-cli-0.23.9.23/trashcli/parse_trashinfo/basket.py
--rw-r--r--   0 andrea     (501) staff       (20)      557 2023-05-04 12:51:31.000000 trash-cli-0.23.9.23/trashcli/parse_trashinfo/maybe_parse_deletion_date.py
--rw-r--r--   0 andrea     (501) staff       (20)      344 2023-05-04 12:51:30.000000 trash-cli-0.23.9.23/trashcli/parse_trashinfo/parse_deletion_date.py
--rw-r--r--   0 andrea     (501) staff       (20)      239 2023-05-04 12:51:30.000000 trash-cli-0.23.9.23/trashcli/parse_trashinfo/parse_original_location.py
--rw-r--r--   0 andrea     (501) staff       (20)      341 2023-05-04 12:51:30.000000 trash-cli-0.23.9.23/trashcli/parse_trashinfo/parse_path.py
--rw-r--r--   0 andrea     (501) staff       (20)     1116 2023-05-04 12:51:30.000000 trash-cli-0.23.9.23/trashcli/parse_trashinfo/parse_trashinfo.py
--rw-r--r--   0 andrea     (501) staff       (20)       76 2023-05-04 12:51:30.000000 trash-cli-0.23.9.23/trashcli/parse_trashinfo/parser_error.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.722461 trash-cli-0.23.9.23/trashcli/put/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2022-09-28 06:15:57.000000 trash-cli-0.23.9.23/trashcli/put/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)     1061 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/put/candidate.py
--rw-r--r--   0 andrea     (501) staff       (20)       78 2022-11-03 21:54:36.000000 trash-cli-0.23.9.23/trashcli/put/class_name_meta.py
--rw-r--r--   0 andrea     (501) staff       (20)      242 2022-10-02 14:15:27.000000 trash-cli-0.23.9.23/trashcli/put/clock.py
--rw-r--r--   0 andrea     (501) staff       (20)     1265 2022-11-08 17:23:59.000000 trash-cli-0.23.9.23/trashcli/put/describer.py
--rw-r--r--   0 andrea     (501) staff       (20)      298 2022-11-08 07:56:16.000000 trash-cli-0.23.9.23/trashcli/put/dir_maker.py
--rw-r--r--   0 andrea     (501) staff       (20)     3009 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/put/file_trasher.py
--rw-r--r--   0 andrea     (501) staff       (20)      665 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/put/format_trash_info.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.724046 trash-cli-0.23.9.23/trashcli/put/fs/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2022-11-08 07:53:59.000000 trash-cli-0.23.9.23/trashcli/put/fs/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)     1219 2023-06-06 17:07:29.000000 trash-cli-0.23.9.23/trashcli/put/fs/fs.py
--rw-r--r--   0 andrea     (501) staff       (20)      200 2022-11-08 07:59:53.000000 trash-cli-0.23.9.23/trashcli/put/fs/parent_realpath.py
--rw-r--r--   0 andrea     (501) staff       (20)     1571 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/put/fs/real_fs.py
--rw-r--r--   0 andrea     (501) staff       (20)      675 2022-11-09 20:49:16.000000 trash-cli-0.23.9.23/trashcli/put/fs/size_counter.py
--rw-r--r--   0 andrea     (501) staff       (20)      515 2023-06-02 18:54:48.000000 trash-cli-0.23.9.23/trashcli/put/fs/volume_of_parent.py
--rw-r--r--   0 andrea     (501) staff       (20)      392 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/put/gate.py
--rw-r--r--   0 andrea     (501) staff       (20)     3012 2023-06-06 17:07:29.000000 trash-cli-0.23.9.23/trashcli/put/gate_impl.py
--rw-r--r--   0 andrea     (501) staff       (20)     2225 2023-05-04 12:51:31.000000 trash-cli-0.23.9.23/trashcli/put/info_dir.py
--rw-r--r--   0 andrea     (501) staff       (20)     3387 2023-06-02 18:54:48.000000 trash-cli-0.23.9.23/trashcli/put/main.py
--rw-r--r--   0 andrea     (501) staff       (20)     1299 2022-11-03 21:54:36.000000 trash-cli-0.23.9.23/trashcli/put/my_logger.py
--rw-r--r--   0 andrea     (501) staff       (20)      928 2023-06-02 18:54:48.000000 trash-cli-0.23.9.23/trashcli/put/original_location.py
--rw-r--r--   0 andrea     (501) staff       (20)     4067 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/put/parser.py
--rw-r--r--   0 andrea     (501) staff       (20)      663 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/put/path_maker.py
--rw-r--r--   0 andrea     (501) staff       (20)     4344 2023-05-04 12:51:31.000000 trash-cli-0.23.9.23/trashcli/put/reporter.py
--rw-r--r--   0 andrea     (501) staff       (20)        0 2022-11-08 18:01:53.000000 trash-cli-0.23.9.23/trashcli/put/same_volume_gate.py
--rw-r--r--   0 andrea     (501) staff       (20)     1115 2022-11-24 10:56:43.000000 trash-cli-0.23.9.23/trashcli/put/security_check.py
--rw-r--r--   0 andrea     (501) staff       (20)      286 2022-09-28 17:59:27.000000 trash-cli-0.23.9.23/trashcli/put/suffix.py
--rw-r--r--   0 andrea     (501) staff       (20)     1312 2022-11-04 22:04:03.000000 trash-cli-0.23.9.23/trashcli/put/trash_all.py
--rw-r--r--   0 andrea     (501) staff       (20)      334 2022-11-03 21:54:36.000000 trash-cli-0.23.9.23/trashcli/put/trash_dir_volume_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)     3152 2023-06-02 18:54:48.000000 trash-cli-0.23.9.23/trashcli/put/trash_directories_finder.py
--rw-r--r--   0 andrea     (501) staff       (20)     1660 2023-05-04 12:51:31.000000 trash-cli-0.23.9.23/trashcli/put/trash_directory_for_put.py
--rw-r--r--   0 andrea     (501) staff       (20)     3094 2022-11-08 07:56:31.000000 trash-cli-0.23.9.23/trashcli/put/trash_file_in.py
--rw-r--r--   0 andrea     (501) staff       (20)     1542 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/put/trash_put_cmd.py
--rw-r--r--   0 andrea     (501) staff       (20)      449 2022-09-28 06:53:23.000000 trash-cli-0.23.9.23/trashcli/put/trash_result.py
--rw-r--r--   0 andrea     (501) staff       (20)      131 2022-11-03 21:54:36.000000 trash-cli-0.23.9.23/trashcli/put/trashee.py
--rw-r--r--   0 andrea     (501) staff       (20)     2946 2022-11-24 11:24:52.000000 trash-cli-0.23.9.23/trashcli/put/trasher.py
--rw-r--r--   0 andrea     (501) staff       (20)      733 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/put/trashing_checker.py
--rw-r--r--   0 andrea     (501) staff       (20)      785 2023-06-02 18:54:48.000000 trash-cli-0.23.9.23/trashcli/put/user.py
--rw-r--r--   0 andrea     (501) staff       (20)      610 2022-11-07 20:56:11.000000 trash-cli-0.23.9.23/trashcli/put/volume_message_formatter.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.736346 trash-cli-0.23.9.23/trashcli/restore/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-05-04 12:51:31.000000 trash-cli-0.23.9.23/trashcli/restore/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      598 2023-06-19 17:06:33.000000 trash-cli-0.23.9.23/trashcli/restore/args.py
--rw-r--r--   0 andrea     (501) staff       (20)     2250 2023-06-06 17:07:29.000000 trash-cli-0.23.9.23/trashcli/restore/file_system.py
--rw-r--r--   0 andrea     (501) staff       (20)     2187 2023-09-21 14:28:43.000000 trash-cli-0.23.9.23/trashcli/restore/handler.py
--rw-r--r--   0 andrea     (501) staff       (20)      143 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/restore/index.py
--rw-r--r--   0 andrea     (501) staff       (20)      970 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/restore/info_dir_searcher.py
--rw-r--r--   0 andrea     (501) staff       (20)      688 2023-05-04 12:51:43.000000 trash-cli-0.23.9.23/trashcli/restore/info_files.py
--rw-r--r--   0 andrea     (501) staff       (20)     1373 2023-06-02 18:54:49.000000 trash-cli-0.23.9.23/trashcli/restore/main.py
--rw-r--r--   0 andrea     (501) staff       (20)      542 2023-06-20 05:43:08.000000 trash-cli-0.23.9.23/trashcli/restore/output.py
--rw-r--r--   0 andrea     (501) staff       (20)      259 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/restore/output_event.py
--rw-r--r--   0 andrea     (501) staff       (20)      847 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/restore/output_recorder.py
--rw-r--r--   0 andrea     (501) staff       (20)      530 2023-06-02 18:54:49.000000 trash-cli-0.23.9.23/trashcli/restore/range.py
--rw-r--r--   0 andrea     (501) staff       (20)     1077 2023-06-05 12:03:33.000000 trash-cli-0.23.9.23/trashcli/restore/real_output.py
--rw-r--r--   0 andrea     (501) staff       (20)     2601 2023-06-19 17:07:50.000000 trash-cli-0.23.9.23/trashcli/restore/restore_arg_parser.py
--rw-r--r--   0 andrea     (501) staff       (20)     5463 2023-06-20 05:43:08.000000 trash-cli-0.23.9.23/trashcli/restore/restore_asking_the_user.py
--rw-r--r--   0 andrea     (501) staff       (20)     2385 2023-06-18 21:13:27.000000 trash-cli-0.23.9.23/trashcli/restore/restore_cmd.py
--rw-r--r--   0 andrea     (501) staff       (20)     1218 2023-05-04 12:51:43.000000 trash-cli-0.23.9.23/trashcli/restore/restorer.py
--rw-r--r--   0 andrea     (501) staff       (20)     1964 2023-09-21 14:28:43.000000 trash-cli-0.23.9.23/trashcli/restore/run_restore_action.py
--rw-r--r--   0 andrea     (501) staff       (20)      295 2023-06-04 21:00:15.000000 trash-cli-0.23.9.23/trashcli/restore/sequences.py
--rw-r--r--   0 andrea     (501) staff       (20)      102 2023-06-02 18:54:49.000000 trash-cli-0.23.9.23/trashcli/restore/single.py
--rw-r--r--   0 andrea     (501) staff       (20)     1537 2023-06-19 17:01:19.000000 trash-cli-0.23.9.23/trashcli/restore/sort_method.py
--rw-r--r--   0 andrea     (501) staff       (20)     2482 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/restore/trash_directories.py
--rw-r--r--   0 andrea     (501) staff       (20)     1092 2023-06-02 18:54:49.000000 trash-cli-0.23.9.23/trashcli/restore/trashed_file.py
--rw-r--r--   0 andrea     (501) staff       (20)     3747 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/restore/trashed_files.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2023-09-23 12:47:29.742312 trash-cli-0.23.9.23/trashcli/rm/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-05-01 16:33:40.000000 trash-cli-0.23.9.23/trashcli/rm/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      584 2023-05-04 12:51:31.000000 trash-cli-0.23.9.23/trashcli/rm/cleanable_trashcan.py
--rw-r--r--   0 andrea     (501) staff       (20)      161 2023-05-01 16:33:40.000000 trash-cli-0.23.9.23/trashcli/rm/file_remover.py
--rw-r--r--   0 andrea     (501) staff       (20)      399 2023-05-01 16:33:40.000000 trash-cli-0.23.9.23/trashcli/rm/filter.py
--rw-r--r--   0 andrea     (501) staff       (20)     1612 2023-06-06 17:07:29.000000 trash-cli-0.23.9.23/trashcli/rm/list_trashinfo.py
--rw-r--r--   0 andrea     (501) staff       (20)      963 2023-06-02 18:55:46.000000 trash-cli-0.23.9.23/trashcli/rm/main.py
--rw-r--r--   0 andrea     (501) staff       (20)     3066 2023-06-06 17:07:29.000000 trash-cli-0.23.9.23/trashcli/rm/rm_cmd.py
--rw-r--r--   0 andrea     (501) staff       (20)     1772 2023-06-10 12:59:11.000000 trash-cli-0.23.9.23/trashcli/shell_completion.py
--rw-r--r--   0 andrea     (501) staff       (20)      202 2022-09-12 06:41:34.000000 trash-cli-0.23.9.23/trashcli/super_enum.py
--rw-r--r--   0 andrea     (501) staff       (20)       84 2023-09-23 12:45:29.000000 trash-cli-0.23.9.23/trashcli/trash.py
--rw-r--r--   0 andrea     (501) staff       (20)     4006 2023-06-06 17:07:29.000000 trash-cli-0.23.9.23/trashcli/trash_dirs_scanner.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.555893 trash_cli-0.24.4.17/
+-rw-r--r--   0 andrea     (501) staff       (20)    17992 2022-08-24 18:45:23.000000 trash_cli-0.24.4.17/COPYING
+-rw-r--r--   0 andrea     (501) staff       (20)     7916 2024-04-17 19:18:15.555816 trash_cli-0.24.4.17/PKG-INFO
+-rw-r--r--   0 andrea     (501) staff       (20)     7349 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/README.rst
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.496624 trash_cli-0.24.4.17/man/
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.506238 trash_cli-0.24.4.17/man/man1/
+-rw-r--r--   0 andrea     (501) staff       (20)     2765 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/man/man1/trash-empty.1
+-rw-r--r--   0 andrea     (501) staff       (20)     2386 2022-08-24 18:45:23.000000 trash_cli-0.24.4.17/man/man1/trash-list.1
+-rw-r--r--   0 andrea     (501) staff       (20)     3216 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/man/man1/trash-put.1
+-rw-r--r--   0 andrea     (501) staff       (20)     2401 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/man/man1/trash-restore.1
+-rw-r--r--   0 andrea     (501) staff       (20)     1433 2022-08-24 18:45:23.000000 trash_cli-0.24.4.17/man/man1/trash-rm.1
+-rw-r--r--   0 andrea     (501) staff       (20)     3216 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/man/man1/trash.1
+-rw-r--r--   0 andrea     (501) staff       (20)       90 2022-10-04 20:03:09.000000 trash_cli-0.24.4.17/pyproject.toml
+-rw-r--r--   0 andrea     (501) staff       (20)     1075 2024-04-17 19:18:15.556277 trash_cli-0.24.4.17/setup.cfg
+-rw-r--r--   0 andrea     (501) staff       (20)       99 2023-05-04 13:06:54.000000 trash_cli-0.24.4.17/setup.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.514993 trash_cli-0.24.4.17/tests/
+-rw-r--r--   0 andrea     (501) staff       (20)     1428 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_bump.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1779 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_candidate_shrink_user.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1363 2022-08-24 18:45:23.000000 trash_cli-0.24.4.17/tests/test_fake_file_system.py
+-rw-r--r--   0 andrea     (501) staff       (20)      728 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_fake_fstab.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1255 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_fake_ismount.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1780 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_filesystem.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1126 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_generate_scripts.py
+-rw-r--r--   0 andrea     (501) staff       (20)      426 2022-08-24 18:45:23.000000 trash_cli-0.24.4.17/tests/test_joining_paths.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1662 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_list_all_trashinfo_contents.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2056 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_make_script.py
+-rw-r--r--   0 andrea     (501) staff       (20)      893 2022-09-22 13:29:20.000000 trash_cli-0.24.4.17/tests/test_mock_dir_reader.py
+-rw-r--r--   0 andrea     (501) staff       (20)      355 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_my_mock.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3760 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_parsing_trashinfo_contents.py
+-rw-r--r--   0 andrea     (501) staff       (20)      958 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_partitions.py
+-rw-r--r--   0 andrea     (501) staff       (20)      291 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/tests/test_tox_version_matches.py
+-rw-r--r--   0 andrea     (501) staff       (20)      663 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_trash_dir_reader.py
+-rw-r--r--   0 andrea     (501) staff       (20)      856 2023-12-09 10:55:16.000000 trash_cli-0.24.4.17/tests/test_trash_put_reporter.py
+-rw-r--r--   0 andrea     (501) staff       (20)      665 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_volume_of.py
+-rwxr-xr-x   0 andrea     (501) staff       (20)      132 2024-04-17 19:18:03.000000 trash_cli-0.24.4.17/trash
+-rwxr-xr-x   0 andrea     (501) staff       (20)      134 2024-04-17 19:18:03.000000 trash_cli-0.24.4.17/trash-empty
+-rwxr-xr-x   0 andrea     (501) staff       (20)      133 2024-04-17 19:18:03.000000 trash_cli-0.24.4.17/trash-list
+-rwxr-xr-x   0 andrea     (501) staff       (20)      132 2024-04-17 19:18:03.000000 trash_cli-0.24.4.17/trash-put
+-rwxr-xr-x   0 andrea     (501) staff       (20)      136 2024-04-17 19:18:03.000000 trash_cli-0.24.4.17/trash-restore
+-rwxr-xr-x   0 andrea     (501) staff       (20)      131 2024-04-17 19:18:03.000000 trash_cli-0.24.4.17/trash-rm
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.555339 trash_cli-0.24.4.17/trash_cli.egg-info/
+-rw-r--r--   0 andrea     (501) staff       (20)     7916 2024-04-17 19:18:15.000000 trash_cli-0.24.4.17/trash_cli.egg-info/PKG-INFO
+-rw-r--r--   0 andrea     (501) staff       (20)     5575 2024-04-17 19:18:15.000000 trash_cli-0.24.4.17/trash_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 andrea     (501) staff       (20)        1 2024-04-17 19:18:15.000000 trash_cli-0.24.4.17/trash_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 andrea     (501) staff       (20)      117 2024-04-17 19:18:15.000000 trash_cli-0.24.4.17/trash_cli.egg-info/requires.txt
+-rw-r--r--   0 andrea     (501) staff       (20)        9 2024-04-17 19:18:15.000000 trash_cli-0.24.4.17/trash_cli.egg-info/top_level.txt
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.519984 trash_cli-0.24.4.17/trashcli/
+-rw-r--r--   0 andrea     (501) staff       (20)       87 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      223 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/compat.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.525762 trash_cli-0.24.4.17/trashcli/empty/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2022-09-09 17:05:55.000000 trash_cli-0.24.4.17/trashcli/empty/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      642 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/clock.py
+-rw-r--r--   0 andrea     (501) staff       (20)      655 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/console.py
+-rw-r--r--   0 andrea     (501) staff       (20)      952 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/delete_according_date.py
+-rw-r--r--   0 andrea     (501) staff       (20)      307 2022-09-06 20:19:17.000000 trash_cli-0.24.4.17/trashcli/empty/description.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2328 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/emptier.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2991 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/empty_action.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3298 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/empty_cmd.py
+-rw-r--r--   0 andrea     (501) staff       (20)      306 2022-09-16 20:46:37.000000 trash_cli-0.24.4.17/trashcli/empty/errors.py
+-rw-r--r--   0 andrea     (501) staff       (20)      143 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/existing_file_remover.py
+-rw-r--r--   0 andrea     (501) staff       (20)      270 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/file_system_dir_reader.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1477 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/guard.py
+-rw-r--r--   0 andrea     (501) staff       (20)       64 2022-09-06 20:19:17.000000 trash_cli-0.24.4.17/trashcli/empty/is_input_interactive.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1361 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/main.py
+-rw-r--r--   0 andrea     (501) staff       (20)      179 2022-09-06 20:19:17.000000 trash_cli-0.24.4.17/trashcli/empty/older_than.py
+-rw-r--r--   0 andrea     (501) staff       (20)       61 2022-09-06 20:19:17.000000 trash_cli-0.24.4.17/trashcli/empty/parse_reply.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3538 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/parser.py
+-rw-r--r--   0 andrea     (501) staff       (20)      512 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/trashcli/empty/prepare_output_message.py
+-rw-r--r--   0 andrea     (501) staff       (20)      618 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/print_time_action.py
+-rw-r--r--   0 andrea     (501) staff       (20)      257 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/top_trash_dir_rules_file_system_reader.py
+-rw-r--r--   0 andrea     (501) staff       (20)      490 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/user.py
+-rw-r--r--   0 andrea     (501) staff       (20)      514 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/file_system_reader.py
+-rw-r--r--   0 andrea     (501) staff       (20)     6321 2024-03-28 21:52:00.000000 trash_cli-0.24.4.17/trashcli/fs.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.526729 trash_cli-0.24.4.17/trashcli/fstab/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/fstab/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1823 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/trashcli/fstab/mount_points_listing.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1171 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/fstab/volume_listing.py
+-rw-r--r--   0 andrea     (501) staff       (20)      818 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/fstab/volume_of.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1920 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/fstab/volumes.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.530482 trash_cli-0.24.4.17/trashcli/lib/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      145 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/dir_checker.py
+-rw-r--r--   0 andrea     (501) staff       (20)      328 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/dir_reader.py
+-rw-r--r--   0 andrea     (501) staff       (20)      126 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/enum_repr.py
+-rw-r--r--   0 andrea     (501) staff       (20)      237 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/environ.py
+-rw-r--r--   0 andrea     (501) staff       (20)      279 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/exit_codes.py
+-rw-r--r--   0 andrea     (501) staff       (20)      207 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/logger.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1040 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/my_input.py
+-rw-r--r--   0 andrea     (501) staff       (20)      227 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/my_permission_error.py
+-rw-r--r--   0 andrea     (501) staff       (20)      281 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/path_of_backup_copy.py
+-rw-r--r--   0 andrea     (501) staff       (20)      774 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/trashcli/lib/print_version.py
+-rw-r--r--   0 andrea     (501) staff       (20)      919 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/trash_dir_reader.py
+-rw-r--r--   0 andrea     (501) staff       (20)      926 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/trash_dirs.py
+-rw-r--r--   0 andrea     (501) staff       (20)      860 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/user_info.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.531844 trash_cli-0.24.4.17/trashcli/list/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/list/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      691 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/list/extractors.py
+-rw-r--r--   0 andrea     (501) staff       (20)      336 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/list/fs.py
+-rw-r--r--   0 andrea     (501) staff       (20)     5915 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/list/list_trash_action.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3834 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/list/main.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.532701 trash_cli-0.24.4.17/trashcli/list/minor_actions/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/list/minor_actions/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      647 2024-03-28 21:52:14.000000 trash_cli-0.24.4.17/trashcli/list/minor_actions/debug_volumes.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1344 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/list/minor_actions/list_trash_dirs.py
+-rw-r--r--   0 andrea     (501) staff       (20)      482 2024-03-28 21:52:14.000000 trash_cli-0.24.4.17/trashcli/list/minor_actions/list_volumes.py
+-rw-r--r--   0 andrea     (501) staff       (20)      230 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/list/minor_actions/print_python_executable.py
+-rw-r--r--   0 andrea     (501) staff       (20)     5083 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/list/parser.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2342 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/list/trash_dir_selector.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.534476 trash_cli-0.24.4.17/trashcli/parse_trashinfo/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      200 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/basket.py
+-rw-r--r--   0 andrea     (501) staff       (20)      557 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/maybe_parse_deletion_date.py
+-rw-r--r--   0 andrea     (501) staff       (20)      344 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/parse_deletion_date.py
+-rw-r--r--   0 andrea     (501) staff       (20)      239 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/parse_original_location.py
+-rw-r--r--   0 andrea     (501) staff       (20)      341 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/parse_path.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1116 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/parse_trashinfo.py
+-rw-r--r--   0 andrea     (501) staff       (20)       76 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/parser_error.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.541111 trash_cli-0.24.4.17/trashcli/put/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      324 2024-01-04 21:53:23.000000 trash_cli-0.24.4.17/trashcli/put/check_cast.py
+-rw-r--r--   0 andrea     (501) staff       (20)      242 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/clock.py
+-rw-r--r--   0 andrea     (501) staff       (20)      511 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/context.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.544371 trash_cli-0.24.4.17/trashcli/put/core/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1139 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/candidate.py
+-rw-r--r--   0 andrea     (501) staff       (20)      189 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/check_type.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1824 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/either.py
+-rw-r--r--   0 andrea     (501) staff       (20)      715 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/failure_reason.py
+-rw-r--r--   0 andrea     (501) staff       (20)      237 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/int_generator.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1434 2024-03-19 22:29:51.000000 trash_cli-0.24.4.17/trashcli/put/core/logs.py
+-rw-r--r--   0 andrea     (501) staff       (20)      414 2023-12-16 16:38:07.000000 trash_cli-0.24.4.17/trashcli/put/core/mode.py
+-rw-r--r--   0 andrea     (501) staff       (20)      123 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/path_maker_type.py
+-rw-r--r--   0 andrea     (501) staff       (20)      217 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/trash_all_result.py
+-rw-r--r--   0 andrea     (501) staff       (20)       97 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/trash_result.py
+-rw-r--r--   0 andrea     (501) staff       (20)      267 2023-12-16 16:39:59.000000 trash_cli-0.24.4.17/trashcli/put/core/trashee.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1265 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/describer.py
+-rw-r--r--   0 andrea     (501) staff       (20)      298 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/dir_maker.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3324 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/file_trasher.py
+-rw-r--r--   0 andrea     (501) staff       (20)      665 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/format_trash_info.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.545410 trash_cli-0.24.4.17/trashcli/put/fs/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/fs/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2112 2024-03-24 16:22:41.000000 trash_cli-0.24.4.17/trashcli/put/fs/fs.py
+-rw-r--r--   0 andrea     (501) staff       (20)      275 2023-12-16 22:43:22.000000 trash_cli-0.24.4.17/trashcli/put/fs/parent_realpath.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2633 2024-03-28 21:52:14.000000 trash_cli-0.24.4.17/trashcli/put/fs/real_fs.py
+-rw-r--r--   0 andrea     (501) staff       (20)      675 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/fs/size_counter.py
+-rw-r--r--   0 andrea     (501) staff       (20)      531 2023-12-16 22:43:22.000000 trash_cli-0.24.4.17/trashcli/put/fs/volume_of_parent.py
+-rw-r--r--   0 andrea     (501) staff       (20)      197 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/gate.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3358 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/janitor.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.546785 trash_cli-0.24.4.17/trashcli/put/janitor_tools/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/janitor_tools/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2108 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/janitor_tools/info_creator.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2896 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/janitor_tools/info_file_persister.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1534 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/janitor_tools/put_trash_dir.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2545 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/janitor_tools/security_check.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3073 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/janitor_tools/trash_dir_checker.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1155 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/janitor_tools/trash_dir_creator.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2137 2024-01-04 20:33:42.000000 trash_cli-0.24.4.17/trashcli/put/jobs.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3535 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/main.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1815 2023-12-09 21:05:26.000000 trash_cli-0.24.4.17/trashcli/put/my_logger.py
+-rw-r--r--   0 andrea     (501) staff       (20)      282 2023-12-09 10:03:26.000000 trash_cli-0.24.4.17/trashcli/put/octal.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1305 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/original_location.py
+-rw-r--r--   0 andrea     (501) staff       (20)     4803 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/parser.py
+-rw-r--r--   0 andrea     (501) staff       (20)     6843 2024-01-04 21:54:10.000000 trash_cli-0.24.4.17/trashcli/put/reporter.py
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/same_volume_gate.py
+-rw-r--r--   0 andrea     (501) staff       (20)      411 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/suffix.py
+-rw-r--r--   0 andrea     (501) staff       (20)      838 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/trash_all.py
+-rw-r--r--   0 andrea     (501) staff       (20)      514 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/trash_dir_volume_reader.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3214 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/trash_directories_finder.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1605 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/trash_put_cmd.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2325 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/trasher.py
+-rw-r--r--   0 andrea     (501) staff       (20)      775 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/user.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.552393 trash_cli-0.24.4.17/trashcli/restore/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      447 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/args.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2250 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/file_system.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2187 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/handler.py
+-rw-r--r--   0 andrea     (501) staff       (20)      143 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/index.py
+-rw-r--r--   0 andrea     (501) staff       (20)      970 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/info_dir_searcher.py
+-rw-r--r--   0 andrea     (501) staff       (20)      688 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/info_files.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1377 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/main.py
+-rw-r--r--   0 andrea     (501) staff       (20)      542 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/output.py
+-rw-r--r--   0 andrea     (501) staff       (20)      271 2024-03-28 21:52:14.000000 trash_cli-0.24.4.17/trashcli/restore/output_event.py
+-rw-r--r--   0 andrea     (501) staff       (20)      847 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/output_recorder.py
+-rw-r--r--   0 andrea     (501) staff       (20)      530 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/range.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1077 2024-03-28 21:52:14.000000 trash_cli-0.24.4.17/trashcli/restore/real_output.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2595 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/restore_arg_parser.py
+-rw-r--r--   0 andrea     (501) staff       (20)     5528 2024-03-28 21:52:14.000000 trash_cli-0.24.4.17/trashcli/restore/restore_asking_the_user.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2385 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/restore_cmd.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1218 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/restorer.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1964 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/run_restore_action.py
+-rw-r--r--   0 andrea     (501) staff       (20)      295 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/sequences.py
+-rw-r--r--   0 andrea     (501) staff       (20)      102 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/single.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1526 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/sort_method.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2510 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/trash_directories.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1092 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/trashed_file.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3747 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/trashed_files.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.555116 trash_cli-0.24.4.17/trashcli/rm/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/rm/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      584 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/rm/cleanable_trashcan.py
+-rw-r--r--   0 andrea     (501) staff       (20)      161 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/rm/file_remover.py
+-rw-r--r--   0 andrea     (501) staff       (20)      399 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/rm/filter.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1612 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/rm/list_trashinfo.py
+-rw-r--r--   0 andrea     (501) staff       (20)      963 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/rm/main.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3066 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/rm/rm_cmd.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1775 2024-03-28 21:52:14.000000 trash_cli-0.24.4.17/trashcli/shell_completion.py
+-rw-r--r--   0 andrea     (501) staff       (20)       84 2024-04-17 18:48:54.000000 trash_cli-0.24.4.17/trashcli/trash.py
+-rw-r--r--   0 andrea     (501) staff       (20)     4006 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/trash_dirs_scanner.py
```

### Comparing `trash-cli-0.23.9.23/COPYING` & `trash_cli-0.24.4.17/COPYING`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/PKG-INFO` & `trash_cli-0.24.4.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: trash-cli
-Version: 0.23.9.23
+Version: 0.24.4.17
 Summary: Command line interface to FreeDesktop.org Trash.
 Home-page: https://github.com/andreafrancia/trash-cli
 Author: Andrea Francia
 Author-email: andrea@andreafrancia.it
 License: GPL v2
 Description-Content-Type: text/x-rst
 License-File: COPYING
 Requires-Dist: psutil
 Requires-Dist: six
 Requires-Dist: typing; python_version < "3.8"
 Requires-Dist: typing_extensions; python_version < "3.8"
+Requires-Dist: enum34; python_version < "3.4"
 Provides-Extra: completion
 Requires-Dist: shtab; extra == "completion"
 
 trash-cli - Command Line Interface to FreeDesktop.org Trash.
 ============================================================
 
 |Downloads|
```

### Comparing `trash-cli-0.23.9.23/README.rst` & `trash_cli-0.24.4.17/README.rst`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/man/man1/trash-empty.1` & `trash_cli-0.24.4.17/man/man1/trash-empty.1`

 * *Files 3% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 
 .SH "SYNOPSIS"
 .B trash-empty
 .RI [ arguments ]
 
 .SH "DESCRIPTION"
 .PP
-Remove for ever any trashed file and trashed directory.
-This command is a part of trash-cli package that provides a command 
+Permanently remove any trashed file and trashed directory.
+This command is a part of the trash-cli package that provides a command 
 line interface trashcan utility compliant with the FreeDesktop.org 
 Trash Specification.
 It remembers the name, original path, deletion date, and permissions of
 each trashed file.
 
 .SH "ARGUMENTS"
 .TP
 To remove all trashed files, use 'trash-empty' without arguments.
 .TP
-To remove files that have been in the trash more than a given number of
+To remove files that have been in the trash for more than a given number of
 days, use 'trash-empty x', 'x' representing the number of days.
 
 .SH "EXAMPLES"
 .nf
 $ date
 Tue Feb 19 20:26:52 CET 2008
 $ trash-list
```

### Comparing `trash-cli-0.23.9.23/man/man1/trash-list.1` & `trash_cli-0.24.4.17/man/man1/trash-list.1`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/man/man1/trash-put.1` & `trash_cli-0.24.4.17/man/man1/trash-put.1`

 * *Files 5% similar despite different names*

```diff
@@ -37,52 +37,51 @@
 .PP
 Trash-cli package provides a command line interface trashcan utility
 compliant with the FreeDesktop.org Trash Specification.
 It remembers the name, original path, deletion date, and permissions of
 each trashed file.
 .br
 
-The file trashed from the home partition are trashed in a directory called
-"home trash" directory in the path $XDG_DATA_HOME/Trash or ~/.local/share/Trash/
-if $XDG_DATA_HOME is not defined or empty.
+Files trashed from the home partition will be in either $XDG_DATA_HOME/Trash
+or ~/.local/share/Trash/ (if $XDG_DATA_HOME is not defined or empty).
 
-File trashed from other partitions will can be trashed in one of the two places:
+Files trashed from other partitions will be in one of the two places:
 
  - $top_dir/.Trash/$uid
  - $top_dir/.Trash-$uid
 
 Where:
- - $top_dir is the mount point of the volume containing the file to be removed.
- - $uid is the numeri ID of the deleting user
+ - $top_dir is the mount point of the volume containing the file to be removed
+ - $uid is the numeric ID of the deleting user
 
 The first option $top_dir/.Trash/$uid works only when .Trash dir has the sticky
 bit set. The second option is used when the first is not viable.
 
 .SH "ARGUMENTS"
 .TP
-Names of files or directories to move in the trashcan.
+Names of files or directories to move to the trash can.
 
 .SH "OPTIONS"
 .IP "-f"
 .br
 Silently ignore any files or directories that do not exist.
 Do not print error messages, and do not return a nonzero status
 to the caller, because of any such nonexistent arguments.
 
 .IP "-h, --help"
 Show help message and exit.
 
 .IP "--trash-dir=TRASHDIR"
-Use TRASHDIR as trash folder.
+Use TRASHDIR as the trash folder.
 
 .IP "-v, --verbose"
 Explain what is being done.
 
 .IP "--version"
-Show program's version number and exit.
+Show the program's version number and exit.
 
 .SH "EXAMPLES"
 .nf
 $ trash-put foo   # trashes foo 
 .fi
 
 .SH "BUGS"
```

### Comparing `trash-cli-0.23.9.23/man/man1/trash-restore.1` & `trash_cli-0.24.4.17/man/man1/trash-restore.1`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 trash-restore \- Restore for Command line trash utility.
 
 .SH "SYNOPSIS"
 .B trash-restore
 
 .SH "DESCRIPTION"
 .PP
-Use for restore a trashed file or directory, in the original path.
-This command is a part of trash-cli package that provides a command 
+Use to restore a trashed file or directory to the original path.
+This command is a part of the trash-cli package that provides a command 
 line interface trashcan utility compliant with the FreeDesktop.org 
 Trash Specification.
 It remembers the name, original path, deletion date, and permissions of
 each trashed file.
 
 .SH "EXAMPLES"
 .nf
```

### Comparing `trash-cli-0.23.9.23/man/man1/trash-rm.1` & `trash_cli-0.24.4.17/man/man1/trash-rm.1`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/man/man1/trash.1` & `trash_cli-0.24.4.17/man/man1/trash.1`

 * *Files 5% similar despite different names*

```diff
@@ -37,52 +37,51 @@
 .PP
 Trash-cli package provides a command line interface trashcan utility
 compliant with the FreeDesktop.org Trash Specification.
 It remembers the name, original path, deletion date, and permissions of
 each trashed file.
 .br
 
-The file trashed from the home partition are trashed in a directory called
-"home trash" directory in the path $XDG_DATA_HOME/Trash or ~/.local/share/Trash/
-if $XDG_DATA_HOME is not defined or empty.
+Files trashed from the home partition will be in either $XDG_DATA_HOME/Trash
+or ~/.local/share/Trash/ (if $XDG_DATA_HOME is not defined or empty).
 
-File trashed from other partitions will can be trashed in one of the two places:
+Files trashed from other partitions will be in one of the two places:
 
  - $top_dir/.Trash/$uid
  - $top_dir/.Trash-$uid
 
 Where:
- - $top_dir is the mount point of the volume containing the file to be removed.
- - $uid is the numeri ID of the deleting user
+ - $top_dir is the mount point of the volume containing the file to be removed
+ - $uid is the numeric ID of the deleting user
 
 The first option $top_dir/.Trash/$uid works only when .Trash dir has the sticky
 bit set. The second option is used when the first is not viable.
 
 .SH "ARGUMENTS"
 .TP
-Names of files or directories to move in the trashcan.
+Names of files or directories to move to the trash can.
 
 .SH "OPTIONS"
 .IP "-f"
 .br
 Silently ignore any files or directories that do not exist.
 Do not print error messages, and do not return a nonzero status
 to the caller, because of any such nonexistent arguments.
 
 .IP "-h, --help"
 Show help message and exit.
 
 .IP "--trash-dir=TRASHDIR"
-Use TRASHDIR as trash folder.
+Use TRASHDIR as the trash folder.
 
 .IP "-v, --verbose"
 Explain what is being done.
 
 .IP "--version"
-Show program's version number and exit.
+Show the program's version number and exit.
 
 .SH "EXAMPLES"
 .nf
 $ trash-put foo   # trashes foo 
 .fi
 
 .SH "BUGS"
```

### Comparing `trash-cli-0.23.9.23/setup.cfg` & `trash_cli-0.24.4.17/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 packages = 
 	trashcli
 	trashcli.empty
 	trashcli.lib
 	trashcli.list
 	trashcli.list.minor_actions
 	trashcli.put
+	trashcli.put.core
+	trashcli.put.janitor_tools
 	trashcli.put.fs
 	trashcli.restore
 	trashcli.rm
 	trashcli.fstab
 	trashcli.parse_trashinfo
 scripts = 
 	trash
@@ -30,14 +32,15 @@
 	trash-empty
 	trash-rm
 install_requires = 
 	psutil
 	six
 	typing; python_version < '3.8'
 	typing_extensions; python_version < '3.8'
+	enum34; python_version < '3.4'
 
 [options.extras_require]
 completion = 
 	shtab
 
 [options.data_files]
 share/man/man1 =
```

### Comparing `trash-cli-0.23.9.23/tests/test_bump.py` & `trash_cli-0.24.4.17/tests/test_bump.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/tests/test_candidate_shrink_user.py` & `trash_cli-0.24.4.17/tests/test_candidate_shrink_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from trashcli.put.candidate import Candidate
+from trashcli.put.core.candidate import Candidate
 
 
 class TestCandidateShrinkUser(unittest.TestCase):
     def setUp(self):
         self.environ = {}
 
     def test_should_substitute_tilde_in_place_of_home_dir(self):
```

### Comparing `trash-cli-0.23.9.23/tests/test_fake_file_system.py` & `trash_cli-0.24.4.17/tests/test_fake_file_system.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/tests/test_fake_fstab.py` & `trash_cli-0.24.4.17/tests/test_fake_fstab.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/tests/test_fake_ismount.py` & `trash_cli-0.24.4.17/tests/test_fake_ismount.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/tests/test_filesystem.py` & `trash_cli-0.24.4.17/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/tests/test_generate_scripts.py` & `trash_cli-0.24.4.17/tests/test_generate_scripts.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/tests/test_list_all_trashinfo_contents.py` & `trash_cli-0.24.4.17/tests/test_list_all_trashinfo_contents.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/tests/test_make_script.py` & `trash_cli-0.24.4.17/tests/test_make_script.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/tests/test_mock_dir_reader.py` & `trash_cli-0.24.4.17/tests/test_mock_dir_reader.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/tests/test_parsing_trashinfo_contents.py` & `trash_cli-0.24.4.17/tests/test_parsing_trashinfo_contents.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/tests/test_partitions.py` & `trash_cli-0.24.4.17/tests/test_partitions.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/tests/test_trash_dir_reader.py` & `trash_cli-0.24.4.17/tests/test_trash_dir_reader.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/tests/test_trash_put_reporter.py` & `trash_cli-0.24.4.17/tests/test_trash_put_reporter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import unittest
 
-from mock import Mock, call
+from mock import Mock
+from six import StringIO
 
 from trashcli.put.my_logger import LogData
+from trashcli.put.my_logger import MyLogger
+from trashcli.put.my_logger import StreamBackend
 from trashcli.put.reporter import TrashPutReporter
 
 
 class TestTrashPutReporter(unittest.TestCase):
     def setUp(self):
-        self.logger = Mock(['warning2'])
+        self.stderr = StringIO()
+        self.backend = StreamBackend(self.stderr)
+        self.logger = MyLogger(self.backend)
         describer = Mock()
         describer.describe.return_value = "file-description"
         self.reporter = TrashPutReporter(self.logger, describer)
 
     def test_it_should_record_failures(self):
-        self.reporter.unable_to_trash_file('a file', LogData('trash-put', 99))
+        self.reporter.unable_to_trash_file_non_existent('a file', LogData('trash-put', 99))
 
-        assert [call('cannot trash file-description \'a file\'', 'trash-put')] == \
-               self.logger.warning2.mock_calls
+        assert (self.stderr.getvalue() ==
+                "trash-put: cannot trash file-description 'a file'\n")
```

### Comparing `trash-cli-0.23.9.23/tests/test_volume_of.py` & `trash_cli-0.24.4.17/tests/test_volume_of.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trash_cli.egg-info/PKG-INFO` & `trash_cli-0.24.4.17/trash_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: trash-cli
-Version: 0.23.9.23
+Version: 0.24.4.17
 Summary: Command line interface to FreeDesktop.org Trash.
 Home-page: https://github.com/andreafrancia/trash-cli
 Author: Andrea Francia
 Author-email: andrea@andreafrancia.it
 License: GPL v2
 Description-Content-Type: text/x-rst
 License-File: COPYING
 Requires-Dist: psutil
 Requires-Dist: six
 Requires-Dist: typing; python_version < "3.8"
 Requires-Dist: typing_extensions; python_version < "3.8"
+Requires-Dist: enum34; python_version < "3.4"
 Provides-Extra: completion
 Requires-Dist: shtab; extra == "completion"
 
 trash-cli - Command Line Interface to FreeDesktop.org Trash.
 ============================================================
 
 |Downloads|
```

### Comparing `trash-cli-0.23.9.23/trash_cli.egg-info/SOURCES.txt` & `trash_cli-0.24.4.17/trash_cli.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -25,29 +25,28 @@
 tests/test_joining_paths.py
 tests/test_list_all_trashinfo_contents.py
 tests/test_make_script.py
 tests/test_mock_dir_reader.py
 tests/test_my_mock.py
 tests/test_parsing_trashinfo_contents.py
 tests/test_partitions.py
-tests/test_top_trash_dir_rules.py
+tests/test_tox_version_matches.py
 tests/test_trash_dir_reader.py
 tests/test_trash_put_reporter.py
 tests/test_volume_of.py
 trash_cli.egg-info/PKG-INFO
 trash_cli.egg-info/SOURCES.txt
 trash_cli.egg-info/dependency_links.txt
 trash_cli.egg-info/requires.txt
 trash_cli.egg-info/top_level.txt
 trashcli/__init__.py
 trashcli/compat.py
 trashcli/file_system_reader.py
 trashcli/fs.py
 trashcli/shell_completion.py
-trashcli/super_enum.py
 trashcli/trash.py
 trashcli/trash_dirs_scanner.py
 trashcli/empty/__init__.py
 trashcli/empty/clock.py
 trashcli/empty/console.py
 trashcli/empty/delete_according_date.py
 trashcli/empty/description.py
@@ -71,14 +70,16 @@
 trashcli/fstab/mount_points_listing.py
 trashcli/fstab/volume_listing.py
 trashcli/fstab/volume_of.py
 trashcli/fstab/volumes.py
 trashcli/lib/__init__.py
 trashcli/lib/dir_checker.py
 trashcli/lib/dir_reader.py
+trashcli/lib/enum_repr.py
+trashcli/lib/environ.py
 trashcli/lib/exit_codes.py
 trashcli/lib/logger.py
 trashcli/lib/my_input.py
 trashcli/lib/my_permission_error.py
 trashcli/lib/path_of_backup_copy.py
 trashcli/lib/print_version.py
 trashcli/lib/trash_dir_reader.py
@@ -101,51 +102,63 @@
 trashcli/parse_trashinfo/maybe_parse_deletion_date.py
 trashcli/parse_trashinfo/parse_deletion_date.py
 trashcli/parse_trashinfo/parse_original_location.py
 trashcli/parse_trashinfo/parse_path.py
 trashcli/parse_trashinfo/parse_trashinfo.py
 trashcli/parse_trashinfo/parser_error.py
 trashcli/put/__init__.py
-trashcli/put/candidate.py
-trashcli/put/class_name_meta.py
+trashcli/put/check_cast.py
 trashcli/put/clock.py
+trashcli/put/context.py
 trashcli/put/describer.py
 trashcli/put/dir_maker.py
 trashcli/put/file_trasher.py
 trashcli/put/format_trash_info.py
 trashcli/put/gate.py
-trashcli/put/gate_impl.py
-trashcli/put/info_dir.py
+trashcli/put/janitor.py
+trashcli/put/jobs.py
 trashcli/put/main.py
 trashcli/put/my_logger.py
+trashcli/put/octal.py
 trashcli/put/original_location.py
 trashcli/put/parser.py
-trashcli/put/path_maker.py
 trashcli/put/reporter.py
 trashcli/put/same_volume_gate.py
-trashcli/put/security_check.py
 trashcli/put/suffix.py
 trashcli/put/trash_all.py
 trashcli/put/trash_dir_volume_reader.py
 trashcli/put/trash_directories_finder.py
-trashcli/put/trash_directory_for_put.py
-trashcli/put/trash_file_in.py
 trashcli/put/trash_put_cmd.py
-trashcli/put/trash_result.py
-trashcli/put/trashee.py
 trashcli/put/trasher.py
-trashcli/put/trashing_checker.py
 trashcli/put/user.py
-trashcli/put/volume_message_formatter.py
+trashcli/put/core/__init__.py
+trashcli/put/core/candidate.py
+trashcli/put/core/check_type.py
+trashcli/put/core/either.py
+trashcli/put/core/failure_reason.py
+trashcli/put/core/int_generator.py
+trashcli/put/core/logs.py
+trashcli/put/core/mode.py
+trashcli/put/core/path_maker_type.py
+trashcli/put/core/trash_all_result.py
+trashcli/put/core/trash_result.py
+trashcli/put/core/trashee.py
 trashcli/put/fs/__init__.py
 trashcli/put/fs/fs.py
 trashcli/put/fs/parent_realpath.py
 trashcli/put/fs/real_fs.py
 trashcli/put/fs/size_counter.py
 trashcli/put/fs/volume_of_parent.py
+trashcli/put/janitor_tools/__init__.py
+trashcli/put/janitor_tools/info_creator.py
+trashcli/put/janitor_tools/info_file_persister.py
+trashcli/put/janitor_tools/put_trash_dir.py
+trashcli/put/janitor_tools/security_check.py
+trashcli/put/janitor_tools/trash_dir_checker.py
+trashcli/put/janitor_tools/trash_dir_creator.py
 trashcli/restore/__init__.py
 trashcli/restore/args.py
 trashcli/restore/file_system.py
 trashcli/restore/handler.py
 trashcli/restore/index.py
 trashcli/restore/info_dir_searcher.py
 trashcli/restore/info_files.py
```

### Comparing `trash-cli-0.23.9.23/trashcli/empty/clock.py` & `trash_cli-0.24.4.17/trashcli/empty/clock.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/empty/console.py` & `trash_cli-0.24.4.17/trashcli/empty/console.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/empty/delete_according_date.py` & `trash_cli-0.24.4.17/trashcli/empty/delete_according_date.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/empty/emptier.py` & `trash_cli-0.24.4.17/trashcli/empty/emptier.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/empty/empty_action.py` & `trash_cli-0.24.4.17/trashcli/empty/empty_action.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, NamedTuple, List
+from typing import NamedTuple, List
 
 from trashcli.empty.clock import Clock
 from trashcli.empty.console import Console
 from trashcli.empty.delete_according_date import (
     DeleteAccordingDate,
 )
 from trashcli.empty.emptier import Emptier
@@ -11,29 +11,30 @@
 from trashcli.empty.parse_reply import parse_reply
 from trashcli.empty.prepare_output_message import prepare_output_message
 from trashcli.empty.user import User
 from trashcli.fs import ContentsOf
 from trashcli.fstab.volume_listing import VolumesListing
 from trashcli.fstab.volume_of import VolumeOf
 from trashcli.lib.dir_reader import DirReader
-from trashcli.lib.my_input import MyInput
+from trashcli.lib.environ import Environ
+from trashcli.lib.my_input import RealInput
 from trashcli.lib.trash_dir_reader import TrashDirReader
 from trashcli.list.trash_dir_selector import TrashDirsSelector
 from trashcli.trash_dirs_scanner import TopTrashDirRules
 
 
 class EmptyActionArgs(
     NamedTuple('EmptyActionArgs', [
         ('user_specified_trash_dirs', List[str]),
         ('all_users', bool),
         ('interactive', bool),
         ('days', int),
         ('dry_run', bool),
         ('verbose', int),
-        ('environ', Dict[str, str]),
+        ('environ', Environ),
         ('uid', int),
     ])):
     pass
 
 
 class EmptyAction:
     def __init__(self,
@@ -48,15 +49,15 @@
                  ):  # type: (...) -> None
         self.selector = TrashDirsSelector.make(volumes_listing,
                                                file_reader,
                                                volumes)
         trash_dir_reader = TrashDirReader(dir_reader)
         delete_mode = DeleteAccordingDate(content_reader,
                                           clock)
-        user = User(prepare_output_message, MyInput(), parse_reply)
+        user = User(prepare_output_message, RealInput(), parse_reply)
         self.emptier = Emptier(delete_mode, trash_dir_reader, file_remover,
                                console)
         self.guard = Guard(user)
 
     def run_action(self,
                    args,  # type: EmptyActionArgs
                    ):  # type: (...) -> None
```

### Comparing `trash-cli-0.23.9.23/trashcli/empty/empty_cmd.py` & `trash_cli-0.24.4.17/trashcli/empty/empty_cmd.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/empty/guard.py` & `trash_cli-0.24.4.17/trashcli/empty/guard.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/empty/main.py` & `trash_cli-0.24.4.17/trashcli/empty/main.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/empty/parser.py` & `trash_cli-0.24.4.17/trashcli/empty/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import argparse
-from typing import List, Dict
+
+from typing import List
 
 from trashcli.empty.empty_action import EmptyActionArgs
 from trashcli.empty.print_time_action import PrintTimeArgs
+from trashcli.lib.environ import Environ
 from trashcli.lib.print_version import PrintVersionArgs
 from trashcli.shell_completion import TRASH_DIRS, add_argument_to
 
 
 class Parser:
     def parse(self,
               default_is_interactive,  # type: bool
-              environ,  # type: Dict[str, str]
+              environ,  # type: Environ
               args,  # type: List[str]
               uid,  # type: int
               argv0,  # type: str
               ):
         parser = self.make_parser(default_is_interactive)
         namespace = parser.parse_args(args)
```

### Comparing `trash-cli-0.23.9.23/trashcli/empty/prepare_output_message.py` & `trash_cli-0.24.4.17/trashcli/empty/prepare_output_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,11 +5,11 @@
     result = []
     if trash_dirs:
         result.append("Would empty the following trash directories:")
         for event, args in trash_dirs:
             if event == trash_dir_found:
                 trash_dir, volume = args
                 result.append("    - %s" % trash_dir)
-        result.append("Proceed? (y/n) ")
+        result.append("Proceed? (y/N) ")
         return "\n".join(result)
     else:
         return 'No trash directories to empty.\n'
```

### Comparing `trash-cli-0.23.9.23/trashcli/empty/print_time_action.py` & `trash_cli-0.24.4.17/trashcli/empty/print_time_action.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Copyright (C) 2007-2023 Andrea Francia Trivolzio(PV) Italy
 from __future__ import print_function
 
-from typing import NamedTuple, Dict
+from typing import NamedTuple
+
+from trashcli.lib.environ import Environ
 
 
 class PrintTimeArgs(
     NamedTuple('PrintTimeArgs', [
-        ('environ', Dict[str, str]),
+        ('environ', Environ),
     ])):
     pass
 
 
 class PrintTimeAction:
     def __init__(self, out, clock):
         self.out = out
```

### Comparing `trash-cli-0.23.9.23/trashcli/file_system_reader.py` & `trash_cli-0.24.4.17/trashcli/file_system_reader.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/fs.py` & `trash_cli-0.24.4.17/trashcli/fs.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/fstab/mount_points_listing.py` & `trash_cli-0.24.4.17/trashcli/fstab/mount_points_listing.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         'nfs4',
         'p9',  # file system used in WSL 2 (Windows Subsystem for Linux)
         'btrfs',
         'fuse',  # https://github.com/andreafrancia/trash-cli/issues/250
         'fuse.glusterfs',
         # https://github.com/andreafrancia/trash-cli/issues/255
         'fuse.mergerfs',
+        'fuse.gocryptfs',
     ]
 
     # Append fstypes of physical devices to list
     fstypes += set([p.fstype for p in psutil.disk_partitions()])
 
     partitions = Partitions(fstypes)
```

### Comparing `trash-cli-0.23.9.23/trashcli/fstab/volume_listing.py` & `trash_cli-0.24.4.17/trashcli/fstab/volume_listing.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/fstab/volume_of.py` & `trash_cli-0.24.4.17/trashcli/fstab/volume_of.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/fstab/volumes.py` & `trash_cli-0.24.4.17/trashcli/fstab/volumes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABCMeta
 
 import six
-
+import os
 from trashcli.fstab.mount_points_listing import MountPointsListing, \
     RealMountPointsListing
 from trashcli.fstab.volume_of import VolumeOf, RealVolumeOf
 
 
 @six.add_metaclass(ABCMeta)
 class Volumes(VolumeOf, MountPointsListing):
@@ -32,25 +32,35 @@
         return self.volumes.volume_of(path)
 
     def list_mount_points(self):
         return self.mount_point_listing.list_mount_points()
 
 
 class FakeVolumes(Volumes):
-    def __init__(self, mount_points):
+    def __init__(self,
+                 mount_points,  # type Iterable[str]
+                 ):
         self.mount_points = mount_points
 
     def list_mount_points(self):
         return self.mount_points
 
     def volume_of(self, path):
-        for mount_point in self.mount_points:
-            if path.startswith(mount_point):
-                return mount_point
-        return "/"
+        while path != os.path.dirname(path):
+            if self.is_a_mount_point(path):
+                break
+            path = os.path.dirname(path)
+        return path
+
+    def is_a_mount_point(self, path):
+        return path in self.mount_points
+
+    def add_volume(self, path):
+        self.mount_points.append(path)
+
 
 class FakeVolumes2(Volumes):
     def __init__(self, volume_of_string, volumes_list):
         self.volume_of_string = volume_of_string
         self.volumes_list = volumes_list
 
     def volume_of(self, path):
```

### Comparing `trash-cli-0.23.9.23/trashcli/lib/my_input.py` & `trash_cli-0.24.4.17/trashcli/lib/my_input.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 @six.add_metaclass(ABCMeta)
 class Input:
     @abstractmethod
     def read_input(self, prompt):  # type: (str) -> str
         raise NotImplementedError
 
 
-class MyInput(Input):
+class RealInput(Input):
     def read_input(self, prompt):  # type: (str) -> str
         return _my_input(prompt)
 
 
 class HardCodedInput(Input):
     def __init__(self, reply=None):
         self.reply, self.exception = self._reply(reply)
```

### Comparing `trash-cli-0.23.9.23/trashcli/lib/print_version.py` & `trash_cli-0.24.4.17/trashcli/lib/print_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         ('argv0', str),
     ])):
 
     def program_name(self):
         return os.path.basename(self.argv0)
 
 
-class PrintVersionAction:
+class PrintVersionAction(object):
     def __init__(self, out, version):
         self.out = out
         self.version = version
 
     def run_action(self,
                    args,  # type: PrintVersionArgs
                    ):
```

### Comparing `trash-cli-0.23.9.23/trashcli/lib/trash_dir_reader.py` & `trash_cli-0.24.4.17/trashcli/lib/trash_dir_reader.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/lib/trash_dirs.py` & `trash_cli-0.24.4.17/trashcli/lib/trash_dirs.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/lib/user_info.py` & `trash_cli-0.24.4.17/trashcli/lib/user_info.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/list/extractors.py` & `trash_cli-0.24.4.17/trashcli/list/extractors.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/list/list_trash_action.py` & `trash_cli-0.24.4.17/trashcli/list/list_trash_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from __future__ import print_function
 
 import os
-
-from typing import NamedTuple, List
+from typing import List
+from typing import NamedTuple
 
 from trashcli.lib.dir_reader import DirReader
 from trashcli.lib.path_of_backup_copy import path_of_backup_copy
 from trashcli.lib.trash_dir_reader import TrashDirReader
-from trashcli.list.extractors import DeletionDateExtractor, SizeExtractor
+from trashcli.list.extractors import DeletionDateExtractor
+from trashcli.list.extractors import SizeExtractor
 from trashcli.parse_trashinfo.parse_path import parse_path
 from trashcli.parse_trashinfo.parser_error import ParseError
-from trashcli.trash_dirs_scanner import trash_dir_found, \
-    trash_dir_skipped_because_parent_not_sticky, \
+from trashcli.trash_dirs_scanner import trash_dir_found
+from trashcli.trash_dirs_scanner import \
     trash_dir_skipped_because_parent_is_symlink
+from trashcli.trash_dirs_scanner import \
+    trash_dir_skipped_because_parent_not_sticky
 
 
 class ListTrashArgs(
     NamedTuple('ListTrashArgs', [
         ('trash_dirs', List[str]),
         ('attribute_to_print', str),
         ('show_files', bool),
@@ -90,33 +93,33 @@
                                           self.environ,
                                           self.uid)
         for event, event_args in trash_dirs:
             if event == trash_dir_found:
                 path, volume = event_args
                 trash_dir = TrashDirReader(self.dir_reader)
                 for trash_info in trash_dir.list_trashinfo(path):
-                    for msg in self.print_trashinfo(volume, trash_info,
-                                                    extractor, show_files):
+                    for msg in self._print_trashinfo(volume, trash_info,
+                                                     extractor, show_files):
                         yield msg
             elif event == trash_dir_skipped_because_parent_not_sticky:
                 path, = event_args
                 msg = Error(
                     self.top_trashdir_skipped_because_parent_not_sticky(path))
                 yield msg
             elif event == trash_dir_skipped_because_parent_is_symlink:
                 path, = event_args
                 msg = Error(
                     self.top_trashdir_skipped_because_parent_is_symlink(path))
                 yield msg
 
-    def print_trashinfo(self,
-                        volume,
-                        trashinfo_path,
-                        extractor,
-                        show_files):
+    def _print_trashinfo(self,
+                         volume,
+                         trashinfo_path,
+                         extractor,
+                         show_files):
         try:
             contents = self.content_reader.contents_of(trashinfo_path)
         except IOError as e:
             yield Error(str(e))
         else:
             try:
                 relative_location = parse_path(contents)
```

### Comparing `trash-cli-0.23.9.23/trashcli/list/main.py` & `trash_cli-0.24.4.17/trashcli/list/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,16 @@
         self.volumes_listing = volumes_listing
         self.selector = TrashDirsSelector.make(volumes_listing,
                                                file_reader,
                                                volumes)
         self.actions = {PrintVersionArgs: PrintVersionAction(self.out,
                                                              self.version),
                         PrintVolumesArgs: PrintVolumesList(self.environ,
-                                                           self.volumes_listing),
+                                                           self.volumes_listing,
+                                                           self.out),
                         DebugVolumesArgs: DebugVolumes(),
                         ListTrashDirsArgs: ListTrashDirs(self.environ,
                                                          self.uid,
                                                          self.selector),
                         ListTrashArgs: ListTrashAction(self.environ,
                                                        self.uid,
                                                        self.selector,
```

### Comparing `trash-cli-0.23.9.23/trashcli/list/minor_actions/debug_volumes.py` & `trash_cli-0.24.4.17/trashcli/list/minor_actions/debug_volumes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from pprint import pprint
 
+
 class DebugVolumesArgs:
     pass
 
-class DebugVolumes:
+
+class DebugVolumes(object):
     def run_action(self,
-                   _args, # type: DebugVolumesArgs
+                   _args,  # type: DebugVolumesArgs
                    ):
         import psutil
         import os
         all = sorted([p for p in psutil.disk_partitions(all=True)],
                      key=lambda p: p.device)
         physical = sorted([p for p in psutil.disk_partitions()],
                           key=lambda p: p.device)
```

### Comparing `trash-cli-0.23.9.23/trashcli/list/minor_actions/list_trash_dirs.py` & `trash_cli-0.24.4.17/trashcli/list/minor_actions/list_trash_dirs.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/list/parser.py` & `trash_cli-0.24.4.17/trashcli/list/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import argparse
+from enum import Enum
 from typing import List, Union
 
 from trashcli.lib.print_version import PrintVersionArgs
 from trashcli.list.list_trash_action import ListTrashArgs
 from trashcli.list.minor_actions.debug_volumes import DebugVolumesArgs
 from trashcli.list.minor_actions.list_trash_dirs import ListTrashDirsArgs
 from trashcli.list.minor_actions.list_volumes import PrintVolumesArgs
 from trashcli.list.minor_actions.print_python_executable import \
     PrintPythonExecutableArgs
 from trashcli.shell_completion import add_argument_to, TRASH_DIRS
-from trashcli.super_enum import SuperEnum
 
 Args = Union[
     PrintVersionArgs,
     PrintVolumesArgs,
     DebugVolumesArgs,
     ListTrashDirsArgs,
     ListTrashArgs,
@@ -26,31 +26,31 @@
         self.parser = argparse.ArgumentParser(prog=prog,
                                               description='List trashed files',
                                               epilog='Report bugs to https://github.com/andreafrancia/trash-cli/issues')
         add_argument_to(self.parser)
         self.parser.add_argument('--version',
                                  dest='action',
                                  action='store_const',
-                                 const=Action.print_version,
-                                 default=Action.list_trash,
+                                 const=ListAction.print_version,
+                                 default=ListAction.list_trash,
                                  help="show program's version number and exit")
         self.parser.add_argument('--debug-volumes',
                                  dest='action',
                                  action='store_const',
-                                 const=Action.debug_volumes,
+                                 const=ListAction.debug_volumes,
                                  help=argparse.SUPPRESS)
         self.parser.add_argument('--volumes',
                                  dest='action',
                                  action='store_const',
-                                 const=Action.list_volumes,
+                                 const=ListAction.list_volumes,
                                  help="list volumes")
         self.parser.add_argument('--trash-dirs',
                                  dest='action',
                                  action='store_const',
-                                 const=Action.list_trash_dirs,
+                                 const=ListAction.list_trash_dirs,
                                  help="list trash dirs")
         self.parser.add_argument('--trash-dir',
                                  action='append',
                                  default=[],
                                  dest='trash_dirs',
                                  help='specify the trash directory to use'
                                  ).complete = TRASH_DIRS
@@ -68,48 +68,48 @@
         self.parser.add_argument('--all-users',
                                  action='store_true',
                                  dest='all_users',
                                  help='list trashcans of all the users')
         self.parser.add_argument('--python',
                                  dest='action',
                                  action='store_const',
-                                 const=Action.print_python_executable,
+                                 const=ListAction.print_python_executable,
                                  help=argparse.SUPPRESS)
 
     def parse_list_args(self,
                         args,  # type: List[str]
                         argv0,  # type: str
                         ):  # type: (...) -> Args
 
         parsed = self.parser.parse_args(args)
 
-        if parsed.action == Action.print_version:
+        if parsed.action == ListAction.print_version:
             return PrintVersionArgs(argv0=argv0)
-        if parsed.action == Action.list_volumes:
+        if parsed.action == ListAction.list_volumes:
             return PrintVolumesArgs()
-        if parsed.action == Action.debug_volumes:
+        if parsed.action == ListAction.debug_volumes:
             return DebugVolumesArgs()
-        if parsed.action == Action.list_trash_dirs:
+        if parsed.action == ListAction.list_trash_dirs:
             return ListTrashDirsArgs(
                 trash_dirs=parsed.trash_dirs,
                 all_users=parsed.all_users
             )
-        if parsed.action == Action.list_trash:
+        if parsed.action == ListAction.list_trash:
             return ListTrashArgs(
                 trash_dirs=parsed.trash_dirs,
                 attribute_to_print=parsed.attribute_to_print,
                 show_files=parsed.show_files,
                 all_users=parsed.all_users
             )
-        if parsed.action == Action.print_python_executable:
+        if parsed.action == ListAction.print_python_executable:
             return PrintPythonExecutableArgs()
 
         raise ValueError('Unknown action: {}'.format(parsed.action))
 
 
-class Action(SuperEnum):
+class ListAction(Enum):
     debug_volumes = 'debug_volumes'
     print_version = 'print_version'
     list_trash = 'list_trash'
     list_volumes = 'list_volumes'
     list_trash_dirs = 'list_trash_dirs'
     print_python_executable = 'print_python_executable'
```

### Comparing `trash-cli-0.23.9.23/trashcli/list/trash_dir_selector.py` & `trash_cli-0.24.4.17/trashcli/list/trash_dir_selector.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/parse_trashinfo/maybe_parse_deletion_date.py` & `trash_cli-0.24.4.17/trashcli/parse_trashinfo/maybe_parse_deletion_date.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/parse_trashinfo/parse_trashinfo.py` & `trash_cli-0.24.4.17/trashcli/parse_trashinfo/parse_trashinfo.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/put/describer.py` & `trash_cli-0.24.4.17/trashcli/put/describer.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/put/file_trasher.py` & `trash_cli-0.24.4.17/trashcli/put/file_trasher.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,73 @@
 # Copyright (C) 2007-2023 Andrea Francia Trivolzio(PV) Italy
-from typing import Dict
 
 from trashcli.fstab.volume_of import VolumeOf
-from trashcli.put.fs.parent_realpath import ParentRealpath
+from trashcli.lib.environ import Environ
+from trashcli.put.context import Context
+from trashcli.put.core.trash_result import TrashResult
+from trashcli.put.core.trashee import Trashee
+from trashcli.put.fs.parent_realpath import ParentRealpathFs
 from trashcli.put.fs.volume_of_parent import VolumeOfParent
-from trashcli.put.my_logger import MyLogger, LogData
+from trashcli.put.janitor import Janitor
+from trashcli.put.my_logger import LogData
+from trashcli.put.my_logger import MyLogger
 from trashcli.put.reporter import TrashPutReporter
 from trashcli.put.trash_directories_finder import TrashDirectoriesFinder
-from trashcli.put.trash_file_in import TrashFileIn
-from trashcli.put.trash_result import TrashResult
-from trashcli.put.trashee import Trashee
 
 
 class FileTrasher:
 
     def __init__(self,
                  volumes,  # type: VolumeOf
                  trash_directories_finder,  # type: TrashDirectoriesFinder
-                 parent_realpath,  # type: ParentRealpath
+                 parent_realpath_fs,  # type: ParentRealpathFs
                  logger,  # type: MyLogger
                  reporter,  # type: TrashPutReporter
-                 trash_file_in,  # type: TrashFileIn
+                 janitor,  # type: Janitor
                  volume_of_parent,  # type: VolumeOfParent
                  ):  # type: (...) -> None
         self.volumes = volumes
         self.trash_directories_finder = trash_directories_finder
-        self.parent_realpath = parent_realpath
+        self.parent_realpath_fs = parent_realpath_fs
         self.logger = logger
         self.reporter = reporter
-        self.trash_file_in = trash_file_in
+        self.janitor = janitor
         self.volume_of_parent = volume_of_parent or volume_of_parent
 
     def trash_file(self,
                    path,  # type: str
-                   forced_volume,
-                   user_trash_dir,
-                   home_fallback,
-                   result,  # type: TrashResult
-                   environ,  # type: Dict[str, str]
-                   uid,  # type: int
-                   log_data,  # type: LogData
+                   context,  # type: Context
                    ):
-        volume_of_file_to_be_trashed = forced_volume or \
-                                       self.volume_of_parent.volume_of_parent(
-                                           path)
-        file_be_trashed = Trashee(path, volume_of_file_to_be_trashed)
-        candidates = self.trash_directories_finder. \
-            possible_trash_directories_for(volume_of_file_to_be_trashed,
+        volume = self._figure_out_volume(path, context.forced_volume)
+        trashee = Trashee(path, volume)
+        candidates = self._select_candidates(volume, context.user_trash_dir,
+                                             context.environ,
+                                             context.uid, context.home_fallback)
+        failures = []
+        for candidate in candidates:
+            self.reporter.trash_dir_with_volume(candidate, context.log_data)
+            trashing = self.janitor.trash_file_in(
+                candidate, context.log_data, context.environ, trashee)
+            if trashing.succeeded():
+                self.reporter.file_has_been_trashed_in_as(path,
+                                                          candidate,
+                                                          context.log_data,
+                                                          context.environ)
+                return TrashResult.Success
+            else:
+                failures.append((candidate, trashing.reason))
+        self.reporter.unable_to_trash_file2(trashee, context.log_data, failures,
+                                            context.environ)
+        return TrashResult.Failure
+
+    def _figure_out_volume(self, path, default_volume):
+        if default_volume:
+            return default_volume
+        else:
+            return self.volume_of_parent.volume_of_parent(path)
+
+    def _select_candidates(self, volume, user_trash_dir, environ, uid,
+                           home_fallback):
+        return self.trash_directories_finder. \
+            possible_trash_directories_for(volume,
                                            user_trash_dir, environ, uid,
                                            home_fallback)
-        self.reporter.volume_of_file(volume_of_file_to_be_trashed, log_data)
-        file_has_been_trashed = False
-        for candidate in candidates:
-            file_has_been_trashed = file_has_been_trashed or \
-                                    self.trash_file_in.trash_file_in(candidate,
-                                                                     log_data,
-                                                                     environ,
-                                                                     file_be_trashed)
-            if file_has_been_trashed: break
-
-        if not file_has_been_trashed:
-            result = result.mark_unable_to_trash_file()
-            self.reporter.unable_to_trash_file(path, log_data)
-
-        return result
```

### Comparing `trash-cli-0.23.9.23/trashcli/put/format_trash_info.py` & `trash_cli-0.24.4.17/trashcli/put/format_trash_info.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/put/fs/real_fs.py` & `trash_cli-0.24.4.17/trashcli/put/fs/real_fs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,54 @@
+import grp
 import os
+import pwd
 import stat
+from typing import NamedTuple
+from typing import Optional
 
 from trashcli import fs
 from trashcli.fs import write_file
 from trashcli.put.fs.fs import Fs
 
 
+class Names:
+    def username(self, uid):  # type: (int) -> Optional[str]
+        try:
+            return pwd.getpwuid(uid).pw_name
+        except KeyError as e:
+            return None
+
+    def groupname(self, gid):
+        try:
+            return grp.getgrgid(gid).gr_name
+        except KeyError as e:
+            return None
+
+
+class Stat(NamedTuple('Stat', [
+    ('mode', int),
+    ('uid', int),
+    ('gid', int),
+])):
+    pass
+
+
 class RealFs(Fs):
 
+    def readlink(self, path):
+        return os.readlink(path)
+
+    def symlink(self, src, dest):  # type: (str, str) -> None
+        os.symlink(src, dest)
+
+    def touch(self, path):  # type: (str) -> None
+        with open(path, 'a'):
+            import os
+            os.utime(path, None)
+
     def atomic_write(self, path, content):
         fs.atomic_write(path, content)
 
     def chmod(self, path, mode):
         os.chmod(path, mode)
 
     def isdir(self, path):
@@ -34,14 +71,24 @@
 
     def exists(self, path):
         return os.path.exists(path)
 
     def makedirs(self, path, mode):
         os.makedirs(path, mode)
 
+    def lstat(self, path):
+        stat = os.lstat(path)
+        return Stat(mode=stat.st_mode, uid=stat.st_uid, gid=stat.st_gid)
+
+    def mkdir(self, path):
+        os.mkdir(path)
+
+    def mkdir_with_mode(self, path, mode):
+        os.mkdir(path, mode)
+
     def move(self, path, dest):
         return fs.move(path, dest)
 
     def remove_file(self, path):
         fs.remove_file(path)
 
     def islink(self, path):
```

### Comparing `trash-cli-0.23.9.23/trashcli/put/fs/size_counter.py` & `trash_cli-0.24.4.17/trashcli/put/fs/size_counter.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/put/fs/volume_of_parent.py` & `trash_cli-0.24.4.17/trashcli/put/fs/volume_of_parent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from trashcli.fstab.volume_of import VolumeOf
-from trashcli.put.fs.parent_realpath import ParentRealpath
+from trashcli.put.fs.parent_realpath import ParentRealpathFs
 
 
 class VolumeOfParent:
     def __init__(self,
                  volumes,  # type: VolumeOf
-                 parent_realpath,  # type: ParentRealpath
+                 parent_realpath_fs,  # type: ParentRealpathFs
                  ):
         self.volumes = volumes
-        self.parent_realpath = parent_realpath
+        self.parent_realpath_fs = parent_realpath_fs
 
     def volume_of_parent(self, path):
-        parent_realpath = self.parent_realpath.parent_realpath(path)
+        parent_realpath = self.parent_realpath_fs.parent_realpath(path)
         return self.volumes.volume_of(parent_realpath)
```

### Comparing `trash-cli-0.23.9.23/trashcli/put/info_dir.py` & `trash_cli-0.24.4.17/trashcli/put/janitor_tools/info_file_persister.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,80 @@
 import errno
 import os
+from typing import NamedTuple, Iterator
 
+from trashcli.lib.path_of_backup_copy import path_of_backup_copy
 from trashcli.put.fs.fs import Fs
-from trashcli.put.my_logger import MyLogger, LogData
+from trashcli.put.jobs import JobStatus, NeedsMoreAttempts, Succeeded, \
+    JobExecutor
+from trashcli.put.my_logger import LogData, MyLogger
 from trashcli.put.suffix import Suffix
-from trashcli.lib.path_of_backup_copy import path_of_backup_copy
 
 
-class InfoDir:
+class TrashinfoData(NamedTuple('TrashinfoData', [
+    ('basename', str),
+    ('content', str),
+    ('info_dir_path', str),
+])):
+    pass
+
+
+class TrashedFile(NamedTuple('TrashedFile', [
+    ('trashinfo_path', str),
+])):
+    @property
+    def backup_copy_path(self):  # type: () -> str
+        return path_of_backup_copy(self.trashinfo_path)
+
+
+class InfoFilePersister:
     def __init__(self,
                  fs,  # type: Fs
                  logger,  # type: MyLogger
                  suffix,  # type: Suffix
                  ):  # type: (...) -> None
         self.fs = fs
         self.logger = logger
         self.suffix = suffix
 
-    def persist_trash_info(self,
-                           basename, #type: str
-                           content, #type: str
-                           log_data, #type: LogData
-                           info_dir_path, #type: str
-                           ):
-        """
-        Create a .trashinfo file in the $trash/info directory.
-        returns the created TrashInfoFile.
-        """
-
-        index = -1
+    def create_trashinfo_file(self,
+                              trashinfo_data,  # type: TrashinfoData
+                              log_data,  # type: LogData
+                              ):  # type: (...) -> TrashedFile
+        return JobExecutor(self.logger, TrashedFile).execute(
+            self.try_persist(trashinfo_data), log_data)
+
+    Result = Iterator[JobStatus[TrashedFile]]
+
+    def try_persist(self,
+                    data,  # type: TrashinfoData
+                    ):  # type: (...) -> Result
+        index = 0
         name_too_long = False
         while True:
-            index += 1
-
             suffix = self.suffix.suffix_for_index(index)
-            trashinfo_basename = create_trashinfo_basename(basename,
+            trashinfo_basename = create_trashinfo_basename(data.basename,
                                                            suffix,
                                                            name_too_long)
-            trashinfo_path = os.path.join(info_dir_path, trashinfo_basename)
+            trashinfo_path = os.path.join(data.info_dir_path,
+                                          trashinfo_basename)
             if os.path.exists(path_of_backup_copy(trashinfo_path)):
+                index += 1
                 continue
             try:
-                self.fs.atomic_write(trashinfo_path, content)
-                self.logger.debug(".trashinfo created as %s." % trashinfo_path,
-                                  log_data)
-                return trashinfo_path
+                self.fs.atomic_write(trashinfo_path, data.content)
+                yield Succeeded(TrashedFile(trashinfo_path),
+                                ".trashinfo created as %s." % trashinfo_path)
             except OSError as e:
                 if e.errno == errno.ENAMETOOLONG:
                     name_too_long = True
-                self.logger.debug(
-                    "attempt for creating %s failed." % trashinfo_path,
-                    log_data)
+                yield NeedsMoreAttempts(trashinfo_path,
+                                        "attempt for creating %s failed." % trashinfo_path)
 
+            index += 1
 
 
 def create_trashinfo_basename(basename, suffix, name_too_long):
     after_basename = suffix + ".trashinfo"
     if name_too_long:
         truncated_basename = basename[0:len(basename) - len(after_basename)]
     else:
```

### Comparing `trash-cli-0.23.9.23/trashcli/put/main.py` & `trash_cli-0.24.4.17/trashcli/put/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,91 @@
 import os
 import random
 import sys
 
 from trashcli.fstab.volume_of import RealVolumeOf
-from trashcli.lib.my_input import MyInput
+from trashcli.lib.environ import cast_environ
+from trashcli.lib.my_input import Input
+from trashcli.lib.my_input import RealInput
 from trashcli.put.clock import RealClock
+from trashcli.put.core.int_generator import IntGenerator
 from trashcli.put.describer import Describer
-from trashcli.put.dir_maker import DirMaker
 from trashcli.put.file_trasher import FileTrasher
-from trashcli.put.fs.parent_realpath import ParentRealpath
+from trashcli.put.fs.fs import Fs
+from trashcli.put.fs.parent_realpath import ParentRealpathFs
 from trashcli.put.fs.real_fs import RealFs
 from trashcli.put.fs.volume_of_parent import VolumeOfParent
-from trashcli.put.gate import ClosedGate, HomeFallbackGate, SameVolumeGate
-from trashcli.put.gate_impl import ClosedGateImpl, HomeFallbackGateImpl, \
-    SameVolumeGateImpl
-from trashcli.put.info_dir import InfoDir
+from trashcli.put.janitor import Janitor
+from trashcli.put.janitor_tools.info_creator import \
+    TrashInfoCreator
+from trashcli.put.janitor_tools.info_file_persister import InfoFilePersister
+from trashcli.put.janitor_tools.put_trash_dir import PutTrashDir
+from trashcli.put.janitor_tools.trash_dir_checker import TrashDirChecker
+from trashcli.put.my_logger import LoggerBackend
 from trashcli.put.my_logger import MyLogger
+from trashcli.put.my_logger import StreamBackend
 from trashcli.put.original_location import OriginalLocation
-from trashcli.put.path_maker import PathMaker
 from trashcli.put.reporter import TrashPutReporter
 from trashcli.put.suffix import Suffix
 from trashcli.put.trash_all import TrashAll
-from trashcli.put.trash_dir_volume_reader import TrashDirVolumeReader
 from trashcli.put.trash_directories_finder import TrashDirectoriesFinder
-from trashcli.put.trash_directory_for_put import TrashDirectoryForPut
-from trashcli.put.trash_file_in import TrashFileIn
 from trashcli.put.trash_put_cmd import TrashPutCmd
 from trashcli.put.trasher import Trasher
-from trashcli.put.trashing_checker import TrashingChecker
 from trashcli.put.user import User
 
 
 def main():
-    cmd = make_cmd(clock=RealClock(), fs=RealFs(),
-                   my_input=MyInput(), randint=random.randint,
-                   stderr=sys.stderr, volumes=RealVolumeOf())
-    return cmd.run(sys.argv, os.environ, os.getuid())
+    cmd = make_cmd(clock=RealClock(),
+                   fs=RealFs(),
+                   user_input=RealInput(),
+                   randint=RandomIntGenerator(),
+                   backend=StreamBackend(sys.stderr),
+                   volumes=RealVolumeOf())
+    try:
+        uid = int(os.environ["TRASH_PUT_FAKE_UID_FOR_TESTING"])
+    except KeyError:
+        uid = os.getuid()
+    return cmd.run_put(sys.argv, cast_environ(os.environ), uid)
 
 
 def make_cmd(clock,
-             fs,
-             my_input, # type: MyInput
-             randint,
-             stderr,
-             volumes):
-    logger = MyLogger(stderr)
+             fs,  # type: Fs
+             user_input,  # type: Input
+             randint,  # type: IntGenerator
+             backend,  # type: LoggerBackend
+             volumes,
+             ):  # type: (...) -> TrashPutCmd
+    logger = MyLogger(backend)
     describer = Describer(fs)
     reporter = TrashPutReporter(logger, describer)
     suffix = Suffix(randint)
-    dir_maker = DirMaker(fs)
-    info_dir = InfoDir(fs, logger, suffix)
-    path_maker = PathMaker()
-    parent_realpath = ParentRealpath(fs)
-    original_location = OriginalLocation(parent_realpath, path_maker)
-    trash_dir = TrashDirectoryForPut(fs,
-                                     info_dir,
-                                     original_location,
-                                     clock)
-    trash_dir_volume = TrashDirVolumeReader(volumes, fs)
-    trashing_checker = TrashingChecker({
-        ClosedGate: ClosedGateImpl(),
-        HomeFallbackGate: HomeFallbackGateImpl(fs),
-        SameVolumeGate: SameVolumeGateImpl(trash_dir_volume),
-    })
-    trash_file_in = TrashFileIn(fs,
-                                reporter,
-                                trash_dir,
-                                trashing_checker,
-                                dir_maker)
-    volume_of_parent = VolumeOfParent(volumes, parent_realpath)
+    persister = InfoFilePersister(fs, logger, suffix)
+    original_location = OriginalLocation(fs)
+    info_dir2 = TrashInfoCreator(persister, original_location, clock)
+    trash_dir = PutTrashDir(fs)
+    trashing_checker = TrashDirChecker(fs, volumes)
+    janitor = Janitor(fs,
+                      trash_dir,
+                      trashing_checker,
+                      info_dir2,
+                      persister,
+                      logger)
+    volume_of_parent = VolumeOfParent(volumes, ParentRealpathFs(fs))
     file_trasher = FileTrasher(volumes,
                                TrashDirectoriesFinder(volumes),
-                               parent_realpath,
+                               ParentRealpathFs(fs),
                                logger,
                                reporter,
-                               trash_file_in,
+                               janitor,
                                volume_of_parent)
-    user = User(my_input, describer)
+    user = User(user_input, describer)
     trasher = Trasher(file_trasher, user, reporter, fs)
     trash_all = TrashAll(logger, trasher)
     return TrashPutCmd(trash_all, reporter)
+
+
+class RandomIntGenerator(IntGenerator):
+    def new_int(self,
+                min,  # type: int
+                max,  # type: int
+                ):
+        return random.randint(min, max)
```

### Comparing `trash-cli-0.23.9.23/trashcli/put/parser.py` & `trash_cli-0.24.4.17/trashcli/put/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import os
-from argparse import SUPPRESS, ArgumentParser, RawDescriptionHelpFormatter
-from typing import NamedTuple, Any, Union, List, Optional
-
-from trashcli.shell_completion import TRASH_DIRS, TRASH_FILES, add_argument_to
+import pprint
+from argparse import ArgumentParser
+from argparse import RawDescriptionHelpFormatter
+from argparse import SUPPRESS
+from typing import Any
+from typing import List
+from typing import NamedTuple
+from typing import Optional
+from typing import Union
+
+from trashcli.put.core.mode import Mode
+from trashcli.shell_completion import TRASH_DIRS
+from trashcli.shell_completion import TRASH_FILES
+from trashcli.shell_completion import add_argument_to
 from trashcli.trash import version
 
-mode_force = 'force'
-mode_interactive = 'interactive'
-
 ExitWithCode = NamedTuple('ExitWithCode', [
     ('type', type),
-    ('exit_code', Union[str, int, None]),
+    ('exit_code', int),
 ])
 
 Trash = NamedTuple('Trash', [
     ('type', type),
     ('program_name', str),
     ('options', Any),
     ('files', List[str]),
     ('trash_dir', Optional[str]),
-    ('mode', str),
+    ('mode', Mode),
     ('forced_volume', Optional[str]),
     ('verbose', int),
     ('home_fallback', bool),
 ])
 
 
 class Parser:
@@ -32,33 +39,46 @@
         program_name = os.path.basename(argv[0])
         arg_parser = make_parser(program_name)
         try:
             options = arg_parser.parse_args(argv[1:])
             if len(options.files) <= 0:
                 arg_parser.error("Please specify the files to trash.")
         except SystemExit as e:
-            return ExitWithCode(type=ExitWithCode, exit_code=e.code)
+            return ExitWithCode(type=ExitWithCode, exit_code=ensure_int(e.code))
 
         return Trash(type=Trash,
                      program_name=program_name,
                      options=options,
                      files=options.files,
                      trash_dir=options.trashdir,
                      mode=options.mode,
                      forced_volume=options.forced_volume,
                      verbose=options.verbose,
                      home_fallback=options.home_fallback)
 
 
+def ensure_int(code):
+    if not isinstance(code, int):
+        raise ValueError("code must be an int, got %s" % pprint.pformat(code))
+    return code
+
+
 def make_parser(program_name):
     parser = ArgumentParser(prog=program_name,
                             usage="%(prog)s [OPTION]... FILE...",
                             description="Put files in trash",
                             formatter_class=RawDescriptionHelpFormatter,
                             epilog="""\
+all trash-cli commands:
+  trash-put             trash files and directories.
+  trash-empty           empty the trashcan(s).
+  trash-list            list trashed files.
+  trash-restore         restore a trashed file.
+  trash-rm              remove individual files from the trashcan
+
 To remove a file whose name starts with a '-', for example '-foo',
 use one of these commands:
 
     trash -- -foo
 
     trash ./-foo
 
@@ -66,20 +86,22 @@
     add_argument_to(parser)
     parser.add_argument("-d", "--directory",
                         action="store_true",
                         help="ignored (for GNU rm compatibility)")
     parser.add_argument("-f", "--force",
                         action="store_const",
                         dest="mode",
-                        const=mode_force,
+                        const=Mode.mode_force,
+                        default=Mode.mode_unspecified,
                         help="silently ignore nonexistent files")
     parser.add_argument("-i", "--interactive",
                         action="store_const",
                         dest="mode",
-                        const=mode_interactive,
+                        const=Mode.mode_interactive,
+                        default=Mode.mode_unspecified,
                         help="prompt before every removal")
     parser.add_argument("-r", "-R", "--recursive",
                         action="store_true",
                         help="ignored (for GNU rm compatibility)")
     parser.add_argument("--trash-dir",
                         type=str,
                         action="store", dest='trashdir',
```

### Comparing `trash-cli-0.23.9.23/trashcli/put/trash_directories_finder.py` & `trash_cli-0.24.4.17/trashcli/put/trash_directories_finder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 # Copyright (C) 2007-2023 Andrea Francia Trivolzio(PV) Italy
-from typing import Dict, List
+from typing import List
 
 from trashcli.fstab.volume_of import VolumeOf
+from trashcli.lib.environ import Environ
 from trashcli.lib.trash_dirs import (
     volume_trash_dir1, volume_trash_dir2, home_trash_dir)
-from trashcli.put.candidate import Candidate
-from trashcli.put.gate import SameVolumeGate, HomeFallbackGate
-from trashcli.put.path_maker import AbsolutePaths, RelativePaths
-from trashcli.put.security_check import NoCheck, TopTrashDirCheck
+from trashcli.put.core.candidate import Candidate
+from trashcli.put.core.check_type import NoCheck, TopTrashDirCheck
+from trashcli.put.core.path_maker_type import PathMakerType
+from trashcli.put.gate import Gate
 
 
 class TrashDirectoriesFinder:
     def __init__(self,
                  volumes,  # type: VolumeOf
                  ):
         self.volumes = volumes
 
     def possible_trash_directories_for(self,
                                        volume,  # type: str
                                        specific_trash_dir,  # type: str
-                                       environ,  # type: Dict[str, str]
+                                       environ,  # type: Environ
                                        uid,  # type: int
                                        home_fallback,  # type: bool
                                        ):  # type: (...) -> List[Candidate]
         trash_dirs = []
 
         def add_home_trash(path, volume, gate):
             trash_dirs.append(
                 Candidate(trash_dir_path=path,
                           volume=volume,
-                          path_maker_type=AbsolutePaths,
+                          path_maker_type=PathMakerType.AbsolutePaths,
                           check_type=NoCheck,
                           gate=gate))
 
         def add_top_trash_dir(path, volume):
             trash_dirs.append(
                 Candidate(trash_dir_path=path,
                           volume=volume,
-                          path_maker_type=RelativePaths,
+                          path_maker_type=PathMakerType.RelativePaths,
                           check_type=TopTrashDirCheck,
-                          gate=SameVolumeGate))
+                          gate=Gate.SameVolume))
 
         def add_alt_top_trash_dir(path, volume):
             trash_dirs.append(
                 Candidate(trash_dir_path=path,
                           volume=volume,
-                          path_maker_type=RelativePaths,
+                          path_maker_type=PathMakerType.RelativePaths,
                           check_type=NoCheck,
-                          gate=SameVolumeGate))
+                          gate=Gate.SameVolume))
 
         if specific_trash_dir:
             path = specific_trash_dir
             volume = self.volumes.volume_of(path)
             trash_dirs.append(
                 Candidate(trash_dir_path=path,
                           volume=volume,
-                          path_maker_type=RelativePaths,
+                          path_maker_type=PathMakerType.RelativePaths,
                           check_type=NoCheck,
-                          gate=SameVolumeGate))
+                          gate=Gate.SameVolume))
         else:
             for path, dir_volume in home_trash_dir(environ,
                                                    self.volumes):
-                add_home_trash(path, dir_volume, SameVolumeGate)
+                add_home_trash(path, dir_volume, Gate.SameVolume)
             for path, dir_volume in volume_trash_dir1(volume, uid):
                 add_top_trash_dir(path, dir_volume)
             for path, dir_volume in volume_trash_dir2(volume, uid):
                 add_alt_top_trash_dir(path, dir_volume)
             if home_fallback:
                 for path, dir_volume in home_trash_dir(environ,
                                                        self.volumes):
-                    add_home_trash(path, dir_volume, HomeFallbackGate)
+                    add_home_trash(path, dir_volume, Gate.HomeFallback)
         return trash_dirs
```

### Comparing `trash-cli-0.23.9.23/trashcli/put/trash_directory_for_put.py` & `trash_cli-0.24.4.17/trashcli/put/janitor_tools/info_creator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 import os
+from typing import NamedTuple
 
-from trashcli.put.candidate import Candidate
 from trashcli.put.clock import PutClock
+from trashcli.put.core.candidate import Candidate
+from trashcli.put.core.either import Either, Right, Left
+from trashcli.put.core.failure_reason import FailureReason
+from trashcli.put.core.failure_reason import LogContext
 from trashcli.put.format_trash_info import format_trashinfo
-from trashcli.put.fs.fs import Fs
-from trashcli.put.info_dir import InfoDir
-from trashcli.put.my_logger import LogData
+from trashcli.put.janitor_tools.info_file_persister import InfoFilePersister
+from trashcli.put.janitor_tools.info_file_persister import TrashinfoData
 from trashcli.put.original_location import OriginalLocation
-from trashcli.lib.path_of_backup_copy import path_of_backup_copy
 
 
-class TrashDirectoryForPut:
+class UnableToCreateTrashInfoContent(
+    NamedTuple('UnableToCreateTrashInfoContent', [
+        ('error', Exception),
+    ]), FailureReason):
+    def log_entries(self, context):  # type: (LogContext) -> str
+        return "failed to generate trashinfo content: %s" % (
+            self.error)
+
+
+class TrashInfoCreator:
     def __init__(self,
-                 fs,  # type: Fs
-                 info_dir,  # type: InfoDir
+                 persister,  # type: InfoFilePersister
                  original_location,  # type: OriginalLocation
                  clock,  # type: PutClock
                  ):
-        self.fs = fs
-        self.info_dir = info_dir
         self.original_location = original_location
         self.clock = clock
 
-    def trash2(self,
-               path,
-               candidate,  # type: Candidate
-               log_data,  # type: LogData
-               ):
-        original_location = self.original_location.for_file(
-            path, candidate.path_maker_type, candidate.volume)
-        basename = os.path.basename(original_location)
-        content = format_trashinfo(original_location, self.clock.now())
-        trash_info_file = self.info_dir.persist_trash_info(basename, content,
-                                                           log_data,
-                                                           candidate.info_dir())
-        where_to_store_trashed_file = path_of_backup_copy(trash_info_file)
+    Result = Either[TrashinfoData, UnableToCreateTrashInfoContent]
 
+    def make_trashinfo_data(self,
+                            path,  # type: str
+                            candidate,  # type: Candidate
+                            ):  # type: (...) -> Result
         try:
-            self.fs.move(path, where_to_store_trashed_file)
-        except IOError as e:
-            self.fs.remove_file(trash_info_file)
-            raise e
+            original_location = self.original_location.for_file(path,
+                                                                candidate.path_maker_type,
+                                                                candidate.volume)
+            content = format_trashinfo(original_location, self.clock.now())
+            basename = os.path.basename(original_location)
+            trash_info_data = TrashinfoData(basename, content,
+                                            candidate.info_dir())
+            return Right(trash_info_data)
+        except (IOError, OSError) as error:
+            return Left(UnableToCreateTrashInfoContent(error))
```

### Comparing `trash-cli-0.23.9.23/trashcli/put/trash_file_in.py` & `trash_cli-0.24.4.17/trashcli/put/janitor_tools/trash_dir_checker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,87 @@
-from typing import Dict
+from typing import NamedTuple
 
-from trashcli.put.candidate import Candidate
-from trashcli.put.dir_maker import DirMaker
+from trashcli.fstab.volume_of import VolumeOf
+from trashcli.lib.environ import Environ
+from trashcli.put.core.candidate import Candidate
+from trashcli.put.core.either import Either, Right, Left
+from trashcli.put.core.failure_reason import FailureReason, LogContext
+from trashcli.put.core.trashee import Trashee
 from trashcli.put.fs.fs import Fs
-from trashcli.put.my_logger import LogData
-from trashcli.put.reporter import TrashPutReporter
-from trashcli.put.security_check import SecurityCheck
-from trashcli.put.trash_directory_for_put import TrashDirectoryForPut
-from trashcli.put.trashee import Trashee
-from trashcli.put.trashing_checker import TrashingChecker
+from trashcli.put.gate import Gate
+from trashcli.put.trash_dir_volume_reader import TrashDirVolumeReader
 
 
-class TrashFileIn:
+class DifferentVolumes(NamedTuple('DifferentVolumes', [
+    ('trash_dir_volume', str),
+    ('file_volume', str),
+]), FailureReason):
+    def log_entries(self, context):  # type: (LogContext) -> str
+        return (
+                "trash dir and file to be trashed are not in the same volume, trash-dir volume: %s, file volume: %s"
+                % (self.trash_dir_volume, self.file_volume))
+
+
+class HomeFallBackNotEnabled(FailureReason):
+    def log_entries(self, context):  # type: (LogContext) -> str
+        return "home fallback not enabled"
+
+    def __eq__(self, other):
+        return isinstance(other, HomeFallBackNotEnabled)
+
+
+GateCheckResult = Either[None, FailureReason]
+
+
+class TrashDirChecker:
+    def __init__(self, fs, volumes):  # type: (Fs, VolumeOf) -> None
+        self.fs = fs
+        self.volumes = volumes
+
+    def file_could_be_trashed_in(self,
+                                 trashee,  # type: Trashee
+                                 candidate,  # type: Candidate
+                                 environ,  # type: Environ
+                                 ):  # type: (...) -> GateCheckResult
+        if candidate.gate is Gate.HomeFallback:
+            return self._can_be_trashed_in_home_trash_dir(environ)
+        elif candidate.gate is Gate.SameVolume:
+            return SameVolumeGateImpl(self.volumes, self.fs).can_trash_in(
+                trashee, candidate)
+        else:
+            raise ValueError("Unknown gate: %s" % candidate.gate)
+
+    @staticmethod
+    def _can_be_trashed_in_home_trash_dir(environ,  # type: Environ
+                                          ):
+        if environ.get('TRASH_ENABLE_HOME_FALLBACK', None) == "1":
+            return make_ok()
+        return Left(HomeFallBackNotEnabled())
+
+
+def make_ok():
+    return Right(None)
+
+
+class SameVolumeGateImpl:
     def __init__(self,
+                 volumes,  # type: VolumeOf
                  fs,  # type: Fs
-                 reporter,  # type: TrashPutReporter
-                 trash_dir,  # type: TrashDirectoryForPut
-                 trashing_checker,  # type: TrashingChecker
-                 dir_maker,  # type: DirMaker
                  ):
-        self.reporter = reporter
-        self.security_check = SecurityCheck(fs)
-        self.trash_dir = trash_dir
-        self.dir_maker = dir_maker
-        self.trashing_checker = trashing_checker
-
-    def trash_file_in(self,
-                      candidate,  # type: Candidate
-                      log_data,  # type: LogData
-                      environ,  # type: Dict[str, str]
-                      trashee,  # type: Trashee
-                      ):  # type: (...) -> bool
-        trash_dir_is_secure, messages = self.security_check. \
-            check_trash_dir_is_secure(candidate)
-        self.reporter.log_info_messages(messages, log_data)
-
-        if not trash_dir_is_secure:
-            self.reporter.trash_dir_is_not_secure(candidate.norm_path(),
-                                                  log_data)
-            return False
-        self.reporter.trash_dir_with_volume(candidate, log_data)
-
-        could_be_trashed_in = self.trashing_checker.file_could_be_trashed_in(
-            trashee, candidate, environ)
-        if not could_be_trashed_in.ok:
-            self.reporter.log_info(could_be_trashed_in.reason, log_data)
-            return False
-
-        error = self.try_trash(candidate, log_data, environ, trashee)
-        if error:
-            self.reporter.unable_to_trash_file_in_because(
-                trashee.path, candidate, error, log_data,
-                environ)
-            return False
-
-        return True
-
-    def try_trash(self,
-                  candidate,  # type: Candidate
-                  log_data,  # type : LogData
-                  environ,  # type: Dict[str, str]
-                  trashee,  # type: Trashee
-                  ):
-        try:
-            self.dir_maker.mkdir_p(candidate.trash_dir_path, 0o700)
-            self.dir_maker.mkdir_p(candidate.files_dir(), 0o700)
-            self.dir_maker.mkdir_p(candidate.info_dir(), 0o700)
-
-            self.trash_dir.trash2(trashee.path, candidate, log_data)
-            self.reporter.file_has_been_trashed_in_as(trashee.path,
-                                                      candidate,
-                                                      log_data,
-                                                      environ)
-            return None
-        except (IOError, OSError) as error:
-            return error
+        self.volumes = volumes
+        self.fs = fs
+
+    def can_trash_in(self,
+                     trashee,  # type: Trashee
+                     candidate,  # type: Candidate
+                     ):
+        trash_dir_volume = self._volume_of_trash_dir(candidate)
+        same_volume = trash_dir_volume == trashee.volume
+
+        if not same_volume:
+            return Left(DifferentVolumes(trash_dir_volume, trashee.volume))
+
+        return make_ok()
+
+    def _volume_of_trash_dir(self, candidate):  # type: (Candidate) -> str
+        return (TrashDirVolumeReader(self.volumes, self.fs)
+                .volume_of_trash_dir(candidate.trash_dir_path))
```

### Comparing `trash-cli-0.23.9.23/trashcli/put/trash_put_cmd.py` & `trash_cli-0.24.4.17/trashcli/put/trash_put_cmd.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-from typing import Union, List, Dict
+from typing import List
 
+from trashcli.lib.environ import Environ
+from trashcli.put.context import Context
 from trashcli.put.my_logger import LogData
 from trashcli.put.parser import Parser, ExitWithCode, Trash
 from trashcli.put.reporter import TrashPutReporter
 from trashcli.put.trash_all import TrashAll
 
 
 class TrashPutCmd:
     def __init__(self,
                  trash_all,  # type: TrashAll
                  reporter,  # type: TrashPutReporter
                  ):
         self.trash_all = trash_all
         self.reporter = reporter
 
-    def run(self,
-            argv,  # type: List[str]
-            environ,  # type: Dict[str, str]
-            uid,  # type: int
-            ):  # type: (...) -> Union[str, int, None]
+    def run_put(self,
+                argv,  # type: List[str]
+                environ,  # type: Environ
+                uid,  # type: int
+                ):  # type: (...) -> int
         parser = Parser()
         parsed = parser.parse_args(argv)
         if isinstance(parsed, ExitWithCode):
             return parsed.exit_code
         elif isinstance(parsed, Trash):
             program_name = parsed.program_name
             log_data = LogData(program_name, parsed.verbose)
-            result = self.trash_all.trash_all(parsed.files,
-                                              parsed.trash_dir,
-                                              parsed.mode,
-                                              parsed.forced_volume,
-                                              parsed.home_fallback,
-                                              program_name,
-                                              log_data,
-                                              environ,
-                                              uid)
+            context = Context(paths=parsed.files,
+                              user_trash_dir=parsed.trash_dir,
+                              mode=parsed.mode,
+                              forced_volume=parsed.forced_volume,
+                              home_fallback=parsed.home_fallback,
+                              program_name=program_name,
+                              log_data=log_data,
+                              environ=environ,
+                              uid=uid)
+            result = self.trash_all.trash_all(context)
 
             return self.reporter.exit_code(result)
```

### Comparing `trash-cli-0.23.9.23/trashcli/put/trasher.py` & `trash_cli-0.24.4.17/trashcli/put/trasher.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,33 @@
-import os
-
-from typing import Dict
-
+from trashcli.put.context import Context
+from trashcli.put.core.trash_result import TrashResult
+from trashcli.put.core.trashee import should_skipped_by_specs
 from trashcli.put.file_trasher import FileTrasher
 from trashcli.put.fs.fs import Fs
-from trashcli.put.fs.real_fs import RealFs
-from trashcli.put.my_logger import LogData
-from trashcli.put.parser import mode_force, mode_interactive
 from trashcli.put.reporter import TrashPutReporter
-from trashcli.put.trash_result import TrashResult
-from trashcli.put.user import User, user_replied_no
+from trashcli.put.user import User
+from trashcli.put.user import user_replied_no
 
 
 class Trasher:
     def __init__(self,
                  file_trasher,  # type: FileTrasher
                  user,  # type: User
                  reporter,  # type: TrashPutReporter
                  fs,  # type: Fs
                  ):
         self.file_trasher = file_trasher
         self.user = user
         self.reporter = reporter
         self.fs = fs
 
-    def trash(self,
-              path,
-              user_trash_dir,
-              result,  # type: TrashResult
-              mode,
-              forced_volume,
-              home_fallback,
-              program_name,
-              log_data,  # type: LogData
-              environ,  # type: Dict[str, str]
-              uid,  # type: int
-              ):
+    def trash_single(self,
+                     path,  # type: str
+                     context,  # type: Context
+                     ):
         """
         Trash a file in the appropriate trash directory.
         If the file belong to the same volume of the trash home directory it
         will be trashed in the home trash directory.
         Otherwise it will be trashed in one of the relevant volume trash
         directories.
 
@@ -47,36 +35,26 @@
             - $volume/.Trash/$uid
             - $volume/.Trash-$uid
 
         Firstly the software attempt to trash the file in the first directory
         then try to trash in the second trash directory.
         """
 
-        if self._should_skipped_by_specs(path):
-            self.reporter.unable_to_trash_dot_entries(path, program_name)
-            return result
+        if should_skipped_by_specs(path):
+            self.reporter.unable_to_trash_dot_entries(path, context.log_data)
+            return TrashResult.Failure
 
         if not self.fs.lexists(path):
-            if mode == mode_force:
-                return result
+            if context.mode.can_ignore_not_existent_path():
+                return TrashResult.Success
             else:
-                self.reporter.unable_to_trash_file(path, log_data)
-                return result.mark_unable_to_trash_file()
-
-        if mode == mode_interactive and self.fs.is_accessible(path):
-            reply = self.user.ask_user_about_deleting_file(program_name, path)
+                self.reporter.unable_to_trash_file_non_existent(path,
+                                                                context.log_data)
+                return TrashResult.Failure
+
+        if context.mode.should_we_ask_to_the_user(self.fs.is_accessible(path)):
+            reply = self.user.ask_user_about_deleting_file(context.program_name,
+                                                           path)
             if reply == user_replied_no:
-                return result
+                return TrashResult.Success
 
-        return self.file_trasher.trash_file(path,
-                                            forced_volume,
-                                            user_trash_dir,
-                                            home_fallback,
-                                            result,
-                                            environ,
-                                            uid,
-                                            log_data,
-                                            )
-
-    def _should_skipped_by_specs(self, file):
-        basename = os.path.basename(file)
-        return (basename == ".") or (basename == "..")
+        return self.file_trasher.trash_file(path, context)
```

### Comparing `trash-cli-0.23.9.23/trashcli/put/user.py` & `trash_cli-0.24.4.17/trashcli/put/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from trashcli.lib.my_input import MyInput
+from trashcli.lib.my_input import Input
 from trashcli.put.describer import Describer
 
 
 class User:
     def __init__(self,
-                 my_input,  # type: MyInput
+                 my_input,  # type: Input
                  describer,  # type: Describer
                  ):
-        self.my_input = my_input
+        self.input = my_input
         self.describer = describer
 
     def ask_user_about_deleting_file(self, program_name, path):
-        reply = self.my_input.read_input(
+        reply = self.input.read_input(
             "%s: trash %s '%s'? " % (program_name,
                                      self.describer.describe(path), path))
         return parse_user_reply(reply)
 
 
 user_replied_no = "user_replied_no"
 user_replied_yes = "user_replied_yes"
```

### Comparing `trash-cli-0.23.9.23/trashcli/restore/file_system.py` & `trash_cli-0.24.4.17/trashcli/restore/file_system.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/restore/handler.py` & `trash_cli-0.24.4.17/trashcli/restore/handler.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/restore/info_dir_searcher.py` & `trash_cli-0.24.4.17/trashcli/restore/info_dir_searcher.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/restore/info_files.py` & `trash_cli-0.24.4.17/trashcli/restore/info_files.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/restore/main.py` & `trash_cli-0.24.4.17/trashcli/restore/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .info_dir_searcher import InfoDirSearcher
 from .info_files import InfoFiles
 from .restore_cmd import RestoreCmd
 from .trash_directories import TrashDirectoriesImpl
 from .trashed_files import TrashedFiles
 from ..fstab.volumes import RealVolumes
 from ..lib.logger import my_logger
-from ..lib.my_input import MyInput
+from ..lib.my_input import RealInput
 
 
 def main():
     info_files = InfoFiles(RealListingFileSystem())
     volumes = RealVolumes()
     trash_directories = TrashDirectoriesImpl(volumes,
                                              os.getuid(),
@@ -26,14 +26,14 @@
     trashed_files = TrashedFiles(my_logger,
                                  RealFileReader(),
                                  searcher)
     RestoreCmd.make(
         stdout=sys.stdout,
         stderr=sys.stderr,
         exit=sys.exit,
-        input=MyInput(),
+        input=RealInput(),
         version=trashcli.trash.version,
         trashed_files=trashed_files,
         read_fs=RealRestoreReadFileSystem(),
         write_fs=RealRestoreWriteFileSystem(),
         read_cwd=RealReadCwd()
     ).run(sys.argv)
```

### Comparing `trash-cli-0.23.9.23/trashcli/restore/output.py` & `trash_cli-0.24.4.17/trashcli/restore/output.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/restore/output_recorder.py` & `trash_cli-0.24.4.17/trashcli/restore/output_recorder.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/restore/range.py` & `trash_cli-0.24.4.17/trashcli/restore/range.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/restore/real_output.py` & `trash_cli-0.24.4.17/trashcli/restore/real_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,10 +32,10 @@
         if isinstance(event, Println):
             self.println(event.msg)
         elif isinstance(event, Die):
             self.die(event.msg)
         elif isinstance(event, Quit):
             self.quit()
         elif isinstance(event, Exiting):
-            self.println("Exiting")
+            self.println(event.msg)
         else:
             raise Exception("Unknown call %s" % event)
```

### Comparing `trash-cli-0.23.9.23/trashcli/restore/restore_arg_parser.py` & `trash_cli-0.24.4.17/trashcli/restore/restore_arg_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-
 from typing import Union, List, cast
 
 from trashcli.lib.print_version import PrintVersionArgs
 from trashcli.restore.args import RunRestoreArgs, Sort
 from trashcli.shell_completion import add_argument_to, TRASH_FILES, TRASH_DIRS, \
     complete_with
 
@@ -52,14 +51,14 @@
         if parsed.version:
             return PrintVersionArgs(argv0=sys_argv[0])
         else:
             path = os.path.normpath(
                 os.path.join(curdir + os.path.sep, parsed.path))
 
             return RunRestoreArgs(path=path,
-                                  sort=cast(Sort.Type, {
+                                  sort=cast(Sort, {
                                       'path': Sort.ByPath,
                                       'date': Sort.ByDate,
                                       'none': Sort.DoNot
                                   }[parsed.sort]),
                                   trash_dir=parsed.trash_dir,
                                   overwrite=parsed.overwrite)
```

### Comparing `trash-cli-0.23.9.23/trashcli/restore/restore_asking_the_user.py` & `trash_cli-0.24.4.17/trashcli/restore/restore_asking_the_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import TypeVar, Generic, List, NamedTuple, Callable
 
 from six.moves import range
 
 from trashcli.lib.my_input import Input
 from trashcli.restore.index import Sequence
 from trashcli.restore.output import Output
-from trashcli.restore.output_event import Die, Exiting, OutputEvent, Quit
+from trashcli.restore.output_event import Die, OutputEvent, Quit
+from trashcli.restore.output_event import Exiting
 from trashcli.restore.range import Range
 from trashcli.restore.sequences import Sequences
 from trashcli.restore.single import Single
 from trashcli.restore.trashed_file import TrashedFile
 
 SelectedFiles = NamedTuple('SelectedFiles', [
     ('files_to_restore', List[TrashedFile]),
@@ -48,15 +49,15 @@
 
         except KeyboardInterrupt:
             return Left(Quit())
         except EOFError:
             return Left(Quit())
         else:
             if user_input == "":
-                return Left(Exiting())
+                return Left(Exiting("No files were restored"))
             else:
                 return Right(
                     InputRead(user_input, args.trashed_files, args.overwrite))
 
     def restore_asking_the_user(self, trashed_files, overwrite):
         input = Right(Context(trashed_files, overwrite))
         compose(input, [
```

### Comparing `trash-cli-0.23.9.23/trashcli/restore/restore_cmd.py` & `trash_cli-0.24.4.17/trashcli/restore/restore_cmd.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/restore/restorer.py` & `trash_cli-0.24.4.17/trashcli/restore/restorer.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/restore/run_restore_action.py` & `trash_cli-0.24.4.17/trashcli/restore/run_restore_action.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/restore/sort_method.py` & `trash_cli-0.24.4.17/trashcli/restore/sort_method.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from abc import abstractmethod
-
 from typing import Callable, Any, Iterable
 
 from trashcli.compat import Protocol
 from trashcli.restore.args import Sort
 from trashcli.restore.trashed_file import TrashedFile
 
 
-def sort_files(sort,  # type: Sort.Type
+def sort_files(sort,  # type: Sort
                trashed_files,  # type: Iterable[TrashedFile]
                ):  # type: (...) -> Iterable[TrashedFile]
     return sorter_for(sort).sort_files(trashed_files)
 
 
 class Sorter(Protocol):
     @abstractmethod
@@ -32,15 +31,15 @@
         self.sort_func = sort_func
 
     def sort_files(self, trashed_files,  # type: Iterable[TrashedFile]
                    ):  # type: (...) -> Iterable[TrashedFile]
         return sorted(trashed_files, key=self.sort_func)
 
 
-def sorter_for(sort,  # type: Sort.Type
+def sorter_for(sort,  # type: Sort
                ):  # type (...) -> Sorter
 
     path_ranking = lambda x: x.original_location + str(x.deletion_date)
     date_rankking = lambda x: x.deletion_date
     return {
         Sort.ByPath: SortFunction(path_ranking),
         Sort.ByDate: SortFunction(date_rankking),
```

### Comparing `trash-cli-0.23.9.23/trashcli/restore/trash_directories.py` & `trash_cli-0.24.4.17/trashcli/restore/trash_directories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (C) 2007-2023 Andrea Francia Trivolzio(PV) Italy
 from abc import abstractmethod, ABCMeta
-from typing import Dict, Optional
 
 import six
+from typing import Optional
 
 from trashcli.fstab.volume_of import VolumeOf
 from trashcli.fstab.volumes import Volumes
+from trashcli.lib.environ import Environ
 from trashcli.lib.trash_dirs import (
     volume_trash_dir1, volume_trash_dir2, home_trash_dir)
 
 
 @six.add_metaclass(ABCMeta)
 class TrashDirectories:
     @abstractmethod
@@ -52,15 +53,15 @@
 
 
 
 class TrashDirectories1:
     def __init__(self,
                  volumes,  # type: Volumes
                  uid,  # type: int
-                 environ,  # type: Dict[str, str]
+                 environ,  # type: Environ
                  ):
         self.volumes = volumes
         self.uid = uid
         self.environ = environ
 
     def all_trash_directories(self):
         volumes_to_check = self.volumes.list_mount_points()
```

### Comparing `trash-cli-0.23.9.23/trashcli/restore/trashed_file.py` & `trash_cli-0.24.4.17/trashcli/restore/trashed_file.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/restore/trashed_files.py` & `trash_cli-0.24.4.17/trashcli/restore/trashed_files.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/rm/cleanable_trashcan.py` & `trash_cli-0.24.4.17/trashcli/rm/cleanable_trashcan.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/rm/list_trashinfo.py` & `trash_cli-0.24.4.17/trashcli/rm/list_trashinfo.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/rm/main.py` & `trash_cli-0.24.4.17/trashcli/rm/main.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/rm/rm_cmd.py` & `trash_cli-0.24.4.17/trashcli/rm/rm_cmd.py`

 * *Files identical despite different names*

### Comparing `trash-cli-0.23.9.23/trashcli/shell_completion.py` & `trash_cli-0.24.4.17/trashcli/shell_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,8 +58,8 @@
 
     def complete_with(completion,  # type: Dict[str, str]
                       action,  # type: argparse.Action
                       ):
         pass
 
 TRASH_FILES.update({"zsh": "_trash_files"})
-TRASH_DIRS.update({"zsh": "(${$(trash-list --trash-dirs)#parent_*:})"})
+TRASH_DIRS.update({"zsh": "(\\${\\$(trash-list --trash-dirs)#parent_*})"})
```

### Comparing `trash-cli-0.23.9.23/trashcli/trash_dirs_scanner.py` & `trash_cli-0.24.4.17/trashcli/trash_dirs_scanner.py`

 * *Files identical despite different names*

