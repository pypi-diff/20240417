# Comparing `tmp/libfwps-python-20240310.tar.gz` & `tmp/libfwps-python-20240417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfwps-python-20240310.tar", last modified: Sun Mar 10 12:53:01 2024, max compression
+gzip compressed data, was "libfwps-python-20240417.tar", last modified: Wed Apr 17 04:08:30 2024, max compression
```

## Comparing `libfwps-python-20240310.tar` & `libfwps-python-20240417.tar`

### file list

```diff
@@ -1,538 +1,538 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-03-10 10:29:59.000000 libfwps-20240310/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-03-10 12:40:13.000000 libfwps-20240310/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 10:29:59.000000 libfwps-20240310/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-03-10 12:40:14.000000 libfwps-20240310/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:52:59.000000 libfwps-20240310/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-10 12:40:00.000000 libfwps-20240310/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-03-10 12:40:00.000000 libfwps-20240310/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-03-10 12:40:00.000000 libfwps-20240310/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-10 12:40:00.000000 libfwps-20240310/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-03-10 12:40:00.000000 libfwps-20240310/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-10 12:40:00.000000 libfwps-20240310/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-10 12:40:00.000000 libfwps-20240310/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-03-10 12:40:00.000000 libfwps-20240310/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-03-10 12:40:00.000000 libfwps-20240310/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-03-10 12:40:00.000000 libfwps-20240310/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-03-10 12:40:00.000000 libfwps-20240310/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25886 2024-03-10 12:40:14.000000 libfwps-20240310/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-10 12:40:00.000000 libfwps-20240310/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:52:59.000000 libfwps-20240310/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18420 2024-03-10 10:30:00.000000 libfwps-20240310/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:09:33.000000 libfwps-20240310/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:09:33.000000 libfwps-20240310/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:09:33.000000 libfwps-20240310/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31438 2024-03-10 10:30:00.000000 libfwps-20240310/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:09:33.000000 libfwps-20240310/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:09:33.000000 libfwps-20240310/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8411 2024-03-10 10:30:00.000000 libfwps-20240310/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17322 2024-03-10 10:30:00.000000 libfwps-20240310/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-03-10 10:30:00.000000 libfwps-20240310/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11295 2024-03-10 10:30:00.000000 libfwps-20240310/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-03-10 12:40:08.000000 libfwps-20240310/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-03-10 12:40:08.000000 libfwps-20240310/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:09:33.000000 libfwps-20240310/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-03-10 12:40:08.000000 libfwps-20240310/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:09:33.000000 libfwps-20240310/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6438 2024-03-10 10:30:00.000000 libfwps-20240310/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5819 2024-03-10 10:30:00.000000 libfwps-20240310/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5815 2024-03-10 10:30:00.000000 libfwps-20240310/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:09:33.000000 libfwps-20240310/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-03-10 12:40:08.000000 libfwps-20240310/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:09:33.000000 libfwps-20240310/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:09:33.000000 libfwps-20240310/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-03-10 12:40:08.000000 libfwps-20240310/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:09:33.000000 libfwps-20240310/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:09:33.000000 libfwps-20240310/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:09:33.000000 libfwps-20240310/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-03-10 10:30:00.000000 libfwps-20240310/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:52:59.000000 libfwps-20240310/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16990 2024-03-10 10:30:00.000000 libfwps-20240310/include/libfwps.h.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:52:59.000000 libfwps-20240310/include/libfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3345 2024-03-10 10:30:00.000000 libfwps-20240310/include/libfwps/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3343 2024-03-10 12:40:27.000000 libfwps-20240310/include/libfwps/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5001 2024-03-10 10:30:00.000000 libfwps-20240310/include/libfwps/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4870 2024-03-10 12:40:27.000000 libfwps-20240310/include/libfwps/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-03-10 10:31:06.000000 libfwps-20240310/include/libfwps/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-03-10 10:30:00.000000 libfwps-20240310/include/libfwps/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-03-10 10:30:00.000000 libfwps-20240310/include/libfwps/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-03-10 12:40:27.000000 libfwps-20240310/include/libfwps/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2024-03-10 10:30:00.000000 libfwps-20240310/include/libfwps/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      459 2024-03-10 10:31:06.000000 libfwps-20240310/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16990 2024-03-10 12:40:27.000000 libfwps-20240310/include/libfwps.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24413 2024-03-10 12:40:14.000000 libfwps-20240310/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/libfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2490 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_set.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3829 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1820 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_store.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1585 2024-02-25 15:14:47.000000 libfwps-20240310/libfwps/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3827 2024-03-10 12:40:27.000000 libfwps-20240310/libfwps/libfwps_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1080 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3731 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_format_class_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9704 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_store.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3967 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1078 2024-03-10 12:40:27.000000 libfwps-20240310/libfwps/libfwps.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2244 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_property_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_format_class_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7534 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_property_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6987 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81635 2024-03-10 12:11:24.000000 libfwps-20240310/libfwps/libfwps_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16442 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_set.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30376 2024-03-10 12:40:14.000000 libfwps-20240310/libfwps/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-10 10:30:00.000000 libfwps-20240310/libfwps/libfwps_unused.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:52:59.000000 libfwps-20240310/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-03-10 10:29:59.000000 libfwps-20240310/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-03-10 10:29:59.000000 libfwps-20240310/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-03-10 10:29:59.000000 libfwps-20240310/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-03-10 10:29:59.000000 libfwps-20240310/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-03-10 10:29:59.000000 libfwps-20240310/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-03-10 10:29:59.000000 libfwps-20240310/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-03-10 10:29:59.000000 libfwps-20240310/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-03-10 10:29:59.000000 libfwps-20240310/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-03-10 10:29:59.000000 libfwps-20240310/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-03-10 12:40:27.000000 libfwps-20240310/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12130 2024-03-10 12:40:13.000000 libfwps-20240310/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12838 2024-03-10 12:40:27.000000 libfwps-20240310/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-03-10 10:29:59.000000 libfwps-20240310/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-03-10 10:29:59.000000 libfwps-20240310/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-03-10 10:29:59.000000 libfwps-20240310/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21439 2024-03-10 12:40:13.000000 libfwps-20240310/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:52:59.000000 libfwps-20240310/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-03-10 12:39:55.000000 libfwps-20240310/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-03-10 12:39:55.000000 libfwps-20240310/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-03-10 12:39:55.000000 libfwps-20240310/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-03-10 12:39:55.000000 libfwps-20240310/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-10 12:39:55.000000 libfwps-20240310/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-10 12:39:55.000000 libfwps-20240310/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-03-10 12:39:55.000000 libfwps-20240310/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-03-10 12:39:55.000000 libfwps-20240310/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-03-10 12:39:55.000000 libfwps-20240310/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-03-10 12:39:55.000000 libfwps-20240310/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26442 2024-03-10 12:40:14.000000 libfwps-20240310/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-10 12:39:55.000000 libfwps-20240310/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-03-10 12:39:55.000000 libfwps-20240310/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-03-10 12:39:55.000000 libfwps-20240310/libclocale/libclocale_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1849 2023-12-27 14:01:07.000000 libfwps-20240310/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:09:29.000000 libfwps-20240310/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-03-10 12:40:13.000000 libfwps-20240310/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:52:59.000000 libfwps-20240310/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-03-10 10:30:00.000000 libfwps-20240310/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:52:59.000000 libfwps-20240310/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-03-10 10:29:59.000000 libfwps-20240310/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2024-03-10 10:29:59.000000 libfwps-20240310/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      703 2024-03-10 10:29:59.000000 libfwps-20240310/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-03-10 10:29:59.000000 libfwps-20240310/dpkg/libfwps-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-03-10 10:29:59.000000 libfwps-20240310/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-03-10 12:40:27.000000 libfwps-20240310/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-03-10 10:29:59.000000 libfwps-20240310/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-03-10 10:29:59.000000 libfwps-20240310/dpkg/libfwps-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-03-10 10:29:59.000000 libfwps-20240310/dpkg/libfwps.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2024-03-10 12:40:27.000000 libfwps-20240310/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-03-10 10:29:59.000000 libfwps-20240310/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1489483 2024-03-10 12:40:12.000000 libfwps-20240310/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-03-10 12:40:13.000000 libfwps-20240310/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-03-10 12:40:13.000000 libfwps-20240310/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/fwps_test_set/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5305 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/fwps_test_set/fwps_test_set.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/fwps_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5074 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/fwps_test_support/fwps_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/fwps_test_property_identifier/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5353 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/fwps_test_property_identifier/fwps_test_property_identifier.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/libfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7079 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/libfwps/libfwps.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/libclocale/libclocale.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12534 2024-03-10 10:30:27.000000 libfwps-20240310/msvscpp/libfwps.sln
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      760 2024-03-10 10:30:27.000000 libfwps-20240310/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/fwps_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5068 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/fwps_test_error/fwps_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/fwps_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5154 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/fwps_test_notify/fwps_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/fwps_test_store/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5311 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/fwps_test_store/fwps_test_store.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/fwps_test_record/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5314 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/fwps_test_record/fwps_test_record.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19167 2024-03-10 12:40:14.000000 libfwps-20240310/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/msvscpp/pyfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6809 2024-03-10 10:30:12.000000 libfwps-20240310/msvscpp/pyfwps/pyfwps.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      492 2024-03-10 10:29:59.000000 libfwps-20240310/libfwps.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-03-10 10:29:59.000000 libfwps-20240310/AUTHORS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      292 2024-03-10 10:29:59.000000 libfwps-20240310/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-03-10 12:40:13.000000 libfwps-20240310/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:52:59.000000 libfwps-20240310/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28890 2024-03-10 12:40:14.000000 libfwps-20240310/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-10 12:39:52.000000 libfwps-20240310/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-03-10 10:29:59.000000 libfwps-20240310/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-03-10 10:29:59.000000 libfwps-20240310/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-03-10 12:40:13.000000 libfwps-20240310/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-03-10 10:29:59.000000 libfwps-20240310/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      752 2024-03-10 10:31:06.000000 libfwps-20240310/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:09:29.000000 libfwps-20240310/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:52:59.000000 libfwps-20240310/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29296 2024-03-10 12:40:14.000000 libfwps-20240310/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-03-10 12:39:57.000000 libfwps-20240310/libcthreads/libcthreads_queue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-03-10 12:40:27.000000 libfwps-20240310/libfwps.spec
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-03-10 12:40:14.000000 libfwps-20240310/test-driver
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      298 2023-12-03 09:09:29.000000 libfwps-20240310/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      126 2023-12-03 09:09:32.000000 libfwps-20240310/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7224 2024-03-10 10:30:00.000000 libfwps-20240310/manuals/libfwps.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21643 2024-03-10 12:40:14.000000 libfwps-20240310/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-03-10 10:30:00.000000 libfwps-20240310/tests/fwps_test_libfwps.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-10 10:30:00.000000 libfwps-20240310/tests/fwps_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12381 2024-03-10 11:22:32.000000 libfwps-20240310/tests/fwps_test_store.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-03-10 10:30:00.000000 libfwps-20240310/tests/fwps_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2470 2024-03-10 10:31:06.000000 libfwps-20240310/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-03-10 10:30:00.000000 libfwps-20240310/tests/pyfwps_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-03-10 10:30:00.000000 libfwps-20240310/tests/fwps_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5848 2024-03-10 10:31:06.000000 libfwps-20240310/tests/pyfwps_test_record.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12231 2024-03-10 11:21:56.000000 libfwps-20240310/tests/fwps_test_set.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-03-10 10:30:00.000000 libfwps-20240310/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4086 2024-03-10 10:31:16.000000 libfwps-20240310/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18231 2024-03-10 11:21:15.000000 libfwps-20240310/tests/fwps_test_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-03-10 10:30:00.000000 libfwps-20240310/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-03-10 10:30:00.000000 libfwps-20240310/tests/fwps_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-03-10 10:31:06.000000 libfwps-20240310/tests/pyfwps_test_set.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-03-10 10:30:00.000000 libfwps-20240310/tests/fwps_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2029 2024-03-10 10:31:06.000000 libfwps-20240310/tests/fwps_test_property_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2748 2024-03-10 10:31:06.000000 libfwps-20240310/tests/pyfwps_test_store.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-03-10 10:30:00.000000 libfwps-20240310/tests/fwps_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45245 2024-03-10 12:40:14.000000 libfwps-20240310/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2024-03-10 10:30:00.000000 libfwps-20240310/tests/fwps_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-03-10 10:30:00.000000 libfwps-20240310/tests/fwps_test_unused.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4095 2024-03-10 10:31:06.000000 libfwps-20240310/tests/test_library.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2485 2024-03-10 10:29:59.000000 libfwps-20240310/libfwps.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-03-10 10:30:00.000000 libfwps-20240310/ossfuzz/ossfuzz_libfwps.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1097 2023-12-03 09:09:30.000000 libfwps-20240310/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1347 2024-03-10 10:30:00.000000 libfwps-20240310/ossfuzz/store_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-03-10 10:30:00.000000 libfwps-20240310/ossfuzz/record_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30301 2024-03-10 12:40:14.000000 libfwps-20240310/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1329 2024-03-10 10:30:00.000000 libfwps-20240310/ossfuzz/set_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-03-10 12:40:08.000000 libfwps-20240310/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:09:33.000000 libfwps-20240310/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:09:33.000000 libfwps-20240310/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:09:33.000000 libfwps-20240310/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:09:33.000000 libfwps-20240310/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:09:33.000000 libfwps-20240310/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:09:33.000000 libfwps-20240310/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:09:33.000000 libfwps-20240310/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:09:33.000000 libfwps-20240310/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:09:33.000000 libfwps-20240310/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-03-10 12:40:27.000000 libfwps-20240310/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:09:33.000000 libfwps-20240310/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:09:33.000000 libfwps-20240310/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:52:59.000000 libfwps-20240310/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50008 2024-03-10 12:40:14.000000 libfwps-20240310/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-03-10 12:40:03.000000 libfwps-20240310/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37040 2024-03-10 12:40:13.000000 libfwps-20240310/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:52:59.000000 libfwps-20240310/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-10 12:39:56.000000 libfwps-20240310/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-10 12:39:56.000000 libfwps-20240310/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-03-10 12:39:56.000000 libfwps-20240310/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-03-10 12:39:56.000000 libfwps-20240310/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-03-10 12:39:56.000000 libfwps-20240310/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-10 12:39:56.000000 libfwps-20240310/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-03-10 12:39:56.000000 libfwps-20240310/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-03-10 12:39:56.000000 libfwps-20240310/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-03-10 12:39:56.000000 libfwps-20240310/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-03-10 12:39:56.000000 libfwps-20240310/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-03-10 12:39:56.000000 libfwps-20240310/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26318 2024-03-10 12:40:14.000000 libfwps-20240310/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-10 12:39:56.000000 libfwps-20240310/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-03-10 12:39:56.000000 libfwps-20240310/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:52:59.000000 libfwps-20240310/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-03-10 12:39:53.000000 libfwps-20240310/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-03-10 12:39:53.000000 libfwps-20240310/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-10 12:39:53.000000 libfwps-20240310/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-03-10 12:39:53.000000 libfwps-20240310/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-03-10 12:39:53.000000 libfwps-20240310/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-10 12:39:53.000000 libfwps-20240310/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-03-10 12:39:53.000000 libfwps-20240310/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-03-10 12:39:53.000000 libfwps-20240310/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-03-10 12:39:53.000000 libfwps-20240310/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-03-10 12:39:53.000000 libfwps-20240310/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-10 12:39:53.000000 libfwps-20240310/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25831 2024-03-10 12:40:14.000000 libfwps-20240310/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:52:59.000000 libfwps-20240310/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29057 2024-03-10 12:40:14.000000 libfwps-20240310/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-03-10 12:39:58.000000 libfwps-20240310/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56623 2024-03-10 12:40:10.000000 libfwps-20240310/aclocal.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 12:53:00.000000 libfwps-20240310/pyfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2343 2024-03-10 10:31:06.000000 libfwps-20240310/pyfwps/pyfwps_set.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14766 2024-03-10 10:31:06.000000 libfwps-20240310/pyfwps/pyfwps_set.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_guid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12160 2024-03-10 10:31:06.000000 libfwps-20240310/pyfwps/pyfwps_store.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3254 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3014 2024-03-10 10:31:06.000000 libfwps-20240310/pyfwps/pyfwps_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9101 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_records.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8868 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2133 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_store.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2852 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_guid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-12-03 09:09:31.000000 libfwps-20240310/pyfwps/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8919 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_sets.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2359 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_records.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_libfwps.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31395 2024-03-10 10:31:06.000000 libfwps-20240310/pyfwps/pyfwps_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43555 2024-03-10 12:40:14.000000 libfwps-20240310/pyfwps/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2296 2024-03-10 10:30:00.000000 libfwps-20240310/pyfwps/pyfwps_sets.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5339 2024-03-10 10:29:59.000000 libfwps-20240310/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-03-10 12:53:01.191435 libfwps-20240310/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-17 03:30:09.000000 libfwps-20240417/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-17 03:54:58.000000 libfwps-20240417/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:30:09.000000 libfwps-20240417/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-17 03:54:58.000000 libfwps-20240417/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:28.000000 libfwps-20240417/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-17 03:54:45.000000 libfwps-20240417/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-04-17 03:54:45.000000 libfwps-20240417/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-04-17 03:54:45.000000 libfwps-20240417/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-17 03:54:45.000000 libfwps-20240417/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-04-17 03:54:45.000000 libfwps-20240417/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-17 03:54:45.000000 libfwps-20240417/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-17 03:54:45.000000 libfwps-20240417/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-04-17 03:54:45.000000 libfwps-20240417/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-04-17 03:54:45.000000 libfwps-20240417/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-04-17 03:54:45.000000 libfwps-20240417/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-04-17 03:54:45.000000 libfwps-20240417/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26036 2024-04-17 03:54:58.000000 libfwps-20240417/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-17 03:54:45.000000 libfwps-20240417/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:26.000000 libfwps-20240417/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-17 03:30:13.000000 libfwps-20240417/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:09:33.000000 libfwps-20240417/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:09:33.000000 libfwps-20240417/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:09:33.000000 libfwps-20240417/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-17 03:30:13.000000 libfwps-20240417/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:09:33.000000 libfwps-20240417/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:09:33.000000 libfwps-20240417/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-04-17 03:30:13.000000 libfwps-20240417/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-17 03:30:13.000000 libfwps-20240417/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-03-10 10:30:00.000000 libfwps-20240417/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-17 03:30:13.000000 libfwps-20240417/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-17 03:54:53.000000 libfwps-20240417/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-17 03:54:53.000000 libfwps-20240417/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:09:33.000000 libfwps-20240417/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-17 03:54:53.000000 libfwps-20240417/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:09:33.000000 libfwps-20240417/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-17 03:30:13.000000 libfwps-20240417/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-17 03:30:13.000000 libfwps-20240417/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-04-17 03:30:13.000000 libfwps-20240417/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:09:33.000000 libfwps-20240417/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-17 03:54:53.000000 libfwps-20240417/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:09:33.000000 libfwps-20240417/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:09:33.000000 libfwps-20240417/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-17 03:54:53.000000 libfwps-20240417/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:09:33.000000 libfwps-20240417/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6400 2024-04-17 03:30:13.000000 libfwps-20240417/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:09:33.000000 libfwps-20240417/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-03-10 10:30:00.000000 libfwps-20240417/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:26.000000 libfwps-20240417/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17244 2024-04-17 03:30:11.000000 libfwps-20240417/include/libfwps.h.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:26.000000 libfwps-20240417/include/libfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3345 2024-04-17 03:30:11.000000 libfwps-20240417/include/libfwps/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3343 2024-04-17 03:55:14.000000 libfwps-20240417/include/libfwps/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5001 2024-04-17 03:30:11.000000 libfwps-20240417/include/libfwps/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4870 2024-04-17 03:55:14.000000 libfwps-20240417/include/libfwps/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-17 03:32:33.000000 libfwps-20240417/include/libfwps/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-04-17 03:30:11.000000 libfwps-20240417/include/libfwps/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-17 03:30:11.000000 libfwps-20240417/include/libfwps/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-17 03:55:14.000000 libfwps-20240417/include/libfwps/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2024-04-17 03:30:11.000000 libfwps-20240417/include/libfwps/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      410 2024-04-17 03:39:41.000000 libfwps-20240417/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17244 2024-04-17 03:55:14.000000 libfwps-20240417/include/libfwps.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24393 2024-04-17 03:54:58.000000 libfwps-20240417/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:29.000000 libfwps-20240417/libfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2490 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_set.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3829 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1820 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_store.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1571 2024-04-17 03:40:02.000000 libfwps-20240417/libfwps/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3827 2024-04-17 03:55:14.000000 libfwps-20240417/libfwps/libfwps_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1080 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3731 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_format_class_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9704 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_store.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3967 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1078 2024-04-17 03:55:14.000000 libfwps-20240417/libfwps/libfwps.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2244 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_property_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_format_class_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7534 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_property_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7144 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    83917 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16442 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_set.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30800 2024-04-17 03:54:58.000000 libfwps-20240417/libfwps/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-17 03:30:11.000000 libfwps-20240417/libfwps/libfwps_unused.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:27.000000 libfwps-20240417/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-17 03:30:10.000000 libfwps-20240417/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-17 03:30:10.000000 libfwps-20240417/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-17 03:30:10.000000 libfwps-20240417/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-17 03:30:10.000000 libfwps-20240417/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-17 03:30:10.000000 libfwps-20240417/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-17 03:30:10.000000 libfwps-20240417/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-17 03:30:10.000000 libfwps-20240417/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-17 03:39:41.000000 libfwps-20240417/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-17 03:30:10.000000 libfwps-20240417/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-04-17 03:55:14.000000 libfwps-20240417/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12130 2024-04-17 03:54:57.000000 libfwps-20240417/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12838 2024-04-17 03:55:15.000000 libfwps-20240417/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-17 03:30:10.000000 libfwps-20240417/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-17 03:30:10.000000 libfwps-20240417/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-17 03:30:10.000000 libfwps-20240417/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21446 2024-04-17 03:54:58.000000 libfwps-20240417/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:27.000000 libfwps-20240417/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-04-17 03:54:40.000000 libfwps-20240417/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-17 03:54:40.000000 libfwps-20240417/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-04-17 03:54:40.000000 libfwps-20240417/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-04-17 03:54:40.000000 libfwps-20240417/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-17 03:54:40.000000 libfwps-20240417/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-17 03:54:40.000000 libfwps-20240417/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-04-17 03:54:40.000000 libfwps-20240417/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-04-17 03:54:40.000000 libfwps-20240417/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-04-17 03:54:40.000000 libfwps-20240417/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-04-17 03:54:40.000000 libfwps-20240417/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26644 2024-04-17 03:54:58.000000 libfwps-20240417/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-17 03:54:40.000000 libfwps-20240417/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-17 03:54:40.000000 libfwps-20240417/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-17 03:54:40.000000 libfwps-20240417/libclocale/libclocale_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1657 2024-04-17 03:40:51.000000 libfwps-20240417/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:09:29.000000 libfwps-20240417/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-17 03:54:58.000000 libfwps-20240417/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:26.000000 libfwps-20240417/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-04-17 03:30:12.000000 libfwps-20240417/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:26.000000 libfwps-20240417/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-17 03:30:09.000000 libfwps-20240417/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2024-04-17 03:30:09.000000 libfwps-20240417/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      703 2024-04-17 03:30:09.000000 libfwps-20240417/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-17 03:30:09.000000 libfwps-20240417/dpkg/libfwps-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-04-17 03:30:09.000000 libfwps-20240417/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-04-17 03:55:14.000000 libfwps-20240417/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-17 03:30:09.000000 libfwps-20240417/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-17 03:30:09.000000 libfwps-20240417/dpkg/libfwps-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-17 03:30:09.000000 libfwps-20240417/dpkg/libfwps.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2024-04-17 03:55:14.000000 libfwps-20240417/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-17 03:30:09.000000 libfwps-20240417/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1490064 2024-04-17 03:54:56.000000 libfwps-20240417/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-17 03:54:58.000000 libfwps-20240417/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-17 03:54:58.000000 libfwps-20240417/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/fwps_test_set/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5305 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/fwps_test_set/fwps_test_set.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/fwps_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5074 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/fwps_test_support/fwps_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/fwps_test_property_identifier/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5353 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/fwps_test_property_identifier/fwps_test_property_identifier.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/libfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7079 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/libfwps/libfwps.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/libclocale/libclocale.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12534 2024-04-17 03:32:21.000000 libfwps-20240417/msvscpp/libfwps.sln
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      731 2024-04-17 03:41:02.000000 libfwps-20240417/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/fwps_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5068 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/fwps_test_error/fwps_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/fwps_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5154 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/fwps_test_notify/fwps_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/fwps_test_store/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5311 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/fwps_test_store/fwps_test_store.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/fwps_test_record/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5314 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/fwps_test_record/fwps_test_record.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19167 2024-04-17 03:54:58.000000 libfwps-20240417/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/msvscpp/pyfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6809 2024-04-17 03:30:25.000000 libfwps-20240417/msvscpp/pyfwps/pyfwps.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      492 2024-04-17 03:30:09.000000 libfwps-20240417/libfwps.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-17 03:30:10.000000 libfwps-20240417/AUTHORS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      292 2024-04-17 03:30:09.000000 libfwps-20240417/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-17 03:54:58.000000 libfwps-20240417/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:27.000000 libfwps-20240417/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29390 2024-04-17 03:54:58.000000 libfwps-20240417/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-17 03:54:38.000000 libfwps-20240417/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-17 03:30:09.000000 libfwps-20240417/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-04-17 03:30:09.000000 libfwps-20240417/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-17 03:54:58.000000 libfwps-20240417/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-17 03:30:09.000000 libfwps-20240417/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      752 2024-04-17 03:32:21.000000 libfwps-20240417/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:09:29.000000 libfwps-20240417/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:27.000000 libfwps-20240417/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29829 2024-04-17 03:54:58.000000 libfwps-20240417/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-17 03:54:43.000000 libfwps-20240417/libcthreads/libcthreads_queue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-04-17 03:55:14.000000 libfwps-20240417/libfwps.spec
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-17 03:54:58.000000 libfwps-20240417/test-driver
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      298 2023-12-03 09:09:29.000000 libfwps-20240417/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:29.000000 libfwps-20240417/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       97 2024-04-17 03:41:16.000000 libfwps-20240417/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7351 2024-04-17 03:30:12.000000 libfwps-20240417/manuals/libfwps.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21643 2024-04-17 03:54:58.000000 libfwps-20240417/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:29.000000 libfwps-20240417/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-17 03:30:12.000000 libfwps-20240417/tests/fwps_test_libfwps.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-17 03:30:12.000000 libfwps-20240417/tests/fwps_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12381 2024-04-17 03:32:21.000000 libfwps-20240417/tests/fwps_test_store.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-04-17 03:30:12.000000 libfwps-20240417/tests/fwps_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2487 2024-04-17 03:45:54.000000 libfwps-20240417/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-17 03:30:12.000000 libfwps-20240417/tests/pyfwps_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-04-17 03:30:12.000000 libfwps-20240417/tests/fwps_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5848 2024-04-17 03:32:21.000000 libfwps-20240417/tests/pyfwps_test_record.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12231 2024-04-17 03:32:21.000000 libfwps-20240417/tests/fwps_test_set.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-17 03:30:12.000000 libfwps-20240417/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4397 2024-04-17 03:34:42.000000 libfwps-20240417/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18356 2024-04-17 03:32:21.000000 libfwps-20240417/tests/fwps_test_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-17 03:30:12.000000 libfwps-20240417/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-04-17 03:30:12.000000 libfwps-20240417/tests/fwps_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-04-17 03:32:21.000000 libfwps-20240417/tests/pyfwps_test_set.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-04-17 03:30:12.000000 libfwps-20240417/tests/fwps_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2029 2024-04-17 03:32:21.000000 libfwps-20240417/tests/fwps_test_property_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2748 2024-04-17 03:32:21.000000 libfwps-20240417/tests/pyfwps_test_store.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-04-17 03:30:12.000000 libfwps-20240417/tests/fwps_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45621 2024-04-17 03:54:58.000000 libfwps-20240417/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2024-04-17 03:30:12.000000 libfwps-20240417/tests/fwps_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-17 03:30:12.000000 libfwps-20240417/tests/fwps_test_unused.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4064 2024-04-17 03:32:51.000000 libfwps-20240417/tests/test_library.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2485 2024-04-17 03:30:09.000000 libfwps-20240417/libfwps.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:30.000000 libfwps-20240417/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-04-17 03:30:11.000000 libfwps-20240417/ossfuzz/ossfuzz_libfwps.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1093 2024-04-17 03:41:46.000000 libfwps-20240417/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1347 2024-04-17 03:30:11.000000 libfwps-20240417/ossfuzz/store_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-04-17 03:30:11.000000 libfwps-20240417/ossfuzz/record_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30434 2024-04-17 03:54:58.000000 libfwps-20240417/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1329 2024-04-17 03:30:11.000000 libfwps-20240417/ossfuzz/set_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-17 03:54:53.000000 libfwps-20240417/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:29.000000 libfwps-20240417/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:09:33.000000 libfwps-20240417/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:09:33.000000 libfwps-20240417/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:09:33.000000 libfwps-20240417/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:09:33.000000 libfwps-20240417/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:09:33.000000 libfwps-20240417/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:09:33.000000 libfwps-20240417/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:09:33.000000 libfwps-20240417/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:09:33.000000 libfwps-20240417/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:09:33.000000 libfwps-20240417/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-04-17 03:55:14.000000 libfwps-20240417/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:09:33.000000 libfwps-20240417/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:09:33.000000 libfwps-20240417/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:28.000000 libfwps-20240417/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53156 2024-04-17 03:54:58.000000 libfwps-20240417/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-17 03:54:48.000000 libfwps-20240417/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36922 2024-04-17 03:54:58.000000 libfwps-20240417/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:27.000000 libfwps-20240417/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-17 03:54:41.000000 libfwps-20240417/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-17 03:54:41.000000 libfwps-20240417/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-17 03:54:41.000000 libfwps-20240417/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-17 03:54:41.000000 libfwps-20240417/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-17 03:54:41.000000 libfwps-20240417/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-17 03:54:41.000000 libfwps-20240417/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-17 03:54:41.000000 libfwps-20240417/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-17 03:54:41.000000 libfwps-20240417/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-17 03:54:41.000000 libfwps-20240417/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-17 03:54:41.000000 libfwps-20240417/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-17 03:54:41.000000 libfwps-20240417/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26513 2024-04-17 03:54:58.000000 libfwps-20240417/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-17 03:54:41.000000 libfwps-20240417/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-17 03:54:41.000000 libfwps-20240417/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:27.000000 libfwps-20240417/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-17 03:54:39.000000 libfwps-20240417/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-17 03:54:39.000000 libfwps-20240417/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-17 03:54:39.000000 libfwps-20240417/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-17 03:54:39.000000 libfwps-20240417/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-17 03:54:39.000000 libfwps-20240417/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-17 03:54:39.000000 libfwps-20240417/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-17 03:54:39.000000 libfwps-20240417/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-17 03:54:39.000000 libfwps-20240417/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-17 03:54:39.000000 libfwps-20240417/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-17 03:54:39.000000 libfwps-20240417/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-17 03:54:39.000000 libfwps-20240417/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25980 2024-04-17 03:54:58.000000 libfwps-20240417/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:28.000000 libfwps-20240417/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29564 2024-04-17 03:54:58.000000 libfwps-20240417/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-17 03:54:44.000000 libfwps-20240417/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56623 2024-04-17 03:54:55.000000 libfwps-20240417/aclocal.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:29.000000 libfwps-20240417/pyfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2343 2024-04-17 03:32:21.000000 libfwps-20240417/pyfwps/pyfwps_set.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14766 2024-04-17 03:32:21.000000 libfwps-20240417/pyfwps/pyfwps_set.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_guid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12160 2024-04-17 03:32:21.000000 libfwps-20240417/pyfwps/pyfwps_store.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3254 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3014 2024-04-17 03:32:21.000000 libfwps-20240417/pyfwps/pyfwps_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9101 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_records.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8868 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2133 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_store.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2852 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_guid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-04-17 03:41:58.000000 libfwps-20240417/pyfwps/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8919 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_sets.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2359 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_records.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_libfwps.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31395 2024-04-17 03:32:21.000000 libfwps-20240417/pyfwps/pyfwps_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44097 2024-04-17 03:54:58.000000 libfwps-20240417/pyfwps/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2296 2024-04-17 03:30:12.000000 libfwps-20240417/pyfwps/pyfwps_sets.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5339 2024-04-17 03:30:09.000000 libfwps-20240417/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-04-17 04:08:30.850905 libfwps-20240417/PKG-INFO
```

### Comparing `libfwps-20240310/COPYING` & `libfwps-20240417/COPYING`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/install-sh` & `libfwps-20240417/install-sh`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/depcomp` & `libfwps-20240417/depcomp`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfguid/libfguid_error.c` & `libfwps-20240417/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfguid/libfguid_support.h` & `libfwps-20240417/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfguid/libfguid_identifier.h` & `libfwps-20240417/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfguid/libfguid_libcerror.h` & `libfwps-20240417/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfguid/Makefile.am` & `libfwps-20240417/libfguid/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFGUID
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfguid.la
 
 libfguid_la_SOURCES = \
 	libfguid_definitions.h \
 	libfguid_extern.h \
@@ -13,19 +13,17 @@
 	libfguid_libcerror.h \
 	libfguid_identifier.c libfguid_identifier.h \
 	libfguid_support.c libfguid_support.h \
 	libfguid_types.h \
 	libfguid_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
```

### Comparing `libfwps-20240310/libfguid/libfguid_unused.h` & `libfwps-20240417/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfguid/libfguid_extern.h` & `libfwps-20240417/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfguid/libfguid_types.h` & `libfwps-20240417/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfguid/libfguid_identifier.c` & `libfwps-20240417/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfguid/libfguid_support.c` & `libfwps-20240417/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfguid/libfguid_definitions.h` & `libfwps-20240417/libfguid/libfguid_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfguid/definitions.h> are copied here
  * for local use of libfguid
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFGUID_VERSION					20240116
+#define LIBFGUID_VERSION					20240415
 
 /* The version string
  */
-#define LIBFGUID_VERSION_STRING					"20240116"
+#define LIBFGUID_VERSION_STRING					"20240415"
 
 /* The byte order definitions
  */
 #define LIBFGUID_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFGUID_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The GUID identifier version definitions
```

### Comparing `libfwps-20240310/libfguid/Makefile.in` & `libfwps-20240417/libfguid/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -443,30 +443,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFGUID_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFGUID_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFGUID_TRUE@noinst_LTLIBRARIES = libfguid.la
 @HAVE_LOCAL_LIBFGUID_TRUE@libfguid_la_SOURCES = \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_definitions.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_extern.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_error.c libfguid_error.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_libcerror.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_identifier.c libfguid_identifier.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_support.c libfguid_support.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_types.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -668,24 +669,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfguid_error.Plo
+	-rm -f ./$(DEPDIR)/libfguid_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfguid_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -771,17 +777,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwps-20240310/libfguid/libfguid_error.h` & `libfwps-20240417/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/libfdatetime.m4` & `libfwps-20240417/m4/libfdatetime.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libfdatetime required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libfdatetime is available
 dnl ac_libfdatetime_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno],
     [ac_cv_libfdatetime=no],
@@ -459,15 +459,15 @@
           [ac_cv_libfdatetime_dummy=yes],
           [ac_cv_libfdatetime=no])
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
+      [test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime],
         [1])
       ])
     ])
 
   AS_IF(
@@ -489,15 +489,15 @@
     ])
   ])
 
 dnl Function to detect if libfdatetime dependencies are available
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
   ])
 
 dnl Function to detect how to enable libfdatetime
 AC_DEFUN([AX_LIBFDATETIME_CHECK_ENABLE],
```

### Comparing `libfwps-20240310/m4/tests.m4` & `libfwps-20240417/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/lib-prefix.m4` & `libfwps-20240417/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/progtest.m4` & `libfwps-20240417/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/libuna.m4` & `libfwps-20240417/m4/libuna.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -942,15 +942,15 @@
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -972,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libfwps-20240310/m4/gettext.m4` & `libfwps-20240417/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/lib-ld.m4` & `libfwps-20240417/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/libclocale.m4` & `libfwps-20240417/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
@@ -126,15 +126,15 @@
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -219,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libfwps-20240310/m4/libcdata.m4` & `libfwps-20240417/m4/libcdata.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
@@ -497,15 +497,15 @@
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -527,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libfwps-20240310/m4/common.m4` & `libfwps-20240417/m4/common.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/libcthreads.m4` & `libfwps-20240417/m4/libcthreads.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
@@ -246,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -288,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libfwps-20240310/m4/ltversion.m4` & `libfwps-20240417/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/ltsugar.m4` & `libfwps-20240417/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/host-cpu-c-abi.m4` & `libfwps-20240417/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/libtool.m4` & `libfwps-20240417/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/po.m4` & `libfwps-20240417/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/libcerror.m4` & `libfwps-20240417/m4/libcerror.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
@@ -99,15 +99,15 @@
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -165,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libfwps-20240310/m4/libcnotify.m4` & `libfwps-20240417/m4/libcnotify.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
@@ -96,15 +96,15 @@
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -137,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libfwps-20240310/m4/libfguid.m4` & `libfwps-20240417/m4/libfguid.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libfguid required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libfguid is available
 dnl ac_libfguid_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFGUID_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno],
     [ac_cv_libfguid=no],
@@ -107,15 +107,15 @@
           [ac_cv_libfguid_dummy=yes],
           [ac_cv_libfguid=no])
 
         ac_cv_libfguid_LIBADD="-lfguid"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
+      [test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfguid in directory: $ac_cv_with_libfguid],
         [1])
       ])
     ])
 
   AS_IF(
@@ -137,15 +137,15 @@
     ])
   ])
 
 dnl Function to detect if libfguid dependencies are available
 AC_DEFUN([AX_LIBFGUID_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
   ])
 
 
 dnl Function to detect how to enable libfguid
```

### Comparing `libfwps-20240310/m4/intlmacosx.m4` & `libfwps-20240417/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/lt~obsolete.m4` & `libfwps-20240417/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/lib-link.m4` & `libfwps-20240417/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/iconv.m4` & `libfwps-20240417/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/ltoptions.m4` & `libfwps-20240417/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/nls.m4` & `libfwps-20240417/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/python.m4` & `libfwps-20240417/m4/python.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240416
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,19 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
       [$host_os],
       [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libfwps-20240310/m4/types.m4` & `libfwps-20240417/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/m4/pthread.m4` & `libfwps-20240417/m4/pthread.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/include/libfwps.h.in` & `libfwps-20240417/include/libfwps.h.in`

 * *Files 1% similar despite different names*

```diff
@@ -315,14 +315,23 @@
  */
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_64bit_integer(
      libfwps_record_t *record,
      uint64_t *value_64bit,
      libfwps_error_t **error );
 
+/* Retrieves the data as a 64-bit floatingtime value
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_floatingtime(
+     libfwps_record_t *record,
+     uint64_t *floatingtime,
+     libfwps_error_t **error );
+
 /* Retrieves the data as a 64-bit FILETIME value
  * Returns 1 if successful or -1 on error
  */
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_filetime(
      libfwps_record_t *record,
      uint64_t *filetime,
```

### Comparing `libfwps-20240310/include/libfwps/definitions.h.in` & `libfwps-20240417/include/libfwps/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/include/libfwps/definitions.h` & `libfwps-20240417/include/libfwps/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBFWPS_DEFINITIONS_H )
 #define _LIBFWPS_DEFINITIONS_H
 
 #include <libfwps/types.h>
 
-#define LIBFWPS_VERSION					20240310
+#define LIBFWPS_VERSION					20240417
 
 /* The version string
  */
-#define LIBFWPS_VERSION_STRING				"20240310"
+#define LIBFWPS_VERSION_STRING				"20240417"
 
 /* The byte order definitions
  */
 enum LIBFWPS_ENDIAN
 {
 	LIBFWPS_ENDIAN_BIG				= (int) 'b',
 	LIBFWPS_ENDIAN_LITTLE				= (int) 'l'
```

### Comparing `libfwps-20240310/include/libfwps/types.h.in` & `libfwps-20240417/include/libfwps/types.h.in`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/include/libfwps/types.h` & `libfwps-20240417/include/libfwps/types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/include/libfwps/features.h.in` & `libfwps-20240417/include/libfwps/features.h.in`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/include/libfwps/error.h` & `libfwps-20240417/include/libfwps/error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/include/libfwps/extern.h` & `libfwps-20240417/include/libfwps/extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/include/libfwps/features.h` & `libfwps-20240417/include/libfwps/features.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/include/libfwps/codepage.h` & `libfwps-20240417/include/libfwps/codepage.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/include/libfwps.h` & `libfwps-20240417/include/libfwps.h`

 * *Files 1% similar despite different names*

```diff
@@ -315,14 +315,23 @@
  */
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_64bit_integer(
      libfwps_record_t *record,
      uint64_t *value_64bit,
      libfwps_error_t **error );
 
+/* Retrieves the data as a 64-bit floatingtime value
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_floatingtime(
+     libfwps_record_t *record,
+     uint64_t *floatingtime,
+     libfwps_error_t **error );
+
 /* Retrieves the data as a 64-bit FILETIME value
  * Returns 1 if successful or -1 on error
  */
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_filetime(
      libfwps_record_t *record,
      uint64_t *filetime,
```

### Comparing `libfwps-20240310/include/Makefile.in` & `libfwps-20240417/include/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -449,15 +449,20 @@
 
 EXTRA_DIST = \
 	libfwps.h.in \
 	libfwps/definitions.h.in \
 	libfwps/features.h.in \
 	libfwps/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfwps.h \
+	libfwps/definitions.h \
+	libfwps/features.h \
+	libfwps/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -654,23 +659,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -752,17 +759,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfwps.h
-	-rm -f libfwps/definitions.h
-	-rm -f libfwps/features.h
-	-rm -f libfwps/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwps-20240310/libfwps/libfwps_set.h` & `libfwps-20240417/libfwps/libfwps_set.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_types.h` & `libfwps-20240417/libfwps/libfwps_types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_notify.h` & `libfwps-20240417/libfwps/libfwps_notify.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_definitions.h.in` & `libfwps-20240417/libfwps/libfwps_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_libfguid.h` & `libfwps-20240417/libfwps/libfwps_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps.c` & `libfwps-20240417/libfwps/libfwps.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_libcerror.h` & `libfwps-20240417/libfwps/libfwps_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_libcnotify.h` & `libfwps-20240417/libfwps/libfwps_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_store.h` & `libfwps-20240417/libfwps/libfwps_store.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_libcdata.h` & `libfwps-20240417/libfwps/libfwps_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_debug.h` & `libfwps-20240417/libfwps/libfwps_debug.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_error.c` & `libfwps-20240417/libfwps/libfwps_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/Makefile.am` & `libfwps-20240417/libfwps/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
@@ -48,21 +48,19 @@
 libfwps_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libfwps_definitions.h.in \
 	libfwps.rc \
 	libfwps.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfwps_definitions.h \
+	libfwps.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libfwps_definitions.h
-	-rm -f libfwps.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwps ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwps_la_SOURCES)
```

### Comparing `libfwps-20240310/libfwps/libfwps_definitions.h` & `libfwps-20240417/libfwps/libfwps_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwps/definitions.h> are copied here
  * for local use of libfwps
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWPS_VERSION					20240310
+#define LIBFWPS_VERSION					20240417
 
 /* The version string
  */
-#define LIBFWPS_VERSION_STRING				"20240310"
+#define LIBFWPS_VERSION_STRING				"20240417"
 
 /* The byte order definitions
  */
 #define LIBFWPS_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWPS_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The value types
```

### Comparing `libfwps-20240310/libfwps/libfwps_notify.c` & `libfwps-20240417/libfwps/libfwps_notify.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_error.h` & `libfwps-20240417/libfwps/libfwps_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_libuna.h` & `libfwps-20240417/libfwps/libfwps_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps.rc.in` & `libfwps-20240417/libfwps/libfwps.rc.in`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_support.h` & `libfwps-20240417/libfwps/libfwps_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_format_class_identifier.c` & `libfwps-20240417/libfwps/libfwps_format_class_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_codepage.h` & `libfwps-20240417/libfwps/libfwps_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_support.c` & `libfwps-20240417/libfwps/libfwps_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_extern.h` & `libfwps-20240417/libfwps/libfwps_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_store.c` & `libfwps-20240417/libfwps/libfwps_store.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_debug.c` & `libfwps-20240417/libfwps/libfwps_debug.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps.rc` & `libfwps-20240417/libfwps/libfwps.rc`

 * *Files 10% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Windows Property Store format\0"
-      VALUE "FileVersion",		"20240310" "\0"
+      VALUE "FileVersion",		"20240417" "\0"
       VALUE "InternalName",		"libfwps.dll\0"
       VALUE "LegalCopyright",		"(C) 2013-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfwps.dll\0"
       VALUE "ProductName",		"libfwps\0"
-      VALUE "ProductVersion",		"20240310" "\0"
+      VALUE "ProductVersion",		"20240417" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfwps/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfwps-20240310/libfwps/libfwps_property_identifier.h` & `libfwps-20240417/libfwps/libfwps_property_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_format_class_identifier.h` & `libfwps-20240417/libfwps/libfwps_format_class_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_property_identifier.c` & `libfwps-20240417/libfwps/libfwps_property_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/libfwps_record.h` & `libfwps-20240417/libfwps/libfwps_record.h`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,20 @@
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_64bit_integer(
      libfwps_record_t *record,
      uint64_t *value_64bit,
      libcerror_error_t **error );
 
 LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_floatingtime(
+     libfwps_record_t *record,
+     uint64_t *floatingtime,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_filetime(
      libfwps_record_t *record,
      uint64_t *filetime,
      libcerror_error_t **error );
 
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_floating_point(
```

### Comparing `libfwps-20240310/libfwps/libfwps_record.c` & `libfwps-20240417/libfwps/libfwps_record.c`

 * *Files 1% similar despite different names*

```diff
@@ -470,33 +470,38 @@
 			break;
 
 		case LIBFWPS_VALUE_TYPE_INTEGER_16BIT_SIGNED:
 		case LIBFWPS_VALUE_TYPE_INTEGER_16BIT_UNSIGNED:
 			internal_record->value_data_size = 2;
 			break;
 
+		case LIBFWPS_VALUE_TYPE_ERROR:
 		case LIBFWPS_VALUE_TYPE_FLOAT_32BIT:
 		case LIBFWPS_VALUE_TYPE_INTEGER_32BIT_SIGNED:
 		case LIBFWPS_VALUE_TYPE_INTEGER_32BIT_UNSIGNED:
+		case LIBFWPS_VALUE_TYPE_INTEGER_SIGNED:
+		case LIBFWPS_VALUE_TYPE_INTEGER_UNSIGNED:
 			internal_record->value_data_size = 4;
 			break;
 
+		case LIBFWPS_VALUE_TYPE_APPLICATION_TIME:
 		case LIBFWPS_VALUE_TYPE_CURRENCY:
 		case LIBFWPS_VALUE_TYPE_DOUBLE_64BIT:
 		case LIBFWPS_VALUE_TYPE_FILETIME:
 		case LIBFWPS_VALUE_TYPE_INTEGER_64BIT_SIGNED:
 		case LIBFWPS_VALUE_TYPE_INTEGER_64BIT_UNSIGNED:
 			internal_record->value_data_size = 8;
 			break;
 
 		case LIBFWPS_VALUE_TYPE_FIXED_POINT_128BIT:
 		case LIBFWPS_VALUE_TYPE_GUID:
 			internal_record->value_data_size = 16;
 			break;
 
+		case LIBFWPS_VALUE_TYPE_BINARY_DATA:
 		case LIBFWPS_VALUE_TYPE_BINARY_STRING:
 		case LIBFWPS_VALUE_TYPE_STREAM:
 		case LIBFWPS_VALUE_TYPE_STRING_ASCII:
 		case LIBFWPS_VALUE_TYPE_STRING_UNICODE:
 			has_variable_data_size = 1;
 			break;
 
@@ -1820,17 +1825,19 @@
 		 "%s: invalid record entry.",
 		 function );
 
 		return( -1 );
 	}
 	internal_record = (libfwps_internal_record_t *) record;
 
-	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_32BIT_SIGNED )
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_ERROR )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_32BIT_SIGNED )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_32BIT_UNSIGNED )
-	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_ERROR ) )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_SIGNED )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_UNSIGNED ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
 		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
 		 function,
@@ -1898,18 +1905,19 @@
 		 "%s: invalid record entry.",
 		 function );
 
 		return( -1 );
 	}
 	internal_record = (libfwps_internal_record_t *) record;
 
-	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_64BIT_SIGNED )
-	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_64BIT_UNSIGNED )
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_APPLICATION_TIME )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_CURRENCY )
-	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_FILETIME ) )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_FILETIME )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_64BIT_SIGNED )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_64BIT_UNSIGNED ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
 		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
 		 function,
@@ -1953,14 +1961,90 @@
 	byte_stream_copy_to_uint64_little_endian(
 	 internal_record->value_data,
 	 *value_64bit );
 
 	return( 1 );
 }
 
+/* Retrieves the data as a 64-bit floatingtime value
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_data_as_floatingtime(
+     libfwps_record_t *record,
+     uint64_t *floatingtime,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_data_as_floatingtime";
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record entry.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( internal_record->value_type != LIBFWPS_VALUE_TYPE_APPLICATION_TIME )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
+
+		return( -1 );
+	}
+	if( internal_record->value_data == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
+		 "%s: invalid record entry - missing value data.",
+		 function );
+
+		return( -1 );
+	}
+	if( internal_record->value_data_size != 8 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported value data size.",
+		 function );
+
+		return( -1 );
+	}
+	if( floatingtime == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid floatingtime.",
+		 function );
+
+		return( -1 );
+	}
+	byte_stream_copy_to_uint64_little_endian(
+	 internal_record->value_data,
+	 *floatingtime );
+
+	return( 1 );
+}
+
 /* Retrieves the data as a 64-bit FILETIME value
  * Returns 1 if successful or -1 on error
  */
 int libfwps_record_get_data_as_filetime(
      libfwps_record_t *record,
      uint64_t *filetime,
      libcerror_error_t **error )
@@ -2056,15 +2140,16 @@
 		 "%s: invalid record entry.",
 		 function );
 
 		return( -1 );
 	}
 	internal_record = (libfwps_internal_record_t *) record;
 
-	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_FLOAT_32BIT )
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_APPLICATION_TIME )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_FLOAT_32BIT )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_DOUBLE_64BIT ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
 		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
```

### Comparing `libfwps-20240310/libfwps/libfwps_set.c` & `libfwps-20240417/libfwps/libfwps_set.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps/Makefile.in` & `libfwps-20240417/libfwps/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -474,16 +474,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
@@ -525,15 +525,18 @@
 
 libfwps_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libfwps_definitions.h.in \
 	libfwps.rc \
 	libfwps.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfwps_definitions.h \
+	libfwps.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -773,24 +776,36 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfwps.Plo
+	-rm -f ./$(DEPDIR)/libfwps_debug.Plo
+	-rm -f ./$(DEPDIR)/libfwps_error.Plo
+	-rm -f ./$(DEPDIR)/libfwps_format_class_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwps_notify.Plo
+	-rm -f ./$(DEPDIR)/libfwps_property_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwps_record.Plo
+	-rm -f ./$(DEPDIR)/libfwps_set.Plo
+	-rm -f ./$(DEPDIR)/libfwps_store.Plo
+	-rm -f ./$(DEPDIR)/libfwps_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -883,19 +898,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfwps_definitions.h
-	-rm -f libfwps.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwps ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwps_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwps-20240310/libfwps/libfwps_unused.h` & `libfwps-20240417/libfwps/libfwps_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/common/config_borlandc.h` & `libfwps-20240417/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/common/file_stream.h` & `libfwps-20240417/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/common/memory.h` & `libfwps-20240417/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/common/byte_stream.h` & `libfwps-20240417/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/common/common.h` & `libfwps-20240417/common/common.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/common/config_winapi.h` & `libfwps-20240417/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/common/system_string.h` & `libfwps-20240417/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/common/types.h.in` & `libfwps-20240417/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/common/types.h` & `libfwps-20240417/common/types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/common/config.h.in` & `libfwps-20240417/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/common/config.h` & `libfwps-20240417/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -385,24 +385,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfwps"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfwps 20240310"
+#define PACKAGE_STRING "libfwps 20240417"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfwps"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240310"
+#define PACKAGE_VERSION "20240417"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -420,15 +420,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240310"
+#define VERSION "20240417"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfwps-20240310/common/wide_string.h` & `libfwps-20240417/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/common/narrow_string.h` & `libfwps-20240417/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/common/config_msc.h` & `libfwps-20240417/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/common/Makefile.in` & `libfwps-20240417/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -402,15 +402,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -418,15 +420,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -594,23 +599,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -690,15 +697,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwps-20240310/libclocale/libclocale_wide_string.c` & `libfwps-20240417/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libclocale/libclocale_support.h` & `libfwps-20240417/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libclocale/Makefile.am` & `libfwps-20240417/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libfwps-20240310/libclocale/libclocale_definitions.h` & `libfwps-20240417/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libfwps-20240310/libclocale/libclocale_unused.h` & `libfwps-20240417/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libclocale/libclocale_libcerror.h` & `libfwps-20240417/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libclocale/libclocale_locale.h` & `libfwps-20240417/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libclocale/libclocale_support.c` & `libfwps-20240417/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libclocale/libclocale_codepage.c` & `libfwps-20240417/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libclocale/libclocale_locale.c` & `libfwps-20240417/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libclocale/Makefile.in` & `libfwps-20240417/libclocale/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -448,30 +448,31 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -674,24 +675,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -778,17 +785,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwps-20240310/libclocale/libclocale_extern.h` & `libfwps-20240417/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libclocale/libclocale_wide_string.h` & `libfwps-20240417/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libclocale/libclocale_codepage.h` & `libfwps-20240417/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/Makefile.am` & `libfwps-20240417/Makefile.am`

 * *Files 9% similar despite different names*

```diff
@@ -51,16 +51,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libfwps.pc \
+	libfwps.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libfwps.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -77,19 +84,7 @@
 	(cd $(srcdir)/libcnotify && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libuna && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwps && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfwps.pc
-	-rm -f libfwps.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libfwps-20240310/config.guess` & `libfwps-20240417/config.guess`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/dpkg/copyright` & `libfwps-20240417/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/dpkg/control` & `libfwps-20240417/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/dpkg/rules` & `libfwps-20240417/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/COPYING.LESSER` & `libfwps-20240417/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/configure` & `libfwps-20240417/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfwps 20240310.
+# Generated by GNU Autoconf 2.71 for libfwps 20240417.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libfwps'
 PACKAGE_TARNAME='libfwps'
-PACKAGE_VERSION='20240310'
-PACKAGE_STRING='libfwps 20240310'
+PACKAGE_VERSION='20240417'
+PACKAGE_STRING='libfwps 20240417'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfwps.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1552,15 +1552,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfwps 20240310 to adapt to many kinds of systems.
+\`configure' configures libfwps 20240417 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1623,15 +1623,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfwps 20240310:";;
+     short | recursive ) echo "Configuration of libfwps 20240417:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1822,15 +1822,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfwps configure 20240310
+libfwps configure 20240417
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2543,15 +2543,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfwps $as_me 20240310, which was
+It was created by libfwps $as_me 20240417, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4032,15 +4032,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfwps'
- VERSION='20240310'
+ VERSION='20240417'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -24073,15 +24073,15 @@
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24223,15 +24223,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -25965,15 +25965,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26885,15 +26885,15 @@
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -30761,15 +30761,15 @@
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -30794,15 +30794,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31428,15 +31428,15 @@
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31592,15 +31592,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -32129,15 +32129,15 @@
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32192,15 +32192,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -39481,15 +39481,15 @@
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -39514,15 +39514,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -43037,15 +43037,15 @@
 
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
+    if test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43070,15 +43070,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -43731,15 +43731,15 @@
 
 
         ac_cv_libfguid_LIBADD="-lfguid"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
+    if test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfguid in directory: $ac_cv_with_libfguid
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43764,15 +43764,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -44079,14 +44079,16 @@
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
         case $host_os in #(
   cygwin*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
         BACKUP_CPPFLAGS="${CPPFLAGS}"
@@ -45008,15 +45010,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfwps $as_me 20240310, which was
+This file was extended by libfwps $as_me 20240417, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -45076,15 +45078,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfwps config.status 20240310
+libfwps config.status 20240417
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfwps-20240310/compile` & `libfwps-20240417/compile`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/missing` & `libfwps-20240417/missing`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/fwps_test_set/fwps_test_set.vcproj` & `libfwps-20240417/msvscpp/fwps_test_set/fwps_test_set.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/fwps_test_support/fwps_test_support.vcproj` & `libfwps-20240417/msvscpp/fwps_test_support/fwps_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/fwps_test_property_identifier/fwps_test_property_identifier.vcproj` & `libfwps-20240417/msvscpp/fwps_test_property_identifier/fwps_test_property_identifier.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/libfguid/libfguid.vcproj` & `libfwps-20240417/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/libfwps/libfwps.vcproj` & `libfwps-20240417/msvscpp/libfwps/libfwps.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/libclocale/libclocale.vcproj` & `libfwps-20240417/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/libfwps.sln` & `libfwps-20240417/msvscpp/libfwps.sln`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/Makefile.am` & `libfwps-20240417/msvscpp/Makefile.am`

 * *Files 22% similar despite different names*

```diff
@@ -17,13 +17,11 @@
 	libuna/libuna.vcproj \
 	pyfwps/pyfwps.vcproj \
 	libfwps.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libfwps-20240310/msvscpp/fwps_test_error/fwps_test_error.vcproj` & `libfwps-20240417/msvscpp/fwps_test_error/fwps_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/fwps_test_notify/fwps_test_notify.vcproj` & `libfwps-20240417/msvscpp/fwps_test_notify/fwps_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/libcdata/libcdata.vcproj` & `libfwps-20240417/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/libcthreads/libcthreads.vcproj` & `libfwps-20240417/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/fwps_test_store/fwps_test_store.vcproj` & `libfwps-20240417/msvscpp/fwps_test_store/fwps_test_store.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/fwps_test_record/fwps_test_record.vcproj` & `libfwps-20240417/msvscpp/fwps_test_record/fwps_test_record.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/libuna/libuna.vcproj` & `libfwps-20240417/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/Makefile.in` & `libfwps-20240417/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -407,15 +407,16 @@
 	libuna/libuna.vcproj \
 	pyfwps/pyfwps.vcproj \
 	libfwps.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -519,23 +520,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -614,13 +617,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwps-20240310/msvscpp/libcnotify/libcnotify.vcproj` & `libfwps-20240417/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/libcerror/libcerror.vcproj` & `libfwps-20240417/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/libfdatetime/libfdatetime.vcproj` & `libfwps-20240417/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/msvscpp/pyfwps/pyfwps.vcproj` & `libfwps-20240417/msvscpp/pyfwps/pyfwps.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/INSTALL` & `libfwps-20240417/INSTALL`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_list_element.h` & `libfwps-20240417/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_array.h` & `libfwps-20240417/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_definitions.h` & `libfwps-20240417/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libfwps-20240310/libcdata/libcdata_libcerror.h` & `libfwps-20240417/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_unused.h` & `libfwps-20240417/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_btree.h` & `libfwps-20240417/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_btree.c` & `libfwps-20240417/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_support.c` & `libfwps-20240417/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_list.c` & `libfwps-20240417/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_extern.h` & `libfwps-20240417/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_list.h` & `libfwps-20240417/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_btree_values_list.h` & `libfwps-20240417/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/Makefile.am` & `libfwps-20240417/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libfwps-20240310/libcdata/libcdata_btree_node.h` & `libfwps-20240417/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_range_list_value.h` & `libfwps-20240417/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_range_list.h` & `libfwps-20240417/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_range_list.c` & `libfwps-20240417/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_array.c` & `libfwps-20240417/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_list_element.c` & `libfwps-20240417/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_libcthreads.h` & `libfwps-20240417/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_tree_node.h` & `libfwps-20240417/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_error.h` & `libfwps-20240417/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_types.h` & `libfwps-20240417/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_btree_node.c` & `libfwps-20240417/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_tree_node.c` & `libfwps-20240417/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_support.h` & `libfwps-20240417/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/Makefile.in` & `libfwps-20240417/libcdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -464,16 +464,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -490,15 +490,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -708,24 +709,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -819,17 +833,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwps-20240310/libcdata/libcdata_range_list_value.c` & `libfwps-20240417/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_btree_values_list.c` & `libfwps-20240417/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcdata/libcdata_error.c` & `libfwps-20240417/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/config.sub` & `libfwps-20240417/config.sub`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/setup.py` & `libfwps-20240417/setup.py`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/acinclude.m4` & `libfwps-20240417/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/config.rpath` & `libfwps-20240417/config.rpath`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_thread.h` & `libfwps-20240417/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_read_write_lock.h` & `libfwps-20240417/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_thread.c` & `libfwps-20240417/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_thread_pool.h` & `libfwps-20240417/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_support.h` & `libfwps-20240417/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_lock.h` & `libfwps-20240417/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_unused.h` & `libfwps-20240417/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_lock.c` & `libfwps-20240417/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_condition.h` & `libfwps-20240417/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_repeating_thread.h` & `libfwps-20240417/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/Makefile.am` & `libfwps-20240417/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libfwps-20240310/libcthreads/libcthreads_support.c` & `libfwps-20240417/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_mutex.c` & `libfwps-20240417/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_queue.c` & `libfwps-20240417/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_mutex.h` & `libfwps-20240417/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_types.h` & `libfwps-20240417/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_thread_attributes.h` & `libfwps-20240417/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_condition.c` & `libfwps-20240417/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_error.c` & `libfwps-20240417/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_read_write_lock.c` & `libfwps-20240417/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_libcerror.h` & `libfwps-20240417/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_definitions.h` & `libfwps-20240417/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libfwps-20240310/libcthreads/libcthreads_thread_pool.c` & `libfwps-20240417/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_error.h` & `libfwps-20240417/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_thread_attributes.c` & `libfwps-20240417/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_extern.h` & `libfwps-20240417/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/libcthreads_repeating_thread.c` & `libfwps-20240417/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcthreads/Makefile.in` & `libfwps-20240417/libcthreads/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -468,16 +468,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -492,15 +492,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -710,24 +711,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -821,17 +835,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwps-20240310/libcthreads/libcthreads_queue.h` & `libfwps-20240417/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfwps.spec` & `libfwps-20240417/libfwps.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libfwps
-Version: 20240310
+Version: 20240417
 Release: 1
 Summary: Library to access the Windows Property Store format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfwps
         
@@ -76,10 +76,10 @@
 %files -n libfwps-python3
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %changelog
-* Sun Mar 10 2024 Joachim Metz <joachim.metz@gmail.com> 20240310-1
+* Wed Apr 17 2024 Joachim Metz <joachim.metz@gmail.com> 20240417-1
 - Auto-generated
```

### Comparing `libfwps-20240310/test-driver` & `libfwps-20240417/test-driver`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/manuals/libfwps.3` & `libfwps-20240417/manuals/libfwps.3`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.Dd February 25, 2024
+.Dd March 13, 2024
 .Dt libfwps 3
 .Os libfwps
 .Sh NAME
 .Nm libfwps.h
 .Nd Library to access the Windows Property Store format
 .Sh SYNOPSIS
 .In libfwps.h
@@ -73,14 +73,16 @@
 .Ft int
 .Fn libfwps_record_get_data_as_16bit_integer "libfwps_record_t *record" "uint16_t *value_16bit" "libfwps_error_t **error"
 .Ft int
 .Fn libfwps_record_get_data_as_32bit_integer "libfwps_record_t *record" "uint32_t *value_32bit" "libfwps_error_t **error"
 .Ft int
 .Fn libfwps_record_get_data_as_64bit_integer "libfwps_record_t *record" "uint64_t *value_64bit" "libfwps_error_t **error"
 .Ft int
+.Fn libfwps_record_get_data_as_floatingtime "libfwps_record_t *record" "uint64_t *floatingtime" "libfwps_error_t **error"
+.Ft int
 .Fn libfwps_record_get_data_as_filetime "libfwps_record_t *record" "uint64_t *filetime" "libfwps_error_t **error"
 .Ft int
 .Fn libfwps_record_get_data_as_floating_point "libfwps_record_t *record" "double *value_floating_point" "libfwps_error_t **error"
 .Ft int
 .Fn libfwps_record_get_data_as_utf8_string_size "libfwps_record_t *record" "size_t *utf8_string_size" "libfwps_error_t **error"
 .Ft int
 .Fn libfwps_record_get_data_as_utf8_string "libfwps_record_t *record" "uint8_t *utf8_string" "size_t utf8_string_size" "libfwps_error_t **error"
```

### Comparing `libfwps-20240310/manuals/Makefile.in` & `libfwps-20240417/manuals/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -421,15 +421,16 @@
 top_srcdir = @top_srcdir@
 man_MANS = \
 	libfwps.3
 
 EXTRA_DIST = \
 	libfwps.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -579,23 +580,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -676,13 +679,10 @@
 	mostlyclean mostlyclean-generic mostlyclean-libtool pdf pdf-am \
 	ps ps-am sources-am sources-local splint-am splint-local \
 	tags-am uninstall uninstall-am uninstall-man uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwps-20240310/tests/fwps_test_libfwps.h` & `libfwps-20240417/tests/fwps_test_libfwps.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/fwps_test_libcerror.h` & `libfwps-20240417/tests/fwps_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/fwps_test_store.c` & `libfwps-20240417/tests/fwps_test_store.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/fwps_test_memory.h` & `libfwps-20240417/tests/fwps_test_memory.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/Makefile.am` & `libfwps-20240417/tests/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
@@ -115,13 +115,12 @@
 	fwps_test_macros.h \
 	fwps_test_support.c \
 	fwps_test_unused.h
 
 fwps_test_support_LDADD = \
 	../libfwps/libfwps.la
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libfwps-20240310/tests/pyfwps_test_support.py` & `libfwps-20240417/tests/pyfwps_test_support.py`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/fwps_test_notify.c` & `libfwps-20240417/tests/fwps_test_notify.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/pyfwps_test_record.py` & `libfwps-20240417/tests/pyfwps_test_record.py`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/fwps_test_set.c` & `libfwps-20240417/tests/fwps_test_set.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/test_python_module.sh` & `libfwps-20240417/tests/test_python_module.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240416
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="record set store support";
 TEST_FUNCTIONS_WITH_INPUT="";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libfwps";
+PYTHON_MODULE="pyfwps";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyfwps_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyfwps_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyfwps");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/${LIBRARY_NAME}-1.dll ../${PYTHON_MODULE}/libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libfwps-20240310/tests/fwps_test_record.c` & `libfwps-20240417/tests/fwps_test_record.c`

 * *Files 1% similar despite different names*

```diff
@@ -789,25 +789,27 @@
 
 #endif /* !defined( __BORLANDC__ ) || ( __BORLANDC__ >= 0x0560 ) */
 #endif /* defined( __GNUC__ ) && !defined( LIBFWPS_DLL_IMPORT ) */
 
 	return( EXIT_SUCCESS );
 
 on_error:
+#if defined( __GNUC__ ) && !defined( LIBFWPS_DLL_IMPORT )
 #if !defined( __BORLANDC__ ) || ( __BORLANDC__ >= 0x0560 )
 
 	if( error != NULL )
 	{
 		libcerror_error_free(
 		 &error );
 	}
 	if( record != NULL )
 	{
 		libfwps_internal_record_free(
 		 (libfwps_internal_record_t **) &record,
 		 NULL );
 	}
 #endif /* !defined( __BORLANDC__ ) || ( __BORLANDC__ >= 0x0560 ) */
+#endif /* defined( __GNUC__ ) && !defined( LIBFWPS_DLL_IMPORT ) */
 
 	return( EXIT_FAILURE );
 }
```

### Comparing `libfwps-20240310/tests/test_runner.sh` & `libfwps-20240417/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/fwps_test_memory.c` & `libfwps-20240417/tests/fwps_test_memory.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/pyfwps_test_set.py` & `libfwps-20240417/tests/pyfwps_test_set.py`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/fwps_test_macros.h` & `libfwps-20240417/tests/fwps_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/fwps_test_property_identifier.c` & `libfwps-20240417/tests/fwps_test_property_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/pyfwps_test_store.py` & `libfwps-20240417/tests/pyfwps_test_store.py`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/fwps_test_error.c` & `libfwps-20240417/tests/fwps_test_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/Makefile.in` & `libfwps-20240417/tests/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -676,16 +676,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
@@ -785,16 +785,18 @@
 	fwps_test_macros.h \
 	fwps_test_support.c \
 	fwps_test_unused.h
 
 fwps_test_support_LDADD = \
 	../libfwps/libfwps.la
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1198,24 +1200,34 @@
 	-test -z "$(TEST_SUITE_LOG)" || rm -f $(TEST_SUITE_LOG)
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/fwps_test_error.Po
+	-rm -f ./$(DEPDIR)/fwps_test_memory.Po
+	-rm -f ./$(DEPDIR)/fwps_test_notify.Po
+	-rm -f ./$(DEPDIR)/fwps_test_property_identifier.Po
+	-rm -f ./$(DEPDIR)/fwps_test_record.Po
+	-rm -f ./$(DEPDIR)/fwps_test_set.Po
+	-rm -f ./$(DEPDIR)/fwps_test_store.Po
+	-rm -f ./$(DEPDIR)/fwps_test_support.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1306,13 +1318,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwps-20240310/tests/fwps_test_support.c` & `libfwps-20240417/tests/fwps_test_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/fwps_test_unused.h` & `libfwps-20240417/tests/fwps_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/tests/test_library.sh` & `libfwps-20240417/tests/test_library.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="error notify property_identifier record set store support";
 LIBRARY_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libfwps-20240310/libfwps.spec.in` & `libfwps-20240417/libfwps.spec.in`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/ossfuzz/ossfuzz_libfwps.h` & `libfwps-20240417/ossfuzz/ossfuzz_libfwps.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/ossfuzz/Makefile.am` & `libfwps-20240417/ossfuzz/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common
 
 bin_PROGRAMS = \
 	record_fuzzer \
 	set_fuzzer \
 	store_fuzzer
 
 record_fuzzer_SOURCES = \
@@ -29,20 +29,18 @@
 	store_fuzzer.cc
 
 store_fuzzer_LDADD = \
 	@LIB_FUZZING_ENGINE@ \
 	../libfwps/libfwps.la
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on record_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(record_fuzzer_SOURCES)
 	@echo "Running splint on set_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(set_fuzzer_SOURCES)
 	@echo "Running splint on store_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(store_fuzzer_SOURCES)
```

### Comparing `libfwps-20240310/ossfuzz/store_fuzzer.cc` & `libfwps-20240417/ossfuzz/store_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/ossfuzz/record_fuzzer.cc` & `libfwps-20240417/ossfuzz/record_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/ossfuzz/Makefile.in` & `libfwps-20240417/ossfuzz/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -474,16 +474,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@record_fuzzer_SOURCES = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libfwps.h \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	record_fuzzer.cc
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@record_fuzzer_LDADD = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
@@ -501,15 +501,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libfwps.h \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	store_fuzzer.cc
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@store_fuzzer_LDADD = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfwps/libfwps.la
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -761,23 +762,28 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/record_fuzzer.Po
+	-rm -f ./$(DEPDIR)/set_fuzzer.Po
+	-rm -f ./$(DEPDIR)/store_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -863,17 +869,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on record_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(record_fuzzer_SOURCES)
 	@echo "Running splint on set_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(set_fuzzer_SOURCES)
 	@echo "Running splint on store_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(store_fuzzer_SOURCES)
```

### Comparing `libfwps-20240310/ossfuzz/set_fuzzer.cc` & `libfwps-20240417/ossfuzz/set_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/ltmain.sh` & `libfwps-20240417/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/po/remove-potcdate.sin` & `libfwps-20240417/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/po/Makefile.in.in` & `libfwps-20240417/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/po/en@quot.header` & `libfwps-20240417/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/po/en@boldquot.header` & `libfwps-20240417/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/po/insert-header.sin` & `libfwps-20240417/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/po/Makevars` & `libfwps-20240417/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/po/Makevars.in` & `libfwps-20240417/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/po/Rules-quot` & `libfwps-20240417/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1251.c` & `libfwps-20240417/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_utf16_string.c` & `libfwps-20240417/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_base16_stream.c` & `libfwps-20240417/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_utf8_stream.h` & `libfwps-20240417/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_2.h` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_932.c` & `libfwps-20240417/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_dingbats.h` & `libfwps-20240417/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_utf8_string.c` & `libfwps-20240417/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_base64_stream.c` & `libfwps-20240417/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_error.h` & `libfwps-20240417/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_turkish.h` & `libfwps-20240417/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_unicode_character.c` & `libfwps-20240417/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_gaelic.c` & `libfwps-20240417/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_arabic.h` & `libfwps-20240417/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_thai.c` & `libfwps-20240417/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_874.h` & `libfwps-20240417/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_15.h` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_utf8_string.h` & `libfwps-20240417/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_16.c` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1255.c` & `libfwps-20240417/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_utf7_stream.c` & `libfwps-20240417/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_byte_stream.h` & `libfwps-20240417/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_koi8_u.c` & `libfwps-20240417/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_unused.h` & `libfwps-20240417/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_6.c` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_14.c` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_base64_stream.h` & `libfwps-20240417/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_error.c` & `libfwps-20240417/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_centraleurroman.h` & `libfwps-20240417/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_romanian.c` & `libfwps-20240417/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_6.h` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_9.c` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_russian.h` & `libfwps-20240417/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_dingbats.c` & `libfwps-20240417/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_15.c` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_936.c` & `libfwps-20240417/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_croatian.h` & `libfwps-20240417/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_scsu.h` & `libfwps-20240417/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/Makefile.am` & `libfwps-20240417/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,19 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libfwps-20240310/libuna/libuna_utf32_stream.c` & `libfwps-20240417/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_936.h` & `libfwps-20240417/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_10.c` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_roman.c` & `libfwps-20240417/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_utf7_stream.h` & `libfwps-20240417/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_3.h` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_thai.h` & `libfwps-20240417/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_farsi.h` & `libfwps-20240417/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_ukrainian.c` & `libfwps-20240417/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_inuit.c` & `libfwps-20240417/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_932.h` & `libfwps-20240417/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_874.c` & `libfwps-20240417/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_5.c` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_10.h` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_definitions.h` & `libfwps-20240417/libuna/libuna_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20240130
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20240130"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libfwps-20240310/libuna/libuna_url_stream.h` & `libfwps-20240417/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_icelandic.h` & `libfwps-20240417/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_koi8_u.h` & `libfwps-20240417/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_utf16_stream.c` & `libfwps-20240417/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1253.c` & `libfwps-20240417/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_4.h` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_greek.c` & `libfwps-20240417/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_libcerror.h` & `libfwps-20240417/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_centraleurroman.c` & `libfwps-20240417/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1254.c` & `libfwps-20240417/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_13.h` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_7.h` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1255.h` & `libfwps-20240417/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_unicode_character.h` & `libfwps-20240417/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_8.h` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_13.c` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_949.h` & `libfwps-20240417/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_cyrillic.c` & `libfwps-20240417/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_celtic.c` & `libfwps-20240417/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_support.h` & `libfwps-20240417/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_4.c` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_949.c` & `libfwps-20240417/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_utf16_stream.h` & `libfwps-20240417/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_symbol.c` & `libfwps-20240417/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_roman.h` & `libfwps-20240417/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1257.c` & `libfwps-20240417/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1254.h` & `libfwps-20240417/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_950.c` & `libfwps-20240417/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_extern.h` & `libfwps-20240417/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1256.c` & `libfwps-20240417/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_types.h` & `libfwps-20240417/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_base32_stream.h` & `libfwps-20240417/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1253.h` & `libfwps-20240417/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_16.h` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_utf8_stream.c` & `libfwps-20240417/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1250.h` & `libfwps-20240417/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_2.c` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_support.c` & `libfwps-20240417/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_koi8_r.c` & `libfwps-20240417/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_5.h` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_utf16_string.h` & `libfwps-20240417/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_utf32_string.c` & `libfwps-20240417/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_icelandic.c` & `libfwps-20240417/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1256.h` & `libfwps-20240417/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_utf32_string.h` & `libfwps-20240417/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_romanian.h` & `libfwps-20240417/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_8.c` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_koi8_r.h` & `libfwps-20240417/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_cyrillic.h` & `libfwps-20240417/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_arabic.c` & `libfwps-20240417/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_croatian.c` & `libfwps-20240417/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_9.h` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_greek.h` & `libfwps-20240417/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1258.h` & `libfwps-20240417/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_7.c` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/Makefile.in` & `libfwps-20240417/libuna/Makefile.in`

 * *Files 7% similar despite different names*

```diff
@@ -622,16 +622,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -697,15 +697,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -967,24 +968,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1130,17 +1196,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_3.c` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1250.c` & `libfwps-20240417/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_scsu.c` & `libfwps-20240417/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1252.c` & `libfwps-20240417/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_turkish.c` & `libfwps-20240417/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_ukrainian.h` & `libfwps-20240417/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_russian.c` & `libfwps-20240417/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1258.c` & `libfwps-20240417/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_celtic.h` & `libfwps-20240417/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_byte_stream.c` & `libfwps-20240417/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_gaelic.h` & `libfwps-20240417/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_utf32_stream.h` & `libfwps-20240417/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_symbol.h` & `libfwps-20240417/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1257.h` & `libfwps-20240417/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_inuit.h` & `libfwps-20240417/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_mac_farsi.c` & `libfwps-20240417/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_950.h` & `libfwps-20240417/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_url_stream.c` & `libfwps-20240417/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1251.h` & `libfwps-20240417/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_windows_1252.h` & `libfwps-20240417/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_codepage_iso_8859_14.h` & `libfwps-20240417/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_base16_stream.h` & `libfwps-20240417/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libuna/libuna_base32_stream.c` & `libfwps-20240417/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/Makefile.in` & `libfwps-20240417/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -559,16 +559,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libfwps.pc \
+	libfwps.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libfwps.pc
 
 all: all-recursive
 
@@ -985,23 +992,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1106,22 +1116,10 @@
 	(cd $(srcdir)/libcnotify && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libuna && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwps && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfwps.pc
-	-rm -f libfwps.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwps-20240310/libcnotify/libcnotify_definitions.h` & `libfwps-20240417/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libfwps-20240310/libcnotify/libcnotify_extern.h` & `libfwps-20240417/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcnotify/libcnotify_support.c` & `libfwps-20240417/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcnotify/libcnotify_stream.h` & `libfwps-20240417/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcnotify/Makefile.am` & `libfwps-20240417/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libfwps-20240310/libcnotify/libcnotify_unused.h` & `libfwps-20240417/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcnotify/libcnotify_verbose.h` & `libfwps-20240417/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcnotify/libcnotify_print.h` & `libfwps-20240417/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcnotify/libcnotify_stream.c` & `libfwps-20240417/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcnotify/libcnotify_support.h` & `libfwps-20240417/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcnotify/libcnotify_verbose.c` & `libfwps-20240417/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcnotify/Makefile.in` & `libfwps-20240417/libcnotify/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -446,30 +446,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -672,24 +673,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -776,17 +783,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwps-20240310/libcnotify/libcnotify_libcerror.h` & `libfwps-20240417/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcnotify/libcnotify_print.c` & `libfwps-20240417/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcerror/libcerror_system.c` & `libfwps-20240417/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcerror/libcerror_error.c` & `libfwps-20240417/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcerror/libcerror_extern.h` & `libfwps-20240417/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcerror/Makefile.am` & `libfwps-20240417/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libfwps-20240310/libcerror/libcerror_types.h` & `libfwps-20240417/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcerror/libcerror_support.h` & `libfwps-20240417/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcerror/libcerror_error.h` & `libfwps-20240417/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcerror/libcerror_system.h` & `libfwps-20240417/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcerror/libcerror_definitions.h` & `libfwps-20240417/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libfwps-20240310/libcerror/libcerror_support.c` & `libfwps-20240417/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcerror/libcerror_unused.h` & `libfwps-20240417/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libcerror/Makefile.in` & `libfwps-20240417/libcerror/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -443,28 +443,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -666,24 +667,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -769,17 +775,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_floatingtime.h` & `libfwps-20240417/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_nsf_timedate.c` & `libfwps-20240417/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_error.h` & `libfwps-20240417/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_floatingtime.c` & `libfwps-20240417/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_support.h` & `libfwps-20240417/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_hfs_time.h` & `libfwps-20240417/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_definitions.h` & `libfwps-20240417/libfdatetime/libfdatetime_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfdatetime/definitions.h> are copied here
  * for local use of libfdatetime
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFDATETIME_VERSION					20240115
+#define LIBFDATETIME_VERSION					20240415
 
 /* The version string
  */
-#define LIBFDATETIME_VERSION_STRING				"20240115"
+#define LIBFDATETIME_VERSION_STRING				"20240415"
 
 /* The byte order definitions
  */
 #define LIBFDATETIME_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFDATETIME_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The string format definition flags
```

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_hfs_time.c` & `libfwps-20240417/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/Makefile.am` & `libfwps-20240417/libfdatetime/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATETIME
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfdatetime.la
 
 libfdatetime_la_SOURCES = \
 	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 	libfdatetime_definitions.h \
@@ -20,19 +20,17 @@
 	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 	libfdatetime_support.c libfdatetime_support.h \
 	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 	libfdatetime_types.h \
 	libfdatetime_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
```

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_filetime.c` & `libfwps-20240417/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_systemtime.h` & `libfwps-20240417/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_extern.h` & `libfwps-20240417/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_posix_time.c` & `libfwps-20240417/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_unused.h` & `libfwps-20240417/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_fat_date_time.h` & `libfwps-20240417/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_systemtime.c` & `libfwps-20240417/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_nsf_timedate.h` & `libfwps-20240417/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_libcerror.h` & `libfwps-20240417/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_support.c` & `libfwps-20240417/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_error.c` & `libfwps-20240417/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_posix_time.h` & `libfwps-20240417/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_date_time_values.h` & `libfwps-20240417/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_filetime.h` & `libfwps-20240417/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_date_time_values.c` & `libfwps-20240417/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_types.h` & `libfwps-20240417/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/libfdatetime/Makefile.in` & `libfwps-20240417/libfdatetime/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -465,16 +465,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFDATETIME_TRUE@noinst_LTLIBRARIES = libfdatetime.la
 @HAVE_LOCAL_LIBFDATETIME_TRUE@libfdatetime_la_SOURCES = \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_definitions.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_extern.h \
@@ -487,15 +487,16 @@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_nsf_timedate.c libfdatetime_nsf_timedate.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_support.c libfdatetime_support.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_types.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -704,24 +705,36 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdatetime_date_time_values.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_error.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_fat_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_floatingtime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_hfs_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_nsf_timedate.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_posix_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_support.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_systemtime.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -814,17 +827,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwps-20240310/libfdatetime/libfdatetime_fat_date_time.c` & `libfwps-20240417/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/aclocal.m4` & `libfwps-20240417/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_set.h` & `libfwps-20240417/pyfwps/pyfwps_set.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_set.c` & `libfwps-20240417/pyfwps/pyfwps_set.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_guid.h` & `libfwps-20240417/pyfwps/pyfwps_guid.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_libfguid.h` & `libfwps-20240417/pyfwps/pyfwps_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_store.c` & `libfwps-20240417/pyfwps/pyfwps_store.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_libuna.h` & `libfwps-20240417/pyfwps/pyfwps_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_codepage.c` & `libfwps-20240417/pyfwps/pyfwps_codepage.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_record.h` & `libfwps-20240417/pyfwps/pyfwps_record.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_records.c` & `libfwps-20240417/pyfwps/pyfwps_records.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_string.c` & `libfwps-20240417/pyfwps/pyfwps_string.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_integer.c` & `libfwps-20240417/pyfwps/pyfwps_integer.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_store.h` & `libfwps-20240417/pyfwps/pyfwps_store.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_guid.c` & `libfwps-20240417/pyfwps/pyfwps_guid.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/Makefile.am` & `libfwps-20240417/pyfwps/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
 	@LIBFWPS_DLL_IMPORT@
 
@@ -40,13 +40,11 @@
 	@LIBFGUID_LIBADD@
 
 pyfwps_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyfwps_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libfwps-20240310/pyfwps/pyfwps_error.c` & `libfwps-20240417/pyfwps/pyfwps_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_sets.c` & `libfwps-20240417/pyfwps/pyfwps_sets.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_codepage.h` & `libfwps-20240417/pyfwps/pyfwps_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_error.h` & `libfwps-20240417/pyfwps/pyfwps_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps.c` & `libfwps-20240417/pyfwps/pyfwps.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps.h` & `libfwps-20240417/pyfwps/pyfwps.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_integer.h` & `libfwps-20240417/pyfwps/pyfwps_integer.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_libcerror.h` & `libfwps-20240417/pyfwps/pyfwps_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_records.h` & `libfwps-20240417/pyfwps/pyfwps_records.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_python.h` & `libfwps-20240417/pyfwps/pyfwps_python.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_unused.h` & `libfwps-20240417/pyfwps/pyfwps_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_libfwps.h` & `libfwps-20240417/pyfwps/pyfwps_libfwps.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_string.h` & `libfwps-20240417/pyfwps/pyfwps_string.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_libclocale.h` & `libfwps-20240417/pyfwps/pyfwps_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/pyfwps_record.c` & `libfwps-20240417/pyfwps/pyfwps_record.c`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/pyfwps/Makefile.in` & `libfwps-20240417/pyfwps/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -494,16 +494,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBFGUID_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBFWPS_DLL_IMPORT@
 
@@ -534,15 +534,16 @@
 @HAVE_PYTHON_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBFGUID_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyfwps_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyfwps_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -856,24 +857,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps.Plo
+	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_codepage.Plo
+	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_error.Plo
+	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_guid.Plo
+	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_integer.Plo
+	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_record.Plo
+	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_records.Plo
+	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_set.Plo
+	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_sets.Plo
+	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_store.Plo
+	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -968,13 +982,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwps-20240310/pyfwps/pyfwps_sets.h` & `libfwps-20240417/pyfwps/pyfwps_sets.h`

 * *Files identical despite different names*

### Comparing `libfwps-20240310/configure.ac` & `libfwps-20240417/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfwps],
- [20240310],
+ [20240417],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfwps.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

