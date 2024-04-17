# Comparing `tmp/mwalib-1.2.3.tar.gz` & `tmp/mwalib-1.3.0.tar.gz`

## Comparing `mwalib-1.2.3.tar` & `mwalib-1.3.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     2236 1970-01-01 00:00:00.000000 mwalib-1.2.3/Cargo.toml
--rw-r--r--   0     1000     1000      531 2024-03-11 06:25:51.000000 mwalib-1.2.3/.gitignore
--rw-r--r--   0     1000     1000    18964 2024-03-12 08:59:05.000000 mwalib-1.2.3/CHANGELOG.md
--rw-r--r--   0     1000     1000    33191 2024-03-12 08:57:45.000000 mwalib-1.2.3/Cargo.lock
--rw-r--r--   0     1000     1000    15332 2023-06-16 05:40:58.000000 mwalib-1.2.3/LICENSE
--rw-r--r--   0     1000     1000     1460 2023-06-16 05:40:58.000000 mwalib-1.2.3/LICENSE-cfitsio
--rw-r--r--   0     1000     1000    17532 2023-09-15 02:50:14.000000 mwalib-1.2.3/README.md
--rw-r--r--   0     1000     1000     1992 2024-03-11 06:25:51.000000 mwalib-1.2.3/build.rs
--rwxr-xr-x   0     1000     1000      744 2024-03-11 06:25:51.000000 mwalib-1.2.3/examples/build_c_examples.sh
--rw-r--r--   0     1000     1000     5196 2023-06-16 05:40:58.000000 mwalib-1.2.3/examples/mwalib-data-dump.rs
--rw-r--r--   0     1000     1000     9271 2024-03-11 08:19:05.000000 mwalib-1.2.3/examples/mwalib-print-context.c
--rwxr-xr-x   0     1000     1000     2285 2023-09-11 07:16:02.000000 mwalib-1.2.3/examples/mwalib-print-context.py
--rwxr-xr-x   0     1000     1000      442 2023-09-11 07:16:02.000000 mwalib-1.2.3/examples/mwalib-print-corr-context.py
--rw-r--r--   0     1000     1000     1182 2023-06-16 05:40:58.000000 mwalib-1.2.3/examples/mwalib-print-corr-context.rs
--rwxr-xr-x   0     1000     1000     1088 2024-03-11 06:25:51.000000 mwalib-1.2.3/examples/mwalib-print-tile-info.py
--rw-r--r--   0     1000     1000     4492 2024-03-12 08:46:22.000000 mwalib-1.2.3/examples/mwalib-print-volt-context.c
--rw-r--r--   0     1000     1000      970 2023-06-16 05:40:58.000000 mwalib-1.2.3/examples/mwalib-print-volt-context.rs
--rw-r--r--   0     1000     1000     4562 2023-06-16 05:40:58.000000 mwalib-1.2.3/examples/mwalib-sum-all-hdus.c
--rw-r--r--   0     1000     1000     3605 2023-09-11 07:16:02.000000 mwalib-1.2.3/examples/mwalib-sum-all-hdus.py
--rw-r--r--   0     1000     1000     2346 2023-06-16 05:40:58.000000 mwalib-1.2.3/examples/mwalib-sum-first-fine-channel-gpubox-hdus.rs
--rw-r--r--   0     1000     1000     3076 2023-06-16 05:40:58.000000 mwalib-1.2.3/examples/mwalib-sum-gpubox-hdus.rs
--rw-r--r--   0     1000     1000     4085 2023-09-11 07:16:02.000000 mwalib-1.2.3/examples/mwalib-sum-vcs.py
--rw-r--r--   0     1000     1000       13 2023-09-11 07:16:02.000000 mwalib-1.2.3/examples/requirements.txt
--rw-r--r--   0     1000     1000    42698 2023-09-11 07:16:02.000000 mwalib-1.2.3/examples/view_fits.py
--rwxr-xr-x   0     1000     1000   121853 2023-06-16 05:40:58.000000 mwalib-1.2.3/img/CIRA_Rust_Evangelism_Strike_Force.png
--rwxr-xr-x   0     1000     1000    62088 2023-06-16 05:40:58.000000 mwalib-1.2.3/img/mwalib_logo.png
--rw-r--r--   0     1000     1000     4026 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/antenna/mod.rs
--rw-r--r--   0     1000     1000     8327 2024-03-11 06:25:51.000000 mwalib-1.2.3/src/antenna/test.rs
--rw-r--r--   0     1000     1000     1891 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/baseline/mod.rs
--rw-r--r--   0     1000     1000      847 2023-06-16 05:40:58.000000 mwalib-1.2.3/src/baseline/test.rs
--rw-r--r--   0     1000     1000      779 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/coarse_channel/error.rs
--rw-r--r--   0     1000     1000    19362 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/coarse_channel/mod.rs
--rw-r--r--   0     1000     1000    30779 2023-06-16 05:40:58.000000 mwalib-1.2.3/src/coarse_channel/test.rs
--rw-r--r--   0     1000     1000    24365 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/convert/mod.rs
--rw-r--r--   0     1000     1000    24226 2023-06-16 05:40:58.000000 mwalib-1.2.3/src/convert/test.rs
--rw-r--r--   0     1000     1000    41183 2023-09-15 02:01:33.000000 mwalib-1.2.3/src/correlator_context/mod.rs
--rw-r--r--   0     1000     1000     7965 2023-09-15 02:22:22.000000 mwalib-1.2.3/src/correlator_context/python.rs
--rw-r--r--   0     1000     1000    45705 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/correlator_context/test.rs
--rw-r--r--   0     1000     1000     1458 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/error.rs
--rw-r--r--   0     1000     1000   113606 2024-03-12 08:46:22.000000 mwalib-1.2.3/src/ffi/mod.rs
--rw-r--r--   0     1000     1000    78176 2023-09-14 03:40:08.000000 mwalib-1.2.3/src/ffi/test.rs
--rw-r--r--   0     1000     1000     2349 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/fits_read/error.rs
--rw-r--r--   0     1000     1000    19245 2023-09-11 07:31:18.000000 mwalib-1.2.3/src/fits_read/mod.rs
--rw-r--r--   0     1000     1000    23681 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/fits_read/test.rs
--rw-r--r--   0     1000     1000    11384 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/gpubox_files/error.rs
--rw-r--r--   0     1000     1000    29630 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/gpubox_files/mod.rs
--rw-r--r--   0     1000     1000    43422 2024-03-11 06:25:51.000000 mwalib-1.2.3/src/gpubox_files/test.rs
--rw-r--r--   0     1000     1000     2841 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/lib.rs
--rw-r--r--   0     1000     1000      540 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/metafits_context/error.rs
--rw-r--r--   0     1000     1000    48524 2024-03-12 08:46:22.000000 mwalib-1.2.3/src/metafits_context/mod.rs
--rw-r--r--   0     1000     1000     1439 2023-09-15 01:33:54.000000 mwalib-1.2.3/src/metafits_context/python.rs
--rw-r--r--   0     1000     1000    24464 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/metafits_context/test.rs
--rw-r--r--   0     1000     1000     7779 2024-03-11 06:25:51.000000 mwalib-1.2.3/src/misc/mod.rs
--rw-r--r--   0     1000     1000    14508 2024-03-11 06:25:51.000000 mwalib-1.2.3/src/misc/test.rs
--rw-r--r--   0     1000     1000     6007 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/python.rs
--rw-r--r--   0     1000     1000     1416 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/rfinput/error.rs
--rw-r--r--   0     1000     1000    20647 2024-03-11 06:25:51.000000 mwalib-1.2.3/src/rfinput/mod.rs
--rw-r--r--   0     1000     1000     9130 2024-03-11 06:25:51.000000 mwalib-1.2.3/src/rfinput/test.rs
--rw-r--r--   0     1000     1000    14887 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/timestep/mod.rs
--rw-r--r--   0     1000     1000    19265 2023-06-16 05:40:58.000000 mwalib-1.2.3/src/timestep/test.rs
--rw-r--r--   0     1000     1000    43346 2024-03-11 08:16:34.000000 mwalib-1.2.3/src/voltage_context/mod.rs
--rw-r--r--   0     1000     1000    10625 2023-09-15 02:36:10.000000 mwalib-1.2.3/src/voltage_context/python.rs
--rw-r--r--   0     1000     1000    63481 2023-09-13 06:06:00.000000 mwalib-1.2.3/src/voltage_context/test.rs
--rw-r--r--   0     1000     1000     9534 2023-09-11 07:16:02.000000 mwalib-1.2.3/src/voltage_files/error.rs
--rw-r--r--   0     1000     1000    24792 2024-03-12 08:46:22.000000 mwalib-1.2.3/src/voltage_files/mod.rs
--rw-r--r--   0     1000     1000    23162 2024-03-11 06:25:51.000000 mwalib-1.2.3/src/voltage_files/test.rs
--rw-r--r--   0     1000     1000      469 2023-09-15 01:57:14.000000 mwalib-1.2.3/tests/README.md
--rw-r--r--   0     1000     1000       12 2023-09-11 07:16:02.000000 mwalib-1.2.3/tests/requirements.txt
--rw-r--r--   0     1000     1000     2841 2023-09-15 02:26:09.000000 mwalib-1.2.3/tests/test_correlator_context.py
--rw-r--r--   0     1000     1000     4111 2023-09-11 07:16:02.000000 mwalib-1.2.3/tests/test_metafits_context.py
--rw-r--r--   0     1000     1000     7659 2023-09-14 08:29:16.000000 mwalib-1.2.3/tests/test_voltage_context.py
--rw-r--r--   0     1000     1000     1463 2024-03-12 08:55:10.000000 mwalib-1.2.3/pyproject.toml
--rw-r--r--   0        0        0    18982 1970-01-01 00:00:00.000000 mwalib-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2236 1970-01-01 00:00:00.000000 mwalib-1.3.0/Cargo.toml
+-rw-r--r--   0     1000     1000      531 2023-11-24 00:17:00.000000 mwalib-1.3.0/.gitignore
+-rw-r--r--   0     1000     1000    19132 2024-04-12 07:43:15.000000 mwalib-1.3.0/CHANGELOG.md
+-rw-r--r--   0     1000     1000    33192 2024-04-12 07:43:16.000000 mwalib-1.3.0/Cargo.lock
+-rw-r--r--   0     1000     1000    15332 2020-12-17 04:57:39.000000 mwalib-1.3.0/LICENSE
+-rw-r--r--   0     1000     1000     1460 2020-12-17 04:57:39.000000 mwalib-1.3.0/LICENSE-cfitsio
+-rw-r--r--   0     1000     1000    17532 2023-10-04 23:56:40.000000 mwalib-1.3.0/README.md
+-rw-r--r--   0     1000     1000     1992 2023-11-24 04:23:25.000000 mwalib-1.3.0/build.rs
+-rwxr-xr-x   0     1000     1000      744 2023-10-05 00:38:36.000000 mwalib-1.3.0/examples/build_c_examples.sh
+-rw-r--r--   0     1000     1000     5196 2023-08-22 00:56:45.000000 mwalib-1.3.0/examples/mwalib-data-dump.rs
+-rw-r--r--   0     1000     1000     9271 2023-09-06 03:43:09.000000 mwalib-1.3.0/examples/mwalib-print-context.c
+-rwxr-xr-x   0     1000     1000     2285 2023-09-07 00:59:15.000000 mwalib-1.3.0/examples/mwalib-print-context.py
+-rwxr-xr-x   0     1000     1000      442 2023-09-07 00:59:15.000000 mwalib-1.3.0/examples/mwalib-print-corr-context.py
+-rw-r--r--   0     1000     1000     1182 2022-04-20 03:24:16.000000 mwalib-1.3.0/examples/mwalib-print-corr-context.rs
+-rwxr-xr-x   0     1000     1000     1088 2023-11-24 00:17:00.000000 mwalib-1.3.0/examples/mwalib-print-tile-info.py
+-rw-r--r--   0     1000     1000     4492 2024-03-25 01:51:16.000000 mwalib-1.3.0/examples/mwalib-print-volt-context.c
+-rw-r--r--   0     1000     1000      970 2022-04-20 03:24:16.000000 mwalib-1.3.0/examples/mwalib-print-volt-context.rs
+-rw-r--r--   0     1000     1000     4562 2021-05-05 05:13:28.000000 mwalib-1.3.0/examples/mwalib-sum-all-hdus.c
+-rw-r--r--   0     1000     1000     3605 2023-09-07 00:59:15.000000 mwalib-1.3.0/examples/mwalib-sum-all-hdus.py
+-rw-r--r--   0     1000     1000     2346 2022-04-20 03:24:16.000000 mwalib-1.3.0/examples/mwalib-sum-first-fine-channel-gpubox-hdus.rs
+-rw-r--r--   0     1000     1000     3076 2022-04-20 03:24:16.000000 mwalib-1.3.0/examples/mwalib-sum-gpubox-hdus.rs
+-rw-r--r--   0     1000     1000     4085 2023-09-07 00:59:15.000000 mwalib-1.3.0/examples/mwalib-sum-vcs.py
+-rw-r--r--   0     1000     1000       13 2023-09-07 00:59:15.000000 mwalib-1.3.0/examples/requirements.txt
+-rw-r--r--   0     1000     1000    42698 2023-09-07 00:59:15.000000 mwalib-1.3.0/examples/view_fits.py
+-rwxr-xr-x   0     1000     1000   121853 2021-11-18 07:06:51.000000 mwalib-1.3.0/img/CIRA_Rust_Evangelism_Strike_Force.png
+-rwxr-xr-x   0     1000     1000    62088 2021-11-18 07:07:22.000000 mwalib-1.3.0/img/mwalib_logo.png
+-rw-r--r--   0     1000     1000     4026 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/antenna/mod.rs
+-rw-r--r--   0     1000     1000     8327 2023-11-24 00:17:00.000000 mwalib-1.3.0/src/antenna/test.rs
+-rw-r--r--   0     1000     1000     1891 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/baseline/mod.rs
+-rw-r--r--   0     1000     1000      847 2022-12-08 00:31:38.000000 mwalib-1.3.0/src/baseline/test.rs
+-rw-r--r--   0     1000     1000      779 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/coarse_channel/error.rs
+-rw-r--r--   0     1000     1000    19362 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/coarse_channel/mod.rs
+-rw-r--r--   0     1000     1000    30779 2022-12-08 00:31:38.000000 mwalib-1.3.0/src/coarse_channel/test.rs
+-rw-r--r--   0     1000     1000    24365 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/convert/mod.rs
+-rw-r--r--   0     1000     1000    24226 2022-12-08 00:31:38.000000 mwalib-1.3.0/src/convert/test.rs
+-rw-r--r--   0     1000     1000    41183 2023-10-04 23:56:40.000000 mwalib-1.3.0/src/correlator_context/mod.rs
+-rw-r--r--   0     1000     1000     7965 2023-10-04 23:56:40.000000 mwalib-1.3.0/src/correlator_context/python.rs
+-rw-r--r--   0     1000     1000    45705 2023-08-31 02:45:12.000000 mwalib-1.3.0/src/correlator_context/test.rs
+-rw-r--r--   0     1000     1000     1458 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/error.rs
+-rw-r--r--   0     1000     1000   113606 2024-03-25 01:51:16.000000 mwalib-1.3.0/src/ffi/mod.rs
+-rw-r--r--   0     1000     1000    78176 2023-10-04 23:56:40.000000 mwalib-1.3.0/src/ffi/test.rs
+-rw-r--r--   0     1000     1000     2349 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/fits_read/error.rs
+-rw-r--r--   0     1000     1000    19245 2023-10-04 23:56:40.000000 mwalib-1.3.0/src/fits_read/mod.rs
+-rw-r--r--   0     1000     1000    23681 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/fits_read/test.rs
+-rw-r--r--   0     1000     1000    11384 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/gpubox_files/error.rs
+-rw-r--r--   0     1000     1000    29630 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/gpubox_files/mod.rs
+-rw-r--r--   0     1000     1000    43422 2023-11-24 00:17:00.000000 mwalib-1.3.0/src/gpubox_files/test.rs
+-rw-r--r--   0     1000     1000     2841 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/lib.rs
+-rw-r--r--   0     1000     1000      540 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/metafits_context/error.rs
+-rw-r--r--   0     1000     1000    48524 2024-03-25 01:51:16.000000 mwalib-1.3.0/src/metafits_context/mod.rs
+-rw-r--r--   0     1000     1000     1439 2024-03-10 02:53:40.000000 mwalib-1.3.0/src/metafits_context/python.rs
+-rw-r--r--   0     1000     1000    24464 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/metafits_context/test.rs
+-rw-r--r--   0     1000     1000     7779 2023-11-24 00:17:00.000000 mwalib-1.3.0/src/misc/mod.rs
+-rw-r--r--   0     1000     1000    14508 2023-11-24 00:17:00.000000 mwalib-1.3.0/src/misc/test.rs
+-rw-r--r--   0     1000     1000     6007 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/python.rs
+-rw-r--r--   0     1000     1000     1416 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/rfinput/error.rs
+-rw-r--r--   0     1000     1000    20951 2024-04-12 07:43:15.000000 mwalib-1.3.0/src/rfinput/mod.rs
+-rw-r--r--   0     1000     1000     9435 2024-04-12 07:43:15.000000 mwalib-1.3.0/src/rfinput/test.rs
+-rw-r--r--   0     1000     1000    14887 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/timestep/mod.rs
+-rw-r--r--   0     1000     1000    19265 2022-12-08 00:31:38.000000 mwalib-1.3.0/src/timestep/test.rs
+-rw-r--r--   0     1000     1000    43346 2023-10-04 23:56:40.000000 mwalib-1.3.0/src/voltage_context/mod.rs
+-rw-r--r--   0     1000     1000    10625 2023-10-04 23:56:40.000000 mwalib-1.3.0/src/voltage_context/python.rs
+-rw-r--r--   0     1000     1000    63481 2023-10-04 23:56:40.000000 mwalib-1.3.0/src/voltage_context/test.rs
+-rw-r--r--   0     1000     1000     9534 2023-09-07 00:59:15.000000 mwalib-1.3.0/src/voltage_files/error.rs
+-rw-r--r--   0     1000     1000    24792 2024-03-25 01:51:16.000000 mwalib-1.3.0/src/voltage_files/mod.rs
+-rw-r--r--   0     1000     1000    23162 2023-11-24 00:17:00.000000 mwalib-1.3.0/src/voltage_files/test.rs
+-rw-r--r--   0     1000     1000      469 2023-10-04 23:56:40.000000 mwalib-1.3.0/tests/README.md
+-rw-r--r--   0     1000     1000       12 2023-09-07 00:59:15.000000 mwalib-1.3.0/tests/requirements.txt
+-rw-r--r--   0     1000     1000     2841 2023-10-04 23:56:40.000000 mwalib-1.3.0/tests/test_correlator_context.py
+-rw-r--r--   0     1000     1000     4111 2023-09-07 00:59:15.000000 mwalib-1.3.0/tests/test_metafits_context.py
+-rw-r--r--   0     1000     1000     7659 2023-10-04 23:56:40.000000 mwalib-1.3.0/tests/test_voltage_context.py
+-rw-r--r--   0     1000     1000     1463 2024-04-17 01:46:04.000000 mwalib-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    18982 1970-01-01 00:00:00.000000 mwalib-1.3.0/PKG-INFO
```

### Comparing `mwalib-1.2.3/Cargo.toml` & `mwalib-1.3.0/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "mwalib"
-version = "1.2.3"
+version = "1.3.0"
 homepage = "https://github.com/MWATelescope/mwalib"
 repository = "https://github.com/MWATelescope/mwalib"
 readme = "README.md"
 authors = ["Greg Sleap <greg.sleap@curtin.edu.au>",
            "Christopher H. Jordan <christopherjordan87@gmail.com>"]
 edition = "2021"
 rust-version = "1.63"
```

### Comparing `mwalib-1.2.3/.gitignore` & `mwalib-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/CHANGELOG.md` & `mwalib-1.3.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # Change Log
 
 Changes in each release are listed below.
 
+## 1.3.0 12-Apr-2024
+
+* Added 'EDA2' and 'SHAO' as new valid `ReceiverType`s to `Rfinput` struct.
+* Release and tests now include MacOS 14 Arm64 architecture binaries.
+
 ## 1.2.3 12-Mar-2024
 
 * Removed error-inducing, unneeded `python_version` requirement from the `[build-system]` `requires` setting.
 
 ## 1.2.2 12-Mar-2024
 
 * Explictly typed the buffer_ptr to be `signed char*` instead of the ambiguous `char*` in FFI VoltageContext read methods to fix portability issue with Arm64 platform. Fixes #67.
-* Updated deprecated call when using `Duration:milliseconds`. 
+* Updated deprecated call when using `Duration:milliseconds`.
 
 ## 1.2.1 24-Nov-2023
 
 * Added pypi release and release wheels and support for Python 3.12.
 * Added pypi release for Python 3.11.
 * Removed release wheels and pypi deployment for Python 3.7.
```

### Comparing `mwalib-1.2.3/Cargo.lock` & `mwalib-1.3.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -24,61 +24,61 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.81"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
+checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 
 [[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
  "hermit-abi",
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "built"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b9c056b9ed43aee5e064b683aa1ec783e19c6acec7559e3ae931b7490472fbe"
 dependencies = [
  "cargo-lock",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "cargo-lock"
 version = "8.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "031718ddb8f78aa5def78a09e90defe30151d1f6c672f937af4dd916429ed996"
 dependencies = [
@@ -104,29 +104,29 @@
  "syn 1.0.109",
  "tempfile",
  "toml",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.35"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eaf5903dcbc0a39312feb77df2ff4c76387d591b9fc7b04a238dcf8bb62639a"
+checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "wasm-bindgen",
  "windows-targets 0.52.4",
@@ -250,17 +250,17 @@
 dependencies = [
  "libc",
  "windows-sys",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.1"
+version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
+checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
 
 [[package]]
 name = "fitsio"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f3c31e99e291587ab50840bdf7e647187355978e93fdfc4c9f0d76b8e53e345d"
 dependencies = [
@@ -370,23 +370,23 @@
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
@@ -435,30 +435,30 @@
 dependencies = [
  "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mwalib"
-version = "1.2.3"
+version = "1.3.0"
 dependencies = [
  "anyhow",
  "built",
  "cbindgen",
  "chrono",
  "clap",
  "csv",
@@ -676,35 +676,35 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.4.6"
@@ -737,17 +737,17 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -808,19 +808,19 @@
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.38.31"
+version = "0.38.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
+checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys",
 ]
 
 [[package]]
@@ -857,33 +857,33 @@
 name = "serde_derive"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
@@ -896,17 +896,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.52"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -965,15 +965,15 @@
 name = "thiserror-impl"
 version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
@@ -1067,15 +1067,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1089,15 +1089,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
```

### Comparing `mwalib-1.2.3/LICENSE` & `mwalib-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/LICENSE-cfitsio` & `mwalib-1.3.0/LICENSE-cfitsio`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/README.md` & `mwalib-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/build.rs` & `mwalib-1.3.0/build.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/examples/build_c_examples.sh` & `mwalib-1.3.0/examples/build_c_examples.sh`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/examples/mwalib-data-dump.rs` & `mwalib-1.3.0/examples/mwalib-data-dump.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/examples/mwalib-print-context.c` & `mwalib-1.3.0/examples/mwalib-print-context.c`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/examples/mwalib-print-context.py` & `mwalib-1.3.0/examples/mwalib-print-context.py`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/examples/mwalib-print-corr-context.rs` & `mwalib-1.3.0/examples/mwalib-print-corr-context.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/examples/mwalib-print-tile-info.py` & `mwalib-1.3.0/examples/mwalib-print-tile-info.py`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/examples/mwalib-print-volt-context.c` & `mwalib-1.3.0/examples/mwalib-print-volt-context.c`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/examples/mwalib-print-volt-context.rs` & `mwalib-1.3.0/examples/mwalib-print-volt-context.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/examples/mwalib-sum-all-hdus.c` & `mwalib-1.3.0/examples/mwalib-sum-all-hdus.c`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/examples/mwalib-sum-all-hdus.py` & `mwalib-1.3.0/examples/mwalib-sum-all-hdus.py`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/examples/mwalib-sum-first-fine-channel-gpubox-hdus.rs` & `mwalib-1.3.0/examples/mwalib-sum-first-fine-channel-gpubox-hdus.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/examples/mwalib-sum-gpubox-hdus.rs` & `mwalib-1.3.0/examples/mwalib-sum-gpubox-hdus.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/examples/mwalib-sum-vcs.py` & `mwalib-1.3.0/examples/mwalib-sum-vcs.py`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/examples/view_fits.py` & `mwalib-1.3.0/examples/view_fits.py`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/img/CIRA_Rust_Evangelism_Strike_Force.png` & `mwalib-1.3.0/img/CIRA_Rust_Evangelism_Strike_Force.png`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/img/mwalib_logo.png` & `mwalib-1.3.0/img/mwalib_logo.png`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/antenna/mod.rs` & `mwalib-1.3.0/src/antenna/mod.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/antenna/test.rs` & `mwalib-1.3.0/src/antenna/test.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/baseline/mod.rs` & `mwalib-1.3.0/src/baseline/mod.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/baseline/test.rs` & `mwalib-1.3.0/src/baseline/test.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/coarse_channel/error.rs` & `mwalib-1.3.0/src/coarse_channel/error.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/coarse_channel/mod.rs` & `mwalib-1.3.0/src/coarse_channel/mod.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/coarse_channel/test.rs` & `mwalib-1.3.0/src/coarse_channel/test.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/convert/mod.rs` & `mwalib-1.3.0/src/convert/mod.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/convert/test.rs` & `mwalib-1.3.0/src/convert/test.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/correlator_context/mod.rs` & `mwalib-1.3.0/src/correlator_context/mod.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/correlator_context/python.rs` & `mwalib-1.3.0/src/correlator_context/python.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/correlator_context/test.rs` & `mwalib-1.3.0/src/correlator_context/test.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/error.rs` & `mwalib-1.3.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/ffi/mod.rs` & `mwalib-1.3.0/src/ffi/mod.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/ffi/test.rs` & `mwalib-1.3.0/src/ffi/test.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/fits_read/error.rs` & `mwalib-1.3.0/src/fits_read/error.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/fits_read/mod.rs` & `mwalib-1.3.0/src/fits_read/mod.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/fits_read/test.rs` & `mwalib-1.3.0/src/fits_read/test.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/gpubox_files/error.rs` & `mwalib-1.3.0/src/gpubox_files/error.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/gpubox_files/mod.rs` & `mwalib-1.3.0/src/gpubox_files/mod.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/gpubox_files/test.rs` & `mwalib-1.3.0/src/gpubox_files/test.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/lib.rs` & `mwalib-1.3.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/metafits_context/error.rs` & `mwalib-1.3.0/src/metafits_context/error.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/metafits_context/mod.rs` & `mwalib-1.3.0/src/metafits_context/mod.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/metafits_context/python.rs` & `mwalib-1.3.0/src/metafits_context/python.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/metafits_context/test.rs` & `mwalib-1.3.0/src/metafits_context/test.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/misc/mod.rs` & `mwalib-1.3.0/src/misc/mod.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/misc/test.rs` & `mwalib-1.3.0/src/misc/test.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/python.rs` & `mwalib-1.3.0/src/python.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/rfinput/error.rs` & `mwalib-1.3.0/src/rfinput/error.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/rfinput/mod.rs` & `mwalib-1.3.0/src/rfinput/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -169,14 +169,16 @@
 #[cfg_attr(feature = "python", pyo3::pyclass)]
 #[allow(clippy::upper_case_acronyms)]
 pub enum ReceiverType {
     Unknown,
     RRI,
     NI,
     Pseudo,
+    SHAO,
+    EDA2
 }
 
 /// Implements fmt::Display for ReceiverType
 ///
 /// # Arguments
 ///
 /// * `f` - A fmt::Formatter
@@ -193,39 +195,44 @@
             f,
             "{}",
             match self {
                 ReceiverType::Unknown => "Unknown",
                 ReceiverType::RRI => "RRI",
                 ReceiverType::NI => "NI",
                 ReceiverType::Pseudo => "Pseudo",
+                ReceiverType::SHAO => "SHAO",
+                ReceiverType::EDA2 => "EDA2",
             }
         )
     }
 }
 
-/// Implements str::FromStr for ReceiverType enum
+/// Implements str::FromStr for ReceiverType enum.
+/// Non uppercase values are coverted to uppercase for comparision.
 ///
 /// # Arguments
 ///
 /// * `input` - A &str which we want to convert to an enum
 ///
 ///
 /// # Returns
 ///
 /// * `Result<ReceiverType, Err>` - Result of this method
 ///
 ///
 impl std::str::FromStr for ReceiverType {
     type Err = ();
 
-    fn from_str(input: &str) -> Result<ReceiverType, Self::Err> {
-        match input {
+    fn from_str(input: &str) -> Result<ReceiverType, Self::Err> {        
+        match input.to_uppercase().as_str() {
             "RRI" => Ok(ReceiverType::RRI),
             "NI" => Ok(ReceiverType::NI),
             "PSEUDO" => Ok(ReceiverType::Pseudo),
+            "SHAO" => Ok(ReceiverType::SHAO),
+            "EDA2" => Ok(ReceiverType::EDA2),
             _ => Ok(ReceiverType::Unknown),
         }
     }
 }
 
 /// Structure for storing MWA rf_chains (tile with polarisation) information from the metafits file
 #[derive(Clone, PartialEq)]
```

### Comparing `mwalib-1.2.3/src/rfinput/test.rs` & `mwalib-1.3.0/src/rfinput/test.rs`

 * *Files 13% similar despite different names*

```diff
@@ -240,14 +240,20 @@
 }
 
 #[test]
 fn test_string_to_receiver_type() {
     assert!(String::from("RRI").parse::<ReceiverType>().unwrap() == ReceiverType::RRI);
     assert!(String::from("NI").parse::<ReceiverType>().unwrap() == ReceiverType::NI);
     assert!(String::from("PSEUDO").parse::<ReceiverType>().unwrap() == ReceiverType::Pseudo);
+    assert!(String::from("SHAO").parse::<ReceiverType>().unwrap() == ReceiverType::SHAO);
+    assert!(String::from("EDA2").parse::<ReceiverType>().unwrap() == ReceiverType::EDA2);
+
+    // what happens for lowercase?
+    assert!(String::from("rri").parse::<ReceiverType>().unwrap() == ReceiverType::RRI);
+
     assert!(
         String::from("something else")
             .parse::<ReceiverType>()
             .unwrap()
             == ReceiverType::Unknown
     );
     assert!(String::from("").parse::<ReceiverType>().unwrap() == ReceiverType::Unknown);
```

### Comparing `mwalib-1.2.3/src/timestep/mod.rs` & `mwalib-1.3.0/src/timestep/mod.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/timestep/test.rs` & `mwalib-1.3.0/src/timestep/test.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/voltage_context/mod.rs` & `mwalib-1.3.0/src/voltage_context/mod.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/voltage_context/python.rs` & `mwalib-1.3.0/src/voltage_context/python.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/voltage_context/test.rs` & `mwalib-1.3.0/src/voltage_context/test.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/voltage_files/error.rs` & `mwalib-1.3.0/src/voltage_files/error.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/voltage_files/mod.rs` & `mwalib-1.3.0/src/voltage_files/mod.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/src/voltage_files/test.rs` & `mwalib-1.3.0/src/voltage_files/test.rs`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/tests/test_correlator_context.py` & `mwalib-1.3.0/tests/test_correlator_context.py`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/tests/test_metafits_context.py` & `mwalib-1.3.0/tests/test_metafits_context.py`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/tests/test_voltage_context.py` & `mwalib-1.3.0/tests/test_voltage_context.py`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/pyproject.toml` & `mwalib-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mwalib-1.2.3/PKG-INFO` & `mwalib-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mwalib
-Version: 1.2.3
+Version: 1.3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

