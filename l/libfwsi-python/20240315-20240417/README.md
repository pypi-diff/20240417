# Comparing `tmp/libfwsi-python-20240315.tar.gz` & `tmp/libfwsi-python-20240417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfwsi-python-20240315.tar", last modified: Sun Mar 17 17:42:49 2024, max compression
+gzip compressed data, was "libfwsi-python-20240417.tar", last modified: Wed Apr 17 16:04:37 2024, max compression
```

## Comparing `libfwsi-python-20240315.tar` & `libfwsi-python-20240417.tar`

### file list

```diff
@@ -1,779 +1,779 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:48.000000 libfwsi-20240315/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:48.000000 libfwsi-20240315/libfole/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-03-17 17:26:55.000000 libfwsi-20240315/libfole/libfole_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-17 17:26:55.000000 libfwsi-20240315/libfole/libfole_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      665 2024-03-17 17:26:55.000000 libfwsi-20240315/libfole/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1555 2024-03-17 17:26:55.000000 libfwsi-20240315/libfole/libfole_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-17 17:26:55.000000 libfwsi-20240315/libfole/libfole_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-03-17 17:26:55.000000 libfwsi-20240315/libfole/libfole_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1407 2024-03-17 17:26:55.000000 libfwsi-20240315/libfole/libfole_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-03-17 17:26:55.000000 libfwsi-20240315/libfole/libfole_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3793 2024-03-17 17:26:55.000000 libfwsi-20240315/libfole/libfole_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-17 17:26:55.000000 libfwsi-20240315/libfole/libfole_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-17 17:26:55.000000 libfwsi-20240315/libfole/libfole_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26640 2024-03-17 17:27:09.000000 libfwsi-20240315/libfole/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-17 17:26:55.000000 libfwsi-20240315/libfole/libfole_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-03-01 11:57:16.000000 libfwsi-20240315/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-03-17 17:27:09.000000 libfwsi-20240315/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-01 11:57:16.000000 libfwsi-20240315/NEWS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2593 2024-03-01 11:57:16.000000 libfwsi-20240315/libfwsi.spec.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-03-17 17:27:09.000000 libfwsi-20240315/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:47.000000 libfwsi-20240315/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-17 17:26:53.000000 libfwsi-20240315/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-03-17 17:26:53.000000 libfwsi-20240315/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-03-17 17:26:53.000000 libfwsi-20240315/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-17 17:26:53.000000 libfwsi-20240315/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-03-17 17:26:53.000000 libfwsi-20240315/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-17 17:26:53.000000 libfwsi-20240315/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-17 17:26:53.000000 libfwsi-20240315/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-03-17 17:26:53.000000 libfwsi-20240315/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-03-17 17:26:53.000000 libfwsi-20240315/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-03-17 17:26:53.000000 libfwsi-20240315/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-03-17 17:26:53.000000 libfwsi-20240315/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26717 2024-03-17 17:27:09.000000 libfwsi-20240315/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-17 17:26:53.000000 libfwsi-20240315/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:47.000000 libfwsi-20240315/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3956 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/libfole.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-03-17 17:27:04.000000 libfwsi-20240315/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-03-17 17:27:04.000000 libfwsi-20240315/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10036 2024-02-25 06:26:28.000000 libfwsi-20240315/m4/libfwps.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-03-17 17:27:04.000000 libfwsi-20240315/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-03-17 17:27:04.000000 libfwsi-20240315/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-03-17 17:27:04.000000 libfwsi-20240315/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:09:43.000000 libfwsi-20240315/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:47.000000 libfwsi-20240315/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25612 2024-03-17 17:07:30.000000 libfwsi-20240315/include/libfwsi.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25612 2024-03-17 17:27:25.000000 libfwsi-20240315/include/libfwsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      459 2024-03-01 11:58:03.000000 libfwsi-20240315/include/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:47.000000 libfwsi-20240315/include/libfwsi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-03-15 20:54:44.000000 libfwsi-20240315/include/libfwsi/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3262 2024-03-17 17:27:26.000000 libfwsi-20240315/include/libfwsi/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5015 2024-03-01 11:57:18.000000 libfwsi-20240315/include/libfwsi/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4884 2024-03-17 17:27:26.000000 libfwsi-20240315/include/libfwsi/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-03-01 11:58:03.000000 libfwsi-20240315/include/libfwsi/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-03-01 11:57:18.000000 libfwsi-20240315/include/libfwsi/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-03-01 11:57:18.000000 libfwsi-20240315/include/libfwsi/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-03-17 17:27:26.000000 libfwsi-20240315/include/libfwsi/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2024-03-01 11:57:18.000000 libfwsi-20240315/include/libfwsi/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25244 2024-03-17 17:27:09.000000 libfwsi-20240315/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:48.000000 libfwsi-20240315/libfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2490 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_set.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_store.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1206 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3827 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3731 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_format_class_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9704 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_store.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3967 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2244 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_property_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_format_class_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7534 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_property_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6987 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81635 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16442 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_set.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29329 2024-03-17 17:27:09.000000 libfwsi-20240315/libfwps/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-17 17:26:56.000000 libfwsi-20240315/libfwps/libfwps_unused.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:47.000000 libfwsi-20240315/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-03-01 11:57:18.000000 libfwsi-20240315/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-03-01 11:57:18.000000 libfwsi-20240315/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-03-01 11:57:18.000000 libfwsi-20240315/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-03-01 11:57:18.000000 libfwsi-20240315/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-03-01 11:57:18.000000 libfwsi-20240315/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-03-01 11:57:18.000000 libfwsi-20240315/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-03-01 11:57:18.000000 libfwsi-20240315/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-03-01 11:57:16.000000 libfwsi-20240315/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-03-01 11:57:18.000000 libfwsi-20240315/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-03-17 17:27:26.000000 libfwsi-20240315/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12626 2024-03-17 17:27:08.000000 libfwsi-20240315/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13364 2024-03-17 17:27:26.000000 libfwsi-20240315/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-03-01 11:57:18.000000 libfwsi-20240315/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-03-01 11:57:18.000000 libfwsi-20240315/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-03-01 11:57:18.000000 libfwsi-20240315/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22270 2024-03-17 17:27:09.000000 libfwsi-20240315/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:47.000000 libfwsi-20240315/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-03-17 17:26:47.000000 libfwsi-20240315/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-03-17 17:26:47.000000 libfwsi-20240315/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-03-17 17:26:47.000000 libfwsi-20240315/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-03-17 17:26:47.000000 libfwsi-20240315/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-17 17:26:47.000000 libfwsi-20240315/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-17 17:26:47.000000 libfwsi-20240315/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-03-17 17:26:47.000000 libfwsi-20240315/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-03-17 17:26:47.000000 libfwsi-20240315/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-03-17 17:26:47.000000 libfwsi-20240315/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-03-17 17:26:47.000000 libfwsi-20240315/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27273 2024-03-17 17:27:09.000000 libfwsi-20240315/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-17 17:26:47.000000 libfwsi-20240315/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-03-17 17:26:47.000000 libfwsi-20240315/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-03-17 17:26:47.000000 libfwsi-20240315/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:48.000000 libfwsi-20240315/pyfwsi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3254 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2413 2024-03-01 11:58:29.000000 libfwsi-20240315/pyfwsi/pyfwsi_extension_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4381 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_control_panel_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4432 2024-03-01 11:57:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_root_folder.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2888 2024-03-01 11:58:29.000000 libfwsi-20240315/pyfwsi/pyfwsi_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8868 2024-03-01 11:57:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7439 2024-03-17 17:14:38.000000 libfwsi-20240315/pyfwsi/pyfwsi_users_property_view.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9661 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_extension_blocks.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_control_panel_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-03-01 11:57:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10914 2024-03-01 11:58:29.000000 libfwsi-20240315/pyfwsi/pyfwsi_network_location.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1815 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1685 2024-03-16 07:13:41.000000 libfwsi-20240315/pyfwsi/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9447 2024-03-16 07:17:29.000000 libfwsi-20240315/pyfwsi/pyfwsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1423 2024-03-16 07:13:24.000000 libfwsi-20240315/pyfwsi/pyfwsi_compressed_folder.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8645 2024-03-16 07:14:40.000000 libfwsi-20240315/pyfwsi/pyfwsi_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2317 2024-03-01 11:57:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_items.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1862 2024-03-01 11:58:29.000000 libfwsi-20240315/pyfwsi/pyfwsi_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_control_panel_category.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8979 2024-03-01 11:57:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_items.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2852 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_guid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16477 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_file_entry_extension.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11207 2024-03-01 11:58:29.000000 libfwsi-20240315/pyfwsi/pyfwsi_extension_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1667 2024-03-01 11:57:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_network_location.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2024-03-01 11:57:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-03-01 11:57:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-01 11:57:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_root_folder.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_file_entry_extension.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-01 11:57:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-03-01 11:57:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5329 2024-03-16 07:16:37.000000 libfwsi-20240315/pyfwsi/pyfwsi_compressed_folder.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-03-01 11:57:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4275 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_control_panel_category.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-03-01 11:57:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_libfwsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15996 2024-03-16 07:31:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_item_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1592 2024-03-17 17:10:09.000000 libfwsi-20240315/pyfwsi/pyfwsi_users_property_view.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2024-03-01 11:57:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22036 2024-03-16 07:31:37.000000 libfwsi-20240315/pyfwsi/pyfwsi_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_guid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    61238 2024-03-17 17:27:09.000000 libfwsi-20240315/pyfwsi/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11390 2024-03-01 11:58:29.000000 libfwsi-20240315/pyfwsi/pyfwsi_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2024-03-01 11:57:21.000000 libfwsi-20240315/pyfwsi/pyfwsi_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2024-03-01 11:58:29.000000 libfwsi-20240315/pyfwsi/pyfwsi_item_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2548 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_extension_blocks.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16593 2024-03-01 11:57:20.000000 libfwsi-20240315/pyfwsi/pyfwsi_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1973 2023-12-03 09:09:40.000000 libfwsi-20240315/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:09:40.000000 libfwsi-20240315/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-03-17 17:27:09.000000 libfwsi-20240315/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:47.000000 libfwsi-20240315/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-03-01 11:57:21.000000 libfwsi-20240315/dpkg/copyright
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-03-01 11:57:16.000000 libfwsi-20240315/dpkg/libfwsi-dev.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:47.000000 libfwsi-20240315/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-03-01 11:57:16.000000 libfwsi-20240315/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1541 2024-03-01 11:57:16.000000 libfwsi-20240315/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      703 2024-03-01 11:57:16.000000 libfwsi-20240315/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-03-01 11:57:16.000000 libfwsi-20240315/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-03-17 17:27:26.000000 libfwsi-20240315/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-03-01 11:57:16.000000 libfwsi-20240315/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-03-01 11:57:16.000000 libfwsi-20240315/dpkg/libfwsi-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-03-01 11:57:16.000000 libfwsi-20240315/dpkg/libfwsi.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-03-17 17:27:26.000000 libfwsi-20240315/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-03-01 11:57:16.000000 libfwsi-20240315/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1558785 2024-03-17 17:27:07.000000 libfwsi-20240315/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-03-17 17:27:09.000000 libfwsi-20240315/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-03-17 17:27:09.000000 libfwsi-20240315/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_file_entry_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_file_entry_values/fwsi_test_file_entry_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_uri_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5376 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_uri_values/fwsi_test_uri_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/libfole/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4605 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/libfole/libfole.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_game_folder_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_game_folder_values/fwsi_test_game_folder_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_volume_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5385 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_volume_values/fwsi_test_volume_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_compressed_folder_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5418 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_compressed_folder_values/fwsi_test_compressed_folder_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0014_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0014_values/fwsi_test_extension_block_0xbeef0014_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block/fwsi_test_extension_block.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5118 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_error/fwsi_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/libfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6465 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/libfwps/libfwps.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34936 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/libfwsi.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0019_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0019_values/fwsi_test_extension_block_0xbeef0019_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/pyfwsi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8591 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/pyfwsi/pyfwsi.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2986 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_mtp_volume_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_mtp_volume_values/fwsi_test_mtp_volume_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_root_folder_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_root_folder_values/fwsi_test_root_folder_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:48.000000 libfwsi-20240315/msvscpp/fwsi_test_cdburn_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5385 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_cdburn_values/fwsi_test_cdburn_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0001_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0001_values/fwsi_test_extension_block_0xbeef0001_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0025_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0025_values/fwsi_test_extension_block_0xbeef0025_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_uri_sub_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5388 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_uri_sub_values/fwsi_test_uri_sub_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_delegate_folder_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5412 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_delegate_folder_values/fwsi_test_delegate_folder_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_control_panel_category_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5433 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_control_panel_category_values/fwsi_test_control_panel_category_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_control_panel_item_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5421 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_control_panel_item_values/fwsi_test_control_panel_item_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/libfwsi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15759 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/libfwsi/libfwsi.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_network_location_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5415 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_network_location_values/fwsi_test_network_location_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_control_panel_cpl_file_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5433 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_control_panel_cpl_file_values/fwsi_test_control_panel_cpl_file_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0000_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0000_values/fwsi_test_extension_block_0xbeef0000_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_users_property_view_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5424 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_users_property_view_values/fwsi_test_users_property_view_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0006_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0006_values/fwsi_test_extension_block_0xbeef0006_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5124 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_support/fwsi_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_file_entry_extension_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5427 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_file_entry_extension_values/fwsi_test_file_entry_extension_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_item/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5358 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_item/fwsi_test_item.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_mtp_file_entry_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5409 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_mtp_file_entry_values/fwsi_test_mtp_file_entry_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0013_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0013_values/fwsi_test_extension_block_0xbeef0013_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22224 2024-03-17 17:27:09.000000 libfwsi-20240315/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef000a_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef000a_values/fwsi_test_extension_block_0xbeef000a_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_item_list/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5373 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_item_list/fwsi_test_item_list.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0005_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0005_values/fwsi_test_extension_block_0xbeef0005_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0003_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0003_values/fwsi_test_extension_block_0xbeef0003_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:49.000000 libfwsi-20240315/msvscpp/fwsi_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5204 2024-03-17 17:08:05.000000 libfwsi-20240315/msvscpp/fwsi_test_notify/fwsi_test_notify.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-03-01 11:57:18.000000 libfwsi-20240315/AUTHORS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      301 2024-03-01 11:57:16.000000 libfwsi-20240315/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-03-17 17:27:09.000000 libfwsi-20240315/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:48.000000 libfwsi-20240315/libfwsi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1888 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_control_panel_cpl_file_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10702 2024-03-16 07:01:34.000000 libfwsi-20240315/libfwsi/libfwsi_compressed_folder.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2824 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_control_panel_category.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1076 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6183 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_known_folder_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8008 2024-03-16 06:38:13.000000 libfwsi-20240315/libfwsi/libfwsi_delegate_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1609 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_uri_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0001_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21171 2024-03-16 07:05:09.000000 libfwsi-20240315/libfwsi/libfwsi_file_entry_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0000_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_libfole.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-03-17 17:04:55.000000 libfwsi-20240315/libfwsi/libfwsi_users_property_view.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5770 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_game_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12685 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_item_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0003_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6750 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_uri_sub_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1074 2024-03-17 17:27:26.000000 libfwsi-20240315/libfwsi/libfwsi.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6785 2024-03-15 18:37:41.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0000_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3733 2024-03-17 17:27:26.000000 libfwsi-20240315/libfwsi/libfwsi_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1377 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_control_panel_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0013_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2792 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_known_folder_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1920 2024-03-16 06:23:56.000000 libfwsi-20240315/libfwsi/libfwsi_compressed_folder.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6330 2024-03-16 08:49:16.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0027_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5972 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0003_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7080 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0026_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0025_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_game_folder_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2941 2024-03-16 07:04:40.000000 libfwsi-20240315/libfwsi/libfwsi_file_entry_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0014_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1903 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_control_panel_category_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0029_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16884 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_mtp_file_entry_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1190 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_file_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0006_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9231 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0014_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1762 2024-03-17 16:58:29.000000 libfwsi-20240315/libfwsi/libfwsi_root_folder_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2305 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_file_entry_extension_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13595 2024-03-17 17:09:26.000000 libfwsi-20240315/libfwsi/libfwsi_users_property_view_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4738 2024-03-16 08:10:02.000000 libfwsi-20240315/libfwsi/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5986 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0013_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6191 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0006_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17787 2024-03-06 18:47:31.000000 libfwsi-20240315/libfwsi/libfwsi_mtp_volume_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11512 2024-03-16 07:05:34.000000 libfwsi-20240315/libfwsi/libfwsi_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12898 2024-03-16 06:37:33.000000 libfwsi-20240315/libfwsi/libfwsi_acronis_tib_file_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_control_panel_category.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_root_folder.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52733 2024-03-17 16:50:38.000000 libfwsi-20240315/libfwsi/libfwsi_shell_folder_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5555 2024-03-16 08:19:55.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0029_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_cdburn_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1673 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_uri_sub_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2646 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2421 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_item_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8940 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_control_panel_cpl_file_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef000a_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2001 2024-03-16 08:25:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0027_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5435 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0005_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_mtp_volume_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2383 2024-03-17 17:03:10.000000 libfwsi-20240315/libfwsi/libfwsi_users_property_view_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2317 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6230 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0019_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0026_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2133 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_network_location_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-03-15 19:38:26.000000 libfwsi-20240315/libfwsi/libfwsi_web_site_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16822 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_file_entry_extension_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1805 2024-03-15 20:59:00.000000 libfwsi-20240315/libfwsi/libfwsi_acronis_tib_file_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3735 2024-03-15 20:54:55.000000 libfwsi-20240315/libfwsi/libfwsi_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26408 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_file_entry_extension.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10306 2024-03-16 06:39:04.000000 libfwsi-20240315/libfwsi/libfwsi_web_site_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9361 2024-03-16 07:07:16.000000 libfwsi-20240315/libfwsi/libfwsi_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6603 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0025_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15636 2024-03-16 09:31:15.000000 libfwsi-20240315/libfwsi/libfwsi_compressed_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0019_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2059 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_control_panel_item_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7525 2024-03-16 06:38:05.000000 libfwsi-20240315/libfwsi/libfwsi_control_panel_item_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2666 2024-03-16 06:46:59.000000 libfwsi-20240315/libfwsi/libfwsi_compressed_folder_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5798 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_cdburn_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5814 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_control_panel_category_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2465 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_control_panel_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13461 2024-03-16 09:26:58.000000 libfwsi-20240315/libfwsi/libfwsi_network_location_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15825 2024-03-16 08:17:59.000000 libfwsi-20240315/libfwsi/libfwsi_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48490 2024-03-16 13:11:56.000000 libfwsi-20240315/libfwsi/libfwsi_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3766 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_control_panel_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3228 2024-03-16 07:06:03.000000 libfwsi-20240315/libfwsi/libfwsi_volume_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3347 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_file_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2794 2024-03-16 08:17:25.000000 libfwsi-20240315/libfwsi/libfwsi_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14142 2024-03-16 06:38:50.000000 libfwsi-20240315/libfwsi/libfwsi_uri_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1514 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_libfwps.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5656 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef000a_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3419 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_file_entry_extension.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5798 2024-03-16 06:38:42.000000 libfwsi-20240315/libfwsi/libfwsi_root_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24188 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_network_location.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3432 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_network_location.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16168 2024-03-16 07:07:43.000000 libfwsi-20240315/libfwsi/libfwsi_volume_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1816 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_mtp_file_entry_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3149 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_root_folder.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45688 2024-03-17 17:27:09.000000 libfwsi-20240315/libfwsi/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1963 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_delegate_folder_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0005_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16465 2024-03-17 16:50:38.000000 libfwsi-20240315/libfwsi/libfwsi_shell_folder_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6198 2024-03-17 17:06:45.000000 libfwsi-20240315/libfwsi/libfwsi_users_property_view.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_control_panel_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4141 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27275 2024-03-16 08:54:31.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0001_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-01 11:57:20.000000 libfwsi-20240315/libfwsi/libfwsi_libcdata.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:47.000000 libfwsi-20240315/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29721 2024-03-17 17:27:09.000000 libfwsi-20240315/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-17 17:26:45.000000 libfwsi-20240315/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-03-01 11:57:16.000000 libfwsi-20240315/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2024-03-01 11:57:16.000000 libfwsi-20240315/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-03-17 17:27:09.000000 libfwsi-20240315/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-03-01 11:57:16.000000 libfwsi-20240315/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      752 2024-03-01 11:57:16.000000 libfwsi-20240315/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:09:40.000000 libfwsi-20240315/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:47.000000 libfwsi-20240315/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30127 2024-03-17 17:27:09.000000 libfwsi-20240315/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-03-17 17:26:50.000000 libfwsi-20240315/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-03-17 17:27:09.000000 libfwsi-20240315/test-driver
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3395 2024-02-25 13:29:58.000000 libfwsi-20240315/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:48.000000 libfwsi-20240315/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      126 2023-12-03 09:09:43.000000 libfwsi-20240315/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22474 2024-03-17 17:27:09.000000 libfwsi-20240315/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11783 2024-03-17 17:07:56.000000 libfwsi-20240315/manuals/libfwsi.3
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:48.000000 libfwsi-20240315/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11887 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_control_panel_cpl_file_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10440 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0006_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10428 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0003_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6792 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_compressed_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17078 2024-03-10 10:55:18.000000 libfwsi-20240315/tests/fwsi_test_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7077 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_control_panel_category_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10355 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef000a_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-01 11:58:38.000000 libfwsi-20240315/tests/pyfwsi_test_item_list.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2024-03-01 11:57:21.000000 libfwsi-20240315/tests/fwsi_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-01 11:57:21.000000 libfwsi-20240315/tests/fwsi_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10355 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0000_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0001_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13523 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_mtp_file_entry_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9733 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_delegate_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11835 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10452 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0025_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12033 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0014_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9691 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_cdburn_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10058 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_users_property_view_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9508 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_file_entry_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9072 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_root_folder_values.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-03-01 11:57:21.000000 libfwsi-20240315/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4075 2024-03-01 11:57:21.000000 libfwsi-20240315/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2024-03-01 11:58:38.000000 libfwsi-20240315/tests/pyfwsi_test_extension_block.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9818 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_control_panel_item_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8871 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_volume_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16618 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_mtp_volume_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1414 2024-03-01 11:58:38.000000 libfwsi-20240315/tests/pyfwsi_test_root_folder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-03-01 11:57:21.000000 libfwsi-20240315/tests/fwsi_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0019_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-03-01 11:57:21.000000 libfwsi-20240315/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-03-01 11:57:21.000000 libfwsi-20240315/tests/fwsi_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-03-01 11:57:21.000000 libfwsi-20240315/tests/fwsi_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-01 11:58:38.000000 libfwsi-20240315/tests/pyfwsi_test_volume.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0005_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6222 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_uri_sub_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10525 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0013_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-03-01 11:58:38.000000 libfwsi-20240315/tests/pyfwsi_test_network_location.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-03-01 11:57:21.000000 libfwsi-20240315/tests/fwsi_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1190 2024-03-01 11:58:38.000000 libfwsi-20240315/tests/pyfwsi_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10376 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_file_entry_extension_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-03-01 11:57:21.000000 libfwsi-20240315/tests/fwsi_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10824 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_uri_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1411 2024-03-01 11:58:38.000000 libfwsi-20240315/tests/pyfwsi_test_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9145 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_game_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82461 2024-03-17 17:27:09.000000 libfwsi-20240315/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11361 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_extension_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9721 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_network_location_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15227 2024-03-01 11:57:54.000000 libfwsi-20240315/tests/fwsi_test_item_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-03-01 11:57:21.000000 libfwsi-20240315/tests/fwsi_test_libfwsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-03-01 11:57:21.000000 libfwsi-20240315/tests/fwsi_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1394 2024-03-01 11:58:38.000000 libfwsi-20240315/tests/pyfwsi_test_item.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4792 2024-03-01 11:58:38.000000 libfwsi-20240315/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:48.000000 libfwsi-20240315/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      822 2023-12-03 09:09:42.000000 libfwsi-20240315/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-03-01 11:57:20.000000 libfwsi-20240315/ossfuzz/ossfuzz_libfwsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2024-03-01 11:57:20.000000 libfwsi-20240315/ossfuzz/item_list_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1330 2024-03-01 11:57:20.000000 libfwsi-20240315/ossfuzz/item_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29928 2024-03-17 17:27:09.000000 libfwsi-20240315/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-03-17 17:27:04.000000 libfwsi-20240315/ltmain.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2024-03-01 11:57:16.000000 libfwsi-20240315/libfwsi.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:48.000000 libfwsi-20240315/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:09:44.000000 libfwsi-20240315/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:09:44.000000 libfwsi-20240315/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:09:44.000000 libfwsi-20240315/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:09:44.000000 libfwsi-20240315/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:09:44.000000 libfwsi-20240315/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:09:44.000000 libfwsi-20240315/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:09:44.000000 libfwsi-20240315/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:09:44.000000 libfwsi-20240315/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:09:44.000000 libfwsi-20240315/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-03-17 17:27:25.000000 libfwsi-20240315/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:09:44.000000 libfwsi-20240315/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:09:44.000000 libfwsi-20240315/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:47.000000 libfwsi-20240315/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50839 2024-03-17 17:27:09.000000 libfwsi-20240315/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-03-17 17:26:59.000000 libfwsi-20240315/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37995 2024-03-17 17:27:09.000000 libfwsi-20240315/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:47.000000 libfwsi-20240315/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-17 17:26:49.000000 libfwsi-20240315/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-17 17:26:49.000000 libfwsi-20240315/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-03-17 17:26:49.000000 libfwsi-20240315/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-03-17 17:26:49.000000 libfwsi-20240315/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-03-17 17:26:49.000000 libfwsi-20240315/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-17 17:26:49.000000 libfwsi-20240315/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-03-17 17:26:49.000000 libfwsi-20240315/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-03-17 17:26:49.000000 libfwsi-20240315/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-03-17 17:26:49.000000 libfwsi-20240315/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-03-17 17:26:49.000000 libfwsi-20240315/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-03-17 17:26:49.000000 libfwsi-20240315/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27149 2024-03-17 17:27:09.000000 libfwsi-20240315/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-17 17:26:49.000000 libfwsi-20240315/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-03-17 17:26:49.000000 libfwsi-20240315/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:47.000000 libfwsi-20240315/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-03-17 17:26:46.000000 libfwsi-20240315/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-03-17 17:26:46.000000 libfwsi-20240315/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-17 17:26:46.000000 libfwsi-20240315/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-03-17 17:26:46.000000 libfwsi-20240315/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-03-17 17:26:46.000000 libfwsi-20240315/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-17 17:26:46.000000 libfwsi-20240315/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-03-17 17:26:46.000000 libfwsi-20240315/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-03-17 17:26:46.000000 libfwsi-20240315/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-03-17 17:26:46.000000 libfwsi-20240315/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-03-17 17:26:46.000000 libfwsi-20240315/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-17 17:26:46.000000 libfwsi-20240315/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26662 2024-03-17 17:27:09.000000 libfwsi-20240315/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-17 17:42:47.000000 libfwsi-20240315/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29888 2024-03-17 17:27:09.000000 libfwsi-20240315/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-03-17 17:26:52.000000 libfwsi-20240315/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56679 2024-03-17 17:27:06.000000 libfwsi-20240315/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-03-15 19:17:10.000000 libfwsi-20240315/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1956 2024-03-17 17:27:26.000000 libfwsi-20240315/libfwsi.spec
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      415 2024-03-17 17:42:49.691007 libfwsi-20240315/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:34.000000 libfwsi-20240417/libfole/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      661 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1555 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1407 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3793 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26787 2024-04-17 05:54:47.000000 libfwsi-20240417/libfole/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-17 04:08:48.000000 libfwsi-20240417/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-17 05:54:47.000000 libfwsi-20240417/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:48.000000 libfwsi-20240417/NEWS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2593 2024-04-17 04:08:48.000000 libfwsi-20240417/libfwsi.spec.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-17 05:54:47.000000 libfwsi-20240417/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:34.000000 libfwsi-20240417/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26867 2024-04-17 05:54:47.000000 libfwsi-20240417/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:32.000000 libfwsi-20240417/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4187 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libfole.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-17 05:54:43.000000 libfwsi-20240417/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-17 05:54:42.000000 libfwsi-20240417/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10266 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libfwps.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-17 05:54:42.000000 libfwsi-20240417/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-17 05:54:43.000000 libfwsi-20240417/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-17 05:54:42.000000 libfwsi-20240417/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6400 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:32.000000 libfwsi-20240417/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25612 2024-04-17 04:08:52.000000 libfwsi-20240417/include/libfwsi.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25612 2024-04-17 05:55:04.000000 libfwsi-20240417/include/libfwsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      410 2024-04-17 04:12:48.000000 libfwsi-20240417/include/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:32.000000 libfwsi-20240417/include/libfwsi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-04-17 04:08:52.000000 libfwsi-20240417/include/libfwsi/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3262 2024-04-17 05:55:04.000000 libfwsi-20240417/include/libfwsi/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5015 2024-04-17 04:08:52.000000 libfwsi-20240417/include/libfwsi/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4884 2024-04-17 05:55:04.000000 libfwsi-20240417/include/libfwsi/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-17 04:09:35.000000 libfwsi-20240417/include/libfwsi/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-04-17 04:08:52.000000 libfwsi-20240417/include/libfwsi/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-17 04:08:52.000000 libfwsi-20240417/include/libfwsi/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-17 05:55:04.000000 libfwsi-20240417/include/libfwsi/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2024-04-17 04:08:52.000000 libfwsi-20240417/include/libfwsi/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25224 2024-04-17 05:54:47.000000 libfwsi-20240417/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:34.000000 libfwsi-20240417/libfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2490 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_set.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_store.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1202 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3827 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3731 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_format_class_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9704 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_store.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3967 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2244 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_property_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_format_class_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7534 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_property_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7144 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    83917 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16442 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_set.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29731 2024-04-17 05:54:47.000000 libfwsi-20240417/libfwps/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_unused.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:32.000000 libfwsi-20240417/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-17 04:08:51.000000 libfwsi-20240417/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-17 04:08:51.000000 libfwsi-20240417/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-17 04:08:51.000000 libfwsi-20240417/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-17 04:08:51.000000 libfwsi-20240417/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-17 04:08:51.000000 libfwsi-20240417/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-17 04:08:51.000000 libfwsi-20240417/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-17 04:08:51.000000 libfwsi-20240417/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-17 04:12:48.000000 libfwsi-20240417/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-17 04:08:51.000000 libfwsi-20240417/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-04-17 05:55:04.000000 libfwsi-20240417/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12626 2024-04-17 05:54:46.000000 libfwsi-20240417/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13364 2024-04-17 05:55:05.000000 libfwsi-20240417/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-17 04:08:51.000000 libfwsi-20240417/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-17 04:08:51.000000 libfwsi-20240417/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-17 04:08:51.000000 libfwsi-20240417/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22277 2024-04-17 05:54:47.000000 libfwsi-20240417/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:33.000000 libfwsi-20240417/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27475 2024-04-17 05:54:47.000000 libfwsi-20240417/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:35.000000 libfwsi-20240417/pyfwsi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3254 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2413 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_extension_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4381 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_control_panel_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4432 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_root_folder.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2888 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8868 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7439 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_users_property_view.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9661 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_extension_blocks.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_control_panel_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10914 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_network_location.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1815 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1681 2024-04-17 04:13:02.000000 libfwsi-20240417/pyfwsi/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9447 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1423 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_compressed_folder.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8645 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2317 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_items.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1862 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_control_panel_category.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8979 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_items.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2852 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_guid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16477 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_file_entry_extension.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11207 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_extension_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1667 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_network_location.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_root_folder.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_file_entry_extension.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5329 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_compressed_folder.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4275 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_control_panel_category.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_libfwsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15996 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_item_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1592 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_users_property_view.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22036 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_guid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    62371 2024-04-17 05:54:47.000000 libfwsi-20240417/pyfwsi/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11390 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_item_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2548 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_extension_blocks.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16593 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-04-17 04:13:42.000000 libfwsi-20240417/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:09:40.000000 libfwsi-20240417/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-17 05:54:47.000000 libfwsi-20240417/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:32.000000 libfwsi-20240417/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-04-17 04:08:56.000000 libfwsi-20240417/dpkg/copyright
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/libfwsi-dev.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:32.000000 libfwsi-20240417/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1541 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      703 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-04-17 05:55:04.000000 libfwsi-20240417/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/libfwsi-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/libfwsi.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-04-17 05:55:04.000000 libfwsi-20240417/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-17 04:08:48.000000 libfwsi-20240417/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1560700 2024-04-17 05:54:46.000000 libfwsi-20240417/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-17 05:54:47.000000 libfwsi-20240417/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-17 05:54:47.000000 libfwsi-20240417/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_file_entry_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_file_entry_values/fwsi_test_file_entry_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_uri_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5376 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_uri_values/fwsi_test_uri_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libfole/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4605 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libfole/libfole.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_game_folder_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_game_folder_values/fwsi_test_game_folder_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_volume_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5385 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_volume_values/fwsi_test_volume_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_compressed_folder_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5418 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_compressed_folder_values/fwsi_test_compressed_folder_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0014_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0014_values/fwsi_test_extension_block_0xbeef0014_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block/fwsi_test_extension_block.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5118 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_error/fwsi_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6465 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libfwps/libfwps.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34936 2024-04-17 04:09:25.000000 libfwsi-20240417/msvscpp/libfwsi.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0019_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0019_values/fwsi_test_extension_block_0xbeef0019_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/pyfwsi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8591 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/pyfwsi/pyfwsi.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2957 2024-04-17 04:13:50.000000 libfwsi-20240417/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_mtp_volume_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_mtp_volume_values/fwsi_test_mtp_volume_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_root_folder_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_root_folder_values/fwsi_test_root_folder_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_cdburn_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5385 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_cdburn_values/fwsi_test_cdburn_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0001_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0001_values/fwsi_test_extension_block_0xbeef0001_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0025_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0025_values/fwsi_test_extension_block_0xbeef0025_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_uri_sub_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5388 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_uri_sub_values/fwsi_test_uri_sub_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_delegate_folder_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5412 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_delegate_folder_values/fwsi_test_delegate_folder_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_control_panel_category_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5433 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_control_panel_category_values/fwsi_test_control_panel_category_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_control_panel_item_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5421 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_control_panel_item_values/fwsi_test_control_panel_item_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libfwsi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15769 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libfwsi/libfwsi.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_network_location_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5415 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_network_location_values/fwsi_test_network_location_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_control_panel_cpl_file_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5433 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_control_panel_cpl_file_values/fwsi_test_control_panel_cpl_file_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0000_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0000_values/fwsi_test_extension_block_0xbeef0000_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_users_property_view_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5424 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_users_property_view_values/fwsi_test_users_property_view_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0006_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0006_values/fwsi_test_extension_block_0xbeef0006_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5124 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_support/fwsi_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_file_entry_extension_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5427 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_file_entry_extension_values/fwsi_test_file_entry_extension_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_item/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5358 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_item/fwsi_test_item.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_mtp_file_entry_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5409 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_mtp_file_entry_values/fwsi_test_mtp_file_entry_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0013_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0013_values/fwsi_test_extension_block_0xbeef0013_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22224 2024-04-17 05:54:47.000000 libfwsi-20240417/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef000a_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef000a_values/fwsi_test_extension_block_0xbeef000a_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_item_list/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5373 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_item_list/fwsi_test_item_list.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0005_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0005_values/fwsi_test_extension_block_0xbeef0005_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0003_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0003_values/fwsi_test_extension_block_0xbeef0003_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5204 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_notify/fwsi_test_notify.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-17 04:08:51.000000 libfwsi-20240417/AUTHORS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      301 2024-04-17 04:08:48.000000 libfwsi-20240417/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-17 05:54:47.000000 libfwsi-20240417/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:35.000000 libfwsi-20240417/libfwsi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1888 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_cpl_file_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10702 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_compressed_folder.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2824 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_category.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1076 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36252 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_known_folder_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8008 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_delegate_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1609 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_uri_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0001_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21171 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0000_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_libfole.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_users_property_view.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5770 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_game_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12685 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_item_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0003_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6750 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_uri_sub_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1074 2024-04-17 05:55:04.000000 libfwsi-20240417/libfwsi/libfwsi.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6785 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0000_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3733 2024-04-17 05:55:04.000000 libfwsi-20240417/libfwsi/libfwsi_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1377 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0013_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11586 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_known_folder_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1920 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_compressed_folder.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6330 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0027_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5972 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0003_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7080 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0026_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0025_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_game_folder_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2941 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0014_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1903 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_category_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0029_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16884 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_mtp_file_entry_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1190 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0006_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9231 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0014_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1762 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_root_folder_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2305 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry_extension_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13595 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_users_property_view_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4734 2024-04-17 04:14:05.000000 libfwsi-20240417/libfwsi/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5986 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0013_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6191 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0006_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17787 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_mtp_volume_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11512 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12898 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_acronis_tib_file_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_category.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_root_folder.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52733 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_shell_folder_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5555 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0029_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_cdburn_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1673 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_uri_sub_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2646 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2421 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_item_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8940 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_cpl_file_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef000a_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2001 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0027_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5435 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0005_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_mtp_volume_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2383 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_users_property_view_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2317 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6230 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0019_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0026_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2133 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_network_location_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_web_site_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16822 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry_extension_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1805 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_acronis_tib_file_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3735 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26408 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry_extension.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10306 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_web_site_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9361 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6603 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0025_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15636 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_compressed_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0019_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2059 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_item_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7535 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_item_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2666 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_compressed_folder_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5798 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_cdburn_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5814 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_category_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2465 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13461 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_network_location_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15825 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48490 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3228 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_volume_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3347 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2794 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14142 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_uri_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1514 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_libfwps.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5656 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef000a_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3419 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry_extension.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5798 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_root_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24188 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_network_location.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3432 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_network_location.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16168 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_volume_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1816 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_mtp_file_entry_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3149 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_root_folder.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48575 2024-04-17 05:54:47.000000 libfwsi-20240417/libfwsi/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1963 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_delegate_folder_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0005_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16451 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_shell_folder_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6198 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_users_property_view.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4141 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27275 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7576 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_item_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0001_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21723 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_item_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_libcdata.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:33.000000 libfwsi-20240417/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30221 2024-04-17 05:54:47.000000 libfwsi-20240417/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-17 04:08:48.000000 libfwsi-20240417/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2024-04-17 04:08:48.000000 libfwsi-20240417/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-17 05:54:47.000000 libfwsi-20240417/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-17 04:08:48.000000 libfwsi-20240417/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      752 2024-04-17 04:09:25.000000 libfwsi-20240417/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:09:40.000000 libfwsi-20240417/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:33.000000 libfwsi-20240417/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30660 2024-04-17 05:54:47.000000 libfwsi-20240417/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-17 05:54:47.000000 libfwsi-20240417/test-driver
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3395 2024-02-25 13:29:58.000000 libfwsi-20240417/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       97 2024-04-17 04:14:14.000000 libfwsi-20240417/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22474 2024-04-17 05:54:47.000000 libfwsi-20240417/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11778 2024-04-17 04:08:55.000000 libfwsi-20240417/manuals/libfwsi.3
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11887 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_control_panel_cpl_file_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10440 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0006_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10428 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0003_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6792 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_compressed_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17078 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7077 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_control_panel_category_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10355 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef000a_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_item_list.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10355 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0000_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0001_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13523 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_mtp_file_entry_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9733 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_delegate_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11852 2024-04-17 05:45:45.000000 libfwsi-20240417/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10452 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0025_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12033 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0014_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9691 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_cdburn_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10058 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_users_property_view_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9508 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_file_entry_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9072 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_root_folder_values.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4386 2024-04-17 04:11:21.000000 libfwsi-20240417/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_extension_block.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9818 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_control_panel_item_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8871 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_volume_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16618 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_mtp_volume_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1414 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_root_folder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0019_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_volume.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0005_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6222 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_uri_sub_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10525 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0013_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_network_location.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1190 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10376 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_file_entry_extension_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10824 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_uri_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1411 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9145 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_game_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84392 2024-04-17 05:54:47.000000 libfwsi-20240417/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11361 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9721 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_network_location_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15227 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_item_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_libfwsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1394 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_item.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4761 2024-04-17 04:09:50.000000 libfwsi-20240417/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      818 2024-04-17 04:14:22.000000 libfwsi-20240417/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-04-17 04:08:54.000000 libfwsi-20240417/ossfuzz/ossfuzz_libfwsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2024-04-17 04:08:54.000000 libfwsi-20240417/ossfuzz/item_list_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1330 2024-04-17 04:08:54.000000 libfwsi-20240417/ossfuzz/item_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30029 2024-04-17 05:54:47.000000 libfwsi-20240417/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-17 05:54:42.000000 libfwsi-20240417/ltmain.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2024-04-17 04:08:48.000000 libfwsi-20240417/libfwsi.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:09:44.000000 libfwsi-20240417/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:09:44.000000 libfwsi-20240417/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:09:44.000000 libfwsi-20240417/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:09:44.000000 libfwsi-20240417/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:09:44.000000 libfwsi-20240417/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:09:44.000000 libfwsi-20240417/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:09:44.000000 libfwsi-20240417/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:09:44.000000 libfwsi-20240417/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:09:44.000000 libfwsi-20240417/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-04-17 05:55:04.000000 libfwsi-20240417/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:09:44.000000 libfwsi-20240417/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:09:44.000000 libfwsi-20240417/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:34.000000 libfwsi-20240417/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53987 2024-04-17 05:54:47.000000 libfwsi-20240417/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37877 2024-04-17 05:54:47.000000 libfwsi-20240417/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:33.000000 libfwsi-20240417/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-17 05:54:29.000000 libfwsi-20240417/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-17 05:54:29.000000 libfwsi-20240417/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27344 2024-04-17 05:54:47.000000 libfwsi-20240417/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:32.000000 libfwsi-20240417/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26811 2024-04-17 05:54:47.000000 libfwsi-20240417/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:34.000000 libfwsi-20240417/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30395 2024-04-17 05:54:47.000000 libfwsi-20240417/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56679 2024-04-17 05:54:45.000000 libfwsi-20240417/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-04-17 04:08:48.000000 libfwsi-20240417/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1956 2024-04-17 05:55:04.000000 libfwsi-20240417/libfwsi.spec
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      415 2024-04-17 16:04:37.411794 libfwsi-20240417/PKG-INFO
```

### Comparing `libfwsi-20240315/libfole/libfole_value_type.h` & `libfwsi-20240417/libfole/libfole_value_type.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfole/libfole_error.c` & `libfwsi-20240417/libfole/libfole_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfole/Makefile.am` & `libfwsi-20240417/libfole/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFOLE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfole.la
 
 libfole_la_SOURCES = \
 	libfole_definitions.h \
 	libfole_extern.h \
@@ -13,19 +13,17 @@
 	libfole_libcerror.h \
 	libfole_support.c libfole_support.h \
 	libfole_types.h \
 	libfole_unused.h \
 	libfole_value_type.c libfole_value_type.h
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
 	@echo "Running splint on libfole ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfole_la_SOURCES)
```

### Comparing `libfwsi-20240315/libfole/libfole_definitions.h` & `libfwsi-20240417/libfole/libfole_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfole/definitions.h> are copied here
  * for local use of libfole
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFOLE_VERSION					20240119
+#define LIBFOLE_VERSION					20240416
 
 /* The version string
  */
-#define LIBFOLE_VERSION_STRING				"20240119"
+#define LIBFOLE_VERSION_STRING				"20240416"
 
 /* The byte order definitions
  */
 #define LIBFOLE_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFOLE_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 #endif /* !defined( HAVE_LOCAL_LIBFOLE ) */
```

### Comparing `libfwsi-20240315/libfole/libfole_error.h` & `libfwsi-20240417/libfole/libfole_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfole/libfole_support.h` & `libfwsi-20240417/libfole/libfole_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfole/libfole_types.h` & `libfwsi-20240417/libfole/libfole_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfole/libfole_support.c` & `libfwsi-20240417/libfole/libfole_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfole/libfole_value_type.c` & `libfwsi-20240417/libfole/libfole_value_type.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfole/libfole_unused.h` & `libfwsi-20240417/libfole/libfole_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfole/libfole_libcerror.h` & `libfwsi-20240417/libfole/libfole_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfole/Makefile.in` & `libfwsi-20240417/libfole/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -461,30 +461,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFOLE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFOLE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFOLE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFOLE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFOLE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFOLE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFOLE_TRUE@noinst_LTLIBRARIES = libfole.la
 @HAVE_LOCAL_LIBFOLE_TRUE@libfole_la_SOURCES = \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_definitions.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_extern.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_error.c libfole_error.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_libcerror.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_support.c libfole_support.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_types.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_unused.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_value_type.c libfole_value_type.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -686,24 +687,29 @@
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
+		-rm -f ./$(DEPDIR)/libfole_error.Plo
+	-rm -f ./$(DEPDIR)/libfole_support.Plo
+	-rm -f ./$(DEPDIR)/libfole_value_type.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -789,17 +795,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfole ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfole_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwsi-20240315/libfole/libfole_extern.h` & `libfwsi-20240417/libfole/libfole_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/COPYING` & `libfwsi-20240417/COPYING`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/install-sh` & `libfwsi-20240417/install-sh`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi.spec.in` & `libfwsi-20240417/libfwsi.spec.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/depcomp` & `libfwsi-20240417/depcomp`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfguid/libfguid_error.c` & `libfwsi-20240417/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfguid/libfguid_support.h` & `libfwsi-20240417/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfguid/libfguid_identifier.h` & `libfwsi-20240417/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfguid/libfguid_libcerror.h` & `libfwsi-20240417/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfguid/Makefile.am` & `libfwsi-20240417/libfguid/Makefile.am`

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

### Comparing `libfwsi-20240315/libfguid/libfguid_unused.h` & `libfwsi-20240417/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfguid/libfguid_extern.h` & `libfwsi-20240417/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfguid/libfguid_types.h` & `libfwsi-20240417/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfguid/libfguid_identifier.c` & `libfwsi-20240417/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfguid/libfguid_support.c` & `libfwsi-20240417/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfguid/libfguid_definitions.h` & `libfwsi-20240417/libfguid/libfguid_definitions.h`

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

### Comparing `libfwsi-20240315/libfguid/Makefile.in` & `libfwsi-20240417/libfguid/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -462,30 +462,31 @@
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
@@ -687,24 +688,29 @@
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
 
@@ -790,17 +796,14 @@
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

### Comparing `libfwsi-20240315/libfguid/libfguid_error.h` & `libfwsi-20240417/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/libfdatetime.m4` & `libfwsi-20240417/m4/libfdatetime.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfdatetime required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfdatetime is available
 dnl ac_libfdatetime_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno],
     [ac_cv_libfdatetime=no],
     [ac_cv_libfdatetime=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdatetime which returns "yes" and --with-libfdatetime= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect],
+      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdatetime"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdatetime],
           [1])
@@ -455,16 +457,17 @@
           fdatetime,
           libfdatetime_systemetime_copy_to_utf32_string_with_index,
           [ac_cv_libfdatetime_dummy=yes],
           [ac_cv_libfdatetime=no])
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes],
+      [test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime],
         [1])
       ])
     ])
 
   AS_IF(
@@ -486,15 +489,15 @@
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

### Comparing `libfwsi-20240315/m4/tests.m4` & `libfwsi-20240417/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/lib-prefix.m4` & `libfwsi-20240417/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/progtest.m4` & `libfwsi-20240417/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/libuna.m4` & `libfwsi-20240417/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
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

### Comparing `libfwsi-20240315/m4/gettext.m4` & `libfwsi-20240417/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/lib-ld.m4` & `libfwsi-20240417/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/libfole.m4` & `libfwsi-20240417/m4/libfole.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfole required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfole is available
 dnl ac_libfole_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFOLE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfole" = xno],
     [ac_cv_libfole=no],
     [ac_cv_libfole=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfole which returns "yes" and --with-libfole= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect],
+      [test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_with_libfole" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfole"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfole}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfole}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfole],
           [1])
@@ -53,16 +55,17 @@
           [ac_cv_libfole_dummy=yes],
           [ac_cv_libfole=no])
 
         dnl TODO add functions
 
         ac_cv_libfole_LIBADD="-lfole"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_libfole" != xyes],
+      [test "x$ac_cv_libfole" != xyes && test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_with_libfole" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfole in directory: $ac_cv_with_libfole],
         [1])
       ])
     ])
 
   AS_IF(
@@ -84,15 +87,15 @@
     ])
   ])
 
 dnl Function to detect if libfole dependencies are available
 AC_DEFUN([AX_LIBFOLE_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfole_CPPFLAGS="-I../libfole";
+  ac_cv_libfole_CPPFLAGS="-I../libfole -I\$(top_srcdir)/libfole";
   ac_cv_libfole_LIBADD="../libfole/libfole.la";
 
   ac_cv_libfole=local
   ])
 
 dnl Function to detect how to enable libfole
 AC_DEFUN([AX_LIBFOLE_CHECK_ENABLE],
```

### Comparing `libfwsi-20240315/m4/libclocale.m4` & `libfwsi-20240417/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
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

### Comparing `libfwsi-20240315/m4/libcdata.m4` & `libfwsi-20240417/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
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

### Comparing `libfwsi-20240315/m4/common.m4` & `libfwsi-20240417/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libfwsi-20240315/m4/libcthreads.m4` & `libfwsi-20240417/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
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

### Comparing `libfwsi-20240315/m4/ltversion.m4` & `libfwsi-20240417/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/ltsugar.m4` & `libfwsi-20240417/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/host-cpu-c-abi.m4` & `libfwsi-20240417/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/libfwps.m4` & `libfwsi-20240417/m4/libfwps.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfwps required headers and functions
 dnl
-dnl Version: 20240224
+dnl Version: 20240413
 
 dnl Function to detect if libfwps is available
 dnl ac_libfwps_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFWPS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwps" = xno],
     [ac_cv_libfwps=no],
     [ac_cv_libfwps=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfwps which returns "yes" and --with-libfwps= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect],
+      [test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect && test "x$ac_cv_with_libfwps" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfwps"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfwps}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwps}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfwps],
           [1])
@@ -246,15 +248,15 @@
           libfwps_record_get_data_as_guid,
           [ac_cv_libfwps_dummy=yes],
           [ac_cv_libfwps=no])
 
         ac_cv_libfwps_LIBADD="-lfwps"])
       ])
     AS_IF(
-      [test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect && test "x$ac_cv_libfwps" != xyes],
+      [test "x$ac_cv_libfwps" != xyes && test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect && test "x$ac_cv_with_libfwps" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfwps in directory: $ac_cv_with_libfwps],
         [1])
       ])
     ])
 
   dnl Check for debug functions
@@ -292,15 +294,15 @@
     ])
   ])
 
 dnl Function to detect if libfwps dependencies are available
 AC_DEFUN([AX_LIBFWPS_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfwps_CPPFLAGS="-I../libfwps";
+  ac_cv_libfwps_CPPFLAGS="-I../libfwps -I\$(top_srcdir)/libfwps";
   ac_cv_libfwps_LIBADD="../libfwps/libfwps.la";
 
   ac_cv_libfwps=local
   ])
 
 dnl Function to detect how to enable libfwps
 AC_DEFUN([AX_LIBFWPS_CHECK_ENABLE],
```

### Comparing `libfwsi-20240315/m4/libtool.m4` & `libfwsi-20240417/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/po.m4` & `libfwsi-20240417/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/libcerror.m4` & `libfwsi-20240417/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
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

### Comparing `libfwsi-20240315/m4/libcnotify.m4` & `libfwsi-20240417/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
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

### Comparing `libfwsi-20240315/m4/libfguid.m4` & `libfwsi-20240417/m4/libfguid.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfguid required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfguid is available
 dnl ac_libfguid_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFGUID_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno],
     [ac_cv_libfguid=no],
     [ac_cv_libfguid=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfguid which returns "yes" and --with-libfguid= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect],
+      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfguid"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfguid],
           [1])
@@ -103,16 +105,17 @@
           fguid,
           libfguid_identifier_copy_to_utf32_string_with_index,
           [ac_cv_libfguid_dummy=yes],
           [ac_cv_libfguid=no])
 
         ac_cv_libfguid_LIBADD="-lfguid"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes],
+      [test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfguid in directory: $ac_cv_with_libfguid],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
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

### Comparing `libfwsi-20240315/m4/intlmacosx.m4` & `libfwsi-20240417/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/lt~obsolete.m4` & `libfwsi-20240417/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/lib-link.m4` & `libfwsi-20240417/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/iconv.m4` & `libfwsi-20240417/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/ltoptions.m4` & `libfwsi-20240417/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/nls.m4` & `libfwsi-20240417/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/python.m4` & `libfwsi-20240417/m4/python.m4`

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

### Comparing `libfwsi-20240315/m4/types.m4` & `libfwsi-20240417/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/m4/pthread.m4` & `libfwsi-20240417/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libfwsi-20240315/include/libfwsi.h.in` & `libfwsi-20240417/include/libfwsi.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/include/libfwsi.h` & `libfwsi-20240417/include/libfwsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/include/libfwsi/definitions.h.in` & `libfwsi-20240417/include/libfwsi/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/include/libfwsi/definitions.h` & `libfwsi-20240417/include/libfwsi/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBFWSI_DEFINITIONS_H )
 #define _LIBFWSI_DEFINITIONS_H
 
 #include <libfwsi/types.h>
 
-#define LIBFWSI_VERSION					20240315
+#define LIBFWSI_VERSION					20240417
 
 /* The version string
  */
-#define LIBFWSI_VERSION_STRING				"20240315"
+#define LIBFWSI_VERSION_STRING				"20240417"
 
 /* The byte order definitions
  */
 enum LIBFWSI_ENDIAN
 {
 	LIBFWSI_ENDIAN_BIG				= (int) 'b',
 	LIBFWSI_ENDIAN_LITTLE				= (int) 'l'
```

### Comparing `libfwsi-20240315/include/libfwsi/types.h.in` & `libfwsi-20240417/include/libfwsi/types.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/include/libfwsi/types.h` & `libfwsi-20240417/include/libfwsi/types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/include/libfwsi/features.h.in` & `libfwsi-20240417/include/libfwsi/features.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/include/libfwsi/error.h` & `libfwsi-20240417/include/libfwsi/error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/include/libfwsi/extern.h` & `libfwsi-20240417/include/libfwsi/extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/include/libfwsi/features.h` & `libfwsi-20240417/include/libfwsi/features.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/include/libfwsi/codepage.h` & `libfwsi-20240417/include/libfwsi/codepage.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/include/Makefile.in` & `libfwsi-20240417/include/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -468,15 +468,20 @@
 
 EXTRA_DIST = \
 	libfwsi.h.in \
 	libfwsi/definitions.h.in \
 	libfwsi/features.h.in \
 	libfwsi/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfwsi.h \
+	libfwsi/definitions.h \
+	libfwsi/features.h \
+	libfwsi/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -673,23 +678,25 @@
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
@@ -771,17 +778,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfwsi.h
-	-rm -f libfwsi/definitions.h
-	-rm -f libfwsi/features.h
-	-rm -f libfwsi/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwsi-20240315/libfwps/libfwps_set.h` & `libfwsi-20240417/libfwps/libfwps_set.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_types.h` & `libfwsi-20240417/libfwps/libfwps_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_notify.h` & `libfwsi-20240417/libfwps/libfwps_notify.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_libfguid.h` & `libfwsi-20240417/libfwps/libfwps_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_libcerror.h` & `libfwsi-20240417/libfwps/libfwps_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_libcnotify.h` & `libfwsi-20240417/libfwps/libfwps_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_store.h` & `libfwsi-20240417/libfwps/libfwps_store.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_libcdata.h` & `libfwsi-20240417/libfwps/libfwps_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_debug.h` & `libfwsi-20240417/libfwps/libfwps_debug.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_error.c` & `libfwsi-20240417/libfwps/libfwps_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/Makefile.am` & `libfwsi-20240417/libfwps/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFWPS
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
@@ -31,19 +31,17 @@
 	libfwps_set.c libfwps_set.h \
 	libfwps_store.c libfwps_store.h \
 	libfwps_support.c libfwps_support.h \
 	libfwps_types.h \
 	libfwps_unused.h
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
 	@echo "Running splint on libfwps ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwps_la_SOURCES)
```

### Comparing `libfwsi-20240315/libfwps/libfwps_definitions.h` & `libfwsi-20240417/libfwps/libfwps_definitions.h`

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

### Comparing `libfwsi-20240315/libfwps/libfwps_notify.c` & `libfwsi-20240417/libfwps/libfwps_notify.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_error.h` & `libfwsi-20240417/libfwps/libfwps_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_libuna.h` & `libfwsi-20240417/libfwps/libfwps_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_support.h` & `libfwsi-20240417/libfwps/libfwps_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_format_class_identifier.c` & `libfwsi-20240417/libfwps/libfwps_format_class_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_codepage.h` & `libfwsi-20240417/libfwps/libfwps_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_support.c` & `libfwsi-20240417/libfwps/libfwps_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_extern.h` & `libfwsi-20240417/libfwps/libfwps_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_store.c` & `libfwsi-20240417/libfwps/libfwps_store.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_debug.c` & `libfwsi-20240417/libfwps/libfwps_debug.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_property_identifier.h` & `libfwsi-20240417/libfwps/libfwps_property_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_format_class_identifier.h` & `libfwsi-20240417/libfwps/libfwps_format_class_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_property_identifier.c` & `libfwsi-20240417/libfwps/libfwps_property_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/libfwps_record.h` & `libfwsi-20240417/libfwps/libfwps_record.h`

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

### Comparing `libfwsi-20240315/libfwps/libfwps_record.c` & `libfwsi-20240417/libfwps/libfwps_record.c`

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

### Comparing `libfwsi-20240315/libfwps/libfwps_set.c` & `libfwsi-20240417/libfwps/libfwps_set.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwps/Makefile.in` & `libfwsi-20240417/libfwps/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -476,16 +476,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFWPS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFWPS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFWPS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFWPS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFWPS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFWPS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWPS_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWPS_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWPS_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWPS_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWPS_TRUE@	@LIBFDATETIME_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWPS_TRUE@	@LIBFGUID_CPPFLAGS@ \
@@ -509,15 +509,16 @@
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_record.c libfwps_record.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_set.c libfwps_set.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_store.c libfwps_store.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_support.c libfwps_support.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_types.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -725,24 +726,35 @@
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
+		-rm -f ./$(DEPDIR)/libfwps_debug.Plo
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
 
@@ -834,17 +846,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwps ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwps_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwsi-20240315/libfwps/libfwps_unused.h` & `libfwsi-20240417/libfwps/libfwps_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/common/config_borlandc.h` & `libfwsi-20240417/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/common/file_stream.h` & `libfwsi-20240417/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/common/memory.h` & `libfwsi-20240417/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/common/byte_stream.h` & `libfwsi-20240417/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/common/common.h` & `libfwsi-20240417/common/common.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/common/config_winapi.h` & `libfwsi-20240417/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/common/system_string.h` & `libfwsi-20240417/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/common/types.h.in` & `libfwsi-20240417/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/common/types.h` & `libfwsi-20240417/common/types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/common/config.h.in` & `libfwsi-20240417/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/common/config.h` & `libfwsi-20240417/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -403,24 +403,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfwsi"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfwsi 20240315"
+#define PACKAGE_STRING "libfwsi 20240417"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfwsi"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240315"
+#define PACKAGE_VERSION "20240417"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -438,15 +438,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240315"
+#define VERSION "20240417"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfwsi-20240315/common/wide_string.h` & `libfwsi-20240417/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/common/narrow_string.h` & `libfwsi-20240417/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/common/config_msc.h` & `libfwsi-20240417/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/common/Makefile.in` & `libfwsi-20240417/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -421,15 +421,17 @@
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
@@ -437,15 +439,18 @@
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
@@ -613,23 +618,25 @@
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
@@ -709,15 +716,10 @@
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

### Comparing `libfwsi-20240315/libclocale/libclocale_wide_string.c` & `libfwsi-20240417/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libclocale/libclocale_support.h` & `libfwsi-20240417/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libclocale/Makefile.am` & `libfwsi-20240417/libclocale/Makefile.am`

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

### Comparing `libfwsi-20240315/libclocale/libclocale_definitions.h` & `libfwsi-20240417/libclocale/libclocale_definitions.h`

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

### Comparing `libfwsi-20240315/libclocale/libclocale_unused.h` & `libfwsi-20240417/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libclocale/libclocale_libcerror.h` & `libfwsi-20240417/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libclocale/libclocale_locale.h` & `libfwsi-20240417/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libclocale/libclocale_support.c` & `libfwsi-20240417/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libclocale/libclocale_codepage.c` & `libfwsi-20240417/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libclocale/libclocale_locale.c` & `libfwsi-20240417/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libclocale/Makefile.in` & `libfwsi-20240417/libclocale/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -467,30 +467,31 @@
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
@@ -693,24 +694,30 @@
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
 
@@ -797,17 +804,14 @@
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

### Comparing `libfwsi-20240315/libclocale/libclocale_extern.h` & `libfwsi-20240417/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libclocale/libclocale_wide_string.h` & `libfwsi-20240417/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libclocale/libclocale_codepage.h` & `libfwsi-20240417/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_codepage.c` & `libfwsi-20240417/pyfwsi/pyfwsi_codepage.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_extension_block.h` & `libfwsi-20240417/pyfwsi/pyfwsi_extension_block.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_control_panel_item.c` & `libfwsi-20240417/pyfwsi/pyfwsi_control_panel_item.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_root_folder.c` & `libfwsi-20240417/pyfwsi/pyfwsi_root_folder.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_item.h` & `libfwsi-20240417/pyfwsi/pyfwsi_item.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_string.c` & `libfwsi-20240417/pyfwsi/pyfwsi_string.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_users_property_view.c` & `libfwsi-20240417/pyfwsi/pyfwsi_users_property_view.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_integer.h` & `libfwsi-20240417/pyfwsi/pyfwsi_integer.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_extension_blocks.c` & `libfwsi-20240417/pyfwsi/pyfwsi_extension_blocks.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_control_panel_item.h` & `libfwsi-20240417/pyfwsi/pyfwsi_control_panel_item.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_libclocale.h` & `libfwsi-20240417/pyfwsi/pyfwsi_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_network_location.c` & `libfwsi-20240417/pyfwsi/pyfwsi_network_location.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_codepage.h` & `libfwsi-20240417/pyfwsi/pyfwsi_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_datetime.h` & `libfwsi-20240417/pyfwsi/pyfwsi_datetime.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/Makefile.am` & `libfwsi-20240417/pyfwsi/Makefile.am`

 * *Files 2% similar despite different names*

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
 	@LIBFWSI_DLL_IMPORT@
 
@@ -50,13 +50,11 @@
 	@LIBFGUID_LIBADD@
 
 pyfwsi_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyfwsi_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi.c` & `libfwsi-20240417/pyfwsi/pyfwsi.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_error.h` & `libfwsi-20240417/pyfwsi/pyfwsi_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_compressed_folder.h` & `libfwsi-20240417/pyfwsi/pyfwsi_compressed_folder.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_volume.c` & `libfwsi-20240417/pyfwsi/pyfwsi_volume.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_items.h` & `libfwsi-20240417/pyfwsi/pyfwsi_items.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_file_entry.h` & `libfwsi-20240417/pyfwsi/pyfwsi_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_control_panel_category.h` & `libfwsi-20240417/pyfwsi/pyfwsi_control_panel_category.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_items.c` & `libfwsi-20240417/pyfwsi/pyfwsi_items.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_guid.c` & `libfwsi-20240417/pyfwsi/pyfwsi_guid.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_file_entry_extension.c` & `libfwsi-20240417/pyfwsi/pyfwsi_file_entry_extension.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_extension_block.c` & `libfwsi-20240417/pyfwsi/pyfwsi_extension_block.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_network_location.h` & `libfwsi-20240417/pyfwsi/pyfwsi_network_location.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_error.c` & `libfwsi-20240417/pyfwsi/pyfwsi_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi.h` & `libfwsi-20240417/pyfwsi/pyfwsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_integer.c` & `libfwsi-20240417/pyfwsi/pyfwsi_integer.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_volume.h` & `libfwsi-20240417/pyfwsi/pyfwsi_volume.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_unused.h` & `libfwsi-20240417/pyfwsi/pyfwsi_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_root_folder.h` & `libfwsi-20240417/pyfwsi/pyfwsi_root_folder.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_file_entry_extension.h` & `libfwsi-20240417/pyfwsi/pyfwsi_file_entry_extension.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_libcerror.h` & `libfwsi-20240417/pyfwsi/pyfwsi_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_python.h` & `libfwsi-20240417/pyfwsi/pyfwsi_python.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_compressed_folder.c` & `libfwsi-20240417/pyfwsi/pyfwsi_compressed_folder.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_libfguid.h` & `libfwsi-20240417/pyfwsi/pyfwsi_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_control_panel_category.c` & `libfwsi-20240417/pyfwsi/pyfwsi_control_panel_category.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_libfwsi.h` & `libfwsi-20240417/pyfwsi/pyfwsi_libfwsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_item_list.c` & `libfwsi-20240417/pyfwsi/pyfwsi_item_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_users_property_view.h` & `libfwsi-20240417/pyfwsi/pyfwsi_users_property_view.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_string.h` & `libfwsi-20240417/pyfwsi/pyfwsi_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_item.c` & `libfwsi-20240417/pyfwsi/pyfwsi_item.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_guid.h` & `libfwsi-20240417/pyfwsi/pyfwsi_guid.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/Makefile.in` & `libfwsi-20240417/pyfwsi/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -543,16 +543,16 @@
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
 @HAVE_PYTHON_TRUE@	@LIBFWSI_DLL_IMPORT@
 
@@ -593,15 +593,16 @@
 @HAVE_PYTHON_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBFGUID_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyfwsi_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyfwsi_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -995,24 +996,47 @@
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
+		-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_codepage.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_compressed_folder.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_control_panel_category.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_control_panel_item.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_datetime.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_error.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_extension_block.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_extension_blocks.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_file_entry.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_file_entry_extension.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_guid.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_integer.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_item.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_item_list.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_items.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_network_location.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_string.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_users_property_view.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_volume.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1117,13 +1141,10 @@
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

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_file_entry.c` & `libfwsi-20240417/pyfwsi/pyfwsi_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_libuna.h` & `libfwsi-20240417/pyfwsi/pyfwsi_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_item_list.h` & `libfwsi-20240417/pyfwsi/pyfwsi_item_list.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_extension_blocks.h` & `libfwsi-20240417/pyfwsi/pyfwsi_extension_blocks.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/pyfwsi/pyfwsi_datetime.c` & `libfwsi-20240417/pyfwsi/pyfwsi_datetime.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/Makefile.am` & `libfwsi-20240417/Makefile.am`

 * *Files 8% similar despite different names*

```diff
@@ -53,16 +53,23 @@
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
+	libfwsi.pc \
+	libfwsi.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libfwsi.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -81,19 +88,7 @@
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfole && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwps && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwsi && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfwsi.pc
-	-rm -f libfwsi.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libfwsi-20240315/config.guess` & `libfwsi-20240417/config.guess`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/dpkg/copyright` & `libfwsi-20240417/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/dpkg/control` & `libfwsi-20240417/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/dpkg/rules` & `libfwsi-20240417/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/COPYING.LESSER` & `libfwsi-20240417/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/configure` & `libfwsi-20240417/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfwsi 20240315.
+# Generated by GNU Autoconf 2.71 for libfwsi 20240417.
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
 PACKAGE_NAME='libfwsi'
 PACKAGE_TARNAME='libfwsi'
-PACKAGE_VERSION='20240315'
-PACKAGE_STRING='libfwsi 20240315'
+PACKAGE_VERSION='20240417'
+PACKAGE_STRING='libfwsi 20240417'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfwsi.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1580,15 +1580,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfwsi 20240315 to adapt to many kinds of systems.
+\`configure' configures libfwsi 20240417 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1651,15 +1651,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfwsi 20240315:";;
+     short | recursive ) echo "Configuration of libfwsi 20240417:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1864,15 +1864,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfwsi configure 20240315
+libfwsi configure 20240417
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2585,15 +2585,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfwsi $as_me 20240315, which was
+It was created by libfwsi $as_me 20240417, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4074,15 +4074,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfwsi'
- VERSION='20240315'
+ VERSION='20240417'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23615,15 +23615,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24114,15 +24114,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24264,15 +24265,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24366,15 +24367,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26006,15 +26007,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26068,47 +26069,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26142,15 +26148,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26184,15 +26190,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26227,15 +26233,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26269,15 +26275,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26311,15 +26317,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26353,15 +26359,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26395,15 +26401,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26438,15 +26444,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26480,15 +26486,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26522,15 +26528,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26564,15 +26570,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26606,15 +26612,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26649,15 +26655,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26691,15 +26697,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26733,15 +26739,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26775,15 +26781,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26817,15 +26823,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26860,67 +26866,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
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
 
@@ -27008,15 +27023,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -30787,15 +30802,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -30820,15 +30836,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -30898,15 +30914,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31453,15 +31469,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31617,15 +31634,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31695,15 +31712,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32153,15 +32170,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32216,15 +32234,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32294,15 +32312,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -39504,15 +39522,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -39537,15 +39556,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -39615,15 +39634,15 @@
 printf "%s\n" "$ac_cv_with_libfdatetime" >&6; }
 
   if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno
 then :
   ac_cv_libfdatetime=no
 else $as_nop
   ac_cv_libfdatetime=check
-        if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect
+                if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   if test -d "$ac_cv_with_libfdatetime"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -43059,15 +43078,16 @@
 fi
 
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes
+
+    if test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43092,15 +43112,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -43170,15 +43190,15 @@
 printf "%s\n" "$ac_cv_with_libfguid" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno
 then :
   ac_cv_libfguid=no
 else $as_nop
   ac_cv_libfguid=check
-        if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect
+                if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   if test -d "$ac_cv_with_libfguid"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -43752,15 +43772,16 @@
 fi
 
 
         ac_cv_libfguid_LIBADD="-lfguid"
 fi
 
 fi
-    if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes
+
+    if test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfguid in directory: $ac_cv_with_libfguid
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43785,15 +43806,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -43863,15 +43884,15 @@
 printf "%s\n" "$ac_cv_with_libfole" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfole" = xno
 then :
   ac_cv_libfole=no
 else $as_nop
   ac_cv_libfole=check
-        if test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect
+                if test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_with_libfole" != xyes
 then :
   if test -d "$ac_cv_with_libfole"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfole}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfole}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -44025,15 +44046,16 @@
 
 
 
         ac_cv_libfole_LIBADD="-lfole"
 fi
 
 fi
-    if test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_libfole" != xyes
+
+    if test "x$ac_cv_libfole" != xyes && test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_with_libfole" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfole in directory: $ac_cv_with_libfole
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -44058,15 +44080,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfole" != xyes
 then :
 
-  ac_cv_libfole_CPPFLAGS="-I../libfole";
+  ac_cv_libfole_CPPFLAGS="-I../libfole -I\$(top_srcdir)/libfole";
   ac_cv_libfole_LIBADD="../libfole/libfole.la";
 
   ac_cv_libfole=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFOLE 1" >>confdefs.h
@@ -44136,15 +44158,15 @@
 printf "%s\n" "$ac_cv_with_libfwps" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwps" = xno
 then :
   ac_cv_libfwps=no
 else $as_nop
   ac_cv_libfwps=check
-        if test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect
+                if test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect && test "x$ac_cv_with_libfwps" != xyes
 then :
   if test -d "$ac_cv_with_libfwps"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfwps}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwps}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45857,15 +45879,15 @@
 fi
 
 
         ac_cv_libfwps_LIBADD="-lfwps"
 fi
 
 fi
-    if test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect && test "x$ac_cv_libfwps" != xyes
+    if test "x$ac_cv_libfwps" != xyes && test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect && test "x$ac_cv_with_libfwps" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfwps in directory: $ac_cv_with_libfwps
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45980,15 +46002,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfwps" != xyes
 then :
 
-  ac_cv_libfwps_CPPFLAGS="-I../libfwps";
+  ac_cv_libfwps_CPPFLAGS="-I../libfwps -I\$(top_srcdir)/libfwps";
   ac_cv_libfwps_LIBADD="../libfwps/libfwps.la";
 
   ac_cv_libfwps=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFWPS 1" >>confdefs.h
@@ -46295,14 +46317,16 @@
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
@@ -47236,15 +47260,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfwsi $as_me 20240315, which was
+This file was extended by libfwsi $as_me 20240417, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -47304,15 +47328,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfwsi config.status 20240315
+libfwsi config.status 20240417
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfwsi-20240315/compile` & `libfwsi-20240417/compile`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/missing` & `libfwsi-20240417/missing`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_file_entry_values/fwsi_test_file_entry_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_file_entry_values/fwsi_test_file_entry_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_uri_values/fwsi_test_uri_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_uri_values/fwsi_test_uri_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/libfole/libfole.vcproj` & `libfwsi-20240417/msvscpp/libfole/libfole.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_game_folder_values/fwsi_test_game_folder_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_game_folder_values/fwsi_test_game_folder_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_volume_values/fwsi_test_volume_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_volume_values/fwsi_test_volume_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_compressed_folder_values/fwsi_test_compressed_folder_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_compressed_folder_values/fwsi_test_compressed_folder_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0014_values/fwsi_test_extension_block_0xbeef0014_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0014_values/fwsi_test_extension_block_0xbeef0014_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/libfguid/libfguid.vcproj` & `libfwsi-20240417/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_extension_block/fwsi_test_extension_block.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_extension_block/fwsi_test_extension_block.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_error/fwsi_test_error.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_error/fwsi_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/libfwps/libfwps.vcproj` & `libfwsi-20240417/msvscpp/libfwps/libfwps.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/libfwsi.sln` & `libfwsi-20240417/msvscpp/libfwsi.sln`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0019_values/fwsi_test_extension_block_0xbeef0019_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0019_values/fwsi_test_extension_block_0xbeef0019_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/libclocale/libclocale.vcproj` & `libfwsi-20240417/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/pyfwsi/pyfwsi.vcproj` & `libfwsi-20240417/msvscpp/pyfwsi/pyfwsi.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/Makefile.am` & `libfwsi-20240417/msvscpp/Makefile.am`

 * *Files 0% similar despite different names*

```diff
@@ -45,13 +45,11 @@
 	libuna/libuna.vcproj \
 	pyfwsi/pyfwsi.vcproj \
 	libfwsi.sln
 
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

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_mtp_volume_values/fwsi_test_mtp_volume_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_mtp_volume_values/fwsi_test_mtp_volume_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_root_folder_values/fwsi_test_root_folder_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_root_folder_values/fwsi_test_root_folder_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_cdburn_values/fwsi_test_cdburn_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_cdburn_values/fwsi_test_cdburn_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0001_values/fwsi_test_extension_block_0xbeef0001_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0001_values/fwsi_test_extension_block_0xbeef0001_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0025_values/fwsi_test_extension_block_0xbeef0025_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0025_values/fwsi_test_extension_block_0xbeef0025_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_uri_sub_values/fwsi_test_uri_sub_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_uri_sub_values/fwsi_test_uri_sub_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_delegate_folder_values/fwsi_test_delegate_folder_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_delegate_folder_values/fwsi_test_delegate_folder_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_control_panel_category_values/fwsi_test_control_panel_category_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_control_panel_category_values/fwsi_test_control_panel_category_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_control_panel_item_values/fwsi_test_control_panel_item_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_control_panel_item_values/fwsi_test_control_panel_item_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/libfwsi/libfwsi.vcproj` & `libfwsi-20240417/msvscpp/libfwsi/libfwsi.vcproj`

 * *Files 0% similar despite different names*

#### Comparing `libfwsi-20240315/msvscpp/libfwsi/libfwsi.vcproj` & `libfwsi-20240417/msvscpp/libfwsi/libfwsi.vcproj`

```diff
@@ -51,16 +51,16 @@
       <File RelativePath="..\..\libfwsi\libfwsi_acronis_tib_file_values.c"/>
       <File RelativePath="..\..\libfwsi\libfwsi_cdburn_values.c"/>
       <File RelativePath="..\..\libfwsi\libfwsi_compressed_folder.c"/>
       <File RelativePath="..\..\libfwsi\libfwsi_compressed_folder_values.c"/>
       <File RelativePath="..\..\libfwsi\libfwsi_control_panel_category.c"/>
       <File RelativePath="..\..\libfwsi\libfwsi_control_panel_category_values.c"/>
       <File RelativePath="..\..\libfwsi\libfwsi_control_panel_cpl_file_values.c"/>
-      <File RelativePath="..\..\libfwsi\libfwsi_control_panel_identifier.c"/>
       <File RelativePath="..\..\libfwsi\libfwsi_control_panel_item.c"/>
+      <File RelativePath="..\..\libfwsi\libfwsi_control_panel_item_identifier.c"/>
       <File RelativePath="..\..\libfwsi\libfwsi_control_panel_item_values.c"/>
       <File RelativePath="..\..\libfwsi\libfwsi_debug.c"/>
       <File RelativePath="..\..\libfwsi\libfwsi_delegate_folder_values.c"/>
       <File RelativePath="..\..\libfwsi\libfwsi_error.c"/>
       <File RelativePath="..\..\libfwsi\libfwsi_extension_block.c"/>
       <File RelativePath="..\..\libfwsi\libfwsi_extension_block_0xbeef0000_values.c"/>
       <File RelativePath="..\..\libfwsi\libfwsi_extension_block_0xbeef0001_values.c"/>
@@ -106,16 +106,16 @@
       <File RelativePath="..\..\libfwsi\libfwsi_cdburn_values.h"/>
       <File RelativePath="..\..\libfwsi\libfwsi_codepage.h"/>
       <File RelativePath="..\..\libfwsi\libfwsi_compressed_folder.h"/>
       <File RelativePath="..\..\libfwsi\libfwsi_compressed_folder_values.h"/>
       <File RelativePath="..\..\libfwsi\libfwsi_control_panel_category.h"/>
       <File RelativePath="..\..\libfwsi\libfwsi_control_panel_category_values.h"/>
       <File RelativePath="..\..\libfwsi\libfwsi_control_panel_cpl_file_values.h"/>
-      <File RelativePath="..\..\libfwsi\libfwsi_control_panel_identifier.h"/>
       <File RelativePath="..\..\libfwsi\libfwsi_control_panel_item.h"/>
+      <File RelativePath="..\..\libfwsi\libfwsi_control_panel_item_identifier.h"/>
       <File RelativePath="..\..\libfwsi\libfwsi_control_panel_item_values.h"/>
       <File RelativePath="..\..\libfwsi\libfwsi_debug.h"/>
       <File RelativePath="..\..\libfwsi\libfwsi_definitions.h"/>
       <File RelativePath="..\..\libfwsi\libfwsi_delegate_folder_values.h"/>
       <File RelativePath="..\..\libfwsi\libfwsi_error.h"/>
       <File RelativePath="..\..\libfwsi\libfwsi_extension_block.h"/>
       <File RelativePath="..\..\libfwsi\libfwsi_extension_block_0xbeef0000_values.h"/>
```

### Comparing `libfwsi-20240315/msvscpp/libcdata/libcdata.vcproj` & `libfwsi-20240417/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_network_location_values/fwsi_test_network_location_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_network_location_values/fwsi_test_network_location_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_control_panel_cpl_file_values/fwsi_test_control_panel_cpl_file_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_control_panel_cpl_file_values/fwsi_test_control_panel_cpl_file_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0000_values/fwsi_test_extension_block_0xbeef0000_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0000_values/fwsi_test_extension_block_0xbeef0000_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_users_property_view_values/fwsi_test_users_property_view_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_users_property_view_values/fwsi_test_users_property_view_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0006_values/fwsi_test_extension_block_0xbeef0006_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0006_values/fwsi_test_extension_block_0xbeef0006_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_support/fwsi_test_support.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_support/fwsi_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/libcthreads/libcthreads.vcproj` & `libfwsi-20240417/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_file_entry_extension_values/fwsi_test_file_entry_extension_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_file_entry_extension_values/fwsi_test_file_entry_extension_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_item/fwsi_test_item.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_item/fwsi_test_item.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_mtp_file_entry_values/fwsi_test_mtp_file_entry_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_mtp_file_entry_values/fwsi_test_mtp_file_entry_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0013_values/fwsi_test_extension_block_0xbeef0013_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0013_values/fwsi_test_extension_block_0xbeef0013_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/libuna/libuna.vcproj` & `libfwsi-20240417/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/Makefile.in` & `libfwsi-20240417/msvscpp/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -454,15 +454,16 @@
 	libuna/libuna.vcproj \
 	pyfwsi/pyfwsi.vcproj \
 	libfwsi.sln
 
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
@@ -566,23 +567,25 @@
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
@@ -661,13 +664,10 @@
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

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef000a_values/fwsi_test_extension_block_0xbeef000a_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef000a_values/fwsi_test_extension_block_0xbeef000a_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/libcnotify/libcnotify.vcproj` & `libfwsi-20240417/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/libcerror/libcerror.vcproj` & `libfwsi-20240417/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/libfdatetime/libfdatetime.vcproj` & `libfwsi-20240417/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_item_list/fwsi_test_item_list.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_item_list/fwsi_test_item_list.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0005_values/fwsi_test_extension_block_0xbeef0005_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0005_values/fwsi_test_extension_block_0xbeef0005_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_extension_block_0xbeef0003_values/fwsi_test_extension_block_0xbeef0003_values.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0003_values/fwsi_test_extension_block_0xbeef0003_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/msvscpp/fwsi_test_notify/fwsi_test_notify.vcproj` & `libfwsi-20240417/msvscpp/fwsi_test_notify/fwsi_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/INSTALL` & `libfwsi-20240417/INSTALL`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_libcerror.h` & `libfwsi-20240417/libfwsi/libfwsi_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_control_panel_cpl_file_values.h` & `libfwsi-20240417/libfwsi/libfwsi_control_panel_cpl_file_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_compressed_folder.c` & `libfwsi-20240417/libfwsi/libfwsi_compressed_folder.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_control_panel_category.c` & `libfwsi-20240417/libfwsi/libfwsi_control_panel_category.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_types.h` & `libfwsi-20240417/libfwsi/libfwsi_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi.rc.in` & `libfwsi-20240417/libfwsi/libfwsi.rc.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extern.h` & `libfwsi-20240417/libfwsi/libfwsi_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_delegate_folder_values.c` & `libfwsi-20240417/libfwsi/libfwsi_delegate_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_uri_values.h` & `libfwsi-20240417/libfwsi/libfwsi_uri_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0001_values.h` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0001_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_file_entry_values.c` & `libfwsi-20240417/libfwsi/libfwsi_file_entry_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0000_values.h` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0000_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_error.h` & `libfwsi-20240417/libfwsi/libfwsi_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_libfole.h` & `libfwsi-20240417/libfwsi/libfwsi_libfole.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_users_property_view.h` & `libfwsi-20240417/libfwsi/libfwsi_users_property_view.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_game_folder_values.c` & `libfwsi-20240417/libfwsi/libfwsi_game_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_item_list.c` & `libfwsi-20240417/libfwsi/libfwsi_item_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0003_values.h` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0003_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_uri_sub_values.c` & `libfwsi-20240417/libfwsi/libfwsi_uri_sub_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi.rc` & `libfwsi-20240417/libfwsi/libfwsi.rc`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Windows Shell Item format\0"
-      VALUE "FileVersion",		"20240315" "\0"
+      VALUE "FileVersion",		"20240417" "\0"
       VALUE "InternalName",		"libfwsi.dll\0"
       VALUE "LegalCopyright",		"(C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfwsi.dll\0"
       VALUE "ProductName",		"libfwsi\0"
-      VALUE "ProductVersion",		"20240315" "\0"
+      VALUE "ProductVersion",		"20240417" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfwsi/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0000_values.c` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0000_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_definitions.h` & `libfwsi-20240417/libfwsi/libfwsi_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwsi/definitions.h> are copied here
  * for local use of libfwsi
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWSI_VERSION					20240315
+#define LIBFWSI_VERSION					20240417
 
 /* The version string
  */
-#define LIBFWSI_VERSION_STRING				"20240315"
+#define LIBFWSI_VERSION_STRING				"20240417"
 
 /* The byte order definitions
  */
 #define LIBFWSI_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWSI_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The item type definitions
```

### Comparing `libfwsi-20240315/libfwsi/libfwsi_control_panel_item.h` & `libfwsi-20240417/libfwsi/libfwsi_control_panel_item.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0013_values.h` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0013_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_libfguid.h` & `libfwsi-20240417/libfwsi/libfwsi_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_compressed_folder.h` & `libfwsi-20240417/libfwsi/libfwsi_compressed_folder.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0027_values.c` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0027_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0003_values.c` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0003_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_support.h` & `libfwsi-20240417/libfwsi/libfwsi_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0026_values.c` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0026_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0025_values.h` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0025_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_game_folder_values.h` & `libfwsi-20240417/libfwsi/libfwsi_game_folder_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_file_entry_values.h` & `libfwsi-20240417/libfwsi/libfwsi_file_entry_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0014_values.h` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0014_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_control_panel_category_values.h` & `libfwsi-20240417/libfwsi/libfwsi_control_panel_category_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0029_values.h` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0029_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_mtp_file_entry_values.c` & `libfwsi-20240417/libfwsi/libfwsi_mtp_file_entry_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_notify.h` & `libfwsi-20240417/libfwsi/libfwsi_notify.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_file_attributes.h` & `libfwsi-20240417/libfwsi/libfwsi_file_attributes.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0006_values.h` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0006_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0014_values.c` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0014_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_root_folder_values.h` & `libfwsi-20240417/libfwsi/libfwsi_root_folder_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_file_entry_extension_values.h` & `libfwsi-20240417/libfwsi/libfwsi_file_entry_extension_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_users_property_view_values.c` & `libfwsi-20240417/libfwsi/libfwsi_users_property_view_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/Makefile.am` & `libfwsi-20240417/libfwsi/Makefile.am`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
 	@LIBFOLE_CPPFLAGS@ \
@@ -19,16 +19,16 @@
 	libfwsi_cdburn_values.c libfwsi_cdburn_values.h \
 	libfwsi_codepage.h \
 	libfwsi_compressed_folder.c libfwsi_compressed_folder.h \
 	libfwsi_compressed_folder_values.c libfwsi_compressed_folder_values.h \
 	libfwsi_control_panel_category.c libfwsi_control_panel_category.h \
 	libfwsi_control_panel_category_values.c libfwsi_control_panel_category_values.h \
 	libfwsi_control_panel_cpl_file_values.c libfwsi_control_panel_cpl_file_values.h \
-	libfwsi_control_panel_identifier.c libfwsi_control_panel_identifier.h \
 	libfwsi_control_panel_item.c libfwsi_control_panel_item.h \
+	libfwsi_control_panel_item_identifier.c libfwsi_control_panel_item_identifier.h \
 	libfwsi_control_panel_item_values.c libfwsi_control_panel_item_values.h \
 	libfwsi_debug.c libfwsi_debug.h \
 	libfwsi_definitions.h \
 	libfwsi_delegate_folder_values.c libfwsi_delegate_folder_values.h \
 	libfwsi_error.c libfwsi_error.h \
 	libfwsi_extern.h \
 	libfwsi_extension_block.c libfwsi_extension_block.h \
@@ -94,21 +94,19 @@
 libfwsi_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libfwsi_definitions.h.in \
 	libfwsi.rc \
 	libfwsi.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfwsi_definitions.h \
+	libfwsi.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libfwsi_definitions.h
-	-rm -f libfwsi.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwsi ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwsi_la_SOURCES)
```

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0013_values.c` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0013_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0006_values.c` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0006_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_mtp_volume_values.c` & `libfwsi-20240417/libfwsi/libfwsi_mtp_volume_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_file_entry.c` & `libfwsi-20240417/libfwsi/libfwsi_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_support.c` & `libfwsi-20240417/libfwsi/libfwsi_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_acronis_tib_file_values.c` & `libfwsi-20240417/libfwsi/libfwsi_acronis_tib_file_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_control_panel_category.h` & `libfwsi-20240417/libfwsi/libfwsi_control_panel_category.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_root_folder.h` & `libfwsi-20240417/libfwsi/libfwsi_root_folder.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_unused.h` & `libfwsi-20240417/libfwsi/libfwsi_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_shell_folder_identifier.c` & `libfwsi-20240417/libfwsi/libfwsi_shell_folder_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0029_values.c` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0029_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_cdburn_values.h` & `libfwsi-20240417/libfwsi/libfwsi_cdburn_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_uri_sub_values.h` & `libfwsi-20240417/libfwsi/libfwsi_uri_sub_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_volume.h` & `libfwsi-20240417/libfwsi/libfwsi_volume.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block.h` & `libfwsi-20240417/libfwsi/libfwsi_extension_block.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_item_list.h` & `libfwsi-20240417/libfwsi/libfwsi_item_list.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_control_panel_cpl_file_values.c` & `libfwsi-20240417/libfwsi/libfwsi_control_panel_cpl_file_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef000a_values.h` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef000a_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0027_values.h` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0027_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0005_values.c` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0005_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_mtp_volume_values.h` & `libfwsi-20240417/libfwsi/libfwsi_mtp_volume_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_users_property_view_values.h` & `libfwsi-20240417/libfwsi/libfwsi_users_property_view_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_file_entry.h` & `libfwsi-20240417/libfwsi/libfwsi_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0019_values.c` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0019_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0026_values.h` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0026_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_error.c` & `libfwsi-20240417/libfwsi/libfwsi_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_network_location_values.h` & `libfwsi-20240417/libfwsi/libfwsi_network_location_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_web_site_values.h` & `libfwsi-20240417/libfwsi/libfwsi_web_site_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_file_entry_extension_values.c` & `libfwsi-20240417/libfwsi/libfwsi_file_entry_extension_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_notify.c` & `libfwsi-20240417/libfwsi/libfwsi_notify.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_acronis_tib_file_values.h` & `libfwsi-20240417/libfwsi/libfwsi_acronis_tib_file_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_definitions.h.in` & `libfwsi-20240417/libfwsi/libfwsi_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_codepage.h` & `libfwsi-20240417/libfwsi/libfwsi_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_file_entry_extension.c` & `libfwsi-20240417/libfwsi/libfwsi_file_entry_extension.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_web_site_values.c` & `libfwsi-20240417/libfwsi/libfwsi_web_site_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_volume.c` & `libfwsi-20240417/libfwsi/libfwsi_volume.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0025_values.c` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0025_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_compressed_folder_values.c` & `libfwsi-20240417/libfwsi/libfwsi_compressed_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0019_values.h` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0019_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_control_panel_item_values.h` & `libfwsi-20240417/libfwsi/libfwsi_control_panel_item_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_control_panel_item_values.c` & `libfwsi-20240417/libfwsi/libfwsi_control_panel_item_values.c`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  */
 
 #include <common.h>
 #include <byte_stream.h>
 #include <memory.h>
 #include <types.h>
 
-#include "libfwsi_control_panel_identifier.h"
+#include "libfwsi_control_panel_item_identifier.h"
 #include "libfwsi_control_panel_item_values.h"
 #include "libfwsi_debug.h"
 #include "libfwsi_libcerror.h"
 #include "libfwsi_libcnotify.h"
 #include "libfwsi_libfguid.h"
 
 /* Creates control panel item values
@@ -237,15 +237,15 @@
 			 function );
 
 			return( -1 );
 		}
 		libcnotify_printf(
 		 "%s: control panel name\t\t: %s\n",
 		 function,
-		 libfwsi_control_panel_identifier_get_name(
+		 libfwsi_control_panel_item_identifier_get_name(
 		  control_panel_item_values->identifier ) );
 
 		libcnotify_printf(
 		 "\n" );
 	}
 #endif /* defined( HAVE_DEBUG_OUTPUT ) */
```

### Comparing `libfwsi-20240315/libfwsi/libfwsi_compressed_folder_values.h` & `libfwsi-20240417/libfwsi/libfwsi_compressed_folder_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_cdburn_values.c` & `libfwsi-20240417/libfwsi/libfwsi_cdburn_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_control_panel_category_values.c` & `libfwsi-20240417/libfwsi/libfwsi_control_panel_category_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_control_panel_item.c` & `libfwsi-20240417/libfwsi/libfwsi_control_panel_item.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_network_location_values.c` & `libfwsi-20240417/libfwsi/libfwsi_network_location_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_debug.c` & `libfwsi-20240417/libfwsi/libfwsi_debug.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_item.c` & `libfwsi-20240417/libfwsi/libfwsi_item.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_volume_values.h` & `libfwsi-20240417/libfwsi/libfwsi_volume_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_file_attributes.c` & `libfwsi-20240417/libfwsi/libfwsi_file_attributes.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_debug.h` & `libfwsi-20240417/libfwsi/libfwsi_debug.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_uri_values.c` & `libfwsi-20240417/libfwsi/libfwsi_uri_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_libfwps.h` & `libfwsi-20240417/libfwsi/libfwsi_libfwps.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_libfdatetime.h` & `libfwsi-20240417/libfwsi/libfwsi_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef000a_values.c` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef000a_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_file_entry_extension.h` & `libfwsi-20240417/libfwsi/libfwsi_file_entry_extension.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_root_folder_values.c` & `libfwsi-20240417/libfwsi/libfwsi_root_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_network_location.c` & `libfwsi-20240417/libfwsi/libfwsi_network_location.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_network_location.h` & `libfwsi-20240417/libfwsi/libfwsi_network_location.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_volume_values.c` & `libfwsi-20240417/libfwsi/libfwsi_volume_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi.c` & `libfwsi-20240417/libfwsi/libfwsi.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_libuna.h` & `libfwsi-20240417/libfwsi/libfwsi_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_mtp_file_entry_values.h` & `libfwsi-20240417/libfwsi/libfwsi_mtp_file_entry_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_root_folder.c` & `libfwsi-20240417/libfwsi/libfwsi_root_folder.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/Makefile.in` & `libfwsi-20240417/libfwsi/Makefile.in`

 * *Files 7% similar despite different names*

```diff
@@ -146,16 +146,16 @@
 libfwsi_la_DEPENDENCIES =
 am_libfwsi_la_OBJECTS = libfwsi.lo libfwsi_acronis_tib_file_values.lo \
 	libfwsi_cdburn_values.lo libfwsi_compressed_folder.lo \
 	libfwsi_compressed_folder_values.lo \
 	libfwsi_control_panel_category.lo \
 	libfwsi_control_panel_category_values.lo \
 	libfwsi_control_panel_cpl_file_values.lo \
-	libfwsi_control_panel_identifier.lo \
 	libfwsi_control_panel_item.lo \
+	libfwsi_control_panel_item_identifier.lo \
 	libfwsi_control_panel_item_values.lo libfwsi_debug.lo \
 	libfwsi_delegate_folder_values.lo libfwsi_error.lo \
 	libfwsi_extension_block.lo \
 	libfwsi_extension_block_0xbeef0000_values.lo \
 	libfwsi_extension_block_0xbeef0001_values.lo \
 	libfwsi_extension_block_0xbeef0003_values.lo \
 	libfwsi_extension_block_0xbeef0005_values.lo \
@@ -210,16 +210,16 @@
 	./$(DEPDIR)/libfwsi_acronis_tib_file_values.Plo \
 	./$(DEPDIR)/libfwsi_cdburn_values.Plo \
 	./$(DEPDIR)/libfwsi_compressed_folder.Plo \
 	./$(DEPDIR)/libfwsi_compressed_folder_values.Plo \
 	./$(DEPDIR)/libfwsi_control_panel_category.Plo \
 	./$(DEPDIR)/libfwsi_control_panel_category_values.Plo \
 	./$(DEPDIR)/libfwsi_control_panel_cpl_file_values.Plo \
-	./$(DEPDIR)/libfwsi_control_panel_identifier.Plo \
 	./$(DEPDIR)/libfwsi_control_panel_item.Plo \
+	./$(DEPDIR)/libfwsi_control_panel_item_identifier.Plo \
 	./$(DEPDIR)/libfwsi_control_panel_item_values.Plo \
 	./$(DEPDIR)/libfwsi_debug.Plo \
 	./$(DEPDIR)/libfwsi_delegate_folder_values.Plo \
 	./$(DEPDIR)/libfwsi_error.Plo \
 	./$(DEPDIR)/libfwsi_extension_block.Plo \
 	./$(DEPDIR)/libfwsi_extension_block_0xbeef0000_values.Plo \
 	./$(DEPDIR)/libfwsi_extension_block_0xbeef0001_values.Plo \
@@ -573,16 +573,16 @@
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
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
 	@LIBFOLE_CPPFLAGS@ \
@@ -596,16 +596,16 @@
 	libfwsi_cdburn_values.c libfwsi_cdburn_values.h \
 	libfwsi_codepage.h \
 	libfwsi_compressed_folder.c libfwsi_compressed_folder.h \
 	libfwsi_compressed_folder_values.c libfwsi_compressed_folder_values.h \
 	libfwsi_control_panel_category.c libfwsi_control_panel_category.h \
 	libfwsi_control_panel_category_values.c libfwsi_control_panel_category_values.h \
 	libfwsi_control_panel_cpl_file_values.c libfwsi_control_panel_cpl_file_values.h \
-	libfwsi_control_panel_identifier.c libfwsi_control_panel_identifier.h \
 	libfwsi_control_panel_item.c libfwsi_control_panel_item.h \
+	libfwsi_control_panel_item_identifier.c libfwsi_control_panel_item_identifier.h \
 	libfwsi_control_panel_item_values.c libfwsi_control_panel_item_values.h \
 	libfwsi_debug.c libfwsi_debug.h \
 	libfwsi_definitions.h \
 	libfwsi_delegate_folder_values.c libfwsi_delegate_folder_values.h \
 	libfwsi_error.c libfwsi_error.h \
 	libfwsi_extern.h \
 	libfwsi_extension_block.c libfwsi_extension_block.h \
@@ -670,15 +670,18 @@
 
 libfwsi_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libfwsi_definitions.h.in \
 	libfwsi.rc \
 	libfwsi.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfwsi_definitions.h \
+	libfwsi.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -763,16 +766,16 @@
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_acronis_tib_file_values.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_cdburn_values.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_compressed_folder.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_compressed_folder_values.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_control_panel_category.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_control_panel_category_values.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_control_panel_cpl_file_values.Plo@am__quote@ # am--include-marker
-@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_control_panel_identifier.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_control_panel_item.Plo@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_control_panel_item_identifier.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_control_panel_item_values.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_debug.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_delegate_folder_values.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_error.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_extension_block.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_extension_block_0xbeef0000_values.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwsi_extension_block_0xbeef0001_values.Plo@am__quote@ # am--include-marker
@@ -961,24 +964,79 @@
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
+		-rm -f ./$(DEPDIR)/libfwsi.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_acronis_tib_file_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_cdburn_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_compressed_folder.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_compressed_folder_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_control_panel_category.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_control_panel_category_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_control_panel_cpl_file_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_control_panel_item.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_control_panel_item_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_control_panel_item_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_debug.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_delegate_folder_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_error.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_extension_block.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_extension_block_0xbeef0000_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_extension_block_0xbeef0001_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_extension_block_0xbeef0003_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_extension_block_0xbeef0005_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_extension_block_0xbeef0006_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_extension_block_0xbeef000a_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_extension_block_0xbeef0013_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_extension_block_0xbeef0014_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_extension_block_0xbeef0019_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_extension_block_0xbeef0025_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_extension_block_0xbeef0026_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_extension_block_0xbeef0027_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_extension_block_0xbeef0029_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_file_attributes.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_file_entry.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_file_entry_extension.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_file_entry_extension_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_file_entry_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_game_folder_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_item.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_item_list.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_known_folder_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_mtp_file_entry_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_mtp_volume_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_network_location.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_network_location_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_notify.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_root_folder.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_root_folder_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_shell_folder_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_support.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_uri_sub_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_uri_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_users_property_view.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_users_property_view_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_volume.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_volume_values.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_web_site_values.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1023,16 +1081,16 @@
 	-rm -f ./$(DEPDIR)/libfwsi_acronis_tib_file_values.Plo
 	-rm -f ./$(DEPDIR)/libfwsi_cdburn_values.Plo
 	-rm -f ./$(DEPDIR)/libfwsi_compressed_folder.Plo
 	-rm -f ./$(DEPDIR)/libfwsi_compressed_folder_values.Plo
 	-rm -f ./$(DEPDIR)/libfwsi_control_panel_category.Plo
 	-rm -f ./$(DEPDIR)/libfwsi_control_panel_category_values.Plo
 	-rm -f ./$(DEPDIR)/libfwsi_control_panel_cpl_file_values.Plo
-	-rm -f ./$(DEPDIR)/libfwsi_control_panel_identifier.Plo
 	-rm -f ./$(DEPDIR)/libfwsi_control_panel_item.Plo
+	-rm -f ./$(DEPDIR)/libfwsi_control_panel_item_identifier.Plo
 	-rm -f ./$(DEPDIR)/libfwsi_control_panel_item_values.Plo
 	-rm -f ./$(DEPDIR)/libfwsi_debug.Plo
 	-rm -f ./$(DEPDIR)/libfwsi_delegate_folder_values.Plo
 	-rm -f ./$(DEPDIR)/libfwsi_error.Plo
 	-rm -f ./$(DEPDIR)/libfwsi_extension_block.Plo
 	-rm -f ./$(DEPDIR)/libfwsi_extension_block_0xbeef0000_values.Plo
 	-rm -f ./$(DEPDIR)/libfwsi_extension_block_0xbeef0001_values.Plo
@@ -1114,19 +1172,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfwsi_definitions.h
-	-rm -f libfwsi.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwsi ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwsi_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwsi-20240315/libfwsi/libfwsi_delegate_folder_values.h` & `libfwsi-20240417/libfwsi/libfwsi_delegate_folder_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_libcnotify.h` & `libfwsi-20240417/libfwsi/libfwsi_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0005_values.h` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0005_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_shell_folder_identifier.h` & `libfwsi-20240417/libfwsi/libfwsi_shell_folder_identifier.h`

 * *Files 1% similar despite different names*

```diff
@@ -34,19 +34,19 @@
 
 /* The CLSID is stored as a little endian GUID
  */
 typedef struct libfwsi_shell_folder_identifier_definition libfwsi_shell_folder_identifier_definition_t;
 
 struct libfwsi_shell_folder_identifier_definition
 {
-	/* The folder identifier
+	/* The identifier
 	 */
 	uint8_t *identifier;
 
-	/* The folder name
+	/* The name
 	 */
 	const char *name;
 };
 
 extern uint8_t libfwsi_shell_folder_identifier_3d_objects[ 16 ];
 extern uint8_t libfwsi_shell_folder_identifier_activex_cache_folder[ 16 ];
 extern uint8_t libfwsi_shell_folder_identifier_add_network_place[ 16 ];
```

### Comparing `libfwsi-20240315/libfwsi/libfwsi_users_property_view.c` & `libfwsi-20240417/libfwsi/libfwsi_users_property_view.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_item.h` & `libfwsi-20240417/libfwsi/libfwsi_item.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block.c` & `libfwsi-20240417/libfwsi/libfwsi_extension_block.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_extension_block_0xbeef0001_values.c` & `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0001_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfwsi/libfwsi_libcdata.h` & `libfwsi-20240417/libfwsi/libfwsi_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_list_element.h` & `libfwsi-20240417/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_array.h` & `libfwsi-20240417/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_definitions.h` & `libfwsi-20240417/libcdata/libcdata_definitions.h`

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

### Comparing `libfwsi-20240315/libcdata/libcdata_libcerror.h` & `libfwsi-20240417/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_unused.h` & `libfwsi-20240417/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_btree.h` & `libfwsi-20240417/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_btree.c` & `libfwsi-20240417/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_support.c` & `libfwsi-20240417/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_list.c` & `libfwsi-20240417/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_extern.h` & `libfwsi-20240417/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_list.h` & `libfwsi-20240417/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_btree_values_list.h` & `libfwsi-20240417/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/Makefile.am` & `libfwsi-20240417/libcdata/Makefile.am`

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

### Comparing `libfwsi-20240315/libcdata/libcdata_btree_node.h` & `libfwsi-20240417/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_range_list_value.h` & `libfwsi-20240417/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_range_list.h` & `libfwsi-20240417/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_range_list.c` & `libfwsi-20240417/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_array.c` & `libfwsi-20240417/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_list_element.c` & `libfwsi-20240417/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_libcthreads.h` & `libfwsi-20240417/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_tree_node.h` & `libfwsi-20240417/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_error.h` & `libfwsi-20240417/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_types.h` & `libfwsi-20240417/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_btree_node.c` & `libfwsi-20240417/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_tree_node.c` & `libfwsi-20240417/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_support.h` & `libfwsi-20240417/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/Makefile.in` & `libfwsi-20240417/libcdata/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -483,16 +483,16 @@
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
@@ -509,15 +509,16 @@
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
@@ -727,24 +728,37 @@
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
 
@@ -838,17 +852,14 @@
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

### Comparing `libfwsi-20240315/libcdata/libcdata_range_list_value.c` & `libfwsi-20240417/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_btree_values_list.c` & `libfwsi-20240417/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcdata/libcdata_error.c` & `libfwsi-20240417/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/config.sub` & `libfwsi-20240417/config.sub`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/setup.py` & `libfwsi-20240417/setup.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/acinclude.m4` & `libfwsi-20240417/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/config.rpath` & `libfwsi-20240417/config.rpath`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_thread.h` & `libfwsi-20240417/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_read_write_lock.h` & `libfwsi-20240417/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_thread.c` & `libfwsi-20240417/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_thread_pool.h` & `libfwsi-20240417/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_support.h` & `libfwsi-20240417/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_lock.h` & `libfwsi-20240417/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_unused.h` & `libfwsi-20240417/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_lock.c` & `libfwsi-20240417/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_condition.h` & `libfwsi-20240417/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_repeating_thread.h` & `libfwsi-20240417/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/Makefile.am` & `libfwsi-20240417/libcthreads/Makefile.am`

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

### Comparing `libfwsi-20240315/libcthreads/libcthreads_support.c` & `libfwsi-20240417/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_mutex.c` & `libfwsi-20240417/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_queue.c` & `libfwsi-20240417/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_mutex.h` & `libfwsi-20240417/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_types.h` & `libfwsi-20240417/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_thread_attributes.h` & `libfwsi-20240417/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_condition.c` & `libfwsi-20240417/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_error.c` & `libfwsi-20240417/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_read_write_lock.c` & `libfwsi-20240417/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_libcerror.h` & `libfwsi-20240417/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_definitions.h` & `libfwsi-20240417/libcthreads/libcthreads_definitions.h`

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

### Comparing `libfwsi-20240315/libcthreads/libcthreads_thread_pool.c` & `libfwsi-20240417/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_error.h` & `libfwsi-20240417/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_thread_attributes.c` & `libfwsi-20240417/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_extern.h` & `libfwsi-20240417/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/libcthreads_repeating_thread.c` & `libfwsi-20240417/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcthreads/Makefile.in` & `libfwsi-20240417/libcthreads/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -487,16 +487,16 @@
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
@@ -511,15 +511,16 @@
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
@@ -729,24 +730,37 @@
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
 
@@ -840,17 +854,14 @@
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

### Comparing `libfwsi-20240315/libcthreads/libcthreads_queue.h` & `libfwsi-20240417/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/test-driver` & `libfwsi-20240417/test-driver`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/ChangeLog` & `libfwsi-20240417/ChangeLog`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/manuals/Makefile.in` & `libfwsi-20240417/manuals/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -440,15 +440,16 @@
 top_srcdir = @top_srcdir@
 man_MANS = \
 	libfwsi.3
 
 EXTRA_DIST = \
 	libfwsi.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -598,23 +599,25 @@
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
@@ -695,13 +698,10 @@
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

### Comparing `libfwsi-20240315/manuals/libfwsi.3` & `libfwsi-20240417/manuals/libfwsi.3`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.Dd March 17, 2024
+.Dd April 17, 2024
 .Dt libfwsi 3
 .Os libfwsi
 .Sh NAME
 .Nm libfwsi.h
 .Nd Library to access the Windows Shell Item format
 .Sh SYNOPSIS
 .In libfwsi.h
@@ -125,15 +125,15 @@
 .Ft int
 .Fn libfwsi_network_location_get_utf8_comments "libfwsi_item_t *network_location" "uint8_t *utf8_string" "size_t utf8_string_size" "libfwsi_error_t **error"
 .Ft int
 .Fn libfwsi_network_location_get_utf16_comments_size "libfwsi_item_t *network_location" "size_t *utf16_string_size" "libfwsi_error_t **error"
 .Ft int
 .Fn libfwsi_network_location_get_utf16_comments "libfwsi_item_t *network_location" "uint16_t *utf16_string" "size_t utf16_string_size" "libfwsi_error_t **error"
 .Pp
-Compressed folder item functions
+Compressed folder functions
 .Ft int
 .Fn libfwsi_compressed_folder_get_utf8_name_size "libfwsi_item_t *compressed_folder" "size_t *utf8_string_size" "libfwsi_error_t **error"
 .Ft int
 .Fn libfwsi_compressed_folder_get_utf8_name "libfwsi_item_t *compressed_folder" "uint8_t *utf8_string" "size_t utf8_string_size" "libfwsi_error_t **error"
 .Ft int
 .Fn libfwsi_compressed_folder_get_utf16_name_size "libfwsi_item_t *compressed_folder" "size_t *utf16_string_size" "libfwsi_error_t **error"
 .Ft int
```

### Comparing `libfwsi-20240315/tests/fwsi_test_control_panel_cpl_file_values.c` & `libfwsi-20240417/tests/fwsi_test_control_panel_cpl_file_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0006_values.c` & `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0006_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0003_values.c` & `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0003_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_compressed_folder_values.c` & `libfwsi-20240417/tests/fwsi_test_compressed_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_item.c` & `libfwsi-20240417/tests/fwsi_test_item.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_control_panel_category_values.c` & `libfwsi-20240417/tests/fwsi_test_control_panel_category_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef000a_values.c` & `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef000a_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/pyfwsi_test_item_list.py` & `libfwsi-20240417/tests/pyfwsi_test_item_list.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_support.c` & `libfwsi-20240417/tests/fwsi_test_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_libcerror.h` & `libfwsi-20240417/tests/fwsi_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0000_values.c` & `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0000_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0001_values.c` & `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0001_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_mtp_file_entry_values.c` & `libfwsi-20240417/tests/fwsi_test_mtp_file_entry_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_delegate_folder_values.c` & `libfwsi-20240417/tests/fwsi_test_delegate_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/Makefile.am` & `libfwsi-20240417/tests/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
 	@LIBFOLE_CPPFLAGS@ \
@@ -457,13 +457,12 @@
 	fwsi_test_unused.h \
 	fwsi_test_volume_values.c
 
 fwsi_test_volume_values_LDADD = \
 	../libfwsi/libfwsi.la \
 	@LIBCERROR_LIBADD@
 
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

### Comparing `libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0025_values.c` & `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0025_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0014_values.c` & `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0014_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_cdburn_values.c` & `libfwsi-20240417/tests/fwsi_test_cdburn_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_users_property_view_values.c` & `libfwsi-20240417/tests/fwsi_test_users_property_view_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_file_entry_values.c` & `libfwsi-20240417/tests/fwsi_test_file_entry_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_root_folder_values.c` & `libfwsi-20240417/tests/fwsi_test_root_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/test_python_module.sh` & `libfwsi-20240417/tests/test_python_module.sh`

 * *Files 5% similar despite different names*

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
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="volume";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libfwsi";
+PYTHON_MODULE="pyfwsi";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyfwsi_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyfwsi_test_${TEST_FUNCTION}.py";
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
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyfwsi");
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

### Comparing `libfwsi-20240315/tests/pyfwsi_test_extension_block.py` & `libfwsi-20240417/tests/pyfwsi_test_extension_block.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_control_panel_item_values.c` & `libfwsi-20240417/tests/fwsi_test_control_panel_item_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_volume_values.c` & `libfwsi-20240417/tests/fwsi_test_volume_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_mtp_volume_values.c` & `libfwsi-20240417/tests/fwsi_test_mtp_volume_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/pyfwsi_test_root_folder.py` & `libfwsi-20240417/tests/pyfwsi_test_root_folder.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_memory.h` & `libfwsi-20240417/tests/fwsi_test_memory.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0019_values.c` & `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0019_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/test_runner.sh` & `libfwsi-20240417/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_error.c` & `libfwsi-20240417/tests/fwsi_test_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_macros.h` & `libfwsi-20240417/tests/fwsi_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/pyfwsi_test_volume.py` & `libfwsi-20240417/tests/pyfwsi_test_volume.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0005_values.c` & `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0005_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_uri_sub_values.c` & `libfwsi-20240417/tests/fwsi_test_uri_sub_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_extension_block_0xbeef0013_values.c` & `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0013_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/pyfwsi_test_network_location.py` & `libfwsi-20240417/tests/pyfwsi_test_network_location.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_notify.c` & `libfwsi-20240417/tests/fwsi_test_notify.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/pyfwsi_test_support.py` & `libfwsi-20240417/tests/pyfwsi_test_support.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_file_entry_extension_values.c` & `libfwsi-20240417/tests/fwsi_test_file_entry_extension_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_memory.c` & `libfwsi-20240417/tests/fwsi_test_memory.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_uri_values.c` & `libfwsi-20240417/tests/fwsi_test_uri_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/pyfwsi_test_file_entry.py` & `libfwsi-20240417/tests/pyfwsi_test_file_entry.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_game_folder_values.c` & `libfwsi-20240417/tests/fwsi_test_game_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/Makefile.in` & `libfwsi-20240417/tests/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -972,16 +972,16 @@
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
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
 	@LIBFOLE_CPPFLAGS@ \
@@ -1397,16 +1397,18 @@
 	fwsi_test_unused.h \
 	fwsi_test_volume_values.c
 
 fwsi_test_volume_values_LDADD = \
 	../libfwsi/libfwsi.la \
 	@LIBCERROR_LIBADD@
 
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
@@ -1940,24 +1942,60 @@
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
+		-rm -f ./$(DEPDIR)/fwsi_test_cdburn_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_compressed_folder_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_control_panel_category_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_control_panel_cpl_file_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_control_panel_item_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_delegate_folder_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_error.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_extension_block.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_extension_block_0xbeef0000_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_extension_block_0xbeef0001_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_extension_block_0xbeef0003_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_extension_block_0xbeef0005_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_extension_block_0xbeef0006_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_extension_block_0xbeef000a_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_extension_block_0xbeef0013_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_extension_block_0xbeef0014_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_extension_block_0xbeef0019_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_extension_block_0xbeef0025_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_file_entry_extension_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_file_entry_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_game_folder_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_item.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_item_list.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_memory.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_mtp_file_entry_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_mtp_volume_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_network_location_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_notify.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_root_folder_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_support.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_uri_sub_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_uri_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_users_property_view_values.Po
+	-rm -f ./$(DEPDIR)/fwsi_test_volume_values.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -2074,13 +2112,10 @@
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

### Comparing `libfwsi-20240315/tests/fwsi_test_extension_block.c` & `libfwsi-20240417/tests/fwsi_test_extension_block.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_network_location_values.c` & `libfwsi-20240417/tests/fwsi_test_network_location_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_item_list.c` & `libfwsi-20240417/tests/fwsi_test_item_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_libfwsi.h` & `libfwsi-20240417/tests/fwsi_test_libfwsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/fwsi_test_unused.h` & `libfwsi-20240417/tests/fwsi_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/pyfwsi_test_item.py` & `libfwsi-20240417/tests/pyfwsi_test_item.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/tests/test_library.sh` & `libfwsi-20240417/tests/test_library.sh`

 * *Files 5% similar despite different names*

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
 
 LIBRARY_TESTS="cdburn_values compressed_folder_values control_panel_category_values control_panel_cpl_file_values control_panel_item_values delegate_folder_values error extension_block extension_block_0xbeef0000_values extension_block_0xbeef0001_values extension_block_0xbeef0003_values extension_block_0xbeef0005_values extension_block_0xbeef0006_values extension_block_0xbeef000a_values extension_block_0xbeef0013_values extension_block_0xbeef0014_values extension_block_0xbeef0019_values extension_block_0xbeef0025_values file_entry_extension_values file_entry_values game_folder_values item item_list mtp_file_entry_values mtp_volume_values network_location_values notify root_folder_values support uri_values uri_sub_values users_property_view_values volume_values";
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

### Comparing `libfwsi-20240315/ossfuzz/Makefile.am` & `libfwsi-20240417/ossfuzz/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common
 
 bin_PROGRAMS = \
 	item_fuzzer \
 	item_list_fuzzer
 
 item_fuzzer_SOURCES = \
 	item_fuzzer.cc \
@@ -20,19 +20,17 @@
 	ossfuzz_libfwsi.h
 
 item_list_fuzzer_LDADD = \
 	@LIB_FUZZING_ENGINE@ \
 	../libfwsi/libfwsi.la
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on item_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(item_fuzzer_SOURCES)
 	@echo "Running splint on item_list_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(item_list_fuzzer_SOURCES)
```

### Comparing `libfwsi-20240315/ossfuzz/ossfuzz_libfwsi.h` & `libfwsi-20240417/ossfuzz/ossfuzz_libfwsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/ossfuzz/item_list_fuzzer.cc` & `libfwsi-20240417/ossfuzz/item_list_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/ossfuzz/item_fuzzer.cc` & `libfwsi-20240417/ossfuzz/item_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/ossfuzz/Makefile.in` & `libfwsi-20240417/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -485,16 +485,16 @@
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
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@item_fuzzer_SOURCES = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	item_fuzzer.cc \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libfwsi.h
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@item_fuzzer_LDADD = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
@@ -504,15 +504,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	item_list_fuzzer.cc \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libfwsi.h
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@item_list_fuzzer_LDADD = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfwsi/libfwsi.la
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -759,23 +760,27 @@
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
+		-rm -f ./$(DEPDIR)/item_fuzzer.Po
+	-rm -f ./$(DEPDIR)/item_list_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -860,17 +865,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on item_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(item_fuzzer_SOURCES)
 	@echo "Running splint on item_list_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(item_list_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwsi-20240315/ltmain.sh` & `libfwsi-20240417/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/po/remove-potcdate.sin` & `libfwsi-20240417/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/po/Makefile.in.in` & `libfwsi-20240417/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/po/en@quot.header` & `libfwsi-20240417/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/po/en@boldquot.header` & `libfwsi-20240417/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/po/insert-header.sin` & `libfwsi-20240417/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/po/Makevars` & `libfwsi-20240417/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/po/Makevars.in` & `libfwsi-20240417/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/po/Rules-quot` & `libfwsi-20240417/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1251.c` & `libfwsi-20240417/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_utf16_string.c` & `libfwsi-20240417/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_base16_stream.c` & `libfwsi-20240417/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_utf8_stream.h` & `libfwsi-20240417/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_2.h` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_932.c` & `libfwsi-20240417/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_dingbats.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_utf8_string.c` & `libfwsi-20240417/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_base64_stream.c` & `libfwsi-20240417/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_error.h` & `libfwsi-20240417/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_turkish.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_unicode_character.c` & `libfwsi-20240417/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_gaelic.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_arabic.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_thai.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_874.h` & `libfwsi-20240417/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_15.h` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_utf8_string.h` & `libfwsi-20240417/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_16.c` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1255.c` & `libfwsi-20240417/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_utf7_stream.c` & `libfwsi-20240417/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_byte_stream.h` & `libfwsi-20240417/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_koi8_u.c` & `libfwsi-20240417/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_unused.h` & `libfwsi-20240417/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_6.c` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_14.c` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_base64_stream.h` & `libfwsi-20240417/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_error.c` & `libfwsi-20240417/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_centraleurroman.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_romanian.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_6.h` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_9.c` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_russian.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_dingbats.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_15.c` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_936.c` & `libfwsi-20240417/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_croatian.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_scsu.h` & `libfwsi-20240417/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/Makefile.am` & `libfwsi-20240417/libuna/Makefile.am`

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

### Comparing `libfwsi-20240315/libuna/libuna_utf32_stream.c` & `libfwsi-20240417/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_936.h` & `libfwsi-20240417/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_10.c` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_roman.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_utf7_stream.h` & `libfwsi-20240417/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_3.h` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_thai.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_farsi.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_ukrainian.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_inuit.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_932.h` & `libfwsi-20240417/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_874.c` & `libfwsi-20240417/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_5.c` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_10.h` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_definitions.h` & `libfwsi-20240417/libuna/libuna_definitions.h`

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

### Comparing `libfwsi-20240315/libuna/libuna_url_stream.h` & `libfwsi-20240417/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_icelandic.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_koi8_u.h` & `libfwsi-20240417/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_utf16_stream.c` & `libfwsi-20240417/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1253.c` & `libfwsi-20240417/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_4.h` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_greek.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_libcerror.h` & `libfwsi-20240417/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_centraleurroman.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1254.c` & `libfwsi-20240417/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_13.h` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_7.h` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1255.h` & `libfwsi-20240417/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_unicode_character.h` & `libfwsi-20240417/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_8.h` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_13.c` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_949.h` & `libfwsi-20240417/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_cyrillic.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_celtic.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_support.h` & `libfwsi-20240417/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_4.c` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_949.c` & `libfwsi-20240417/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_utf16_stream.h` & `libfwsi-20240417/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_symbol.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_roman.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1257.c` & `libfwsi-20240417/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1254.h` & `libfwsi-20240417/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_950.c` & `libfwsi-20240417/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_extern.h` & `libfwsi-20240417/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1256.c` & `libfwsi-20240417/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_types.h` & `libfwsi-20240417/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_base32_stream.h` & `libfwsi-20240417/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1253.h` & `libfwsi-20240417/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_16.h` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_utf8_stream.c` & `libfwsi-20240417/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1250.h` & `libfwsi-20240417/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_2.c` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_support.c` & `libfwsi-20240417/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_koi8_r.c` & `libfwsi-20240417/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_5.h` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_utf16_string.h` & `libfwsi-20240417/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_utf32_string.c` & `libfwsi-20240417/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_icelandic.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1256.h` & `libfwsi-20240417/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_utf32_string.h` & `libfwsi-20240417/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_romanian.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_8.c` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_koi8_r.h` & `libfwsi-20240417/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_cyrillic.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_arabic.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_croatian.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_9.h` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_greek.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1258.h` & `libfwsi-20240417/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_7.c` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/Makefile.in` & `libfwsi-20240417/libuna/Makefile.in`

 * *Files 7% similar despite different names*

```diff
@@ -641,16 +641,16 @@
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
@@ -716,15 +716,16 @@
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
@@ -986,24 +987,89 @@
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
 
@@ -1149,17 +1215,14 @@
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

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_3.c` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1250.c` & `libfwsi-20240417/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_scsu.c` & `libfwsi-20240417/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1252.c` & `libfwsi-20240417/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_turkish.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_ukrainian.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_russian.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1258.c` & `libfwsi-20240417/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_celtic.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_byte_stream.c` & `libfwsi-20240417/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_gaelic.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_utf32_stream.h` & `libfwsi-20240417/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_symbol.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1257.h` & `libfwsi-20240417/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_inuit.h` & `libfwsi-20240417/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_mac_farsi.c` & `libfwsi-20240417/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_950.h` & `libfwsi-20240417/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_url_stream.c` & `libfwsi-20240417/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1251.h` & `libfwsi-20240417/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_windows_1252.h` & `libfwsi-20240417/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_codepage_iso_8859_14.h` & `libfwsi-20240417/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_base16_stream.h` & `libfwsi-20240417/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libuna/libuna_base32_stream.c` & `libfwsi-20240417/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/Makefile.in` & `libfwsi-20240417/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -580,16 +580,23 @@
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
+	libfwsi.pc \
+	libfwsi.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libfwsi.pc
 
 all: all-recursive
 
@@ -1006,23 +1013,26 @@
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
 
@@ -1129,22 +1139,10 @@
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfole && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwps && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwsi && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfwsi.pc
-	-rm -f libfwsi.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwsi-20240315/libcnotify/libcnotify_definitions.h` & `libfwsi-20240417/libcnotify/libcnotify_definitions.h`

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

### Comparing `libfwsi-20240315/libcnotify/libcnotify_extern.h` & `libfwsi-20240417/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcnotify/libcnotify_support.c` & `libfwsi-20240417/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcnotify/libcnotify_stream.h` & `libfwsi-20240417/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcnotify/Makefile.am` & `libfwsi-20240417/libcnotify/Makefile.am`

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

### Comparing `libfwsi-20240315/libcnotify/libcnotify_unused.h` & `libfwsi-20240417/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcnotify/libcnotify_verbose.h` & `libfwsi-20240417/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcnotify/libcnotify_print.h` & `libfwsi-20240417/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcnotify/libcnotify_stream.c` & `libfwsi-20240417/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcnotify/libcnotify_support.h` & `libfwsi-20240417/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcnotify/libcnotify_verbose.c` & `libfwsi-20240417/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcnotify/Makefile.in` & `libfwsi-20240417/libcnotify/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -465,30 +465,31 @@
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
@@ -691,24 +692,30 @@
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
 
@@ -795,17 +802,14 @@
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

### Comparing `libfwsi-20240315/libcnotify/libcnotify_libcerror.h` & `libfwsi-20240417/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcnotify/libcnotify_print.c` & `libfwsi-20240417/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcerror/libcerror_system.c` & `libfwsi-20240417/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcerror/libcerror_error.c` & `libfwsi-20240417/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcerror/libcerror_extern.h` & `libfwsi-20240417/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcerror/Makefile.am` & `libfwsi-20240417/libcerror/Makefile.am`

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

### Comparing `libfwsi-20240315/libcerror/libcerror_types.h` & `libfwsi-20240417/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcerror/libcerror_support.h` & `libfwsi-20240417/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcerror/libcerror_error.h` & `libfwsi-20240417/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcerror/libcerror_system.h` & `libfwsi-20240417/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcerror/libcerror_definitions.h` & `libfwsi-20240417/libcerror/libcerror_definitions.h`

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

### Comparing `libfwsi-20240315/libcerror/libcerror_support.c` & `libfwsi-20240417/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcerror/libcerror_unused.h` & `libfwsi-20240417/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libcerror/Makefile.in` & `libfwsi-20240417/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -462,28 +462,29 @@
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
@@ -685,24 +686,29 @@
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
 
@@ -788,17 +794,14 @@
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

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_floatingtime.h` & `libfwsi-20240417/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_nsf_timedate.c` & `libfwsi-20240417/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_error.h` & `libfwsi-20240417/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_floatingtime.c` & `libfwsi-20240417/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_support.h` & `libfwsi-20240417/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_hfs_time.h` & `libfwsi-20240417/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_definitions.h` & `libfwsi-20240417/libfdatetime/libfdatetime_definitions.h`

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

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_hfs_time.c` & `libfwsi-20240417/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/Makefile.am` & `libfwsi-20240417/libfdatetime/Makefile.am`

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

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_filetime.c` & `libfwsi-20240417/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_systemtime.h` & `libfwsi-20240417/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_extern.h` & `libfwsi-20240417/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_posix_time.c` & `libfwsi-20240417/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_unused.h` & `libfwsi-20240417/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_fat_date_time.h` & `libfwsi-20240417/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_systemtime.c` & `libfwsi-20240417/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_nsf_timedate.h` & `libfwsi-20240417/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_libcerror.h` & `libfwsi-20240417/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_support.c` & `libfwsi-20240417/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_error.c` & `libfwsi-20240417/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_posix_time.h` & `libfwsi-20240417/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_date_time_values.h` & `libfwsi-20240417/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_filetime.h` & `libfwsi-20240417/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_date_time_values.c` & `libfwsi-20240417/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_types.h` & `libfwsi-20240417/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/libfdatetime/Makefile.in` & `libfwsi-20240417/libfdatetime/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -484,16 +484,16 @@
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
@@ -506,15 +506,16 @@
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
@@ -723,24 +724,36 @@
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
 
@@ -833,17 +846,14 @@
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

### Comparing `libfwsi-20240315/libfdatetime/libfdatetime_fat_date_time.c` & `libfwsi-20240417/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/aclocal.m4` & `libfwsi-20240417/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240315/configure.ac` & `libfwsi-20240417/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfwsi],
- [20240315],
+ [20240417],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfwsi.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

### Comparing `libfwsi-20240315/libfwsi.spec` & `libfwsi-20240417/libfwsi.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libfwsi
-Version: 20240315
+Version: 20240417
 Release: 1
 Summary: Library to access the Windows Shell Item format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfwsi
           
@@ -76,10 +76,10 @@
 %files -n libfwsi-python3
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %changelog
-* Sun Mar 17 2024 Joachim Metz <joachim.metz@gmail.com> 20240315-1
+* Wed Apr 17 2024 Joachim Metz <joachim.metz@gmail.com> 20240417-1
 - Auto-generated
```

